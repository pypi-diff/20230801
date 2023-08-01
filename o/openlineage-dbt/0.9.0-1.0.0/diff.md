# Comparing `tmp/openlineage-dbt-0.9.0.tar.gz` & `tmp/openlineage-dbt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openlineage-dbt-0.9.0.tar", last modified: Fri Jun  3 23:03:10 2022, max compression
+gzip compressed data, was "openlineage-dbt-1.0.0.tar", last modified: Tue Aug  1 19:46:05 2023, max compression
```

## Comparing `openlineage-dbt-0.9.0.tar` & `openlineage-dbt-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2011 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1287 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/openlineage_dbt.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2011 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/openlineage_dbt.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      275 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/openlineage_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/openlineage_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/openlineage_dbt.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      185 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/openlineage_dbt.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/openlineage_dbt.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/scripts/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     5554 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/scripts/dbt-ol
--rw-r--r--   0 circleci  (3434) circleci  (3434)      537 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      982 2022-06-03 23:03:10.000000 openlineage-dbt-0.9.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:05.618312 openlineage-dbt-1.0.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1983 2023-08-01 19:46:05.618312 openlineage-dbt-1.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1733 2023-08-01 19:46:02.000000 openlineage-dbt-1.0.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:05.618312 openlineage-dbt-1.0.0/openlineage_dbt.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1983 2023-08-01 19:46:05.000000 openlineage-dbt-1.0.0/openlineage_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      290 2023-08-01 19:46:05.000000 openlineage-dbt-1.0.0/openlineage_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-01 19:46:05.000000 openlineage-dbt-1.0.0/openlineage_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-01 19:46:05.000000 openlineage-dbt-1.0.0/openlineage_dbt.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      182 2023-08-01 19:46:05.000000 openlineage-dbt-1.0.0/openlineage_dbt.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-01 19:46:05.000000 openlineage-dbt-1.0.0/openlineage_dbt.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-08-01 19:46:02.000000 openlineage-dbt-1.0.0/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 19:46:05.618312 openlineage-dbt-1.0.0/scripts/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     6511 2023-08-01 19:46:02.000000 openlineage-dbt-1.0.0/scripts/dbt-ol
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      575 2023-08-01 19:46:05.618312 openlineage-dbt-1.0.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1033 2023-08-01 19:46:02.000000 openlineage-dbt-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `openlineage-dbt-0.9.0/README.md` & `openlineage-dbt-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-<!-- SPDX-License-Identifier: Apache-2.0 -->
-
 # OpenLineage dbt integration
 
-Wrapper script for dbt for automatic metadata collection
+Wrapper script for automatic metadata collection from dbt
 
 ## Features
 
 **Metadata**
 
 * Model run lifecycle
 * Model inputs / outputs
 
 ## Requirements
 
-- [Python >= 3.7](https://www.python.org/downloads)
+- [Python >= 3.8](https://www.python.org/downloads)
 - [dbt >= 0.20](https://www.getdbt.com/)
 
 Right now, `openlineage-dbt` only supports `bigquery`, `snowflake`, `spark` and `redshift` dbt adapters.
 
 ## Installation
 
 ```bash
@@ -31,21 +29,31 @@
 ```
 
 ## Configuration
 
 
 ### `HTTP` Backend Environment Variables
 
-`openlineage-dbt` uses OpenLineage client to push data to OpenLineage backend.
+`openlineage-dbt` uses the OpenLineage client to push data to the OpenLineage backend.
 
-OpenLineage client depends on environment variables:
+The OpenLineage client depends on environment variables:
 
 * `OPENLINEAGE_URL` - point to service which will consume OpenLineage events
 * `OPENLINEAGE_API_KEY` - set if consumer of OpenLineage events requires `Bearer` authentication key
 * `OPENLINEAGE_NAMESPACE` - set if you are using something other than the `default` namespace for job namespace.
 
 
+### Logging
+
+In addition to conventional logging approaches, the OpenLineage dbt wrapper script provides an alternative way of configuring its logging behavior. By setting the `OPENLINEAGE_DBT_LOGGING` environment variable, you can establish the logging level for the `openlineage.dbt` and its child modules.
+
+You can also set log level of `dbtol` which is deprecated.
+
 ## Usage
 
 To begin collecting dbt metadata with OpenLineage, replace `dbt run` with `dbt-ol run`.
 
-Additional table and column level metadata will be available if `catalog.json`, result of running `dbt docs generate` will be found in target directory.
+Additional table and column level metadata will be available if `catalog.json`, a result of running `dbt docs generate`, will be found in the target directory.
+
+----
+SPDX-License-Identifier: Apache-2.0\
+Copyright 2018-2023 contributors to the OpenLineage project
```

### Comparing `openlineage-dbt-0.9.0/scripts/dbt-ol` & `openlineage-dbt-1.0.0/scripts/dbt-ol`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 #!/usr/bin/env python
+#
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
+
 import logging
+import os
 import subprocess
 import sys
 import time
-import os
 import uuid
+from datetime import datetime, timezone
 from typing import Optional
 
