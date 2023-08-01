# Comparing `tmp/sgd_rest-0.0.2.tar.gz` & `tmp/sgd_rest-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgd_rest-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sgd_rest-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sgd_rest-0.0.2.tar` & `sgd_rest-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       83 2023-07-28 20:05:08.942291 sgd_rest-0.0.2/.flake8
--rw-r--r--   0        0        0      170 2023-07-29 16:32:47.775361 sgd_rest-0.0.2/.github/dependabot.yaml
--rw-r--r--   0        0        0      635 2023-07-29 16:33:55.841454 sgd_rest-0.0.2/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     3078 2023-07-26 19:12:59.055162 sgd_rest-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2023-07-26 19:12:59.055317 sgd_rest-0.0.2/LICENSE
--rw-r--r--   0        0        0      897 2023-07-28 20:07:26.866494 sgd_rest-0.0.2/Makefile
--rw-r--r--   0        0        0     5086 2023-07-29 17:03:15.468772 sgd_rest-0.0.2/README.md
--rw-r--r--   0        0        0       26 2023-07-28 19:54:17.063480 sgd_rest-0.0.2/conftest.py
--rw-r--r--   0        0        0      791 2023-07-29 16:36:20.929255 sgd_rest-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       32 2023-07-28 16:33:46.903493 sgd_rest-0.0.2/requirements-dev.txt
--rw-r--r--   0        0        0        9 2023-07-28 16:32:29.411112 sgd_rest-0.0.2/requirements.txt
--rw-r--r--   0        0        0     1169 2023-07-29 16:34:04.470794 sgd_rest-0.0.2/setup.cfg
--rw-r--r--   0        0        0      114 2023-07-29 17:05:13.554796 sgd_rest-0.0.2/sgd/__init__.py
--rw-r--r--   0        0        0     8091 2023-07-28 20:08:01.613736 sgd_rest-0.0.2/sgd/api.py
--rw-r--r--   0        0        0      225 2023-07-28 19:59:01.313282 sgd_rest-0.0.2/sgd/constants.py
--rw-r--r--   0        0        0   305093 2023-07-26 19:44:32.597219 sgd_rest-0.0.2/sgd/data/genes_to_loci.json
--rw-r--r--   0        0        0      109 2023-07-28 19:53:17.407918 sgd_rest-0.0.2/sgd/exceptions.py
--rw-r--r--   0        0        0     4871 2023-07-28 19:53:17.391282 sgd_rest-0.0.2/tests/test_api.py
--rw-r--r--   0        0        0      814 2023-07-28 20:18:05.241377 sgd_rest-0.0.2/tests/test_constants.py
--rw-r--r--   0        0        0      285 2023-07-28 19:54:08.182118 sgd_rest-0.0.2/tests/test_exceptions.py
--rw-r--r--   0        0        0     5829 1970-01-01 00:00:00.000000 sgd_rest-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       83 2023-07-28 20:05:08.942291 sgd_rest-0.0.3/.flake8
+-rw-r--r--   0        0        0      170 2023-07-29 16:32:47.775361 sgd_rest-0.0.3/.github/dependabot.yaml
+-rw-r--r--   0        0        0      635 2023-07-29 16:33:55.841454 sgd_rest-0.0.3/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     3078 2023-07-26 19:12:59.055162 sgd_rest-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2023-07-26 19:12:59.055317 sgd_rest-0.0.3/LICENSE
+-rw-r--r--   0        0        0      897 2023-07-28 20:07:26.866494 sgd_rest-0.0.3/Makefile
+-rw-r--r--   0        0        0     5084 2023-08-01 18:30:43.297909 sgd_rest-0.0.3/README.md
+-rw-r--r--   0        0        0       26 2023-07-28 19:54:17.063480 sgd_rest-0.0.3/conftest.py
+-rw-r--r--   0        0        0      791 2023-07-29 16:36:20.929255 sgd_rest-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-07-28 16:33:46.903493 sgd_rest-0.0.3/requirements-dev.txt
+-rw-r--r--   0        0        0        9 2023-07-28 16:32:29.411112 sgd_rest-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     1169 2023-07-29 16:34:04.470794 sgd_rest-0.0.3/setup.cfg
+-rw-r--r--   0        0        0      114 2023-08-01 18:31:25.472215 sgd_rest-0.0.3/sgd/__init__.py
+-rw-r--r--   0        0        0     8091 2023-08-01 04:05:34.749868 sgd_rest-0.0.3/sgd/api.py
+-rw-r--r--   0        0        0      225 2023-07-28 19:59:01.313282 sgd_rest-0.0.3/sgd/constants.py
+-rw-r--r--   0        0        0   305093 2023-07-26 19:44:32.597219 sgd_rest-0.0.3/sgd/data/genes_to_loci.json
+-rw-r--r--   0        0        0      109 2023-07-28 19:53:17.407918 sgd_rest-0.0.3/sgd/exceptions.py
+-rw-r--r--   0        0        0     4871 2023-07-31 15:09:59.956223 sgd_rest-0.0.3/tests/test_api.py
+-rw-r--r--   0        0        0      818 2023-07-31 15:09:44.015174 sgd_rest-0.0.3/tests/test_constants.py
+-rw-r--r--   0        0        0      285 2023-07-28 19:54:08.182118 sgd_rest-0.0.3/tests/test_exceptions.py
+-rw-r--r--   0        0        0     5827 1970-01-01 00:00:00.000000 sgd_rest-0.0.3/PKG-INFO
```

### Comparing `sgd_rest-0.0.2/.github/workflows/ci.yaml` & `sgd_rest-0.0.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.2/.gitignore` & `sgd_rest-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.2/LICENSE` & `sgd_rest-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.2/Makefile` & `sgd_rest-0.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.2/README.md` & `sgd_rest-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 import sgd
 
 aro1 = sgd.gene("ARO1")
 ```
 
 ### Subclasses
 
-Use the `endpoints` attribute to query a class's subclasses:
+Use the `endpoints` attribute to search a class's subclasses:
 
 ```python
 import sgd
 
 print(sgd.gene.endpoints)
 ```
 
@@ -69,24 +69,24 @@
 | `locus` & `gene` | `regulation_details` | Gets regulation annotations and the references used to make them.
 | `locus` & `gene` | `sequence_details` | Gets sequence for genomic, coding, protein, and +/- 1KB sequence.
 | `phenotype` | `details` | Gets basic information about a phenotype.
 | `phenotype` | `locus_details` | Gets a list of genes annotated to a phenotype with some information about the experiment and strain background.
 | `go` | `details` | Gets basic information about a GO term.
 | `go` | `locus_details` | Gets a list of genes annotated to a GO term.
 
-Use a subclass to retrieve the endpoint's response. This library utilizes the [`requests`](https://github.com/psf/requests) library, returning a `requests.models.Response` instance by default. Use this instance to define the desired processing of the REST API content.
+Use a subclass to retrieve the endpoint's response. This library utilizes the [`requests`](https://github.com/psf/requests) library, returning a `requests.models.Response` instance. Use this instance to define the desired processing of the REST API content.
 
-For example, get GO details and literature details for the gene ARO1 as JSON:
+For example, for the gene ARO1, get GO details as JSON and literature details as text:
 
 ```python
 import sgd
 
 aro1 = sgd.gene("ARO1")
 aro1.go_details.json()
