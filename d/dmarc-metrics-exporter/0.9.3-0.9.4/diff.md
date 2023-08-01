# Comparing `tmp/dmarc_metrics_exporter-0.9.3.tar.gz` & `tmp/dmarc_metrics_exporter-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmarc_metrics_exporter-0.9.3.tar", max compression
+gzip compressed data, was "dmarc_metrics_exporter-0.9.4.tar", max compression
```

## Comparing `dmarc_metrics_exporter-0.9.3.tar` & `dmarc_metrics_exporter-0.9.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1073 2023-07-25 19:54:38.442700 dmarc_metrics_exporter-0.9.3/LICENSE
--rw-r--r--   0        0        0    10258 2023-07-25 19:54:38.442700 dmarc_metrics_exporter-0.9.3/README.rst
--rw-r--r--   0        0        0       22 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/__init__.py
--rw-r--r--   0        0        0      109 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/__main__.py
--rw-r--r--   0        0        0     5096 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/app.py
--rw-r--r--   0        0        0     4581 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/deserialization.py
--rw-r--r--   0        0        0      703 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/dmarc_event.py
--rw-r--r--   0        0        0     1716 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/dmarc_metrics.py
--rw-r--r--   0        0        0     2104 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/expiring_set.py
--rw-r--r--   0        0        0    13739 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/imap_client.py
--rw-r--r--   0        0        0     5784 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/imap_parser.py
--rwxr-xr-x   0        0        0     5172 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/imap_queue.py
--rw-r--r--   0        0        0     1793 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/metrics_persister.py
--rw-r--r--   0        0        0      461 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/model/__init__.py
--rw-r--r--   0        0        0     9773 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/model/dmarc_aggregate_report.py
--rw-r--r--   0        0        0        0 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/model/tests/__init__.py
--rw-r--r--   0        0        0     2990 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/model/tests/sample_data.py
--rw-r--r--   0        0        0      537 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/model/tests/test_deserialization.py
--rw-r--r--   0        0        0     5093 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/prometheus_exporter.py
--rw-r--r--   0        0        0        0 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/__init__.py
--rw-r--r--   0        0        0     2976 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/conftest.py
--rw-r--r--   0        0        0     1769 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/sample_emails.py
--rw-r--r--   0        0        0     2983 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_app.py
--rw-r--r--   0        0        0     1357 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_deserialization.py
--rw-r--r--   0        0        0     1428 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_dmarc_metrics.py
--rw-r--r--   0        0        0     3499 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_e2e.py
--rw-r--r--   0        0        0      932 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_expiring_set.py
--rw-r--r--   0        0        0    16524 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_imap_client.py
--rw-r--r--   0        0        0    10834 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_imap_parser.py
--rw-r--r--   0        0        0     4757 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_imap_queue.py
--rw-r--r--   0        0        0     1192 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_metrics_persister.py
--rw-r--r--   0        0        0     3960 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_prometheus_exporter.py
--rwxr-xr-x   0        0        0     2133 2023-07-25 19:54:38.446700 dmarc_metrics_exporter-0.9.3/pyproject.toml
--rw-r--r--   0        0        0    11550 1970-01-01 00:00:00.000000 dmarc_metrics_exporter-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-01 18:40:31.263415 dmarc_metrics_exporter-0.9.4/LICENSE
+-rw-r--r--   0        0        0    10258 2023-08-01 18:40:31.263415 dmarc_metrics_exporter-0.9.4/README.rst
+-rw-r--r--   0        0        0       22 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/__init__.py
+-rw-r--r--   0        0        0      109 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/__main__.py
+-rw-r--r--   0        0        0     5096 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/app.py
+-rw-r--r--   0        0        0     4581 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/deserialization.py
+-rw-r--r--   0        0        0      703 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/dmarc_event.py
+-rw-r--r--   0        0        0     1716 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/dmarc_metrics.py
+-rw-r--r--   0        0        0     2104 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/expiring_set.py
+-rw-r--r--   0        0        0    13710 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/imap_client.py
+-rw-r--r--   0        0        0     5784 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/imap_parser.py
+-rwxr-xr-x   0        0        0     5172 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/imap_queue.py
+-rw-r--r--   0        0        0     1793 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/metrics_persister.py
+-rw-r--r--   0        0        0      461 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/model/__init__.py
+-rw-r--r--   0        0        0     9773 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/model/dmarc_aggregate_report.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/model/tests/__init__.py
+-rw-r--r--   0        0        0     2990 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/model/tests/sample_data.py
+-rw-r--r--   0        0        0      537 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/model/tests/test_deserialization.py
+-rw-r--r--   0        0        0     5093 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/prometheus_exporter.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/__init__.py
+-rw-r--r--   0        0        0     2976 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/conftest.py
+-rw-r--r--   0        0        0     1769 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/sample_emails.py
+-rw-r--r--   0        0        0     2983 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_app.py
+-rw-r--r--   0        0        0     1357 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_deserialization.py
+-rw-r--r--   0        0        0     1428 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_dmarc_metrics.py
+-rw-r--r--   0        0        0     3499 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_e2e.py
+-rw-r--r--   0        0        0      932 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_expiring_set.py
+-rw-r--r--   0        0        0    16524 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_imap_client.py
+-rw-r--r--   0        0        0    10834 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_imap_parser.py
+-rw-r--r--   0        0        0     4757 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_imap_queue.py
+-rw-r--r--   0        0        0     1192 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_metrics_persister.py
+-rw-r--r--   0        0        0     3960 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_prometheus_exporter.py
+-rwxr-xr-x   0        0        0     2103 2023-08-01 18:40:31.267415 dmarc_metrics_exporter-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0    11500 1970-01-01 00:00:00.000000 dmarc_metrics_exporter-0.9.4/PKG-INFO
```

### Comparing `dmarc_metrics_exporter-0.9.3/LICENSE` & `dmarc_metrics_exporter-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/README.rst` & `dmarc_metrics_exporter-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/app.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/app.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/deserialization.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/deserialization.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/dmarc_event.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/dmarc_event.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/dmarc_metrics.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/dmarc_metrics.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/expiring_set.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/expiring_set.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/imap_client.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/imap_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,18 +12,17 @@
     StreamWriter,
     create_task,
     open_connection,
     wait_for,
 )
 from dataclasses import dataclass
 from enum import Enum
