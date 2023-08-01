# Comparing `tmp/forestadmin_agent_toolkit-1.0.0b4.tar.gz` & `tmp/forestadmin_agent_toolkit-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_toolkit-1.0.0b4.tar", max compression
+gzip compressed data, was "forestadmin_agent_toolkit-1.0.0b5.tar", max compression
```

## Comparing `forestadmin_agent_toolkit-1.0.0b4.tar` & `forestadmin_agent_toolkit-1.0.0b5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/README.md
--rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/__init__.py
--rw-r--r--   0        0        0     5450 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/agent.py
--rw-r--r--   0        0        0      135 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/exceptions.py
--rw-r--r--   0        0        0     1276 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/forest_logger.py
--rw-r--r--   0        0        0      856 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/options.py
--rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/actions/__init__.py
--rw-r--r--   0        0        0     2292 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/actions/requests.py
--rw-r--r--   0        0        0     6127 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/actions/resources.py
--rw-r--r--   0        0        0      464 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/base.py
--rw-r--r--   0        0        0      913 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/__init__.py
--rw-r--r--   0        0        0     2494 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/charts_collection.py
--rw-r--r--   0        0        0     1708 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
--rw-r--r--   0        0        0    15947 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/crud.py
--rw-r--r--   0        0        0    19417 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/crud_related.py
--rw-r--r--   0        0        0     2966 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/decorators.py
--rw-r--r--   0        0        0      148 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/exceptions.py
--rw-r--r--   0        0        0    11045 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/filter.py
--rw-r--r--   0        0        0     5624 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/requests.py
--rw-r--r--   0        0        0     9466 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/stats.py
--rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/security/__init__.py
--rw-r--r--   0        0        0      144 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/security/exceptions.py
--rw-r--r--   0        0        0     3763 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/security/resources.py
--rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/__init__.py
--rw-r--r--   0        0        0     8403 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/permissions/__init__.py
--rw-r--r--   0        0        0      264 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/permissions/options.py
--rw-r--r--   0        0        0     1660 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/serializers/__init__.py
--rw-r--r--   0        0        0     9523 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/serializers/json_api.py
--rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     3227 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/authentication.py
--rw-r--r--   0        0        0     2266 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/context.py
--rw-r--r--   0        0        0     1392 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/csv.py
--rw-r--r--   0        0        0        0 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
--rw-r--r--   0        0        0     3039 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
--rw-r--r--   0        0        0     4367 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
--rw-r--r--   0        0        0     2236 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
--rw-r--r--   0        0        0     4508 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
--rw-r--r--   0        0        0     2288 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
--rw-r--r--   0        0        0     7847 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
--rw-r--r--   0        0        0      506 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
--rw-r--r--   0        0        0     3057 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/type.py
--rw-r--r--   0        0        0     1281 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/validation.py
--rw-r--r--   0        0        0     4265 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/http.py
--rw-r--r--   0        0        0     1683 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/id.py
--rw-r--r--   0        0        0      541 2023-07-31 15:37:46.463579 forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/token.py
--rw-r--r--   0        0        0     1771 2023-07-31 15:38:05.659583 forestadmin_agent_toolkit-1.0.0b4/pyproject.toml
--rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/README.md
+-rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/__init__.py
+-rw-r--r--   0        0        0     5682 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/agent.py
+-rw-r--r--   0        0        0      135 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/exceptions.py
+-rw-r--r--   0        0        0     1276 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/forest_logger.py
+-rw-r--r--   0        0        0      909 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/options.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/actions/__init__.py
+-rw-r--r--   0        0        0     2292 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/actions/requests.py
+-rw-r--r--   0        0        0     6431 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/actions/resources.py
+-rw-r--r--   0        0        0      464 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/base.py
+-rw-r--r--   0        0        0      913 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/__init__.py
+-rw-r--r--   0        0        0     2816 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/charts_collection.py
+-rw-r--r--   0        0        0     1966 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
+-rw-r--r--   0        0        0    17087 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/crud.py
+-rw-r--r--   0        0        0    21321 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/crud_related.py
+-rw-r--r--   0        0        0     2972 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/decorators.py
+-rw-r--r--   0        0        0      148 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/exceptions.py
+-rw-r--r--   0        0        0    11045 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/filter.py
+-rw-r--r--   0        0        0     5624 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/requests.py
+-rw-r--r--   0        0        0     9929 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/stats.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/security/__init__.py
+-rw-r--r--   0        0        0      144 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/security/exceptions.py
+-rw-r--r--   0        0        0     3763 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/security/resources.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/__init__.py
+-rw-r--r--   0        0        0     8403 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/permissions/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/permissions/options.py
+-rw-r--r--   0        0        0     1660 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/serializers/__init__.py
+-rw-r--r--   0        0        0     9523 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/serializers/json_api.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     3227 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/authentication.py
+-rw-r--r--   0        0        0     4044 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/context.py
+-rw-r--r--   0        0        0     1392 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/csv.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
+-rw-r--r--   0        0        0     3039 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
+-rw-r--r--   0        0        0     4367 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
+-rw-r--r--   0        0        0     2236 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
+-rw-r--r--   0        0        0     4508 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
+-rw-r--r--   0        0        0     2288 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
+-rw-r--r--   0        0        0     7847 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
+-rw-r--r--   0        0        0      506 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
+-rw-r--r--   0        0        0     3057 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/type.py
+-rw-r--r--   0        0        0     1281 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/validation.py
+-rw-r--r--   0        0        0     4265 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/http.py
+-rw-r--r--   0        0        0     1683 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/id.py
+-rw-r--r--   0        0        0      541 2023-08-01 13:28:22.846356 forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/token.py
+-rw-r--r--   0        0        0     1771 2023-08-01 13:28:40.426165 forestadmin_agent_toolkit-1.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.0.0b5/PKG-INFO
```

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/agent.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from forestadmin.agent_toolkit.resources.collections.charts_datasource import ChartsDatasourceResource
 from forestadmin.agent_toolkit.resources.collections.crud import CrudResource
 from forestadmin.agent_toolkit.resources.collections.crud_related import CrudRelatedResource
 from forestadmin.agent_toolkit.resources.collections.stats import StatsResource
 from forestadmin.agent_toolkit.resources.security.resources import Authentication
 from forestadmin.agent_toolkit.services.permissions import PermissionService
 from forestadmin.agent_toolkit.services.serializers.json_api import create_json_api_schema
+from forestadmin.agent_toolkit.utils.context import HttpResponseBuilder
 from forestadmin.agent_toolkit.utils.forest_schema.emitter import SchemaEmitter
 from forestadmin.agent_toolkit.utils.forest_schema.type import AgentMeta
 from forestadmin.agent_toolkit.utils.http import ForestHttpApi
 from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
 from forestadmin.datasource_toolkit.datasource_customizer.datasource_customizer import DatasourceCustomizer
 from forestadmin.datasource_toolkit.datasources import Datasource
 from forestadmin.datasource_toolkit.decorators.chart.types import DataSourceChartDefinition
@@ -43,16 +44,20 @@
     META: AgentMeta = None
 
     def __init__(self, options: Options):
         self.options = copy.copy(DEFAULT_OPTIONS)
         self.options.update({k: v for k, v in options.items() if v is not None})
         self.customizer: DatasourceCustomizer = DatasourceCustomizer()
         self._resources = None
+
         ForestLogger.setup_logger(self.options["logger_level"], self.options["logger"])
 
+        if "customize_error_message" in self.options:
+            HttpResponseBuilder.setup_error_message_customizer(self.options["customize_error_message"])
+
         self._permission_service = PermissionService(
             {
                 "env_secret": self.options["env_secret"],
                 "forest_server_url": self.options["forest_server_url"],
                 "is_production": self.options["is_production"],
                 "permission_cache_duration": self.options["permissions_cache_duration_in_seconds"],
             }
```

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/forest_logger.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/forest_logger.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/options.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/options.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,22 +15,23 @@
     env_secret: str
     forest_server_url: str
     is_production: bool
     schema_path: str
     logger: Callable[[str, str], None]
     logger_level: int
     permissions_cache_duration_in_seconds: int
