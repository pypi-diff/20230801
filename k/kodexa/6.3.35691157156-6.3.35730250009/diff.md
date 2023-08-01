# Comparing `tmp/kodexa-6.3.35691157156.tar.gz` & `tmp/kodexa-6.3.35730250009.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-6.3.35691157156.tar", max compression
+gzip compressed data, was "kodexa-6.3.35730250009.tar", max compression
```

## Comparing `kodexa-6.3.35691157156.tar` & `kodexa-6.3.35730250009.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11357 2023-07-28 10:54:19.622015 kodexa-6.3.35691157156/LICENSE
--rw-r--r--   0        0        0     2804 2023-07-28 10:54:19.622015 kodexa-6.3.35691157156/README.md
--rw-r--r--   0        0        0      847 2023-07-28 10:54:19.630015 kodexa-6.3.35691157156/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2023-07-28 10:54:19.630015 kodexa-6.3.35691157156/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    12530 2023-07-28 10:54:19.630015 kodexa-6.3.35691157156/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      297 2023-07-28 10:54:19.630015 kodexa-6.3.35691157156/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0     7722 2023-07-28 10:54:19.630015 kodexa-6.3.35691157156/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      720 2023-07-28 10:54:19.630015 kodexa-6.3.35691157156/kodexa/model/__init__.py
--rw-r--r--   0        0        0      906 2023-07-28 10:54:19.630015 kodexa-6.3.35691157156/kodexa/model/base.py
--rw-r--r--   0        0        0    97073 2023-07-28 10:54:19.630015 kodexa-6.3.35691157156/kodexa/model/model.py
--rw-r--r--   0        0        0   118389 2023-07-28 10:54:19.630015 kodexa-6.3.35691157156/kodexa/model/objects.py
--rw-r--r--   0        0        0    38816 2023-07-28 10:54:19.630015 kodexa-6.3.35691157156/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2023-07-28 10:54:19.630015 kodexa-6.3.35691157156/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    19505 2023-07-28 10:54:19.630015 kodexa-6.3.35691157156/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2023-07-28 10:54:19.630015 kodexa-6.3.35691157156/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   111395 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/platform/client.py
--rw-r--r--   0        0        0    28288 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13499 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3698 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3735 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     2354 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       60 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7054 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       60 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    21267 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       60 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    18991 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     2738 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    34222 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      160 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/steps/__init__.py
--rw-r--r--   0        0        0     9587 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/steps/common.py
--rw-r--r--   0        0        0      159 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/testing/__init__.py
--rw-r--r--   0        0        0      932 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    13596 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 10:54:19.634016 kodexa-6.3.35691157156/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1279 2023-07-28 10:54:38.283686 kodexa-6.3.35691157156/pyproject.toml
--rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 kodexa-6.3.35691157156/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-01 18:01:53.732766 kodexa-6.3.35730250009/LICENSE
+-rw-r--r--   0        0        0     2804 2023-08-01 18:01:53.732766 kodexa-6.3.35730250009/README.md
+-rw-r--r--   0        0        0      847 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    12530 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      297 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0     7722 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      720 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      906 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/model/base.py
+-rw-r--r--   0        0        0    97073 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/model/model.py
+-rw-r--r--   0        0        0   118389 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/model/objects.py
+-rw-r--r--   0        0        0    38816 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    19505 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   111293 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/platform/client.py
+-rw-r--r--   0        0        0    28288 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13499 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3698 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3735 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     2354 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       60 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7054 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       60 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    21267 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       60 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    18991 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     2738 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    34222 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      160 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0     9587 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/steps/common.py
+-rw-r--r--   0        0        0      159 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0      932 2023-08-01 18:01:53.740767 kodexa-6.3.35730250009/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    13596 2023-08-01 18:01:53.744767 kodexa-6.3.35730250009/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2023-08-01 18:01:53.744767 kodexa-6.3.35730250009/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 18:01:53.744767 kodexa-6.3.35730250009/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1279 2023-08-01 18:02:10.957164 kodexa-6.3.35730250009/pyproject.toml
+-rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 kodexa-6.3.35730250009/PKG-INFO
```

### Comparing `kodexa-6.3.35691157156/LICENSE` & `kodexa-6.3.35730250009/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/README.md` & `kodexa-6.3.35730250009/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/__init__.py` & `kodexa-6.3.35730250009/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/assistant/assistant.py` & `kodexa-6.3.35730250009/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/connectors/connectors.py` & `kodexa-6.3.35730250009/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/model/__init__.py` & `kodexa-6.3.35730250009/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/model/base.py` & `kodexa-6.3.35730250009/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/model/model.py` & `kodexa-6.3.35730250009/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/model/objects.py` & `kodexa-6.3.35730250009/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/model/persistence.py` & `kodexa-6.3.35730250009/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/pipeline/pipeline.py` & `kodexa-6.3.35730250009/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/platform/client.py` & `kodexa-6.3.35730250009/kodexa/platform/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,17 +207,17 @@
     def find_by_slug(self, slug, version=None):
         """
         Find a component by slug
         :param slug:
         :param version:
         :return:
         """