-from typing import Callable, Coroutine, Dict, FrozenSet, Optional, Union
+from typing import Callable, Coroutine, Dict, FrozenSet, Literal, Optional, Union
 
 from bite import parse_incremental
-from typing_extensions import Literal
 
 from .imap_parser import response as response_grammar
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
```

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/imap_parser.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/imap_parser.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/imap_queue.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/imap_queue.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/metrics_persister.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/metrics_persister.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/model/dmarc_aggregate_report.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/model/dmarc_aggregate_report.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/model/tests/sample_data.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/model/tests/sample_data.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/model/tests/test_deserialization.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/model/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/prometheus_exporter.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/conftest.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/sample_emails.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/sample_emails.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_app.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_deserialization.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_dmarc_metrics.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_dmarc_metrics.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_e2e.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_expiring_set.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_expiring_set.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_imap_client.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_imap_client.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_imap_parser.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_imap_parser.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_imap_queue.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_imap_queue.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_metrics_persister.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_metrics_persister.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/dmarc_metrics_exporter/tests/test_prometheus_exporter.py` & `dmarc_metrics_exporter-0.9.4/dmarc_metrics_exporter/tests/test_prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `dmarc_metrics_exporter-0.9.3/pyproject.toml` & `dmarc_metrics_exporter-0.9.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -15,36 +15,35 @@
 ]
 description = "Export Prometheus metrics from DMARC reports."
 keywords = ["DMARC", "DKIM", "SPF", "Prometheus"]
 license = "MIT"
 name = "dmarc-metrics-exporter"
 readme = "README.rst"
 repository = "https://github.com/jgosmann/dmarc-metrics-exporter/"
-version = "0.9.3" # Update also in __init__.py!
+version = "0.9.4" # Update also in __init__.py!
 
 [tool.poetry.scripts]
 dmarc-metrics-exporter = "dmarc_metrics_exporter.__main__:run"
 
 [tool.poetry.dependencies]
-bite-parser = "^0.2.2"
+bite-parser = "^0.2.3"
 dataclasses-serialization = "^1.3.1"
-prometheus_client = "^0.15.0"
+prometheus_client = "^0.17.1"
 python = "^3.8"
-typing-extensions = "^4.0.1"
-uvicorn = {extras = ["standard"], version = "^0.19.0"}
+uvicorn = {extras = ["standard"], version = "^0.23.2"}
 xsdata = ">=21.9"
 
 [tool.poetry.dev-dependencies]
 aiohttp = "^3.7.3"
-black = "^22.12.0"
+black = "^23.7.0"
 isort = "^5.11.4"
-mypy = "^0.991"
-pylint = "^2.15.9"
+mypy = "^1.4.1"
+pylint = "^2.16.9"
 pytest = "^7.2.0"
-pytest-asyncio = "^0.20.1"
+pytest-asyncio = "^0.21.1"
 pytest-cov = "^4.0.0"
 requests = "^2.26.0"
 types-requests = "^2.25.11"
 
 [tool.black]
 exclude = '''
 /(
```

### Comparing `dmarc_metrics_exporter-0.9.3/PKG-INFO` & `dmarc_metrics_exporter-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmarc-metrics-exporter
-Version: 0.9.3
+Version: 0.9.4
 Summary: Export Prometheus metrics from DMARC reports.
 Home-page: https://github.com/jgosmann/dmarc-metrics-exporter/
 License: MIT
 Keywords: DMARC,DKIM,SPF,Prometheus
 Author: Jan Gosmann
 Author-email: jan@hyper-world.de
 Requires-Python: >=3.8,<4.0
@@ -16,19 +16,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: bite-parser (>=0.2.2,<0.3.0)
+Requires-Dist: bite-parser (>=0.2.3,<0.3.0)
 Requires-Dist: dataclasses-serialization (>=1.3.1,<2.0.0)
-Requires-Dist: prometheus_client (>=0.15.0,<0.16.0)
-Requires-Dist: typing-extensions (>=4.0.1,<5.0.0)
-Requires-Dist: uvicorn[standard] (>=0.19.0,<0.20.0)
+Requires-Dist: prometheus_client (>=0.17.1,<0.18.0)
+Requires-Dist: uvicorn[standard] (>=0.23.2,<0.24.0)
 Requires-Dist: xsdata (>=21.9)
 Project-URL: Repository, https://github.com/jgosmann/dmarc-metrics-exporter/
 Description-Content-Type: text/x-rst
 
 .. image:: https://github.com/jgosmann/dmarc-metrics-exporter/actions/workflows/ci.yml/badge.svg
   :target: https://github.com/jgosmann/dmarc-metrics-exporter/actions/workflows/ci.yml
   :alt: CI and release pipeline
```

