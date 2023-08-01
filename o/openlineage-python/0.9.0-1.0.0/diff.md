# Comparing `tmp/openlineage-python-0.9.0.tar.gz` & `tmp/openlineage_python-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openlineage-python-0.9.0.tar", last modified: Fri Jun  3 23:03:19 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `openlineage-python-0.9.0.tar` & `openlineage_python-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,41 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3679 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2801 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      185 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2054 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      272 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4732 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/facet.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1339 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/run.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1270 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/serde.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      975 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      513 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/console.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4654 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/factory.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3939 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/http.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1689 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/kafka.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      523 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/noop.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      979 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/transport/transport.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1219 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage/client/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage_python.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3679 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage_python.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      755 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage_python.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage_python.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage_python.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      194 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage_python.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/openlineage_python.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      502 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      954 2022-06-03 23:03:19.000000 openlineage-python-0.9.0/setup.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tox.ini
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/__init__.py
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/client.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/constants.py
+-rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/facet.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/py.typed
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/run.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/serde.py
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/utils.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/transport/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/transport/console.py
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/transport/factory.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/transport/file.py
+-rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/transport/http.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/transport/kafka.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/transport/noop.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/openlineage/client/transport/transport.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/nominal_time_without_end.json
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/serde_example_dataset_event.json
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/serde_example_job_event.json
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/serde_example_run_event.json
+-rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/test_client.py
+-rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/test_events.py
+-rw-r--r--   0        0        0    14173 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/test_facet.py
+-rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/test_factory.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/test_file.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/test_http.py
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/test_kafka.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/transport.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/config/config.yml
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/config/exact_filter.yml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/config/http.yml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/config/openlineage.yml
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/tests/config/regex_filter.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/.gitignore
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/README.md
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 openlineage_python-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `openlineage-python-0.9.0/PKG-INFO` & `openlineage_python-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,79 @@
-Metadata-Version: 2.1
-Name: openlineage-python
-Version: 0.9.0
-Summary: OpenLineage Python Client
-Home-page: UNKNOWN
-Author: OpenLineage
-License: UNKNOWN
-Description: # OpenLineage-python
-        
-        To install from source, run:
-        
-        ```bash
-        $ python setup.py install
-        ```
-        
-        ## Configuration
-        ### Config file
-        
-        Main way of configuring OpenLineage Client is by yaml file, which contains all the
-        details of how to connect to your OpenLineage backend. 
-        
-        Config file is located by
-        1) looking at `OPENLINEAGE_CONFIG` environment variable
-        2) looking for file `openlineage.yml` at current working directory
-        3) looking for file `openlineage.yml` at `$HOME/.openlineage` directory.
-        
-        Different ways of connecting to OpenLineage backend are supported 
-        by standarized `Transport` interface.  
-        This is example config that specifies `http` transport:
-        
-        ```yaml
-        transport:
-          type: "http"
-          url: "https://backend:5000"
-          auth:
-            type: "api_key"
-            api_key: "f048521b-dfe8-47cd-9c65-0cb07d57591e"
-        ```
-        
-        `type` property is required. It can be one of the build-in transports, or custom one.
-        There are three build-in transports, `http`, `kafka` or `console`. 
-        Custom transports `type` is fully qualified class name that can be imported.
-        
-        Rest of the properties are defined by particular transport.  
-        Specification of build-in ones are below.
-        
-        #### HTTP
-        
-        * `url` - required string parameter specifying
-        * `timeout` - optional float parameter specifying timeout when sending event. By default 5 seconds.
-        * `verify` optional boolean attribute specifying if client should verify TLS certificates of backend. By default true.
-        * `auth` - optional dictionary specifying authentication options. Type property is required.
-            * `type`: required property if auth dictionary is set. Set to `api_key` or to fully qualified class name of your TokenProvider
-            * `api_key`: if `api_key` type is set, it sets value at `Authentication` HTTP header as `Bearer` 
-        
-        #### Kafka
-        
-        * `config` - required string parameter - dictionary that contains Kafka producer config as in [Kafka producer config](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html#kafka-client-configuration)
-        * `topic` - required string parameter - topic on what events will be send
-        * `flush` - optional boolean parameter - if it's set to True, then Kafka will flush after each event. By default set to true.
-        
-        
-        ### Custom transport
-        
-        To implement custom transport, follow instructions in `openlineage/client/transport/transport.py` file.
-        
-        ### Config as env vars
-        
-        If there is no config file found, OpenLineage client looks at environment variables.  
-        This way of configuring supports only `http` transport, and only subset of it's config.
-        
-        * `OPENLINEAGE_URL` - point to service which will consume OpenLineage events
-        * `OPENLINEAGE_API_KEY` - set if consumer of OpenLineage events requires `Bearer` authentication key
-        
-        `OPENLINEAGE_URL` and `OPENLINEAGE_API_KEY` can also be set up manually when creating client instance.
-        
-Keywords: openlineage
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: kafka
-Provides-Extra: dev
+# OpenLineage-python
+
+To install from source, run:
+
+```bash
+$ python -m pip install .
+```
+
+## Configuration
+### Config file
+
+The most common way to configure the OpenLineage Client is by `.yaml` file, which contains all the
+details of how to connect to your OpenLineage backend.
+
+The config file is located by:
+1) looking at the `OPENLINEAGE_CONFIG` environment variable
+2) looking for the `openlineage.yml` file in the current working directory
+3) looking for the `openlineage.yml` file in the `$HOME/.openlineage` directory.
+
+Different ways of connecting to OpenLineage backend are supported
+by the standarized `Transport` interface.
+This is an example config for specifying `http` transport:
+
+```yaml
+transport:
+  type: "http"
+  url: "https://backend:5000"
+  auth:
+    type: "api_key"
+    api_key: "f048521b-dfe8-47cd-9c65-0cb07d57591e"
+```
+
+The `type` property is required. It can be one of the built-in transports or a custom one.
+There are four built-in transports, `http`, `kafka`, `console` and `file`.
+Custom transports `type` is a fully qualified class name that can be imported.
+
+The rest of the properties are defined by the particular transport.
+Specifications for the built-in options are below.
+
+#### HTTP
+
+* `url` - required string parameter.
+* `endpoint` - optional string parameter specifying the endpoint to which events are sent. By default `api/v1/lineage`.
+* `timeout` - optional float parameter specifying the timeout when sending events. By default 5 seconds.
+* `verify` optional boolean attribute specifying if the client should verify TLS certificates of the backend. By default true.
+* `auth` - optional dictionary specifying authentication options. The type property is required.
+    * `type`: required property if an auth dictionary is set. Set to `api_key` or to the fully qualified class name of your TokenProvider.
+    * `api_key`: if `api_key` type is set, it sets value at `Authentication` HTTP header as `Bearer`.
+
+#### Kafka
+
+For KafkaTransport, `confluent-kafka` needs to be installed.
+You can also install `pip install openlineage-python[kafka]`
+
+* `config` - required string parameter. A dictionary that contains a Kafka producer config as in [Kafka producer config](https://docs.confluent.io/platform/current/clients/confluent-kafka-python/html/index.html#kafka-client-configuration).
+* `topic` - required string parameter. The topic on what events will be sent.
+* `flush` - optional boolean parameter. If set to True, Kafka will flush after each event. By default true.
+
+#### File
+
+* `log_file_path` - required string parameter specifying the path of the file (if `append` is true a file path is expected, otherwise a file prefix is expected).
+* `append` - optional boolean parameter. If set to True, each event will be appended to a single file (log_file_path), otherwise, all event would be written separatly in distinct files suffixed by a timestring. By default false.
+
+### Custom transport
+
+To implement a custom transport, follow the instructions in the `openlineage/client/transport/transport.py` file.
+
+### Config as env vars
+
+If there is no config file found, the OpenLineage client looks at environment variables.
+This way of configuring the client supports only `http` transport, and only a subset of its config.
+
+* `OPENLINEAGE_URL` - point to the service that will consume OpenLineage events.
+* `OPENLINEAGE_API_KEY` - set if the consumer of OpenLineage events requires a `Bearer` authentication key.
+
+`OPENLINEAGE_URL` and `OPENLINEAGE_API_KEY` can also be set up manually when creating a client instance.
+
+#### Logging level
+In addition to conventional logging approaches, the OpenLineage client library provides an alternative way of configuring its logging behavior. By setting the `OPENLINEAGE_CLIENT_LOGGING` environment variable, you can establish the logging level for the `openlineage.client` and its child modules.
```