+    customize_error_message: Callable[[Exception], str]
     # typingsPath
     # typingsMaxDepth
-    # permissionsCacheDurationInSeconds
     # skipSchemaUpdate
     # forestAdminClient
 
 
 DEFAULT_OPTIONS: Options = {
     "is_production": False,
     "prefix": "forest",
     "forest_server_url": "https://api.forestadmin.com",
     "logger": None,
     "logger_level": logging.INFO,
+    "customize_error_message": None,
     "permissions_cache_duration_in_seconds": 15 * 60,
 }
```

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/actions/requests.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/actions/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/actions/resources.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/actions/resources.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 from typing import Any, Dict, List, Optional, Union
 
+from forestadmin.agent_toolkit.forest_logger import ForestLogger
 from forestadmin.agent_toolkit.resources.actions.requests import ActionRequest, RequestActionException
 from forestadmin.agent_toolkit.resources.collections import BaseCollectionResource
 from forestadmin.agent_toolkit.resources.collections.crud import LiteralMethod
 from forestadmin.agent_toolkit.resources.collections.decorators import authenticate, check_method
 from forestadmin.agent_toolkit.resources.collections.filter import (
     build_filter,
     parse_condition_tree,
     parse_selection_ids,
 )
-from forestadmin.agent_toolkit.utils.context import (
-    FileResponse,
-    Request,
-    RequestMethod,
-    Response,
-    build_client_error_response,
-    build_json_response,
-    build_success_response,
-)
+from forestadmin.agent_toolkit.utils.context import FileResponse, HttpResponseBuilder, Request, RequestMethod, Response
 from forestadmin.agent_toolkit.utils.forest_schema.action_values import ForestValueConverter
 from forestadmin.agent_toolkit.utils.forest_schema.generator_action import SchemaActionGenerator
 from forestadmin.agent_toolkit.utils.forest_schema.type import ForestServerActionField
 from forestadmin.datasource_toolkit.decorators.action.result_builder import ResultBuilder
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.factory import ConditionTreeFactory
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.base import ConditionTree
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.branch import Aggregator, ConditionTreeBranch
@@ -30,52 +23,57 @@
 
 class ActionResource(BaseCollectionResource):
     async def dispatch(self, request: Request, method_name: LiteralMethod) -> Response:
         method = getattr(self, method_name)
         try:
             request_collection = ActionRequest.from_request(request, self.datasource)
         except RequestActionException as e:
-            return build_client_error_response([str(e)])
-        return await method(request_collection)
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
+        try:
+            return await method(request_collection)
+        except Exception as e:
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
     @check_method(RequestMethod.POST)
     @authenticate
     async def execute(self, request: ActionRequest) -> Union[FileResponse, Response]:
         if not request.body or not request.query:
             raise Exception
         filter = await self._get_records_selection(request)
         raw_data: Dict[str, Any] = request.body.get("data", {}).get("attributes", {}).get("values", {})  # type: ignore
         unsafe_data = ForestValueConverter.make_form_unsafe_data(raw_data)
         fields = await request.collection.get_form(request.user, request.action_name, raw_data, filter)
         data = ForestValueConverter.make_form_data(request.collection.datasource, unsafe_data, fields)
         result = await request.collection.execute(request.user, request.action_name, data, filter)
 
         if result["type"] == ResultBuilder.ERROR:
-            return build_json_response(400, {"error": result["message"]})
+            return HttpResponseBuilder.build_json_response(400, {"error": result["message"]})
         elif result["type"] == ResultBuilder.SUCCESS:
             key = "success"
             if result["format"] == "html":
                 key = "html"
-            return build_success_response({key: result["message"]})
+            return HttpResponseBuilder.build_success_response({key: result["message"]})
         elif result["type"] == ResultBuilder.WEBHOOK:
-            return build_success_response(
+            return HttpResponseBuilder.build_success_response(
                 {
                     "webhook": {
                         "url": result["url"],
                         "method": result["method"],
                         "headers": result["headers"],
                         "body": result["body"],
                     }
                 }
             )
         elif result["type"] == ResultBuilder.FILE:
             return FileResponse(result["stream"], result["name"], result["mimeType"])
 
         elif result["type"] == ResultBuilder.REDIRECT:
-            return build_success_response({"redirectTo": result["path"]})
+            return HttpResponseBuilder.build_success_response({"redirectTo": result["path"]})
         raise
 
     @check_method(RequestMethod.POST)
     @authenticate
     async def hook(self, request: ActionRequest) -> Response:
         if not request.body:
             raise Exception
@@ -93,15 +91,15 @@
             request.user,
             request.action_name,
             data,
             _filter,
             {"changed_field": request.body.get("data", {}).get("attributes", {}).get("changed_field")},
         )
 
-        return build_success_response(
+        return HttpResponseBuilder.build_success_response(
             {
                 "fields": [
                     await SchemaActionGenerator.build_field_schema(request.collection.datasource, field)
                     for field in fields
                 ]
             }
         )
```

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/__init__.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/charts_collection.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/charts_collection.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import sys
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+from forestadmin.agent_toolkit.forest_logger import ForestLogger
 from forestadmin.agent_toolkit.resources.collections import BaseCollectionResource
 from forestadmin.agent_toolkit.resources.collections.decorators import authenticate, check_method
 from forestadmin.agent_toolkit.resources.collections.requests import RequestCollection, RequestCollectionException
 from forestadmin.agent_toolkit.services.serializers import json_api
