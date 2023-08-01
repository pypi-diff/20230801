# Comparing `tmp/operatorio-0.1.8.tar.gz` & `tmp/operatorio-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operatorio-0.1.8.tar", last modified: Thu Jul 27 19:52:55 2023, max compression
+gzip compressed data, was "operatorio-0.1.9.tar", last modified: Tue Aug  1 07:29:05 2023, max compression
```

## Comparing `operatorio-0.1.8.tar` & `operatorio-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-27 19:52:55.485983 operatorio-0.1.8/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-27 19:52:55.485751 operatorio-0.1.8/PKG-INFO
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-27 19:52:55.484546 operatorio-0.1.8/operatorio/
--rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.1.8/operatorio/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     1914 2023-07-27 19:51:26.000000 operatorio-0.1.8/operatorio/main.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-27 19:52:55.485506 operatorio-0.1.8/operatorio.egg-info/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-27 19:52:55.000000 operatorio-0.1.8/operatorio.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      219 2023-07-27 19:52:55.000000 operatorio-0.1.8/operatorio.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2023-07-27 19:52:55.000000 operatorio-0.1.8/operatorio.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)        9 2023-07-27 19:52:55.000000 operatorio-0.1.8/operatorio.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)       11 2023-07-27 19:52:55.000000 operatorio-0.1.8/operatorio.egg-info/top_level.txt
--rw-r--r--   0 david      (501) staff       (20)       38 2023-07-27 19:52:55.486059 operatorio-0.1.8/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)      532 2023-07-27 19:52:44.000000 operatorio-0.1.8/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-01 07:29:05.599061 operatorio-0.1.9/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-08-01 07:29:05.598834 operatorio-0.1.9/PKG-INFO
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-01 07:29:05.597161 operatorio-0.1.9/operatorio/
+-rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.1.9/operatorio/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     2536 2023-08-01 07:28:32.000000 operatorio-0.1.9/operatorio/main.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-01 07:29:05.598561 operatorio-0.1.9/operatorio.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-08-01 07:29:05.000000 operatorio-0.1.9/operatorio.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      219 2023-08-01 07:29:05.000000 operatorio-0.1.9/operatorio.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-08-01 07:29:05.000000 operatorio-0.1.9/operatorio.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)        9 2023-08-01 07:29:05.000000 operatorio-0.1.9/operatorio.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)       11 2023-08-01 07:29:05.000000 operatorio-0.1.9/operatorio.egg-info/top_level.txt
+-rw-r--r--   0 david      (501) staff       (20)       38 2023-08-01 07:29:05.599146 operatorio-0.1.9/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)      532 2023-08-01 07:29:04.000000 operatorio-0.1.9/setup.py
```

### Comparing `operatorio-0.1.8/operatorio/main.py` & `operatorio-0.1.9/operatorio/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 import requests
 from dataclasses import dataclass, asdict
 from enum import Enum
-from typing import List, Union, Optional
+from typing import List, Dict, Optional
 from requests.models import PreparedRequest
 
 # Models
 class EntityType(Enum):
     identity = "identity"
     nft = "nft"
     token = "token"
 
 @dataclass
-class Entity:
+class Address:
     address: str
     description: str
     semantic_similarity: float
     network_value: float = 0.0
     rank: float = 0.0
 
 @dataclass
-class Entities:
-    entity: Optional[str]
-    matches: List[Entity]
+class AddressMatch:
+    address: str
+    metadata: Dict[str, any]
+
+@dataclass
+class DescribeInput:
+    address: str
+    blockchain: str
+
+@dataclass
+class DescribeOutput:
+    matches: List[AddressMatch]
 
 @dataclass
 class Query:
     query: str
     blockchain: str
     entity_type: EntityType
     query_by: List[str]
@@ -55,24 +64,38 @@
 
 class OperatorSearchAPI:
     BASE_URL = 'https://api.operator.io/'
 
     def __init__(self, api_key: str):
         self.api_key = api_key
 
-    def search(self, query: Query) -> Entities:
+    def search(self, query: Query) -> Dict[str, any]:
         headers = {"X-API-Key": self.api_key}
         response = requests.post(
             self.BASE_URL + 'search/',
             headers=headers,
             json=query.to_dict()
         )
         
         if response.status_code == 200:
+            return response.json()
+        elif response.status_code == 422:
+            raise ApiException(HTTPValidationError(**response.json()))
+        else:
+            raise ApiException(response.json())
+
+    def describe(self, describe_input: DescribeInput) -> DescribeOutput:
+        headers = {"X-API-Key": self.api_key}
+        response = requests.post(
+            self.BASE_URL + 'describe/',
+            headers=headers,
+            json=asdict(describe_input)
+        )
+
+        if response.status_code == 200:
             data = response.json()
-            entity = data.get('entity')
-            matches = [Entity(**match) for match in data.get('matches', [])]
-            return Entities(entity=entity, matches=matches)
+            matches = [AddressMatch(**match) for match in data.get('matches', [])]
+            return DescribeOutput(matches=matches)
         elif response.status_code == 422:
             raise ApiException(HTTPValidationError(**response.json()))
         else:
             raise ApiException(response.json())
```

### Comparing `operatorio-0.1.8/setup.py` & `operatorio-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="operatorio",
-    version="0.1.8",
+    version="0.1.9",
     description="A Python SDK for the Operator Search API.",
     author="David Shi",
     author_email="david@operator.io",
     url="https://github.com/operatorlabs/sdk/python",
     packages=['operatorio'],  
     install_requires=[
         'requests',
```