+from openlineage.client.client import OpenLineageClient
+from openlineage.client.run import Job, Run, RunEvent, RunState
+from openlineage.common.provider.dbt import (
+    DbtLocalArtifactProcessor,
+    ParentRunMetadata,
+    UnsupportedDbtCommand,
+)
 from tqdm import tqdm
-from datetime import datetime, timezone
-
-from openlineage.client.run import RunEvent, RunState, Run, Job
-from openlineage.client.client import OpenLineageClient, OpenLineageClientOptions
-from openlineage.common.provider.dbt import DbtArtifactProcessor, ParentRunMetadata
 
-__version__ = "0.9.0"
+__version__ = "1.0.0"
 
 from openlineage.common.utils import parse_single_arg
 
 PRODUCER = f'https://github.com/OpenLineage/OpenLineage/tree/{__version__}/integration/dbt'
 
 
-def setup_client() -> Optional[OpenLineageClient]:
-    url = os.getenv("OPENLINEAGE_URL")
-    if not url:
-        return None
-    return OpenLineageClient(
-        url=url,
-        options=OpenLineageClientOptions(
-            api_key=os.getenv("OPENLINEAGE_API_KEY", None)
-        )
-    )
-
-
 def dbt_run_event(
     state: RunState,
     job_name: str,
     job_namespace: str,
     run_id: str = str(uuid.uuid4()),
     parent: Optional[ParentRunMetadata] = None
 ) -> RunEvent:
@@ -53,15 +48,17 @@
             namespace=parent.job_namespace if parent else job_namespace,
             name=job_name
         ),
         producer=PRODUCER
     )
 
 
-def dbt_run_event_start(job_name: str, job_namespace: str, parent_run_metadata: ParentRunMetadata) -> RunEvent:
+def dbt_run_event_start(
+    job_name: str, job_namespace: str, parent_run_metadata: ParentRunMetadata
+) -> RunEvent:
     return dbt_run_event(
         state=RunState.START,
         job_name=job_name,
         job_namespace=job_namespace,
         parent=parent_run_metadata
     )
 
@@ -76,110 +73,144 @@
         state=RunState.COMPLETE,
         job_namespace=job_namespace,
         job_name=job_name,
         run_id=run_id,
         parent=parent_run_metadata
     )
 
+def dbt_run_event_failed(
+    run_id: str,
+    job_namespace: str,
+    job_name: str,
+    parent_run_metadata: Optional[ParentRunMetadata]
+) -> RunEvent:
+    return dbt_run_event(
+        state=RunState.FAIL,
+        job_namespace=job_namespace,
+        job_name=job_name,
+        run_id=run_id,
+        parent=parent_run_metadata
+    )
 
+openlineage_logger = logging.getLogger("openlineage.dbt")
+openlineage_logger.setLevel(os.getenv("OPENLINEAGE_DBT_LOGGING", "INFO"))
+openlineage_logger.addHandler(logging.StreamHandler(sys.stdout))
+# deprecated dbtol logger
 logger = logging.getLogger("dbtol")
-logger.setLevel("INFO")
-logger.addHandler(logging.StreamHandler(sys.stdout))
-
+for handler in openlineage_logger.handlers:
+    logger.addHandler(handler)
+    logger.setLevel(openlineage_logger.level)
 
 def main():
     logger.info(f"Running OpenLineage dbt wrapper version {__version__}")
-    logger.info(f"This wrapper will send OpenLineage events at the end of dbt execution.")
+    logger.info("This wrapper will send OpenLineage events at the end of dbt execution.")
 
-    args = sys.argv[2:]
+    args = sys.argv[1:]
     target = parse_single_arg(args, ['-t', '--target'])
     project_dir = parse_single_arg(args, ['--project-dir'], default='./')
     profile_name = parse_single_arg(args, ['--profile'])
 
-    client = setup_client()
-    if client is None:
-        logger.info("OPENLINEAGE_URL is not set: stopping execution")
-        sys.exit(1)
-
     # We can get this if we have been orchestrated by an external system like airflow
     parent_id = os.getenv("OPENLINEAGE_PARENT_ID")
     parent_run_metadata = None
     job_namespace = os.environ.get(
         'OPENLINEAGE_NAMESPACE',
         'dbt'
     )
 
-    client = OpenLineageClient.from_environment()
+    client = OpenLineageClient()
 
     if parent_id:
         parent_namespace, parent_job_name, parent_run_id = parent_id.split('/')
         parent_run_metadata = ParentRunMetadata(
             run_id=parent_run_id,
             job_name=parent_job_name,
             job_namespace=parent_namespace
         )
 