### Comparing `openlineage-python-0.9.0/openlineage/client/serde.py` & `openlineage_python-1.0.0/openlineage/client/serde.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,58 @@
-# SPDX-License-Identifier: Apache-2.0.
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
 
 import json
+import logging
+import sys
 from enum import Enum
-from typing import List, Dict
+from typing import Any, Dict, List, cast
 
 import attr
 
+log = logging.getLogger(__name__)
+
 try:
     import numpy
 except ImportError:
-    numpy = None
+    log.warning("ImportError occurred when trying to import numpy module.")
 
 
 class Serde:
     @classmethod
-    def remove_nulls_and_enums(cls, obj):
+    def remove_nulls_and_enums(cls, obj: Any) -> Any:  # noqa: ANN401
         if isinstance(obj, Enum):
             return obj.value
         if isinstance(obj, Dict):
-            return dict(filter(
-                lambda x: x[1] is not None,
-                {k: cls.remove_nulls_and_enums(v) for k, v in obj.items()}.items()
-            ))
+            return dict(
+                filter(
+                    lambda x: x[1] is not None,
+                    {k: cls.remove_nulls_and_enums(v) for k, v in obj.items()}.items(),
+                ),
+            )
         if isinstance(obj, List):
-            return list(filter(lambda x: x is not None and (isinstance(x, dict) and x != {}), [
-                cls.remove_nulls_and_enums(v) for v in obj if v is not None
-            ]))
+            return list(
+                filter(
+                    lambda x: x is not None and (isinstance(x, dict) and x != {}),
+                    [cls.remove_nulls_and_enums(v) for v in obj if v is not None],
+                ),
+            )
 
         # Pandas can use numpy.int64 object
