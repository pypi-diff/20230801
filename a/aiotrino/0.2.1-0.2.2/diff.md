# Comparing `tmp/aiotrino-0.2.1.tar.gz` & `tmp/aiotrino-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotrino-0.2.1.tar", last modified: Sat May 27 18:37:27 2023, max compression
+gzip compressed data, was "aiotrino-0.2.2.tar", last modified: Tue Aug  1 12:35:37 2023, max compression
```

## Comparing `aiotrino-0.2.1.tar` & `aiotrino-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 michiel   (1000) michiel   (1000)        0 2023-05-27 18:37:27.218042 aiotrino-0.2.1/
--rw-rw-r--   0 michiel   (1000) michiel   (1000)    11358 2023-05-27 16:11:32.000000 aiotrino-0.2.1/LICENSE
--rw-rw-r--   0 michiel   (1000) michiel   (1000)     8397 2023-05-27 18:37:27.222042 aiotrino-0.2.1/PKG-INFO
--rw-rw-r--   0 michiel   (1000) michiel   (1000)     7178 2023-05-27 18:37:26.000000 aiotrino-0.2.1/README.md
-drwxrwxr-x   0 michiel   (1000) michiel   (1000)        0 2023-05-27 18:37:27.218042 aiotrino-0.2.1/aiotrino/
--rw-rw-r--   0 michiel   (1000) michiel   (1000)      634 2023-05-27 18:35:33.000000 aiotrino-0.2.1/aiotrino/__init__.py
--rw-rw-r--   0 michiel   (1000) michiel   (1000)     4705 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/auth.py
--rw-rw-r--   0 michiel   (1000) michiel   (1000)    23291 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/client.py
--rw-rw-r--   0 michiel   (1000) michiel   (1000)     2089 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/constants.py
--rw-rw-r--   0 michiel   (1000) michiel   (1000)    17444 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/dbapi.py
--rw-rw-r--   0 michiel   (1000) michiel   (1000)     5198 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/exceptions.py
--rw-rw-r--   0 michiel   (1000) michiel   (1000)      765 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/logging.py
--rw-rw-r--   0 michiel   (1000) michiel   (1000)     3580 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/transaction.py
--rw-rw-r--   0 michiel   (1000) michiel   (1000)      431 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/utils.py
-drwxrwxr-x   0 michiel   (1000) michiel   (1000)        0 2023-05-27 18:37:27.218042 aiotrino-0.2.1/aiotrino.egg-info/
--rw-rw-r--   0 michiel   (1000) michiel   (1000)     8397 2023-05-27 18:37:27.000000 aiotrino-0.2.1/aiotrino.egg-info/PKG-INFO
--rw-rw-r--   0 michiel   (1000) michiel   (1000)      442 2023-05-27 18:37:27.000000 aiotrino-0.2.1/aiotrino.egg-info/SOURCES.txt
--rw-rw-r--   0 michiel   (1000) michiel   (1000)        1 2023-05-27 18:37:27.000000 aiotrino-0.2.1/aiotrino.egg-info/dependency_links.txt
--rw-rw-r--   0 michiel   (1000) michiel   (1000)      170 2023-05-27 18:37:27.000000 aiotrino-0.2.1/aiotrino.egg-info/requires.txt
--rw-rw-r--   0 michiel   (1000) michiel   (1000)        9 2023-05-27 18:37:27.000000 aiotrino-0.2.1/aiotrino.egg-info/top_level.txt
--rw-rw-r--   0 michiel   (1000) michiel   (1000)      150 2023-05-27 18:37:27.222042 aiotrino-0.2.1/setup.cfg
--rwxrwxr-x   0 michiel   (1000) michiel   (1000)     2547 2023-05-27 16:48:52.000000 aiotrino-0.2.1/setup.py
-drwxrwxr-x   0 michiel   (1000) michiel   (1000)        0 2023-05-27 18:37:27.218042 aiotrino-0.2.1/tests/
--rw-rw-r--   0 michiel   (1000) michiel   (1000)    24153 2023-05-27 16:11:32.000000 aiotrino-0.2.1/tests/test_client.py
--rw-rw-r--   0 michiel   (1000) michiel   (1000)     2136 2023-05-27 16:11:32.000000 aiotrino-0.2.1/tests/test_exceptions.py
--rw-rw-r--   0 michiel   (1000) michiel   (1000)     1067 2023-05-27 16:11:32.000000 aiotrino-0.2.1/tests/test_http.py
+drwxrwxr-x   0 michiel   (1000) michiel   (1000)        0 2023-08-01 12:35:37.530008 aiotrino-0.2.2/
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)    11358 2023-05-27 16:11:32.000000 aiotrino-0.2.2/LICENSE
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     8373 2023-08-01 12:35:37.530008 aiotrino-0.2.2/PKG-INFO
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     7154 2023-08-01 12:33:16.000000 aiotrino-0.2.2/README.md
+drwxrwxr-x   0 michiel   (1000) michiel   (1000)        0 2023-08-01 12:35:37.530008 aiotrino-0.2.2/aiotrino/
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)      634 2023-08-01 12:32:56.000000 aiotrino-0.2.2/aiotrino/__init__.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     4705 2023-05-27 16:11:32.000000 aiotrino-0.2.2/aiotrino/auth.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)    23291 2023-05-27 16:11:32.000000 aiotrino-0.2.2/aiotrino/client.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     2092 2023-08-01 11:38:41.000000 aiotrino-0.2.2/aiotrino/constants.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)    18032 2023-08-01 11:54:48.000000 aiotrino-0.2.2/aiotrino/dbapi.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     5198 2023-05-27 16:11:32.000000 aiotrino-0.2.2/aiotrino/exceptions.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)      765 2023-05-27 16:11:32.000000 aiotrino-0.2.2/aiotrino/logging.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     3580 2023-05-27 16:11:32.000000 aiotrino-0.2.2/aiotrino/transaction.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)      431 2023-05-27 16:11:32.000000 aiotrino-0.2.2/aiotrino/utils.py
+drwxrwxr-x   0 michiel   (1000) michiel   (1000)        0 2023-08-01 12:35:37.530008 aiotrino-0.2.2/aiotrino.egg-info/
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     8373 2023-08-01 12:35:37.000000 aiotrino-0.2.2/aiotrino.egg-info/PKG-INFO
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)      442 2023-08-01 12:35:37.000000 aiotrino-0.2.2/aiotrino.egg-info/SOURCES.txt
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)        1 2023-08-01 12:35:37.000000 aiotrino-0.2.2/aiotrino.egg-info/dependency_links.txt
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)      170 2023-08-01 12:35:37.000000 aiotrino-0.2.2/aiotrino.egg-info/requires.txt
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)        9 2023-08-01 12:35:37.000000 aiotrino-0.2.2/aiotrino.egg-info/top_level.txt
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)      150 2023-08-01 12:35:37.530008 aiotrino-0.2.2/setup.cfg
+-rwxrwxr-x   0 michiel   (1000) michiel   (1000)     2547 2023-05-27 16:48:52.000000 aiotrino-0.2.2/setup.py
+drwxrwxr-x   0 michiel   (1000) michiel   (1000)        0 2023-08-01 12:35:37.530008 aiotrino-0.2.2/tests/
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)    24153 2023-05-27 16:11:32.000000 aiotrino-0.2.2/tests/test_client.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     2136 2023-05-27 16:11:32.000000 aiotrino-0.2.2/tests/test_exceptions.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     1067 2023-05-27 16:11:32.000000 aiotrino-0.2.2/tests/test_http.py
```

### Comparing `aiotrino-0.2.1/LICENSE` & `aiotrino-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotrino-0.2.1/PKG-INFO` & `aiotrino-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotrino
-Version: 0.2.1
+Version: 0.2.2
 Summary: ASyncIO Client for the Trino distributed SQL Engine
 Home-page: https://github.com/mvanderlee/aiotrino/tree/main
 Author: Michiel Van Der Lee, Trino Team
 Author-email: jmt.vanderlee@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,15 @@
 Classifier: Topic :: Database :: Front-Ends
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: kerberos
 Provides-Extra: tests
 License-File: LICENSE
 
