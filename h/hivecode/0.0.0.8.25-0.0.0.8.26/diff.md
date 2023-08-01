# Comparing `tmp/hivecode-0.0.0.8.25.tar.gz` & `tmp/hivecode-0.0.0.8.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivecode-0.0.0.8.25.tar", last modified: Tue Aug  1 05:26:27 2023, max compression
+gzip compressed data, was "hivecode-0.0.0.8.26.tar", last modified: Tue Aug  1 05:29:09 2023, max compression
```

## Comparing `hivecode-0.0.0.8.25.tar` & `hivecode-0.0.0.8.26.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 05:26:27.907527 hivecode-0.0.0.8.25/
--rw-rw-rw-   0        0        0     1103 2023-07-31 00:53:19.000000 hivecode-0.0.0.8.25/LICENSE
--rw-rw-rw-   0        0        0     3683 2023-08-01 05:26:27.908028 hivecode-0.0.0.8.25/PKG-INFO
--rw-rw-rw-   0        0        0     2818 2023-07-31 00:51:24.000000 hivecode-0.0.0.8.25/README.rst
--rw-rw-rw-   0        0        0     1261 2023-08-01 05:16:42.000000 hivecode-0.0.0.8.25/pyproject.toml
--rw-rw-rw-   0        0        0      249 2023-08-01 04:30:01.000000 hivecode-0.0.0.8.25/requirements.txt
--rw-rw-rw-   0        0        0     1182 2023-08-01 05:26:27.914042 hivecode-0.0.0.8.25/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.25/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 05:26:27.866381 hivecode-0.0.0.8.25/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 05:26:27.873931 hivecode-0.0.0.8.25/src/hiveadb/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.25/src/hiveadb/__init__.py
--rw-rw-rw-   0        0        0    13818 2023-08-01 05:13:10.000000 hivecode-0.0.0.8.25/src/hiveadb/functions.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.25/src/hiveadb/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-01 05:26:27.895585 hivecode-0.0.0.8.25/src/hivecode.egg-info/
--rw-rw-rw-   0        0        0     3683 2023-08-01 05:26:27.000000 hivecode-0.0.0.8.25/src/hivecode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      678 2023-08-01 05:26:27.000000 hivecode-0.0.0.8.25/src/hivecode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 05:26:27.000000 hivecode-0.0.0.8.25/src/hivecode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.25/src/hivecode.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      336 2023-08-01 05:26:27.000000 hivecode-0.0.0.8.25/src/hivecode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-08-01 05:26:27.000000 hivecode-0.0.0.8.25/src/hivecode.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 05:26:27.901950 hivecode-0.0.0.8.25/src/hivecore/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.25/src/hivecore/__init__.py
--rw-rw-rw-   0        0        0     1330 2023-05-08 01:20:28.000000 hivecode-0.0.0.8.25/src/hivecore/constant.py
--rw-rw-rw-   0        0        0     9402 2023-07-15 21:48:03.000000 hivecode-0.0.0.8.25/src/hivecore/decorator.py
--rw-rw-rw-   0        0        0    11298 2023-07-30 23:04:15.000000 hivecode-0.0.0.8.25/src/hivecore/functions.py
--rw-rw-rw-   0        0        0    32180 2023-07-26 05:19:59.000000 hivecode-0.0.0.8.25/src/hivecore/patterns.py
--rw-rw-rw-   0        0        0    31989 2023-07-30 23:56:16.000000 hivecode-0.0.0.8.25/src/hivecore/preprocess.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.25/src/hivecore/py.typed
-drwxrwxrwx   0        0        0        0 2023-08-01 05:26:27.906526 hivecode-0.0.0.8.25/src/hivesignal/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.25/src/hivesignal/__init__.py
--rw-rw-rw-   0        0        0     1683 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.25/src/hivesignal/analysis.py
--rw-rw-rw-   0        0        0      292 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.25/src/hivesignal/eda.py
--rw-rw-rw-   0        0        0     2383 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.25/src/hivesignal/io.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.25/src/hivesignal/py.typed
--rw-rw-rw-   0        0        0     2126 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.25/src/hivesignal/transform.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:29:09.822948 hivecode-0.0.0.8.26/
+-rw-rw-rw-   0        0        0     1103 2023-07-31 00:53:19.000000 hivecode-0.0.0.8.26/LICENSE
+-rw-rw-rw-   0        0        0     3683 2023-08-01 05:29:09.822948 hivecode-0.0.0.8.26/PKG-INFO
+-rw-rw-rw-   0        0        0     2818 2023-07-31 00:51:24.000000 hivecode-0.0.0.8.26/README.rst
+-rw-rw-rw-   0        0        0     1261 2023-08-01 05:28:57.000000 hivecode-0.0.0.8.26/pyproject.toml
+-rw-rw-rw-   0        0        0      249 2023-08-01 04:30:01.000000 hivecode-0.0.0.8.26/requirements.txt
+-rw-rw-rw-   0        0        0     1182 2023-08-01 05:29:09.824459 hivecode-0.0.0.8.26/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.26/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 05:29:09.779412 hivecode-0.0.0.8.26/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 05:29:09.795759 hivecode-0.0.0.8.26/src/hiveadb/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.26/src/hiveadb/__init__.py
+-rw-rw-rw-   0        0        0    13822 2023-08-01 05:28:39.000000 hivecode-0.0.0.8.26/src/hiveadb/functions.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.26/src/hiveadb/py.typed
+drwxrwxrwx   0        0        0        0 2023-08-01 05:29:09.809318 hivecode-0.0.0.8.26/src/hivecode.egg-info/
+-rw-rw-rw-   0        0        0     3683 2023-08-01 05:29:09.000000 hivecode-0.0.0.8.26/src/hivecode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      678 2023-08-01 05:29:09.000000 hivecode-0.0.0.8.26/src/hivecode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 05:29:09.000000 hivecode-0.0.0.8.26/src/hivecode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.26/src/hivecode.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      336 2023-08-01 05:29:09.000000 hivecode-0.0.0.8.26/src/hivecode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-08-01 05:29:09.000000 hivecode-0.0.0.8.26/src/hivecode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 05:29:09.815363 hivecode-0.0.0.8.26/src/hivecore/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.26/src/hivecore/__init__.py
+-rw-rw-rw-   0        0        0     1330 2023-05-08 01:20:28.000000 hivecode-0.0.0.8.26/src/hivecore/constant.py
+-rw-rw-rw-   0        0        0     9402 2023-07-15 21:48:03.000000 hivecode-0.0.0.8.26/src/hivecore/decorator.py
+-rw-rw-rw-   0        0        0    11298 2023-07-30 23:04:15.000000 hivecode-0.0.0.8.26/src/hivecore/functions.py
+-rw-rw-rw-   0        0        0    32180 2023-07-26 05:19:59.000000 hivecode-0.0.0.8.26/src/hivecore/patterns.py
+-rw-rw-rw-   0        0        0    31989 2023-07-30 23:56:16.000000 hivecode-0.0.0.8.26/src/hivecore/preprocess.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.26/src/hivecore/py.typed
+drwxrwxrwx   0        0        0        0 2023-08-01 05:29:09.821400 hivecode-0.0.0.8.26/src/hivesignal/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.26/src/hivesignal/__init__.py
+-rw-rw-rw-   0        0        0     1683 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.26/src/hivesignal/analysis.py
+-rw-rw-rw-   0        0        0      292 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.26/src/hivesignal/eda.py
+-rw-rw-rw-   0        0        0     2383 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.26/src/hivesignal/io.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.26/src/hivesignal/py.typed
+-rw-rw-rw-   0        0        0     2126 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.26/src/hivesignal/transform.py
```

### Comparing `hivecode-0.0.0.8.25/LICENSE` & `hivecode-0.0.0.8.26/LICENSE`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.25/PKG-INFO` & `hivecode-0.0.0.8.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hivecode
-Version: 0.0.0.8.25
+Version: 0.0.0.8.26
 Summary: Hivecode is a versatile and comprehensive Python library, with a focus on efficiency and reusability, Hivecode empowers developers and data enthusiasts alike to streamline their projects.
 Author: Juan Manuel Mejía Botero
 Author-email: Juan Manuel Mejía Botero <juanmam941025@gmail.com>, Sebastian López Valencia <sebaslv12@hotmail.com>
 Project-URL: Homepage, https://github.com/Juanmam/hivecode
 Project-URL: Documentation, https://hivecode.readthedocs.io/en/latest/
 Platform: unix
 Platform: linux
```