-        if numpy and isinstance(obj, numpy.int64):
+        if "numpy" in sys.modules and isinstance(obj, numpy.int64):
             return int(obj)
         return obj
 
     @classmethod
-    def to_dict(cls, obj):
+    def to_dict(cls, obj: Any) -> dict[Any, Any]:  # noqa: ANN401
         if not isinstance(obj, dict):
             obj = attr.asdict(obj)
-        return cls.remove_nulls_and_enums(obj)
+        return cast(Dict[Any, Any], cls.remove_nulls_and_enums(obj))
 
     @classmethod
-    def to_json(cls, obj):
+    def to_json(cls, obj: Any) -> str:  # noqa: ANN401
         return json.dumps(
             cls.to_dict(obj),
             sort_keys=True,
-            default=lambda o: f"<<non-serializable: {type(o).__qualname__}>>"
+            default=lambda o: f"<<non-serializable: {type(o).__qualname__}>>",
         )
```

### Comparing `openlineage-python-0.9.0/openlineage/client/transport/http.py` & `openlineage_python-1.0.0/openlineage/client/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,123 +1,128 @@
-# SPDX-License-Identifier: Apache-2.0.
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
+from __future__ import annotations
+
 import logging
-from urllib.parse import urljoin
+import os
+from typing import TYPE_CHECKING, Any, TypeVar, Union
 
 import attr
 