-aro1.literature_details.json()
+aro1.literature_details.text
 ```
 
 ## Advanced
 
 Just like a subclass returns a `requests.models.Response` instance, the user can pass keyword arguments directly to the `requests.get` method during class instantiation. For example, you can add a header to prevent server-side caching and parse the locus details response as text:
 
 ```python
@@ -136,8 +136,8 @@
 
 ## Support
 
 If you are having issues or would like to propose a new feature, please use the [issues tracker](https://github.com/irahorecka/sgd-rest/issues).
 
 ## License
 
-The project is licensed under the MIT license.
+This project is licensed under the MIT license.
```

### Comparing `sgd_rest-0.0.2/pyproject.toml` & `sgd_rest-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.2/setup.cfg` & `sgd_rest-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.2/sgd/api.py` & `sgd_rest-0.0.3/sgd/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     @lru_cache(maxsize=64)
     def _get_endpoint_response(self):
         """Gets response for an endpoint.
 
         Returns:
             requests.models.Response: Endpoint response.
         """
-        response = requests.get(self.url, **self._kwargs, timeout=60)
+        response = requests.get(self.url, timeout=60, **self._kwargs)
         response.raise_for_status()
         return response
 
 
 class locus(BaseAPI):
     """SGD REST locus API."""
```

### Comparing `sgd_rest-0.0.2/sgd/data/genes_to_loci.json` & `sgd_rest-0.0.3/sgd/data/genes_to_loci.json`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.2/tests/test_api.py` & `sgd_rest-0.0.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sgd_rest-0.0.2/tests/test_constants.py` & `sgd_rest-0.0.3/tests/test_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from sgd.constants import GENES_TO_LOCI
 
 
 # fmt: off
 sgd_instances = (
     sgd.locus('S000002534'),
     sgd.gene('ARO1'),
-    sgd.phenotype('increased_chemical_compound_accumulation'), sgd.go('GO:0000001'),
+    sgd.phenotype('increased_chemical_compound_accumulation'),
+    sgd.go('GO:0000001'),
 )
 # fmt: on
 @mark.parametrize("instance", sgd_instances)
 def test_endpoints(instance):
     """Tests proper return of SGD REST endpoints.
 
     Args:
```

### Comparing `sgd_rest-0.0.2/PKG-INFO` & `sgd_rest-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgd-rest
-Version: 0.0.2
+Version: 0.0.3
 Summary: sgd
 Home-page: https://github.com/irahorecka/sgd-rest
 Author: Ira Horecka
 Author-email: ira89@icloud.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
@@ -64,15 +64,15 @@
 import sgd
 
 aro1 = sgd.gene("ARO1")
 ```
 
 ### Subclasses
 
-Use the `endpoints` attribute to query a class's subclasses:
+Use the `endpoints` attribute to search a class's subclasses:
 
 ```python
 import sgd
 
 print(sgd.gene.endpoints)
 ```
 
@@ -90,24 +90,24 @@
 | `locus` & `gene` | `regulation_details` | Gets regulation annotations and the references used to make them.
 | `locus` & `gene` | `sequence_details` | Gets sequence for genomic, coding, protein, and +/- 1KB sequence.
 | `phenotype` | `details` | Gets basic information about a phenotype.
 | `phenotype` | `locus_details` | Gets a list of genes annotated to a phenotype with some information about the experiment and strain background.
 | `go` | `details` | Gets basic information about a GO term.
 | `go` | `locus_details` | Gets a list of genes annotated to a GO term.
 
-Use a subclass to retrieve the endpoint's response. This library utilizes the [`requests`](https://github.com/psf/requests) library, returning a `requests.models.Response` instance by default. Use this instance to define the desired processing of the REST API content.
+Use a subclass to retrieve the endpoint's response. This library utilizes the [`requests`](https://github.com/psf/requests) library, returning a `requests.models.Response` instance. Use this instance to define the desired processing of the REST API content.
 
-For example, get GO details and literature details for the gene ARO1 as JSON:
+For example, for the gene ARO1, get GO details as JSON and literature details as text:
 
 ```python
 import sgd
 
 aro1 = sgd.gene("ARO1")
 aro1.go_details.json()
-aro1.literature_details.json()
+aro1.literature_details.text
 ```
 
 ## Advanced
 
 Just like a subclass returns a `requests.models.Response` instance, the user can pass keyword arguments directly to the `requests.get` method during class instantiation. For example, you can add a header to prevent server-side caching and parse the locus details response as text:
 
 ```python
@@ -157,9 +157,9 @@
 
 ## Support
 
 If you are having issues or would like to propose a new feature, please use the [issues tracker](https://github.com/irahorecka/sgd-rest/issues).
 
 ## License
 
-The project is licensed under the MIT license.
+This project is licensed under the MIT license.
```

