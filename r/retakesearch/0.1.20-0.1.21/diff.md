# Comparing `tmp/retakesearch-0.1.20.tar.gz` & `tmp/retakesearch-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retakesearch-0.1.20.tar", max compression
+gzip compressed data, was "retakesearch-0.1.21.tar", max compression
```

## Comparing `retakesearch-0.1.20.tar` & `retakesearch-0.1.21.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-31 23:41:14.051745 retakesearch-0.1.20/README.md
--rw-r--r--   0        0        0      429 2023-07-31 23:41:31.127879 retakesearch-0.1.20/pyproject.toml
--rw-r--r--   0        0        0      174 2023-07-31 23:41:14.051745 retakesearch-0.1.20/retakesearch/__init__.py
--rw-r--r--   0        0        0     1818 2023-07-31 23:41:14.051745 retakesearch-0.1.20/retakesearch/client.py
--rw-r--r--   0        0        0     3796 2023-07-31 23:41:14.051745 retakesearch-0.1.20/retakesearch/index.py
--rw-r--r--   0        0        0      159 2023-07-31 23:41:14.051745 retakesearch-0.1.20/retakesearch/search.py
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 retakesearch-0.1.20/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-01 20:36:29.423604 retakesearch-0.1.21/README.md
+-rw-r--r--   0        0        0      429 2023-08-01 20:36:54.251646 retakesearch-0.1.21/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-08-01 20:36:29.423604 retakesearch-0.1.21/retakesearch/__init__.py
+-rw-r--r--   0        0        0     1818 2023-08-01 20:36:29.423604 retakesearch-0.1.21/retakesearch/client.py
+-rw-r--r--   0        0        0     3687 2023-08-01 20:36:29.423604 retakesearch-0.1.21/retakesearch/index.py
+-rw-r--r--   0        0        0      159 2023-08-01 20:36:29.423604 retakesearch-0.1.21/retakesearch/search.py
+-rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 retakesearch-0.1.21/PKG-INFO
```

### Comparing `retakesearch-0.1.20/retakesearch/client.py` & `retakesearch-0.1.21/retakesearch/client.py`

 * *Files identical despite different names*

### Comparing `retakesearch-0.1.20/retakesearch/index.py` & `retakesearch-0.1.21/retakesearch/index.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,25 +70,22 @@
                 raise Exception(response.text)
 
     def upsert(
         self, documents: List[Dict[str, Any]], ids: List[Union[str, int]]
     ) -> Any:
         json = {"index_name": self.index_name, "documents": documents, "ids": ids}
 
-        try:
-            with httpx.Client(timeout=None) as http:
-                response = http.post(
-                    f"{self.url}/index/upsert", headers=self.headers, json=json
-                )
-                response.raise_for_status()
+        with httpx.Client(timeout=None) as http:
+            response = http.post(
+                f"{self.url}/index/upsert", headers=self.headers, json=json
+            )
+            if response.status_code == 200:
                 return response.json()
-        except httpx.HTTPStatusError as exc:
-            return exc.response.json()
-        except Exception as exc:
-            return str(exc)
+            else:
+                raise Exception(response.text)
 
     def create_field(self, field_name: str, field_type: str) -> None:
         json = {
             "index_name": self.index_name,
             "field_name": field_name,
             "field_type": field_type,
         }
```

### Comparing `retakesearch-0.1.20/PKG-INFO` & `retakesearch-0.1.21/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retakesearch
-Version: 0.1.20
+Version: 0.1.21
 Summary: Python client for Retake: universal search infra for developers
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