### Comparing `hivecode-0.0.0.8.25/README.rst` & `hivecode-0.0.0.8.26/README.rst`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.25/pyproject.toml` & `hivecode-0.0.0.8.26/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "hivecode"
 description = "Hivecode is a versatile and comprehensive Python library, with a focus on efficiency and reusability, Hivecode empowers developers and data enthusiasts alike to streamline their projects."
-version = "0.0.0.8.25"
+version = "0.0.0.8.26"
 requires-python = ">=3.8.0"
 readme = "README.rst"
 authors = [
     {name = "Juan Manuel Mejía Botero", email="juanmam941025@gmail.com"},
     {name = "Sebastian López Valencia", email="sebaslv12@hotmail.com"}
 ]
```

### Comparing `hivecode-0.0.0.8.25/setup.cfg` & `hivecode-0.0.0.8.26/setup.cfg`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.25/src/hiveadb/functions.py` & `hivecode-0.0.0.8.26/src/hiveadb/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         - read_secret: Read the value of a secret from Azure Databricks.
         - read_scope: List all secrets within a specific scope in Azure Databricks.
         - list_secrets: List all secrets along with their corresponding scopes in Azure Databricks.
         - list_scopes: List all secret scopes in Azure Databricks.
         - delete_secret: Delete a secret from a specific scope in Azure Databricks.
         - delete_scope: Delete a secret scope in Azure Databricks.
     """
-    def _init_(self, token: str):
+    def __init__(self, token: str):
         self._token = token
         self.workspace_host = spark.conf.get("spark.databricks.workspaceUrl")
         self._databricks_api = DatabricksAPI(host=self.workspace_host, token=self._token)
 
     def create_secret(self, scope: str = None, key: str = None, value: str = None) -> None:
         """
         Store a secret in Azure Databricks.
@@ -263,15 +263,15 @@
     :methods:
         - create_token: Creates a new token with the given token_name and stores it in the token list.
         - get_token: Retrieves the dictionary of a token based on its name.
         - delete_token: Deletes a token based on its name.
         - list_tokens: Retrieves a dictionary containing all the tokens organized by scopes.
     """
 
-    def _init_(self, token: str, token_name: str = "temp_token"):
+    def __init__(self, token: str, token_name: str = "temp_token"):
         self._token = token
         self.workspace_host = spark.conf.get("spark.databricks.workspaceUrl")
         self._databricks_api = DatabricksAPI(host=self.workspace_host, token=self._token)
         self._tokens = list(chain.from_iterable(list(self.list_tokens().values())))
 
         def update_token(tkn):
             """
```