-from typing import Optional, Dict
-
-from requests import Session
-from requests.adapters import HTTPAdapter
-from urllib3.util import parse_url
-
-from openlineage.client.run import RunEvent
+from openlineage.client.filter import Filter, create_filter
 from openlineage.client.serde import Serde
-from openlineage.client.transport.transport import Config, Transport
-from openlineage.client.utils import get_only_specified_fields, try_import_subclass_from_string
-
-log = logging.getLogger(__name__)
+from openlineage.client.utils import load_config
 
-
-class TokenProvider:
-    def __init__(self, config: Dict):
-        pass
-
-    def get_bearer(self) -> Optional[str]:
-        return None
-
-
-class ApiKeyTokenProvider(TokenProvider):
-    def __init__(self, config: Dict):
-        self.api_key = config['api_key']
-
-    def get_bearer(self) -> Optional[str]:
-        return f"Bearer {self.api_key}"
-
-
-def create_token_provider(auth: Dict) -> TokenProvider:
-    if 'type' in auth:
-        if auth['type'] == 'api_key':
-            return ApiKeyTokenProvider(auth)
-        try:
-            clazz = try_import_subclass_from_string(auth['type'], TokenProvider)
-            return clazz(auth)
-        except TypeError:
-            pass  # already logged
-    return TokenProvider({})
+if TYPE_CHECKING:
+    from requests import Session
+    from requests.adapters import HTTPAdapter
+
+from openlineage.client.run import DatasetEvent, JobEvent, RunEvent
+from openlineage.client.transport import Transport, TransportFactory, get_default_factory
+from openlineage.client.transport.http import HttpConfig, HttpTransport
 
 
 @attr.s
-class HttpConfig(Config):
-    url: str = attr.ib()
+class OpenLineageClientOptions:
     timeout: float = attr.ib(default=5.0)
-    # check TLS certificates
     verify: bool = attr.ib(default=True)
-    auth: TokenProvider = attr.ib(factory=lambda: TokenProvider({}))
-    # not set by TransportFactory
-    session: Optional[Session] = attr.ib(factory=Session)
-    # not set by TransportFactory
-    adapter: Optional[HTTPAdapter] = attr.ib(default=None)
+    api_key: str = attr.ib(default=None)
+    adapter: HTTPAdapter = attr.ib(default=None)
 
-    @classmethod
-    def from_dict(cls, params: dict) -> 'HttpConfig':
-        if 'url' not in params:
-            raise RuntimeError("`url` key not passed to HttpConfig")
-        specified_dict = get_only_specified_fields(cls, params)
-        specified_dict['auth'] = create_token_provider(specified_dict.get('auth', {}))
-        return cls(**specified_dict)
-
-    @classmethod
-    def from_options(cls, url: str, options, session: Optional[Session]) -> 'HttpConfig':
-        return cls(
-            url=url,
-            timeout=options.timeout,
-            verify=options.verify,
-            auth=ApiKeyTokenProvider({"api_key": options.api_key})
-            if options.api_key else TokenProvider({}),
-            session=session if session else Session(),
-            adapter=options.adapter
-        )
 
+log = logging.getLogger(__name__)
+_T = TypeVar("_T", bound="OpenLineageClient")
 
-class HttpTransport(Transport):
-    kind = "http"
-    config = HttpConfig
-
-    def __init__(self, config: HttpConfig):
-        url = config.url.strip()
-        try:
-            parsed = parse_url(url)
-            if not (parsed.scheme and parsed.netloc):
-                raise ValueError(f"Need valid url for OpenLineageClient, passed {url}")
-        except Exception as e:
-            raise ValueError(f"Need valid url for OpenLineageClient, passed {url}. Exception: {e}")
-        self.url = url
-        self.session = config.session
-        self.session.headers['Content-Type'] = 'application/json'
-        self.timeout = config.timeout
-        self.verify = config.verify
-
-        self._add_auth(config.auth)
-        if config.adapter:
-            self.set_adapter(config.adapter)
 