-    processor = DbtArtifactProcessor(
+    processor = DbtLocalArtifactProcessor(
         producer=PRODUCER,
         target=target,
         job_namespace=job_namespace,
         project_dir=project_dir,
         profile_name=profile_name,
         logger=logger
     )
 
     # Always emit "wrapping event" around dbt run. This indicates start of dbt execution, since
     # both the start and complete events for dbt models won't get emitted until end of execution.
-    dbt_run_event = dbt_run_event_start(
-        job_name=f"dbt-run-{processor.project['name']}",
+    start_event = dbt_run_event_start(
+        job_name=f"dbt-run-{processor.project_name}",
         job_namespace=job_namespace,
         parent_run_metadata=parent_run_metadata
     )
     dbt_run_metadata = ParentRunMetadata(
-        run_id=dbt_run_event.run.runId,
-        job_name=dbt_run_event.job.name,
-        job_namespace=dbt_run_event.job.namespace
+        run_id=start_event.run.runId,
+        job_name=start_event.job.name,
+        job_namespace=start_event.job.namespace
     )
 
+    # Failed start event emit should not stop dbt command from running.
+    try:
+        client.emit(start_event)
+    except Exception as e:
+        logger.warning("OpenLineage client failed to emit start event. Exception: %s", e)
+
     # Set parent run metadata to use it as parent run facet
     processor.dbt_run_metadata = dbt_run_metadata
 
     pre_run_time = time.time()
     # Execute dbt in external process
     process = subprocess.Popen(
         ["dbt"] + sys.argv[1:],
         stdout=sys.stdout,
         stderr=sys.stderr
     )
-    process.wait()
-
-    if len(sys.argv) < 2 or sys.argv[1] not in ['run', 'test', 'build']:
-        return
+    return_code = process.wait()
 
     # If run_result has modification time before dbt command
     # or does not exist, do not emit dbt events.
     try:
         if os.stat(processor.run_result_path).st_mtime < pre_run_time:
-            logger.info(f"OpenLineage events not emittled: run_result file "
+            logger.info(f"OpenLineage events not emitted: run_result file "
                         f"({processor.run_result_path}) was not modified by dbt")
             return
     except FileNotFoundError:
-        logger.info(f"OpenLineage events not emittled:"
+        logger.info(f"OpenLineage events not emitted:"
                     f"did not find run_result file ({processor.run_result_path})")
         return
 
-    events = processor.parse().events()
+    try:
+        events = processor.parse().events()
+    except UnsupportedDbtCommand as e:
+        # log exception message
+        logger.info(e)
+        events = []
+
+    if return_code == 0:
+        last_event = dbt_run_event_end(
+            run_id=dbt_run_metadata.run_id,
+            job_namespace=dbt_run_metadata.job_namespace,
+            job_name=dbt_run_metadata.job_name,
+            parent_run_metadata=parent_run_metadata
+        )
+    else:
+        last_event = dbt_run_event_failed(
+            run_id=dbt_run_metadata.run_id,
+            job_namespace=dbt_run_metadata.job_namespace,
+            job_name=dbt_run_metadata.job_name,
+            parent_run_metadata=parent_run_metadata
+        )
 
-    for event in tqdm(events, desc="Emitting OpenLineage events"):
+    for event in tqdm(
+        events + [last_event],
+        desc="Emitting OpenLineage events",
+        initial=1,
+        total=len(events) + 2,
+    ):
         client.emit(event)
 
-    client.emit(dbt_run_event_end(
-        run_id=dbt_run_metadata.run_id,
-        job_namespace=dbt_run_metadata.job_namespace,
-        job_name=dbt_run_metadata.job_name,
-        parent_run_metadata=parent_run_metadata
-    ))
     logger.info(f"Emitted {len(events) + 2} openlineage events")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `openlineage-dbt-0.9.0/setup.cfg` & `openlineage-dbt-1.0.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.0
+current_version = 1.0.0
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<rc>.*)
 serialize = 
 	{major}.{minor}.{patch}{rc}
 	{major}.{minor}.{patch}
 
@@ -17,11 +17,14 @@
 
 [flake8]
 max-line-length = 99
 
 [tool:pytest]
 addopts = -p no:warnings
 
+[mypy]
+ignore_missing_imports = True
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `openlineage-dbt-0.9.0/setup.py` & `openlineage-dbt-1.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 #!/usr/bin/env python
 #
-# SPDX-License-Identifier: Apache-2.0.
+# Copyright 2018-2023 contributors to the OpenLineage project
+# SPDX-License-Identifier: Apache-2.0
 #
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
 with open("README.md") as readme_file:
      readme = readme_file.read()
 
-__version__ = "0.9.0"
+__version__ = "1.0.0"
 
 requirements = [
-    f"sqlparse>=0.2.3,<0.4",
-    f"tqdm>=4.62.0",
+    "tqdm>=4.62.0",
     f"openlineage-integration-common[dbt]=={__version__}",
 ]
 
 
 extras_require = {
     "tests": [
         "pytest",
         "pytest-cov",
         "mock",
-        "flake8",
+        "ruff"
+        "mypy>=0.9.6",
         "python-dateutil"
     ],
 }
 extras_require["dev"] = set(sum(extras_require.values(), []))
 
 setup(
     name="openlineage-dbt",
@@ -36,11 +37,11 @@
     long_description=readme,
     long_description_content_type="text/markdown",
     author="OpenLineage",
     scripts=['scripts/dbt-ol'],
     include_package_data=True,
     install_requires=requirements,
     extras_require=extras_require,
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     zip_safe=False,
     keywords="openlineage",
 )
```