### Comparing `hivecode-0.0.0.8.25/src/hivecode.egg-info/PKG-INFO` & `hivecode-0.0.0.8.26/src/hivecode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hivecode
-Version: 0.0.0.8.25
+Version: 0.0.0.8.26
 Summary: Hivecode is a versatile and comprehensive Python library, with a focus on efficiency and reusability, Hivecode empowers developers and data enthusiasts alike to streamline their projects.
 Author: Juan Manuel Mejía Botero
 Author-email: Juan Manuel Mejía Botero <juanmam941025@gmail.com>, Sebastian López Valencia <sebaslv12@hotmail.com>
 Project-URL: Homepage, https://github.com/Juanmam/hivecode
 Project-URL: Documentation, https://hivecode.readthedocs.io/en/latest/
 Platform: unix
 Platform: linux
```

### Comparing `hivecode-0.0.0.8.25/src/hivecode.egg-info/SOURCES.txt` & `hivecode-0.0.0.8.26/src/hivecode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.25/src/hivecore/constant.py` & `hivecode-0.0.0.8.26/src/hivecore/constant.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.25/src/hivecore/decorator.py` & `hivecode-0.0.0.8.26/src/hivecore/decorator.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.25/src/hivecore/functions.py` & `hivecode-0.0.0.8.26/src/hivecore/functions.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.25/src/hivecore/patterns.py` & `hivecode-0.0.0.8.26/src/hivecore/patterns.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.25/src/hivecore/preprocess.py` & `hivecode-0.0.0.8.26/src/hivecore/preprocess.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.25/src/hivesignal/analysis.py` & `hivecode-0.0.0.8.26/src/hivesignal/analysis.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.25/src/hivesignal/io.py` & `hivecode-0.0.0.8.26/src/hivesignal/io.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.25/src/hivesignal/transform.py` & `hivecode-0.0.0.8.26/src/hivesignal/transform.py`

 * *Files identical despite different names*

