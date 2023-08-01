# Comparing `tmp/astronomer_cosmos-1.0.3.tar.gz` & `tmp/astronomer_cosmos-1.0.4.tar.gz`

## Comparing `astronomer_cosmos-1.0.3.tar` & `astronomer_cosmos-1.0.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/__init__.py
--rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/config.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/constants.py
--rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/converter.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dataset.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/airflow/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/airflow/dag.py
--rw-r--r--   0        0        0     9952 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/airflow/graph.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/airflow/task_group.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/core/__init__.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/core/airflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/core/graph/__init__.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/core/graph/entities.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/__init__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/executable.py
--rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/graph.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/project.py
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/selector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/parser/__init__.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/parser/output.py
--rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/dbt/parser/project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/hooks/__init__.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/hooks/subprocess.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/operators/__init__.py
--rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/operators/base.py
--rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/operators/docker.py
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/operators/kubernetes.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/operators/lazy_load.py
--rw-r--r--   0        0        0    18147 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/operators/local.py
--rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/operators/virtualenv.py
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/__init__.py
--rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/base.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/bigquery/__init__.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/bigquery/service_account_file.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/bigquery/service_account_keyfile_dict.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/databricks/__init__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/databricks/token.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/exasol/__init__.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/exasol/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/postgres/__init__.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/postgres/user_pass.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/redshift/__init__.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/redshift/user_pass.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/snowflake/__init__.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/snowflake/user_pass.py
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/snowflake/user_privatekey.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/spark/__init__.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/spark/thrift.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/trino/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/trino/base.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/trino/certificate.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/trino/jwt.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/cosmos/profiles/trino/ldap.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/LICENSE
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/README.rst
--rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/__init__.py
+-rw-r--r--   0        0        0     7387 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/config.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/constants.py
+-rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/converter.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/dataset.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/airflow/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/airflow/dag.py
+-rw-r--r--   0        0        0     9952 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/airflow/graph.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/airflow/task_group.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/core/__init__.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/core/airflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/core/graph/__init__.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/core/graph/entities.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/dbt/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/dbt/executable.py
+-rw-r--r--   0        0        0     9861 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/dbt/graph.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/dbt/project.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/dbt/selector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/dbt/parser/__init__.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/dbt/parser/output.py
+-rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/dbt/parser/project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/hooks/__init__.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/hooks/subprocess.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/operators/__init__.py
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/operators/base.py
+-rw-r--r--   0        0        0     5345 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/operators/docker.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/operators/kubernetes.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/operators/lazy_load.py
+-rw-r--r--   0        0        0    18147 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/operators/local.py
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/operators/virtualenv.py
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/__init__.py
+-rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/base.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/bigquery/__init__.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/bigquery/service_account_file.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/bigquery/service_account_keyfile_dict.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/databricks/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/databricks/token.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/exasol/__init__.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/exasol/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/postgres/__init__.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/postgres/user_pass.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/redshift/__init__.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/redshift/user_pass.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/snowflake/__init__.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/snowflake/user_pass.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/snowflake/user_privatekey.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/spark/__init__.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/spark/thrift.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/trino/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/trino/base.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/trino/certificate.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/trino/jwt.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/cosmos/profiles/trino/ldap.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/LICENSE
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/README.rst
+-rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 astronomer_cosmos-1.0.4/PKG-INFO
```

### Comparing `astronomer_cosmos-1.0.3/cosmos/__init__.py` & `astronomer_cosmos-1.0.4/cosmos/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # type: ignore # ignores "Cannot assign to a type" MyPy error
 
 """
 Astronomer Cosmos is a library for rendering dbt workflows in Airflow.
 
 Contains dags, task groups, and operators.
 """
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 from cosmos.airflow.dag import DbtDag
 from cosmos.airflow.task_group import DbtTaskGroup
 from cosmos.constants import LoadMode, TestBehavior, ExecutionMode
 from cosmos.dataset import get_dbt_dataset
 from cosmos.operators.lazy_load import MissingPackage
 from cosmos.config import (
```

### Comparing `astronomer_cosmos-1.0.3/cosmos/config.py` & `astronomer_cosmos-1.0.4/cosmos/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,23 +112,23 @@
     """
 
     # should always be set to be explicit
     profile_name: str
     target_name: str
 
     # should be set if using a user-supplied profiles.yml
-    profiles_yml_filepath: Path | None = None
+    profiles_yml_filepath: str | Path | None = None
 
     # should be set if using cosmos to map Airflow connections to dbt profiles
     profile_mapping: BaseProfileMapping | None = None
 
     def __post_init__(self) -> None:
         "Validates that we have enough information to render a profile."
         # if using a user-supplied profiles.yml, validate that it exists
-        if self.profiles_yml_filepath and not self.profiles_yml_filepath.exists():
+        if self.profiles_yml_filepath and not Path(self.profiles_yml_filepath).exists():
             raise CosmosValueError(f"The file {self.profiles_yml_filepath} does not exist.")
 
     def validate_profile(self) -> None:
         "Validates that we have enough information to render a profile."
         if not self.profiles_yml_filepath and not self.profile_mapping:
             raise CosmosValueError("Either profiles_yml_filepath or profile_mapping must be set to render a profile")
```

### Comparing `astronomer_cosmos-1.0.3/cosmos/constants.py` & `astronomer_cosmos-1.0.4/cosmos/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,7 +46,8 @@
     Type of dbt node.
     """
 
     MODEL = "model"
     SNAPSHOT = "snapshot"
     SEED = "seed"
     TEST = "test"
+    SOURCE = "source"
```

### Comparing `astronomer_cosmos-1.0.3/cosmos/converter.py` & `astronomer_cosmos-1.0.4/cosmos/converter.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/dataset.py` & `astronomer_cosmos-1.0.4/cosmos/dataset.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/airflow/dag.py` & `astronomer_cosmos-1.0.4/cosmos/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/airflow/graph.py` & `astronomer_cosmos-1.0.4/cosmos/airflow/graph.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/airflow/task_group.py` & `astronomer_cosmos-1.0.4/cosmos/airflow/task_group.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/core/airflow.py` & `astronomer_cosmos-1.0.4/cosmos/core/airflow.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/core/graph/entities.py` & `astronomer_cosmos-1.0.4/cosmos/core/graph/entities.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/dbt/graph.py` & `astronomer_cosmos-1.0.4/cosmos/dbt/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
             except json.decoder.JSONDecodeError:
                 logger.info("Skipping line: %s", line)
             else:
                 node = DbtNode(
                     name=node_dict["name"],
                     unique_id=node_dict["unique_id"],
                     resource_type=DbtResourceType(node_dict["resource_type"]),
-                    depends_on=node_dict["depends_on"].get("nodes", []),
+                    depends_on=node_dict.get("depends_on", {}).get("nodes", []),
                     file_path=self.project.dir / node_dict["original_file_path"],
                     tags=node_dict["tags"],
                     config=node_dict["config"],
                 )
                 nodes[node.unique_id] = node
 
         self.nodes = nodes
```

### Comparing `astronomer_cosmos-1.0.3/cosmos/dbt/project.py` & `astronomer_cosmos-1.0.4/cosmos/dbt/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/dbt/selector.py` & `astronomer_cosmos-1.0.4/cosmos/dbt/selector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 import logging
 from pathlib import Path
 
 from typing import TYPE_CHECKING
 
+from cosmos.exceptions import CosmosValueError
+
 if TYPE_CHECKING:
     from cosmos.dbt.graph import DbtNode
 
 
 SUPPORTED_CONFIG = ["materialized", "schema", "tags"]
 PATH_SELECTOR = "path:"
 TAG_SELECTOR = "tag:"
@@ -128,14 +130,25 @@
     https://docs.getdbt.com/reference/node-selection/yaml-selectors
     """
     select = select or []
     exclude = exclude or []
     if not select and not exclude:
         return nodes
 
+    # validates select and exclude filters
+    filters = [["select", select], ["exclude", exclude]]
+    for filter_type, filter in filters:
+        for filter_parameter in filter:
+            if filter_parameter.startswith(PATH_SELECTOR) or filter_parameter.startswith(TAG_SELECTOR):
+                continue
+            elif any([filter_parameter.startswith(CONFIG_SELECTOR + config + ":") for config in SUPPORTED_CONFIG]):
+                continue
+            else:
+                raise CosmosValueError(f"Invalid {filter_type} filter: {filter_parameter}")
+
     subset_ids: set[str] = set()
 
     for statement in select:
         config = SelectorConfig(project_dir, statement)
         select_ids = select_nodes_ids_by_intersection(nodes, config)
         subset_ids = subset_ids.union(set(select_ids))
```

### Comparing `astronomer_cosmos-1.0.3/cosmos/dbt/parser/output.py` & `astronomer_cosmos-1.0.4/cosmos/dbt/parser/output.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/dbt/parser/project.py` & `astronomer_cosmos-1.0.4/cosmos/dbt/parser/project.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/hooks/subprocess.py` & `astronomer_cosmos-1.0.4/cosmos/hooks/subprocess.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/operators/__init__.py` & `astronomer_cosmos-1.0.4/cosmos/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/operators/base.py` & `astronomer_cosmos-1.0.4/cosmos/operators/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/operators/docker.py` & `astronomer_cosmos-1.0.4/cosmos/operators/docker.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/operators/kubernetes.py` & `astronomer_cosmos-1.0.4/cosmos/operators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/operators/local.py` & `astronomer_cosmos-1.0.4/cosmos/operators/local.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/operators/virtualenv.py` & `astronomer_cosmos-1.0.4/cosmos/operators/virtualenv.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/profiles/__init__.py` & `astronomer_cosmos-1.0.4/cosmos/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/profiles/base.py` & `astronomer_cosmos-1.0.4/cosmos/profiles/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/profiles/bigquery/service_account_file.py` & `astronomer_cosmos-1.0.4/cosmos/profiles/bigquery/service_account_file.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/profiles/bigquery/service_account_keyfile_dict.py` & `astronomer_cosmos-1.0.4/cosmos/profiles/bigquery/service_account_keyfile_dict.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/profiles/databricks/token.py` & `astronomer_cosmos-1.0.4/cosmos/profiles/databricks/token.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/profiles/exasol/user_pass.py` & `astronomer_cosmos-1.0.4/cosmos/profiles/exasol/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/profiles/postgres/user_pass.py` & `astronomer_cosmos-1.0.4/cosmos/profiles/postgres/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/profiles/redshift/user_pass.py` & `astronomer_cosmos-1.0.4/cosmos/profiles/redshift/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/profiles/snowflake/user_pass.py` & `astronomer_cosmos-1.0.4/cosmos/profiles/snowflake/user_pass.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/profiles/snowflake/user_privatekey.py` & `astronomer_cosmos-1.0.4/cosmos/profiles/snowflake/user_privatekey.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/profiles/spark/thrift.py` & `astronomer_cosmos-1.0.4/cosmos/profiles/spark/thrift.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/profiles/trino/base.py` & `astronomer_cosmos-1.0.4/cosmos/profiles/trino/base.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/profiles/trino/certificate.py` & `astronomer_cosmos-1.0.4/cosmos/profiles/trino/certificate.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/profiles/trino/jwt.py` & `astronomer_cosmos-1.0.4/cosmos/profiles/trino/jwt.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/cosmos/profiles/trino/ldap.py` & `astronomer_cosmos-1.0.4/cosmos/profiles/trino/ldap.py`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/.gitignore` & `astronomer_cosmos-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/LICENSE` & `astronomer_cosmos-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/README.rst` & `astronomer_cosmos-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `astronomer_cosmos-1.0.3/pyproject.toml` & `astronomer_cosmos-1.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -42,46 +42,46 @@
     "Jinja2>=3.0.0",
     "typing-extensions; python_version < '3.8'",
     "virtualenv",
 ]
 
 [project.optional-dependencies]
 dbt-all = [
-    "dbt-bigquery",
-    "dbt-databricks",
-    "dbt-exasol",
-    "dbt-postgres",
-    "dbt-redshift",
-    "dbt-snowflake",
-    "dbt-spark",
+    "dbt-bigquery<=1.5.4",
+    "dbt-databricks<=1.5.4",
+    "dbt-exasol<=1.5.4",
+    "dbt-postgres<=1.5.4",
+    "dbt-redshift<=1.5.4",
+    "dbt-snowflake<=1.5.4",
+    "dbt-spark<=1.5.4",
     "astronomer-cosmos[dbt-openlineage]"
 ]
 dbt-bigquery = [
-    "dbt-bigquery",
+    "dbt-bigquery<=1.5.4",
 ]
 dbt-databricks = [
-    "dbt-databricks",
+    "dbt-databricks<=1.5.4",
 ]
 dbt-exasol = [
-    "dbt-exasol",
+    "dbt-exasol<=1.5.4",
 ]
 dbt-postgres = [
-    "dbt-postgres",
+    "dbt-postgres<=1.5.4",
 ]
 dbt-redshift = [
-    "dbt-redshift",
+    "dbt-redshift<=1.5.4",
 ]
 dbt-snowflake = [
-    "dbt-snowflake",
+    "dbt-snowflake<=1.5.4",
 ]
 dbt-spark = [
-    "dbt-spark",
+    "dbt-spark<=1.5.4",
 ]
 dbt-openlineage = [
-    "dbt-core",
+    "dbt-core<=1.5.4",
     "openlineage-dbt>=0.21.1"
 ]
 all = [
     "astronomer-cosmos[dbt-all]",
 ]
 docs =[
     "sphinx",
@@ -103,15 +103,15 @@
     "sqlalchemy-stubs", # Change when sqlalchemy is upgraded https://docs.sqlalchemy.org/en/14/orm/extensions/mypy.html
 ]
 
 docker = [
     "apache-airflow-providers-docker>=3.5.0",
 ]
 kubernetes = [
-    "apache-airflow-providers-cncf-kubernetes>=5.1.1",
+    "apache-airflow-providers-cncf-kubernetes>=5.1.1,<7.3.0",
 ]
 
 
 [project.urls]
 Homepage = "https://github.com/astronomer/astronomer-cosmos"
 Documentation = "https://github.com/astronomer/astronomer-cosmos"
 
@@ -127,15 +127,15 @@
 # TESTING
 ######################################
 
 [tool.hatch.envs.tests]
 dependencies = [
     "astronomer-cosmos[tests]",
     "apache-airflow-providers-docker>=3.5.0",
-    "apache-airflow-providers-cncf-kubernetes>=5.1.1"
+    "apache-airflow-providers-cncf-kubernetes>=5.1.1,<7.3.0"
 ]
 
 [[tool.hatch.envs.tests.matrix]]
 python = ["3.7", "3.8", "3.9", "3.10"]
 airflow = ["2.3", "2.4", "2.5", "2.6"]
 
 [tool.hatch.envs.tests.overrides]
@@ -151,16 +151,15 @@
 test = 'pytest -vv --durations=0 . -m "not integration" --ignore=tests/test_example_dags.py'
 test-cov = 'pytest -vv --cov=cosmos --cov-report=term-missing --cov-report=xml --durations=0 -m "not integration" --ignore=tests/test_example_dags.py'
 # we install using the following workaround to overcome installation conflicts, such as:
 # apache-airflow 2.3.0 and dbt-core [0.13.0 - 1.5.2] and jinja2>=3.0.0 because these package versions have conflicting dependencies
 test-integration-setup = """pip uninstall dbt-postgres; \
 rm -rf airflow.*; \
 airflow db init; \
-pip install dbt-postgres; \
-pip install dbt-databricks"""
+pip install 'dbt-postgres<=1.5.4' 'dbt-databricks<=1.5.4'"""
 test-integration = """pytest -vv \
 --cov=cosmos \
 --cov-report=term-missing \
 --cov-report=xml \
 --durations=0 \
 -m integration  \
 -k 'not test_example_dag[example_cosmos_python_models]'
```

### Comparing `astronomer_cosmos-1.0.3/PKG-INFO` & `astronomer_cosmos-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-cosmos
-Version: 1.0.3
+Version: 1.0.4
 Summary: Render 3rd party workflows in Airflow
 Project-URL: Homepage, https://github.com/astronomer/astronomer-cosmos
 Project-URL: Documentation, https://github.com/astronomer/astronomer-cosmos
 Author-email: Astronomer <humans@astronomer.io>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: airflow,apache-airflow,astronomer,dags,dbt
@@ -28,47 +28,47 @@
 Requires-Dist: pydantic<2.0.0,>=1.10.0
 Requires-Dist: typing-extensions; python_version < '3.8'
 Requires-Dist: virtualenv
 Provides-Extra: all
 Requires-Dist: astronomer-cosmos[dbt-all]; extra == 'all'
 Provides-Extra: dbt-all
 Requires-Dist: astronomer-cosmos[dbt-openlineage]; extra == 'dbt-all'
-Requires-Dist: dbt-bigquery; extra == 'dbt-all'
-Requires-Dist: dbt-databricks; extra == 'dbt-all'
-Requires-Dist: dbt-exasol; extra == 'dbt-all'
-Requires-Dist: dbt-postgres; extra == 'dbt-all'
-Requires-Dist: dbt-redshift; extra == 'dbt-all'
-Requires-Dist: dbt-snowflake; extra == 'dbt-all'
-Requires-Dist: dbt-spark; extra == 'dbt-all'
+Requires-Dist: dbt-bigquery<=1.5.4; extra == 'dbt-all'
+Requires-Dist: dbt-databricks<=1.5.4; extra == 'dbt-all'
+Requires-Dist: dbt-exasol<=1.5.4; extra == 'dbt-all'
+Requires-Dist: dbt-postgres<=1.5.4; extra == 'dbt-all'
+Requires-Dist: dbt-redshift<=1.5.4; extra == 'dbt-all'
+Requires-Dist: dbt-snowflake<=1.5.4; extra == 'dbt-all'
+Requires-Dist: dbt-spark<=1.5.4; extra == 'dbt-all'
 Provides-Extra: dbt-bigquery
-Requires-Dist: dbt-bigquery; extra == 'dbt-bigquery'
+Requires-Dist: dbt-bigquery<=1.5.4; extra == 'dbt-bigquery'
 Provides-Extra: dbt-databricks
-Requires-Dist: dbt-databricks; extra == 'dbt-databricks'
+Requires-Dist: dbt-databricks<=1.5.4; extra == 'dbt-databricks'
 Provides-Extra: dbt-exasol
-Requires-Dist: dbt-exasol; extra == 'dbt-exasol'
+Requires-Dist: dbt-exasol<=1.5.4; extra == 'dbt-exasol'
 Provides-Extra: dbt-openlineage
-Requires-Dist: dbt-core; extra == 'dbt-openlineage'
+Requires-Dist: dbt-core<=1.5.4; extra == 'dbt-openlineage'
 Requires-Dist: openlineage-dbt>=0.21.1; extra == 'dbt-openlineage'
 Provides-Extra: dbt-postgres
-Requires-Dist: dbt-postgres; extra == 'dbt-postgres'
+Requires-Dist: dbt-postgres<=1.5.4; extra == 'dbt-postgres'
 Provides-Extra: dbt-redshift
-Requires-Dist: dbt-redshift; extra == 'dbt-redshift'
+Requires-Dist: dbt-redshift<=1.5.4; extra == 'dbt-redshift'
 Provides-Extra: dbt-snowflake
-Requires-Dist: dbt-snowflake; extra == 'dbt-snowflake'
+Requires-Dist: dbt-snowflake<=1.5.4; extra == 'dbt-snowflake'
 Provides-Extra: dbt-spark
-Requires-Dist: dbt-spark; extra == 'dbt-spark'
+Requires-Dist: dbt-spark<=1.5.4; extra == 'dbt-spark'
 Provides-Extra: docker
 Requires-Dist: apache-airflow-providers-docker>=3.5.0; extra == 'docker'
 Provides-Extra: docs
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-autoapi; extra == 'docs'
 Requires-Dist: sphinx-autobuild; extra == 'docs'
 Provides-Extra: kubernetes
-Requires-Dist: apache-airflow-providers-cncf-kubernetes>=5.1.1; extra == 'kubernetes'
+Requires-Dist: apache-airflow-providers-cncf-kubernetes<7.3.0,>=5.1.1; extra == 'kubernetes'
 Provides-Extra: tests
 Requires-Dist: mypy; extra == 'tests'
 Requires-Dist: packaging; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
 Requires-Dist: pytest-describe; extra == 'tests'
 Requires-Dist: pytest-dotenv; extra == 'tests'
 Requires-Dist: pytest-split; extra == 'tests'
```