-from forestadmin.agent_toolkit.utils.context import (
-    Request,
-    RequestMethod,
-    Response,
-    build_client_error_response,
-    build_success_response,
-)
+from forestadmin.agent_toolkit.utils.context import HttpResponseBuilder, Request, RequestMethod, Response
 from forestadmin.agent_toolkit.utils.id import unpack_id
+from forestadmin.datasource_toolkit.exceptions import ForestException
 
 
 class ChartsCollectionResource(BaseCollectionResource):
     async def dispatch(self, request: Request, method_name: Literal["add"]) -> Response:
         try:
             request_collection = RequestCollection.from_request(request, self.datasource)
         except RequestCollectionException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         if request.method == RequestMethod.POST:
             handle = self.handle_api_chart
         elif request.method == RequestMethod.GET:
             handle = self.handle_smart_chart
         else:
-            return build_client_error_response([f"Method {request.method.value} is not allow for this url."])
+            msg = f"Method {request.method.value} is not allow for this url."
+            ForestLogger.log("error", msg)
+            return HttpResponseBuilder.build_client_error_response([ForestException(msg)])
 
         try:
-            return build_success_response(await handle(request_collection))
+            return HttpResponseBuilder.build_success_response(await handle(request_collection))
         except Exception as exc:
-            return build_client_error_response([str(exc)])
+            ForestLogger.log("exception", exc)
+            return HttpResponseBuilder.build_client_error_response([exc])
 
     @check_method(RequestMethod.POST)
     @authenticate
     async def handle_api_chart(self, request: RequestCollection) -> Response:
         ids = unpack_id(request.collection.schema, request.body.get("record_id") or request.query.get("record_id"))
 
         chart = await request.collection.render_chart(request.user, request.query["chart_name"], ids)
```

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/charts_datasource.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/charts_datasource.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,40 +2,38 @@
 from typing import Union
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+from forestadmin.agent_toolkit.forest_logger import ForestLogger
 from forestadmin.agent_toolkit.resources.collections import BaseCollectionResource
 from forestadmin.agent_toolkit.resources.collections.decorators import authenticate, check_method
 from forestadmin.agent_toolkit.services.serializers import json_api
-from forestadmin.agent_toolkit.utils.context import (
-    FileResponse,
-    Request,
-    RequestMethod,
-    Response,
-    build_client_error_response,
-    build_success_response,
-)
+from forestadmin.agent_toolkit.utils.context import FileResponse, HttpResponseBuilder, Request, RequestMethod, Response
+from forestadmin.datasource_toolkit.exceptions import ForestException
 
 
 class ChartsDatasourceResource(BaseCollectionResource):
     async def dispatch(self, request: Request, method_name: Literal["add"]) -> Union[Response, FileResponse]:
         if request.method.value == "POST":
             handle = self.handle_api_chart
         elif request.method.value == "GET":
             handle = self.handle_smart_chart
         else:
-            return build_client_error_response([f"Method {request.method.value} is not allow for this url."])
+            msg = f"Method {request.method.value} is not allow for this url."
+            ForestLogger.log("error", msg)
+            return HttpResponseBuilder.build_client_error_response([ForestException(msg)])
 
         try:
-            return build_success_response(await handle(request))
+            return HttpResponseBuilder.build_success_response(await handle(request))
         except Exception as exc:
-            return build_client_error_response([str(exc)])
+            ForestLogger.log("exception", exc)
+            return HttpResponseBuilder.build_client_error_response([exc])
 
     @check_method(RequestMethod.POST)
     @authenticate
     async def handle_api_chart(self, request: Request) -> Response:
         chart = await self.datasource.render_chart(request.user, request.query["chart_name"])
         return {"data": json_api.render_chart(chart)}
```

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/crud.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/crud.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,39 +6,30 @@
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 from typing import Any, Awaitable, Dict, List, Tuple, cast
 
+from forestadmin.agent_toolkit.forest_logger import ForestLogger
 from forestadmin.agent_toolkit.resources.collections import BaseCollectionResource
 from forestadmin.agent_toolkit.resources.collections.decorators import authenticate, authorize, check_method
 from forestadmin.agent_toolkit.resources.collections.exceptions import CollectionResourceException
 from forestadmin.agent_toolkit.resources.collections.filter import (
     FilterException,
     build_filter,
     build_paginated_filter,
     parse_condition_tree,
     parse_projection_with_pks,
     parse_selection_ids,
     parse_timezone,
 )
 from forestadmin.agent_toolkit.resources.collections.requests import RequestCollection, RequestCollectionException
 from forestadmin.agent_toolkit.services.serializers.json_api import JsonApiException, JsonApiSerializer