-[![Build Status](https://github.com/mvanderlee/trino-python-client/workflows/ci/badge.svg)](https://github.com/mvanderlee/trino-python-client/actions?query=workflow%3Aci+event%3Apush+branch%3Apy3-async)
+[![Build Status](https://github.com/mvanderlee/aiotrino/workflows/ci/badge.svg)](https://github.com/mvanderlee/aiotrino/actions?query=workflow%3Aci+event%3Apush+branch%3Apy3-async)
 [![Trino Slack](https://img.shields.io/static/v1?logo=slack&logoColor=959DA5&label=Slack&labelColor=333a41&message=join%20conversation&color=3AC358)](https://trino.io/slack.html)
 [![Presto: The Definitive Guide book download](https://img.shields.io/badge/Presto%3A%20The%20Definitive%20Guide-download-brightgreen)](https://www.starburstdata.com/oreilly-presto-guide-download/)
 
 # Introduction
 
 This package provides a asyncio client interface to query [Trino](https://trino.io/)
 a distributed SQL engine. It supports Python 3.7, 3.8, 3.9, 3.10, 3.11.
@@ -51,30 +51,30 @@
 conn = aiotrino.dbapi.connect(
     host='localhost',
     port=8080,
     user='the-user',
     catalog='the-catalog',
     schema='the-schema',
 )
-await cur = conn.cursor()
+cur = await conn.cursor()
 await cur.execute('SELECT * FROM system.runtime.nodes')
 rows = await cur.fetchall()
 await conn.close()
 ```
 Or with context manager 
 ```python
 import aiotrino
 async with aiotrino.dbapi.connect(
     host='localhost',
     port=8080,
     user='the-user',
     catalog='the-catalog',
     schema='the-schema',
 ) as conn:
-    await cur = conn.cursor()
+    cur = await conn.cursor()
     await cur.execute('SELECT * FROM system.runtime.nodes')
     rows = await cur.fetchall()
 ```
 
 This will query the `system.runtime.nodes` system tables that shows the nodes
 in the Trino cluster.
 
@@ -191,15 +191,15 @@
 - When writing a Git commit message, follow these [guidelines](https://chris.beams.io/posts/git-commit/).
 
 ## Running Tests
 
 There is a helper scripts, `run`, that provides commands to run tests.
 Type `./run tests` to run both unit and integration tests.
 
-`trino-python-client` uses [pytest](https://pytest.org/) for its tests. To run
+`aiotrino` uses [pytest](https://pytest.org/) for its tests. To run
 only unit tests, type:
 
 ```
 $ pytest tests
 ```
 
 Then you can pass options like `--pdb` or anything supported by `pytest --help`.
@@ -215,15 +215,15 @@
 
 ```
 $ pytest integration_tests
 ```
 
 They pull a Docker image and then run a container with a Trino server:
 - the image is named `trinodb/trino:${TRINO_VERSION}`
-- the container is named `trino-python-client-tests-{uuid4()[:7]}`
+- the container is named `aiotrino-python-client-tests-{uuid4()[:7]}`
 
 
 ### Test setup
 
 Supported OS Ubuntu 22.04
 
 1. Install [pyenv](https://github.com/pyenv/pyenv#automatic-installer)
@@ -261,24 +261,24 @@
     ```shell
     tox
     ```
 
 ## Releasing
 
 - [Set up your development environment](#Getting-Started-With-Development).
-- Change version in `trino/__init__.py`.
+- Change version in `aiotrino/__init__.py`.
 - Commit and create an annotated tag (`git tag -m '' current_version`)
 - Run the following:
   ```bash
   . .venv/bin/activate &&
   pip install twine wheel &&
   rm -rf dist/ &&
   ./setup.py sdist bdist_wheel &&
   twine upload dist/* &&
-  open https://pypi.org/project/trino/ &&
+  open https://pypi.org/project/aiotrino/ &&
   echo "Released!"
   ```
 - Push the branch and the tag (`git push upstream master current_version`)
 - Send release announcement.
 
 # Need Help?
```

### Comparing `aiotrino-0.2.1/README.md` & `aiotrino-0.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Build Status](https://github.com/mvanderlee/trino-python-client/workflows/ci/badge.svg)](https://github.com/mvanderlee/trino-python-client/actions?query=workflow%3Aci+event%3Apush+branch%3Apy3-async)
+[![Build Status](https://github.com/mvanderlee/aiotrino/workflows/ci/badge.svg)](https://github.com/mvanderlee/aiotrino/actions?query=workflow%3Aci+event%3Apush+branch%3Apy3-async)
 [![Trino Slack](https://img.shields.io/static/v1?logo=slack&logoColor=959DA5&label=Slack&labelColor=333a41&message=join%20conversation&color=3AC358)](https://trino.io/slack.html)
 [![Presto: The Definitive Guide book download](https://img.shields.io/badge/Presto%3A%20The%20Definitive%20Guide-download-brightgreen)](https://www.starburstdata.com/oreilly-presto-guide-download/)
 
 # Introduction
 
 This package provides a asyncio client interface to query [Trino](https://trino.io/)
 a distributed SQL engine. It supports Python 3.7, 3.8, 3.9, 3.10, 3.11.
@@ -21,30 +21,30 @@
 conn = aiotrino.dbapi.connect(
     host='localhost',
     port=8080,
     user='the-user',
     catalog='the-catalog',
     schema='the-schema',
 )
-await cur = conn.cursor()
+cur = await conn.cursor()
 await cur.execute('SELECT * FROM system.runtime.nodes')
 rows = await cur.fetchall()
 await conn.close()
 ```
 Or with context manager 
 ```python
 import aiotrino
 async with aiotrino.dbapi.connect(
     host='localhost',
     port=8080,
     user='the-user',
     catalog='the-catalog',
     schema='the-schema',
 ) as conn:
-    await cur = conn.cursor()
+    cur = await conn.cursor()
     await cur.execute('SELECT * FROM system.runtime.nodes')
     rows = await cur.fetchall()
 ```
 
 This will query the `system.runtime.nodes` system tables that shows the nodes
 in the Trino cluster.
 
@@ -161,15 +161,15 @@
 - When writing a Git commit message, follow these [guidelines](https://chris.beams.io/posts/git-commit/).
 
 ## Running Tests
 
 There is a helper scripts, `run`, that provides commands to run tests.
 Type `./run tests` to run both unit and integration tests.
 
-`trino-python-client` uses [pytest](https://pytest.org/) for its tests. To run
+`aiotrino` uses [pytest](https://pytest.org/) for its tests. To run
 only unit tests, type:
 
 ```
 $ pytest tests
 ```
 
 Then you can pass options like `--pdb` or anything supported by `pytest --help`.
@@ -185,15 +185,15 @@
 
 ```
 $ pytest integration_tests
 ```
 
 They pull a Docker image and then run a container with a Trino server:
 - the image is named `trinodb/trino:${TRINO_VERSION}`
-- the container is named `trino-python-client-tests-{uuid4()[:7]}`
+- the container is named `aiotrino-python-client-tests-{uuid4()[:7]}`
 
 
 ### Test setup
 
 Supported OS Ubuntu 22.04
 
 1. Install [pyenv](https://github.com/pyenv/pyenv#automatic-installer)
@@ -231,24 +231,24 @@
     ```shell
     tox
     ```
 
 ## Releasing
 
 - [Set up your development environment](#Getting-Started-With-Development).
-- Change version in `trino/__init__.py`.
+- Change version in `aiotrino/__init__.py`.
 - Commit and create an annotated tag (`git tag -m '' current_version`)
 - Run the following:
   ```bash
   . .venv/bin/activate &&
   pip install twine wheel &&
   rm -rf dist/ &&
   ./setup.py sdist bdist_wheel &&
   twine upload dist/* &&
-  open https://pypi.org/project/trino/ &&
+  open https://pypi.org/project/aiotrino/ &&
   echo "Released!"
   ```
 - Push the branch and the tag (`git push upstream master current_version`)
 - Send release announcement.
 
 # Need Help?
```

### Comparing `aiotrino-0.2.1/aiotrino/__init__.py` & `aiotrino-0.2.2/aiotrino/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from . import auth, client, constants, dbapi, exceptions, logging
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

### Comparing `aiotrino-0.2.1/aiotrino/auth.py` & `aiotrino-0.2.2/aiotrino/auth.py`

 * *Files identical despite different names*

### Comparing `aiotrino-0.2.1/aiotrino/client.py` & `aiotrino-0.2.2/aiotrino/client.py`

 * *Files identical despite different names*

### Comparing `aiotrino-0.2.1/aiotrino/constants.py` & `aiotrino-0.2.2/aiotrino/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any, Optional, Text  # NOQA: mypy types
 
 DEFAULT_PORT = 8080
-DEFAULT_SOURCE = "trino-python-client"
+DEFAULT_SOURCE = "aiotrino-python-client"
 DEFAULT_CATALOG = None  # type: Optional[Text]
 DEFAULT_SCHEMA = None  # type: Optional[Text]
 DEFAULT_AUTH = None  # type: Optional[Any]
 DEFAULT_MAX_ATTEMPTS = 3
 DEFAULT_REQUEST_TIMEOUT = 30.0  # type: float
 
 HTTP = "http"
```

### Comparing `aiotrino-0.2.1/aiotrino/dbapi.py` & `aiotrino-0.2.2/aiotrino/dbapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -276,14 +276,19 @@
         # Iterate until the 'X-Trino-Added-Prepare' header is found or
         # until there are no more results
         async for _ in result:
             response_headers = result.response_headers
 
             if constants.HEADERS.ADDED_PREPARE in response_headers:
                 return response_headers[constants.HEADERS.ADDED_PREPARE]
+        else:
+            # 406 no longer returns results so there is nothing to loop over.
+            response_headers = result.response_headers
+            if constants.HEADERS.ADDED_PREPARE in response_headers:
+                return response_headers[constants.HEADERS.ADDED_PREPARE]
 
         raise aiotrino.exceptions.FailedToObtainAddedPrepareHeader
 
     def _get_added_prepare_statement_trino_query(
         self,
         statement_name,
         params
@@ -361,14 +366,19 @@
         # Iterate until the 'X-Trino-Deallocated-Prepare' header is found or
         # until there are no more results
         async for _ in result:
             response_headers = result.response_headers
 
             if constants.HEADERS.DEALLOCATED_PREPARE in response_headers:
                 return response_headers[constants.HEADERS.DEALLOCATED_PREPARE]
+        else:
+            # 406 no longer returns results so there is nothing to loop over.
+            response_headers = result.response_headers
+            if constants.HEADERS.DEALLOCATED_PREPARE in response_headers:
+                return response_headers[constants.HEADERS.DEALLOCATED_PREPARE]
 
         raise aiotrino.exceptions.FailedToObtainDeallocatedPrepareHeader
 
     def _generate_unique_statement_name(self):
         return 'st_' + uuid.uuid4().hex.replace('-', '')
 
     async def execute(self, operation, params=None):
```

### Comparing `aiotrino-0.2.1/aiotrino/exceptions.py` & `aiotrino-0.2.2/aiotrino/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotrino-0.2.1/aiotrino/logging.py` & `aiotrino-0.2.2/aiotrino/logging.py`

 * *Files identical despite different names*

### Comparing `aiotrino-0.2.1/aiotrino/transaction.py` & `aiotrino-0.2.2/aiotrino/transaction.py`

 * *Files identical despite different names*

### Comparing `aiotrino-0.2.1/aiotrino.egg-info/PKG-INFO` & `aiotrino-0.2.2/aiotrino.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotrino
-Version: 0.2.1
+Version: 0.2.2
 Summary: ASyncIO Client for the Trino distributed SQL Engine
 Home-page: https://github.com/mvanderlee/aiotrino/tree/main
 Author: Michiel Van Der Lee, Trino Team
 Author-email: jmt.vanderlee@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,15 @@
 Classifier: Topic :: Database :: Front-Ends
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: kerberos
 Provides-Extra: tests
 License-File: LICENSE
 
-[![Build Status](https://github.com/mvanderlee/trino-python-client/workflows/ci/badge.svg)](https://github.com/mvanderlee/trino-python-client/actions?query=workflow%3Aci+event%3Apush+branch%3Apy3-async)
+[![Build Status](https://github.com/mvanderlee/aiotrino/workflows/ci/badge.svg)](https://github.com/mvanderlee/aiotrino/actions?query=workflow%3Aci+event%3Apush+branch%3Apy3-async)
 [![Trino Slack](https://img.shields.io/static/v1?logo=slack&logoColor=959DA5&label=Slack&labelColor=333a41&message=join%20conversation&color=3AC358)](https://trino.io/slack.html)
 [![Presto: The Definitive Guide book download](https://img.shields.io/badge/Presto%3A%20The%20Definitive%20Guide-download-brightgreen)](https://www.starburstdata.com/oreilly-presto-guide-download/)
 
 # Introduction
 
 This package provides a asyncio client interface to query [Trino](https://trino.io/)
 a distributed SQL engine. It supports Python 3.7, 3.8, 3.9, 3.10, 3.11.
@@ -51,30 +51,30 @@
 conn = aiotrino.dbapi.connect(
     host='localhost',
     port=8080,
     user='the-user',
     catalog='the-catalog',
     schema='the-schema',
 )
-await cur = conn.cursor()
+cur = await conn.cursor()
 await cur.execute('SELECT * FROM system.runtime.nodes')
 rows = await cur.fetchall()
 await conn.close()
 ```
 Or with context manager 
 ```python
 import aiotrino
 async with aiotrino.dbapi.connect(
     host='localhost',
     port=8080,
     user='the-user',
     catalog='the-catalog',
     schema='the-schema',
 ) as conn:
-    await cur = conn.cursor()
+    cur = await conn.cursor()
     await cur.execute('SELECT * FROM system.runtime.nodes')
     rows = await cur.fetchall()
 ```
 
 This will query the `system.runtime.nodes` system tables that shows the nodes
 in the Trino cluster.
 
@@ -191,15 +191,15 @@
 - When writing a Git commit message, follow these [guidelines](https://chris.beams.io/posts/git-commit/).
 
 ## Running Tests
 
 There is a helper scripts, `run`, that provides commands to run tests.
 Type `./run tests` to run both unit and integration tests.
 
-`trino-python-client` uses [pytest](https://pytest.org/) for its tests. To run
+`aiotrino` uses [pytest](https://pytest.org/) for its tests. To run
 only unit tests, type:
 
 ```
 $ pytest tests
 ```
 
 Then you can pass options like `--pdb` or anything supported by `pytest --help`.
@@ -215,15 +215,15 @@
 
 ```
 $ pytest integration_tests
 ```
 
 They pull a Docker image and then run a container with a Trino server:
 - the image is named `trinodb/trino:${TRINO_VERSION}`
-- the container is named `trino-python-client-tests-{uuid4()[:7]}`
+- the container is named `aiotrino-python-client-tests-{uuid4()[:7]}`
 
 
 ### Test setup
 
 Supported OS Ubuntu 22.04
 
 1. Install [pyenv](https://github.com/pyenv/pyenv#automatic-installer)
@@ -261,24 +261,24 @@
     ```shell
     tox
     ```
 
 ## Releasing
 
 - [Set up your development environment](#Getting-Started-With-Development).
-- Change version in `trino/__init__.py`.
+- Change version in `aiotrino/__init__.py`.
 - Commit and create an annotated tag (`git tag -m '' current_version`)
 - Run the following:
   ```bash
   . .venv/bin/activate &&
   pip install twine wheel &&
   rm -rf dist/ &&
   ./setup.py sdist bdist_wheel &&
   twine upload dist/* &&
-  open https://pypi.org/project/trino/ &&
+  open https://pypi.org/project/aiotrino/ &&
   echo "Released!"
   ```
 - Push the branch and the tag (`git push upstream master current_version`)
 - Send release announcement.
 
 # Need Help?
```

### Comparing `aiotrino-0.2.1/setup.py` & `aiotrino-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `aiotrino-0.2.1/tests/test_client.py` & `aiotrino-0.2.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aiotrino-0.2.1/tests/test_exceptions.py` & `aiotrino-0.2.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotrino-0.2.1/tests/test_http.py` & `aiotrino-0.2.2/tests/test_http.py`

 * *Files identical despite different names*