-        filters = ["slug=" + slug]
+        filters = ["slug: '" + slug + "'"]
         if version is not None:
-            filters.append("version=" + version)
+            filters.append("version: '" + version + "'")
         component_page = self.list(filters=filters)
         if component_page.empty:
             return None
         return component_page.content[0]
 
     def stream_list(self, query="*", page=1, page_size=10, sort=None, filters: List[str] = None):
         url = f"/api/{self.get_type()}/{self.organization.slug}"
@@ -226,15 +226,14 @@
                   "page": page,
                   "pageSize": page_size}
 
         if sort is not None:
             params["sort"] = sort
 
         if filters is not None:
-            params["legacyFilter"] = True
             params["filter"] = filters
 
         while True:
             list_response = self.client.get(url, params=params)
 
             # If there are no more results, exit the loop
             if not list_response.json()["content"]:
@@ -255,15 +254,14 @@
                   "page": page,
                   "pageSize": page_size}
 
         if sort is not None:
             params["sort"] = sort
 
         if filters is not None:
-            params["legacyFilter"] = True
             params["filter"] = filters
 
         list_response = self.client.get(url, params=params)
         return self.get_page_class(list_response.json()).model_validate(list_response.json()).set_client(
             self.client).to_endpoints()
 
     def create(self, component):
@@ -376,15 +374,14 @@
                   "page": page,
                   "pageSize": page_size}
 
         if sort is not None:
             params["sort"] = sort
 
         if filters is not None:
-            params["legacyFilter"] = True
             params["filter"] = filters
 
         if self.organization is not None:
             if 'filter' not in params:
                 params['filter'] = [f"organization.id: '{self.organization.id}'"]
             else:
                 params['filter'].append(f"organization.id={self.organization.id}")
@@ -433,15 +430,15 @@
 
     def find_by_slug(self, slug) -> Optional["OrganizationEndpoint"]:
         """
         Find an organization by slug
         :param slug:
         :return:
         """
-        organizations = self.list(filters=["slug=" + slug])
+        organizations = self.list(filters=["slug: '" + slug + "'"])
         if organizations.number_of_elements == 0:
             return None
         return organizations.content[0]
 
 
 class PageEndpoint(ClientEndpoint):
     """
```

### Comparing `kodexa-6.3.35691157156/kodexa/platform/kodexa.py` & `kodexa-6.3.35730250009/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/selectors/ast.py` & `kodexa-6.3.35730250009/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/selectors/core.py` & `kodexa-6.3.35730250009/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/selectors/lexrules.py` & `kodexa-6.3.35730250009/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/selectors/lextab.py` & `kodexa-6.3.35730250009/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/selectors/parserules.py` & `kodexa-6.3.35730250009/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/selectors/parsetab.py` & `kodexa-6.3.35730250009/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/spatial/azure_models.py` & `kodexa-6.3.35730250009/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/spatial/bbox_common.py` & `kodexa-6.3.35730250009/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/spatial/table_form_common.py` & `kodexa-6.3.35730250009/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/steps/common.py` & `kodexa-6.3.35730250009/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/testing/test_components.py` & `kodexa-6.3.35730250009/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/kodexa/testing/test_utils.py` & `kodexa-6.3.35730250009/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35691157156/pyproject.toml` & `kodexa-6.3.35730250009/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "6.3.35691157156"
+version = "6.3.35730250009"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-6.3.35691157156/PKG-INFO` & `kodexa-6.3.35730250009/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 6.3.35691157156
+Version: 6.3.35730250009
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