-    def set_adapter(self, adapter: HTTPAdapter):
-        self.session.mount(self.url, adapter)
+class OpenLineageClient:
+    def __init__(  # noqa: PLR0913
+        self,
+        url: str | None = None,
+        options: OpenLineageClientOptions | None = None,
+        session: Session | None = None,
+        transport: Transport | None = None,
+        factory: TransportFactory | None = None,
+    ) -> None:
+        # Set parent's logging level if environment variable is present
+        if "OPENLINEAGE_CLIENT_LOGGING" in os.environ:
+            logging.getLogger(__name__.rpartition(".")[0]).setLevel(
+                os.environ["OPENLINEAGE_CLIENT_LOGGING"],
+            )
+
+        if factory is None:
+            factory = get_default_factory()
+
+        # Make config ellipsis - as a guard value to not try to
+        # reload yaml each time config is referred to.
+        self._config: dict[str, dict[str, str]] | None = None
+        if url:
+            # Backwards compatibility: if URL or options is set, use old path to initialize
+            # HTTP transport.
+            if not options:
+                options = OpenLineageClientOptions()
+            self._initialize_url(url, options, session)
+        elif transport:
+            self.transport = transport
+        else:
+            transport_config = None if "transport" not in self.config else self.config["transport"]
+            self.transport = factory.create(transport_config)
+
+        self._filters: list[Filter] = []
+        if "filters" in self.config:
+            for conf in self.config["filters"]:
+                _filter = create_filter(conf)
+                if _filter:
+                    self._filters.append(_filter)
+
+    def _initialize_url(
+        self,
+        url: str,
+        options: OpenLineageClientOptions,
+        session: Session | None,
+    ) -> None:
+        self.transport = HttpTransport(
+            HttpConfig.from_options(
+                url=url,
+                options=options,
+                session=session,
+            ),
+        )
 
-    def emit(self, event: RunEvent):
-        event = Serde.to_json(event)
+    def emit(self, event: Union[RunEvent, DatasetEvent | JobEvent]) -> None:  # noqa: UP007
+        if not (isinstance(event, (RunEvent, DatasetEvent, JobEvent))):
+            msg = "`emit` only accepts RunEvent, DatasetEvent, JobEvent classes"
+            raise ValueError(msg)  # noqa: TRY004
+        if not self.transport:
+            log.error("Tried to emit OpenLineage event, but transport is not configured.")
+            return
         if log.isEnabledFor(logging.DEBUG):
-            log.debug(f"Sending openlineage event {event}")
-        resp = self.session.post(
-            urljoin(self.url, 'api/v1/lineage'),
-            event,
-            timeout=self.timeout,
-            verify=self.verify
-        )
-        resp.raise_for_status()
-        return resp
+            val = Serde.to_json(event).encode("utf-8")
+            log.debug("OpenLineageClient will emit event %s", val)
+        if self._filters and self.filter_event(event) is None:
+            return
+        if event:
+            self.transport.emit(event)
+
+    @classmethod
+    def from_environment(cls: type[_T]) -> _T:
+        # Deprecated way of creating client, use constructor or from_dict
+        return cls()
+
+    @classmethod
+    def from_dict(cls: type[_T], config: dict[str, str]) -> _T:
+        return cls(transport=get_default_factory().create(config=config))
 
-    def _add_auth(self, token_provider: TokenProvider):
-        self.session.headers.update({
-            "Authorization": token_provider.get_bearer()
-        })
+    def filter_event(
+        self,
+        event: Union[RunEvent, DatasetEvent, JobEvent],  # noqa: UP007
+    ) -> Union[RunEvent, DatasetEvent, JobEvent] | None:  # noqa: UP007
+        """Filters jobs according to config-defined events"""
+        for _filter in self._filters:
+            if isinstance(event, RunEvent) and _filter.filter_event(event) is None:
+                return None
+        return event
+
+    @property
+    def config(self) -> dict[str, Any]:
+        if self._config is None:
+            self._config = load_config()
+        return self._config
```