-from forestadmin.agent_toolkit.utils.context import (
-    Request,
-    RequestMethod,
-    Response,
-    User,
-    build_client_error_response,
-    build_csv_response,
-    build_no_content_response,
-    build_success_response,
-    build_unknown_response,
-)
+from forestadmin.agent_toolkit.utils.context import HttpResponseBuilder, Request, RequestMethod, Response, User
 from forestadmin.agent_toolkit.utils.csv import Csv, CsvException
 from forestadmin.agent_toolkit.utils.id import unpack_id
 from forestadmin.datasource_toolkit.collections import Collection
 from forestadmin.datasource_toolkit.datasources import DatasourceException
 from forestadmin.datasource_toolkit.exceptions import ForestValidationException
 from forestadmin.datasource_toolkit.interfaces.fields import (
     ManyToOne,
@@ -74,180 +65,197 @@
 
 class CrudResource(BaseCollectionResource):
     async def dispatch(self, request: Request, method_name: LiteralMethod) -> Response:
         method = getattr(self, method_name)
         try:
             request_collection = RequestCollection.from_request(request, self.datasource)
         except RequestCollectionException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         try:
             return await method(request_collection)
         except ForestValidationException as e:
-            return build_client_error_response(
-                [{"name": "ForestValidationException", "detail": str(e)[3:], "status": 400}]
-            )
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
     @check_method(RequestMethod.GET)
     @authenticate
     @authorize("read")
     async def get(self, request: RequestCollection) -> Response:
         collection = request.collection
         try:
             ids = unpack_id(collection.schema, request.pks)
         except (FieldValidatorException, CollectionResourceException) as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         trees: List[ConditionTree] = [ConditionTreeFactory.match_ids(collection.schema, [ids])]
         scope_tree = await self.permission.get_scope(request)
         if scope_tree:
             trees.append(scope_tree)
 
         filter = PaginatedFilter({"condition_tree": ConditionTreeFactory.intersect(trees)})
 
         projections = ProjectionFactory.all(cast(Collection, collection))
         records = await collection.list(request.user, filter, projections)
 
         if not len(records):
-            return build_unknown_response()
+            return HttpResponseBuilder.build_unknown_response()
 
         for name, schema in collection.schema["fields"].items():
             if is_many_to_many(schema) or is_one_to_many(schema):
                 projections.append(f"{name}:id")  # type: ignore
                 records[0][name] = None
 
         schema = JsonApiSerializer.get(collection)
         try:
             dumped: Dict[str, Any] = schema(projections=projections).dump(records[0])  # type: ignore
         except JsonApiException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
-        return build_success_response(dumped)
+        return HttpResponseBuilder.build_success_response(dumped)
 
     @check_method(RequestMethod.POST)
     @authenticate
     @authorize("add")
     async def add(self, request: RequestCollection) -> Response:
         collection = request.collection
         schema = JsonApiSerializer.get(collection)
         try:
             data: RecordsDataAlias = schema().load(request.body)  # type: ignore
         except JsonApiException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         record, one_to_one_relations = await self.extract_data(request.user, cast(Collection, collection), data)
 
         try:
             RecordValidator.validate(cast(Collection, collection), record)
         except RecordValidatorException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         try:
             records = await collection.create(request.user, [record])
         except DatasourceException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         try:
             await self._link_one_to_one_relations(request, records[0], one_to_one_relations)
         except CollectionResourceException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
-        return build_success_response(
+        return HttpResponseBuilder.build_success_response(
             schema(projections=list(records[0].keys())).dump(records[0], many=False)  # type: ignore
         )
 
     @check_method(RequestMethod.GET)
     @authenticate
     @authorize("browse")
     async def list(self, request: RequestCollection) -> Response:
         scope_tree = await self.permission.get_scope(request)
         try:
             paginated_filter = build_paginated_filter(request, scope_tree)
         except FilterException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
         try:
             projections = parse_projection_with_pks(request)
         except DatasourceException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         records = await request.collection.list(request.user, paginated_filter, projections)
         schema = JsonApiSerializer.get(request.collection)
         try:
             dumped: Dict[str, Any] = schema(projections=projections).dump(records, many=True)  # type: ignore
         except JsonApiException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         # TODO: add something like this (but between crud and crud related ; function need adaptation)
         # if paginated_filter.search:
         #     dumped = add_search_metadata(dumped, paginated_filter.search)
 
-        return build_success_response(dumped)
+        return HttpResponseBuilder.build_success_response(dumped)
 
     @check_method(RequestMethod.GET)
     @authenticate
     @authorize("browse")
     @authorize("export")
     async def csv(self, request: RequestCollection) -> Response:
         scope_tree = await self.permission.get_scope(request)
         try:
             paginated_filter = build_paginated_filter(request, scope_tree)
         except FilterException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
         try:
             projections = parse_projection_with_pks(request)
         except DatasourceException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         records = await request.collection.list(request.user, paginated_filter, projections)
 
         try:
             csv_str = Csv.make_csv(records, projections)
         except CsvException as e:
-            return build_client_error_response([str(e)])
-        return build_csv_response(csv_str, f"{request.query.get('filename', request.collection.name)}.csv")
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
+        return HttpResponseBuilder.build_csv_response(
+            csv_str, f"{request.query.get('filename', request.collection.name)}.csv"
+        )
 
     @check_method(RequestMethod.GET)
     @authenticate
     @authorize("browse")
     async def count(self, request: RequestCollection) -> Response:
         if request.collection.schema["countable"] is False:
-            return build_success_response({"meta": {"count": "deactivated"}})
+            return HttpResponseBuilder.build_success_response({"meta": {"count": "deactivated"}})
 
         scope_tree = await self.permission.get_scope(request)
         filter = build_filter(request, scope_tree)
         aggregation = Aggregation({"operation": "Count"})
         result = await request.collection.aggregate(request.user, filter, aggregation)
         try:
             count = result[0]["value"]
         except IndexError:
             count = 0
-        return build_success_response({"count": count})
+        return HttpResponseBuilder.build_success_response({"count": count})
 
     @check_method(RequestMethod.PUT)
     @authenticate
     @authorize("edit")
     async def update(self, request: RequestCollection) -> Response:
         collection = request.collection
         try:
             ids = unpack_id(collection.schema, request.pks)
         except (FieldValidatorException, CollectionResourceException) as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         if request.body and "data" in request.body and "relationships" in request.body["data"]:
             del request.body["data"]["relationships"]
 
         schema = JsonApiSerializer.get(collection)
         try:
             data: RecordsDataAlias = schema().load(request.body)  # type: ignore
         except JsonApiException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
         try:
             RecordValidator.validate(cast(Collection, collection), data)
         except RecordValidatorException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         trees: List[ConditionTree] = [ConditionTreeFactory.match_ids(collection.schema, [ids])]
         scope_tree = await self.permission.get_scope(request)
         if scope_tree:
             trees.append(scope_tree)
 
         filter = Filter({"condition_tree": ConditionTreeFactory.intersect(trees)})
@@ -256,38 +264,39 @@
         projection = ProjectionFactory.all(cast(Collection, collection))
         records = await collection.list(request.user, PaginatedFilter.from_base_filter(filter), projection)
 
         schema = JsonApiSerializer.get(collection)
         try:
             dumped: Dict[str, Any] = schema(projections=projection).dump(records[0])  # type: ignore
         except JsonApiException as e:
-            return build_client_error_response([str(e)])
+            return HttpResponseBuilder.build_client_error_response([e])
 
-        return build_success_response(dumped)
+        return HttpResponseBuilder.build_success_response(dumped)
 
     @check_method(RequestMethod.DELETE)
     @authenticate
     @authorize("delete")
     async def delete(self, request: RequestCollection):
         collection = request.collection
         try:
             ids = unpack_id(collection.schema, request.pks)
         except (FieldValidatorException, CollectionResourceException) as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         await self._delete(request, [ids])
-        return build_no_content_response()
+        return HttpResponseBuilder.build_no_content_response()
 
     @check_method(RequestMethod.DELETE)
     @authenticate
     @authorize("delete")
     async def delete_list(self, request: RequestCollection):
         ids, exclude_ids = parse_selection_ids(request)
         await self._delete(request, ids, exclude_ids)
-        return build_no_content_response()
+        return HttpResponseBuilder.build_no_content_response()
 
     async def _delete(self, request: RequestCollection, ids: List[CompositeIdAlias], exclude_ids: bool = False):
         selected_ids = ConditionTreeFactory.match_ids(request.collection.schema, ids)
         if exclude_ids:
             selected_ids = selected_ids.inverse()
         trees = [selected_ids]
         query_param_condition_tree = parse_condition_tree(request)
```

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/crud_related.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/crud_related.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import sys
-
-from forestadmin.agent_toolkit.utils.csv import Csv, CsvException
+from typing import Any, Dict, List, Union, cast
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     import zoneinfo
 else:
     from backports import zoneinfo
 
-from typing import Any, Dict, List, Union, cast
-
+from forestadmin.agent_toolkit.forest_logger import ForestLogger
 from forestadmin.agent_toolkit.resources.collections import BaseCollectionResource
 from forestadmin.agent_toolkit.resources.collections.decorators import authenticate, authorize, check_method
 from forestadmin.agent_toolkit.resources.collections.exceptions import CollectionResourceException
 from forestadmin.agent_toolkit.resources.collections.filter import (
     build_filter,
     build_paginated_filter,
     parse_condition_tree,
@@ -25,26 +23,20 @@
 )
 from forestadmin.agent_toolkit.resources.collections.requests import (
     RequestCollectionException,
     RequestRelationCollection,
 )
 from forestadmin.agent_toolkit.services.serializers import DumpedResult, add_search_metadata
 from forestadmin.agent_toolkit.services.serializers.json_api import JsonApiException, JsonApiSerializer
-from forestadmin.agent_toolkit.utils.context import (
-    Request,
-    RequestMethod,
-    Response,
-    build_client_error_response,
-    build_csv_response,
-    build_no_content_response,
-    build_success_response,
-)
+from forestadmin.agent_toolkit.utils.context import HttpResponseBuilder, Request, RequestMethod, Response
+from forestadmin.agent_toolkit.utils.csv import Csv, CsvException
 from forestadmin.agent_toolkit.utils.id import unpack_id
 from forestadmin.datasource_toolkit.collections import Collection
 from forestadmin.datasource_toolkit.datasources import DatasourceException
+from forestadmin.datasource_toolkit.exceptions import ForestException
 from forestadmin.datasource_toolkit.interfaces.fields import (
     Operator,
     is_many_to_many,
     is_many_to_one,
     is_one_to_many,
     is_one_to_one,
 )
@@ -64,27 +56,30 @@
 
 class CrudRelatedResource(BaseCollectionResource):
     async def dispatch(self, request: Request, method_name: LiteralMethod) -> Response:
         method = getattr(self, method_name)
         try:
             request_collection = RequestRelationCollection.from_request(request, self.datasource)
         except RequestCollectionException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
         return await method(request_collection)
 
     @authenticate
     @authorize("browse")
     @check_method(RequestMethod.GET)
     async def list(self, request: RequestRelationCollection) -> Response:
         if not (is_one_to_many(request.relation) or is_many_to_many(request.relation)):
-            return build_client_error_response(["🌳🌳🌳Unhandled relation type"])
+            ForestLogger.log("error", "Unhandled relation type")
+            return HttpResponseBuilder.build_client_error_response([ForestException("Unhandled relation type")])
         try:
             ids = unpack_id(request.collection.schema, request.pks)
         except (FieldValidatorException, CollectionResourceException) as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
         scope_tree = await self.permission.get_scope(request, request.foreign_collection)
         paginated_filter = build_paginated_filter(request, scope_tree)
         projection = parse_projection_with_pks(request)
         records = await CollectionUtils.list_relation(
             request.user,
             cast(Collection, request.collection),
             ids,
@@ -93,80 +88,91 @@
             paginated_filter,
             projection,
         )
         schema = JsonApiSerializer.get(request.foreign_collection)
         try:
             dumped: DumpedResult = schema(projections=projection).dump(records, many=True)  # type: ignore
         except JsonApiException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         if paginated_filter.search:
             dumped = add_search_metadata(dumped, paginated_filter.search)
 
-        return build_success_response(cast(Dict[str, Any], dumped))
+        return HttpResponseBuilder.build_success_response(cast(Dict[str, Any], dumped))
 
     @authenticate
     @authorize("browse")
     @authorize("export")
     @check_method(RequestMethod.GET)
     async def csv(self, request: RequestRelationCollection) -> Response:
         if not (is_one_to_many(request.relation) or is_many_to_many(request.relation)):
-            return build_client_error_response(["🌳🌳🌳Unhandled relation type"])
+            ForestLogger.log("error", "Unhandled relation type")
+            return HttpResponseBuilder.build_client_error_response([ForestException("Unhandled relation type")])
         try:
             ids = unpack_id(request.collection.schema, request.pks)
         except (FieldValidatorException, CollectionResourceException) as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
         scope_tree = await self.permission.get_scope(request, request.foreign_collection)
         paginated_filter = build_paginated_filter(request, scope_tree)
         try:
             projection = parse_projection_with_pks(request)
         except DatasourceException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
         records = await CollectionUtils.list_relation(
             request.user,
             cast(Collection, request.collection),
             ids,
             cast(Collection, request.foreign_collection),
             request.relation,
             paginated_filter,
             projection,
         )
 
         try:
             csv_str = Csv.make_csv(records, projection)
         except CsvException as e:
-            return build_client_error_response([str(e)])
-        return build_csv_response(csv_str, f"{request.query.get('filename', request.collection.name)}.csv")
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
+        return HttpResponseBuilder.build_csv_response(
+            csv_str, f"{request.query.get('filename', request.collection.name)}.csv"
+        )
 
     @authenticate
     @authorize("edit")
     @check_method(RequestMethod.POST)
     async def add(self, request: RequestRelationCollection) -> Response:
         try:
             parent_ids = unpack_id(request.collection.schema, request.pks)
         except (FieldValidatorException, CollectionResourceException) as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         if (
             not request.body
             or "data" not in request.body
             or len(request.body["data"]) == 0
             or not request.body["data"][0].get("id")
             # TODO: again another hardcoded "id" # SchemaUtils.get_primary_keys(schema)
         ):
-            return build_client_error_response(["🌳🌳🌳missing target's id"])
+            ForestLogger.log("error", "missing target's id")
+            return HttpResponseBuilder.build_client_error_response([ForestException("missing target's id")])
 
         try:
             # TODO: again another hardcoded "id" # SchemaUtils.get_primary_keys(schema)
             targeted_relation_ids = unpack_id(request.foreign_collection.schema, request.body["data"][0]["id"])
         except (FieldValidatorException, CollectionResourceException) as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         if not (is_one_to_many(request.relation) or is_many_to_many(request.relation)):
-            return build_client_error_response(["🌳🌳🌳Unhandled relation type"])
+            ForestLogger.log("error", "Unhandled relation type")
+            return HttpResponseBuilder.build_client_error_response([ForestException("Unhandled relation type")])
 
         pks = SchemaUtils.get_primary_keys(request.foreign_collection.schema)[0]
         value = await CollectionUtils.get_value(
             request.user, cast(Collection, request.foreign_collection), targeted_relation_ids, pks
         )
         if is_one_to_many(request.relation):
             return await self._associate_one_to_many(request, parent_ids, value)
@@ -176,67 +182,74 @@
     @authenticate
     @authorize("edit")
     @check_method(RequestMethod.PUT)
     async def update_list(self, request: RequestRelationCollection) -> Response:
         try:
             parent_id = unpack_id(request.collection.schema, request.pks)
         except (FieldValidatorException, CollectionResourceException) as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
         if not request.body or not request.body.get("data") or "id" not in request.body["data"]:
-            return build_client_error_response(["🌳🌳🌳Relation id is missing"])
+            ForestLogger.log("error", "Relation id is missing")
+            return HttpResponseBuilder.build_client_error_response([ForestException("Relation id is missing")])
         try:
             linked_id = unpack_id(request.foreign_collection.schema, request.body["data"]["id"])
         except (FieldValidatorException, CollectionResourceException) as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         if is_many_to_one(request.relation) or is_one_to_one(request.relation):
             if is_many_to_one(request.relation):
                 meth = self._update_many_to_one
             else:
                 meth = self._update_one_to_one
 
             try:
                 await meth(request, parent_id, linked_id, request.user.timezone)
             except (CollectionResourceException, DatasourceException) as e:
-                return build_client_error_response([str(e)])
-            return build_no_content_response()
-        return build_client_error_response(["🌳🌳🌳Unhandled relation type"])
+                ForestLogger.log("exception", e)
+                return HttpResponseBuilder.build_client_error_response([e])
+            return HttpResponseBuilder.build_no_content_response()
+        ForestLogger.log("error", "Unhandled relation type")
+        return HttpResponseBuilder.build_client_error_response([ForestException("Unhandled relation type")])
 
     @authenticate
     @authorize("browse")
     @check_method(RequestMethod.GET)
     async def count(self, request: RequestRelationCollection) -> Response:
         if request.foreign_collection.schema["countable"] is False:
-            return build_success_response({"meta": {"count": "deactivated"}})
+            return HttpResponseBuilder.build_success_response({"meta": {"count": "deactivated"}})
 
         try:
             parent_id = unpack_id(request.collection.schema, request.pks)
         except (FieldValidatorException, CollectionResourceException) as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
         scope_tree = await self.permission.get_scope(request, request.foreign_collection)
         filter = build_filter(request, scope_tree)
         aggregation = Aggregation({"operation": "Count"})
 
         result = await CollectionUtils.aggregate_relation(
             request.user, cast(Collection, request.collection), parent_id, request.relation_name, filter, aggregation
         )
         try:
             count = result[0]["value"]
         except IndexError:
             count = 0
-        return build_success_response({"count": count})
+        return HttpResponseBuilder.build_success_response({"count": count})
 
     @authenticate
     @authorize("delete")
     @check_method(RequestMethod.DELETE)
     async def delete_list(self, request: RequestRelationCollection) -> Response:
         try:
             parent_ids = unpack_id(request.collection.schema, request.pks)
         except (FieldValidatorException, CollectionResourceException) as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         delete_mode = False
         if request.query:
             delete_mode = bool(request.query.get("delete", False))
 
         filter = await self.get_base_fk_filter(request)
 
@@ -244,62 +257,68 @@
             if is_one_to_many(request.relation):
                 meth = self._delete_one_to_many
             else:
                 meth = self._delete_many_to_many
             try:
                 await meth(request, parent_ids, delete_mode, filter)
             except (DatasourceException, CollectionResourceException) as e:
-                return build_client_error_response([str(e)])
-            return build_no_content_response()
-        return build_client_error_response(["🌳🌳🌳Unhandled relation type"])
+                ForestLogger.log("exception", e)
+                return HttpResponseBuilder.build_client_error_response([e])
+            return HttpResponseBuilder.build_no_content_response()
+
+        ForestLogger.log("error", "Unhandled relation type")
+        return HttpResponseBuilder.build_client_error_response([ForestException("Unhandled relation type")])
 
     async def _associate_one_to_many(
         self, request: RequestRelationCollection, parent_ids: CompositeIdAlias, id_value: Union[str, int]
     ) -> Response:
         if not is_one_to_many(request.relation):
-            return build_client_error_response(["🌳🌳🌳Unhandled relation type"])
+            return HttpResponseBuilder.build_client_error_response([ForestException("Unhandled relation type")])
         scope_tree = await self.permission.get_scope(request, request.foreign_collection)
         filter = build_filter(request, scope_tree)
         trees: List[ConditionTree] = [
             ConditionTreeLeaf(request.relation["origin_key_target"], Operator.EQUAL, id_value),
         ]
         if filter.condition_tree:
             trees.append(filter.condition_tree)
         filter.condition_tree = ConditionTreeFactory.intersect(trees)
         value = await CollectionUtils.get_value(
             request.user, cast(Collection, request.collection), parent_ids, request.relation["origin_key_target"]
         )
         try:
             await request.foreign_collection.update(request.user, filter, {f"{request.relation['origin_key']}": value})
         except DatasourceException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
         else:
-            return build_no_content_response()
+            return HttpResponseBuilder.build_no_content_response()
 
     async def _associate_many_to_many(
         self, request: RequestRelationCollection, parent_ids: CompositeIdAlias, foreign_id_value: Union[str, int]
     ):
         if not is_many_to_many(request.relation):
-            return build_client_error_response(["🌳🌳🌳Unhandled relation type"])
+            ForestLogger.log("error", "Unhandled relation type")
+            return HttpResponseBuilder.build_client_error_response([ForestException("Unhandled relation type")])
         id = SchemaUtils.get_primary_keys(request.collection.schema)
         origin_id_value = await CollectionUtils.get_value(
             request.user, cast(Collection, request.collection), parent_ids, id[0]
         )
 
         record = {
             f"{request.relation['origin_key']}": origin_id_value,
             f"{request.relation['foreign_key']}": foreign_id_value,
         }
         through_collection = request.collection.datasource.get_collection(request.relation["through_collection"])
         try:
             await through_collection.create(request.user, [record])
         except DatasourceException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
         else:
-            return build_no_content_response()
+            return HttpResponseBuilder.build_no_content_response()
 
     async def get_base_fk_filter(self, request: RequestRelationCollection):
         ids, exclude_ids = parse_selection_ids(request)
 
         if len(ids) == 0 and not exclude_ids:
             raise CollectionResourceException("Unable to unpack the id")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/decorators.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from forestadmin.agent_toolkit.resources.collections import BaseCollectionResource
 from forestadmin.agent_toolkit.resources.collections.filter import parse_timezone
 from forestadmin.agent_toolkit.resources.collections.requests import RequestCollection
 from forestadmin.agent_toolkit.services.permissions import PermissionServiceException
 from forestadmin.agent_toolkit.utils.context import (
     FileResponse,
+    HttpResponseBuilder,
     Request,
     RequestMethod,
     Response,
     User,
-    build_method_not_allowed_response,
 )
 from jose import JWTError, jwt
 
 BoundRequest = TypeVar("BoundRequest", bound=Request)
 BoundResource = TypeVar("BoundResource", bound=BaseCollectionResource)
 BoundRequestCollection = TypeVar("BoundRequestCollection", bound=RequestCollection)
 
@@ -69,13 +69,13 @@
     return wrapper
 
 
 def check_method(method: RequestMethod):
     def wrapper(fn: Callable[["BoundResource", BoundRequestCollection], Awaitable[Union[FileResponse, Response]]]):
         async def wrapped(self: "BoundResource", request: BoundRequestCollection) -> Union[FileResponse, Response]:
             if request.method != method:
-                return build_method_not_allowed_response()
+                return HttpResponseBuilder.build_method_not_allowed_response()
             return await fn(self, request)
 
         return wrapped
 
     return wrapper
```

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/filter.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/filter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/requests.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/collections/stats.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/collections/stats.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,26 +6,21 @@
 else:
     from typing_extensions import Literal
 
 from typing import Any, Dict, List, Union, cast
 from uuid import uuid1
 
 import pandas as pd
+from forestadmin.agent_toolkit.forest_logger import ForestLogger
 from forestadmin.agent_toolkit.resources.collections import BaseCollectionResource
 from forestadmin.agent_toolkit.resources.collections.decorators import authenticate, check_method
 from forestadmin.agent_toolkit.resources.collections.filter import build_filter
 from forestadmin.agent_toolkit.resources.collections.requests import RequestCollection, RequestCollectionException
-from forestadmin.agent_toolkit.utils.context import (
-    FileResponse,
-    Request,
-    RequestMethod,
-    Response,
-    build_client_error_response,
-    build_success_response,
-)
+from forestadmin.agent_toolkit.utils.context import FileResponse, HttpResponseBuilder, Request, RequestMethod, Response
+from forestadmin.datasource_toolkit.exceptions import ForestException
 from forestadmin.datasource_toolkit.interfaces.fields import Column, PrimitiveType
 from forestadmin.datasource_toolkit.interfaces.query.aggregation import Aggregation
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.base import ConditionTree
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.branch import Aggregator, ConditionTreeBranch
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.nodes.leaf import ConditionTreeLeaf
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.transforms.time import Frequency
 from forestadmin.datasource_toolkit.interfaces.query.filter.factory import FilterFactory
@@ -47,24 +42,29 @@
             "Leaderboard": self.leader_board,
         }[type]
 
     async def dispatch(self, request: Request, method_name: Literal["add"]) -> Union[Response, FileResponse]:
         try:
             request_collection = RequestCollection.from_request(request, self.datasource)
         except RequestCollectionException as e:
-            return build_client_error_response([str(e)])
+            ForestLogger.log("exception", e)
+            return HttpResponseBuilder.build_client_error_response([e])
 
         try:
             meth = self.stats_method(request_collection.body["type"])  # type: ignore
         except KeyError:
-            return build_client_error_response(
-                [f"Unknown stats type {request_collection.body.get('type')}"]  # type: ignore
+            ForestLogger.log("exception", f"Unknown stats type {request_collection.body.get('type')}")
+            return HttpResponseBuilder.build_client_error_response(
+                [ForestException(f"Unknown stats type {request_collection.body.get('type')}")]  # type: ignore
             )
         except TypeError:
-            return build_client_error_response(["Missing stats type in request body"])
+            ForestLogger.log("exception", "Missing stats type in request body")
+            return HttpResponseBuilder.build_client_error_response(
+                [ForestException("Missing stats type in request body")]
+            )
         return await meth(request_collection)
 
     @check_method(RequestMethod.POST)
     @authenticate
     async def value(self, request: RequestCollection) -> Response:
         current_filter = await self._get_filter(request)
         result = {
@@ -180,15 +180,17 @@
         rows = await request.collection.aggregate(request.user, current_filter, aggregation, int(limit))
         results: List[Dict[str, Union[str, int]]] = []
         for row in rows:
             results.append({"key": row["group"][label_field], "value": row["value"]})
         return self._build_success_response(results)
 
     def _build_success_response(self, result: Any) -> Response:
-        return build_success_response({"data": {"id": uuid1().hex, "type": "stats", "attributes": {"value": result}}})
+        return HttpResponseBuilder.build_success_response(
+            {"data": {"id": uuid1().hex, "type": "stats", "attributes": {"value": result}}}
+        )
 
     def _with_count_previous(self, tree: ConditionTree):
         use_interval_res: List[bool] = []
 
         def _use_interval_res(tree: ConditionTree) -> None:
             if isinstance(tree, ConditionTreeLeaf):
                 use_interval_res.append(tree.use_interval_operator)
```

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/resources/security/resources.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/resources/security/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/permissions/__init__.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/serializers/__init__.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/services/serializers/json_api.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/services/serializers/json_api.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/authentication.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/authentication.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/csv.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/csv.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/action_values.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/action_values.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/emitter.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/emitter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/filterable.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/filterable.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/type.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/type.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/forest_schema/validation.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/forest_schema/validation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/http.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/http.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/id.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/id.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/forestadmin/agent_toolkit/utils/token.py` & `forestadmin_agent_toolkit-1.0.0b5/forestadmin/agent_toolkit/utils/token.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.0.0b4/pyproject.toml` & `forestadmin_agent_toolkit-1.0.0b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-toolkit"
-version = "1.0.0-beta.4"
+version = "1.0.0-beta.5"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.poetry.dependencies]
@@ -16,15 +16,15 @@
 typing-extensions = ">=4.2.0, <5.0"
 tzdata = "~2022.6"
 aiohttp = "~=3.8"
 oic = "~=1.4"
 python-jose = ">=3.3, <4.0"
 cachetools = "~=5.2"
 marshmallow-jsonapi = ">=0.24.0, <1.0"
-forestadmin-datasource-toolkit = "^1.0.0-beta.4"
+forestadmin-datasource-toolkit = "^1.0.0-beta.5"
 [[tool.poetry.dependencies.pandas]]
 version = "<=1.1.5"
 python = "<3.7.1"
 
 [[tool.poetry.dependencies.pandas]]
 version = ">=1.3.4,<=1.3.5"
 python = ">=3.7.1,<3.8"
```

### Comparing `forestadmin_agent_toolkit-1.0.0b4/PKG-INFO` & `forestadmin_agent_toolkit-1.0.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: forestadmin-agent-toolkit
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8,<4.0)
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: cachetools (>=5.2,<6.0)
-Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.4,<2.0.0)
+Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.5,<2.0.0)
 Requires-Dist: marshmallow-jsonapi (>=0.24.0,<1.0)
 Requires-Dist: oic (>=1.4,<2.0)
 Requires-Dist: pandas (<=1.1.5) ; python_full_version < "3.7.1"
 Requires-Dist: pandas (>=1.3.4,<=1.3.5) ; python_full_version >= "3.7.1" and python_version < "3.8"
 Requires-Dist: pandas (>=1.4.0) ; python_version >= "3.8"
 Requires-Dist: python-jose (>=3.3,<4.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0)
```

