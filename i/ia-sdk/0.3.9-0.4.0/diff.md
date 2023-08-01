# Comparing `tmp/ia-sdk-0.3.9.tar.gz` & `tmp/ia-sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ia-sdk-0.3.9.tar", last modified: Wed Jan 25 14:59:51 2023, max compression
+gzip compressed data, was "ia-sdk-0.4.0.tar", last modified: Tue Aug  1 21:00:01 2023, max compression
```

## Comparing `ia-sdk-0.3.9.tar` & `ia-sdk-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,42 @@
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-01-25 14:59:51.881697 ia-sdk-0.3.9/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     5213 2023-01-25 14:59:51.881697 ia-sdk-0.3.9/PKG-INFO
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     4799 2022-05-26 13:05:31.000000 ia-sdk-0.3.9/README.md
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-01-25 14:59:51.877697 ia-sdk-0.3.9/ia/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       22 2023-01-25 14:59:45.000000 ia-sdk-0.3.9/ia/__init__.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-01-25 14:59:51.881697 ia-sdk-0.3.9/ia/gaius/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       79 2022-05-26 13:05:31.000000 ia-sdk-0.3.9/ia/gaius/__init__.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    61594 2023-01-25 14:59:45.000000 ia-sdk-0.3.9/ia/gaius/agent_client.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    22850 2023-01-17 21:26:52.000000 ia-sdk-0.3.9/ia/gaius/back_testing.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      858 2022-05-26 13:05:31.000000 ia-sdk-0.3.9/ia/gaius/data_language.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    21246 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/ia/gaius/data_ops.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     3900 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/ia/gaius/genome_info.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     9382 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/ia/gaius/kb_ops.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     4965 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/ia/gaius/prediction_models.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    52008 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/ia/gaius/pvt.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-01-25 14:59:51.881697 ia-sdk-0.3.9/ia/gaius/tests/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2022-05-26 13:05:31.000000 ia-sdk-0.3.9/ia/gaius/tests/__init__.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2677 2022-05-26 13:05:31.000000 ia-sdk-0.3.9/ia/gaius/tests/classification.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     6907 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/ia/gaius/tests/pvt_utils.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2446 2022-07-29 18:03:36.000000 ia-sdk-0.3.9/ia/gaius/tests/utility.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     5644 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/ia/gaius/utils.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-01-25 14:59:51.881697 ia-sdk-0.3.9/ia_sdk.egg-info/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     5213 2023-01-25 14:59:51.000000 ia-sdk-0.3.9/ia_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      531 2023-01-25 14:59:51.000000 ia-sdk-0.3.9/ia_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        1 2023-01-25 14:59:51.000000 ia-sdk-0.3.9/ia_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       48 2023-01-25 14:59:51.000000 ia-sdk-0.3.9/ia_sdk.egg-info/requires.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        3 2023-01-25 14:59:51.000000 ia-sdk-0.3.9/ia_sdk.egg-info/top_level.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      110 2023-01-25 14:59:51.881697 ia-sdk-0.3.9/setup.cfg
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      766 2023-01-25 14:57:41.000000 ia-sdk-0.3.9/setup.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     1256 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/PKG-INFO
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      751 2023-02-02 14:25:09.000000 ia-sdk-0.4.0/README.md
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/ia/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       22 2023-08-01 17:28:22.000000 ia-sdk-0.4.0/ia/__init__.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/ia/gaius/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       79 2022-05-26 13:05:31.000000 ia-sdk-0.4.0/ia/gaius/__init__.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    75273 2023-08-01 15:18:51.000000 ia-sdk-0.4.0/ia/gaius/agent_client.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    22819 2023-05-08 22:12:27.000000 ia-sdk-0.4.0/ia/gaius/back_testing.py
+-rwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)    12451 2023-07-25 14:50:28.000000 ia-sdk-0.4.0/ia/gaius/comcom_client.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      858 2023-04-14 14:57:27.000000 ia-sdk-0.4.0/ia/gaius/data_language.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     9361 2023-08-01 19:37:22.000000 ia-sdk-0.4.0/ia/gaius/data_ops.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    17348 2023-07-19 12:51:12.000000 ia-sdk-0.4.0/ia/gaius/data_structures.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/ia/gaius/experimental/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2023-07-14 15:07:29.000000 ia-sdk-0.4.0/ia/gaius/experimental/__init__.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    11085 2023-07-14 15:07:29.000000 ia-sdk-0.4.0/ia/gaius/experimental/genome_optimizer.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     3217 2023-06-08 15:56:58.000000 ia-sdk-0.4.0/ia/gaius/genome_info.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    27195 2023-08-01 15:18:51.000000 ia-sdk-0.4.0/ia/gaius/kb_ops.py
+-rwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)    36330 2023-07-25 14:03:17.000000 ia-sdk-0.4.0/ia/gaius/manager.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     8771 2023-06-08 15:56:58.000000 ia-sdk-0.4.0/ia/gaius/prediction_models.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/ia/gaius/pvt/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    76162 2023-08-01 20:44:52.000000 ia-sdk-0.4.0/ia/gaius/pvt/__init__.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    26516 2023-08-01 19:14:20.000000 ia-sdk-0.4.0/ia/gaius/pvt/mongo_interface.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    10707 2023-08-01 15:18:46.000000 ia-sdk-0.4.0/ia/gaius/pvt/offline_sio.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    17596 2023-08-01 18:42:47.000000 ia-sdk-0.4.0/ia/gaius/pvt/pvt_utils.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/ia/gaius/tests/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2022-05-26 13:05:31.000000 ia-sdk-0.4.0/ia/gaius/tests/__init__.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2786 2023-06-08 15:56:58.000000 ia-sdk-0.4.0/ia/gaius/tests/classification.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2679 2023-06-08 15:56:58.000000 ia-sdk-0.4.0/ia/gaius/tests/utility.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    11002 2023-06-08 15:56:58.000000 ia-sdk-0.4.0/ia/gaius/utils.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/ia/scripts/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2023-03-24 19:12:06.000000 ia-sdk-0.4.0/ia/scripts/__init__.py
+-rwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)    40560 2023-08-01 17:33:50.000000 ia-sdk-0.4.0/ia/scripts/spawn_agent.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2762 2023-07-25 13:21:37.000000 ia-sdk-0.4.0/ia/scripts/spawn_general.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/ia_sdk.egg-info/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     1256 2023-08-01 21:00:01.000000 ia-sdk-0.4.0/ia_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      825 2023-08-01 21:00:01.000000 ia-sdk-0.4.0/ia_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        1 2023-08-01 21:00:01.000000 ia-sdk-0.4.0/ia_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      139 2023-08-01 21:00:01.000000 ia-sdk-0.4.0/ia_sdk.egg-info/requires.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        3 2023-08-01 21:00:01.000000 ia-sdk-0.4.0/ia_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      110 2023-08-01 21:00:01.166974 ia-sdk-0.4.0/setup.cfg
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     1176 2023-07-18 13:37:42.000000 ia-sdk-0.4.0/setup.py
```

### Comparing `ia-sdk-0.3.9/ia/gaius/agent_client.py` & `ia-sdk-0.4.0/ia/gaius/agent_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,76 @@
 import functools
-import io
 import json
 import uuid
+import traceback
 from typing import Dict, List, Any, Tuple, Union
-from os.path import join
+from os.path import join, splitext
 from datetime import datetime
 from copy import deepcopy
 import requests
-
+from zipfile import ZipFile, ZIP_DEFLATED, is_zipfile
+import warnings
 from ia.gaius.genome_info import Genome
+
 class AgentQueryError(BaseException):
     """Raised if any query to any node returns an error."""
     pass
 
 
 class AgentConnectionError(BaseException):
     """Raised if connecting to any node returns an error."""
     pass
 
+class AgentQueryWarning(Warning):
+    """Used to warn user that a query partially did not complete"""
 
 def _ensure_connected(f):
     @functools.wraps(f)
     def inner(self, *args, **kwargs):
         if not self._connected:
             raise AgentConnectionError(
-                'Not connected to a agent. You must call `connect()` on a AgentClient instance before making queries'
+                'Not connected to a agent. You must call `connect()` \
+                    on a AgentClient instance before making queries'
             )
         return f(self, *args, **kwargs)
 
     return inner
 
 
 def _remove_unique_id(response: dict) -> dict:
-    """Return *response* with the key 'unique_id' removed regardless of nesting."""
+    """Return *response* with the key 'unique_id'
+        removed regardless of nesting."""
     if isinstance(response, dict):
         if 'unique_id' in response:
             del response['unique_id']
         for value in response.values():
             if isinstance(value, dict):
                 _remove_unique_id(value)
     return response
 
+
 class AgentClient:
     """Interface for interacting with agents."""
 
-    def __init__(self, bottle_info: dict, verify:bool=True):
+    def __init__(self,
+                 bottle_info: dict,
+                 verify: bool = True,
+                 timeout: float = None):
         """
         Provide agent information in a dictionary.
-        
+
         Args:
-            bottle_info (dict, required): the info used to connect and authenticate with a GAIuS agent
-            verify (bool, optional): whether to enable SSL Verification on api commands to an agent
-        
+            bottle_info (dict, required): the info used to connect and
+                authenticate with a GAIuS agent
+            verify (bool, optional): whether to enable SSL Verification
+                on api commands to an agent
+
         Example:
             .. code-block:: python
-            
+
                 from ia.gaius.agent_client import AgentClient
 
                 agent_info = {'api_key': 'ABCD-1234',
                             'name': 'gaius-agent',
                             'domain': 'intelligent-artifacts.com',
                             'secure': False}
 
@@ -66,14 +78,16 @@
                 agent.connect()
 
                 agent.set_ingress_nodes(['P1'])
                 agent.set_query_nodes(['P1'])
 
         """
         self.session = requests.Session()
+        self.session.request = functools.partial(self.session.request, timeout=timeout)
+        self._timeout = timeout
         self.genome = None
         self._bottle_info = bottle_info
         self.name = bottle_info['name']
         self._domain = bottle_info['domain']
         self._api_key = bottle_info['api_key']
         self.ingress_nodes = []
         self.query_nodes = []
@@ -109,97 +123,121 @@
                 self._connected,
                 self.gaius_agent,
                 len(self.ingress_nodes),
                 len(self.query_nodes),
             )
         )
 
+    def set_timeout(self, timeout: float):
+        """Redefine timeout for AgentClient API Calls. Requires re-instantiating requests.Session object
+
+        Args:
+            timeout (float): The requested timeout (in seconds)
+        """
+        self.session = requests.Session()
+        self.session.request = functools.partial(self.session.request, timeout=timeout)
+        return
+    
     def receive_unique_ids(self, should_set: bool = True) -> bool:
         self.send_unique_ids = should_set
         return self.send_unique_ids
 
     def connect(self) -> Dict:
-        """Establishes initial connection to GAIuS agent and grabs the agent's genome for node definitions.
+        """Establishes initial connection to GAIuS agent and grabs the
+            agent's genome for node definitions.
 
             Example:
                     .. code-block:: python
 
                         agent_info = {...}
                         agent = AgentClient(agent_info)
                         agent.connect()
         """
-        response_data = self.session.get(self._url + 'connect', verify=self._verify, headers=self._headers).json()
+        response_data = self.session.get(f'{self._url}connect',
+                                         verify=self._verify,
+                                         headers=self._headers).json()
         if 'status' not in response_data or response_data['status'] != 'okay':
             self._connected = False
             raise AgentConnectionError("Connection failed!", response_data)
 
         self.genome = Genome(response_data['genome'])
         self.gaius_agent = response_data['genome']['agent']
         self.all_nodes = [{"name": i['name'], "id": i['id']} for i in self.genome.primitives.values()]
         if response_data['connection'] == 'okay':
             self._connected = True
         else:
             self._connected = False
 
-        return {'connection': response_data['connection'], 'agent': response_data['genie']}
+        return {'connection': response_data['connection'],
+                'agent': response_data['genie']}
 
     def set_ingress_nodes(self, nodes: List = None) -> List:
         """List of primitive names to define where data will be sent.
-        
+
             Example:
                 .. code-block:: python
-                
+
                     # when observing data, it will be sent to only P1 by default
                     agent.set_ingress_nodes(nodes=["P1"])
         """
         if nodes is None:
             nodes = []
-        self.ingress_nodes = [{'id': self.genome.primitive_map[node], 'name': node} for node in nodes]
+        self.ingress_nodes = [{'id': self.genome.primitive_map[node],
+                               'name': node}
+                              for node in nodes]
         return self.ingress_nodes
 
     def set_query_nodes(self, nodes: List = None) -> List:
         """List of primitive names to define which nodes should return answers.
-        
+
             Example:
                 .. code-block:: python
-                
+
                     # when getting predictions, it will be received only from P1 by default
                     agent.set_query_nodes(nodes=["P1"])
         """
         if nodes is None:
             nodes = []
         self.query_nodes = [{'id': self.genome.primitive_map[node], 'name': node} for node in nodes]
         return self.query_nodes
 
-    def _query(
-        self, query_method: Any, path: str, data: Union[dict, str] = None, nodes: List = None, unique_id: str = None
-    ) -> Union[dict, Tuple[dict, str]]:
+    def _query(self,
+               query_method: Any,
+               path: str,
+               data: Union[dict, str] = None,
+               nodes: List = None,
+               unique_id: str = None) -> Union[dict, Tuple[dict, str]]:
         """Internal helper function to make a REST API call with the given *query* and *data*."""
         if not self._connected:
             raise AgentConnectionError(
                 'Not connected to a agent. You must call `connect()` on a AgentClient instance before making queries'
             )
         result = {}
         if unique_id is not None:
             if data:
                 data['unique_id'] = unique_id
             else:
                 data = {'unique_id': unique_id}
-                
+
         data = json.loads(json.dumps(data))
-        
+
         if isinstance(nodes[0], str):
             nodes = [{'name': name, 'id': self.genome.primitive_map[name]} for name in nodes]
         for node in nodes:
             full_path = f'{self._url}{node["id"]}/{path}'
             try:
                 if data is not None:
-                    response = query_method(full_path, verify=self._verify, headers=self._headers, json={'data': data})
+                    response = query_method(full_path,
+                                            verify=self._verify,
+                                            headers=self._headers,
+                                            json={'data': data})
                 else:
-                    response = query_method(full_path, verify=self._verify, headers=self._headers)
+                    response = query_method(full_path,
+                                            verify=self._verify,
+                                            headers=self._headers)
                 response.raise_for_status()
                 response = response.json()
                 if response['status'] != 'okay':
                     raise AgentQueryError(response['message'])
                 if not self.send_unique_ids:
                     response = _remove_unique_id(response['message'])
                 else:
@@ -211,81 +249,90 @@
             except Exception as exception:
                 raise AgentQueryError(str(exception)) from None
         if unique_id is not None:
             return result, unique_id
         return result
 
     def set_summarize_for_single_node(self, value: bool):
-        """When True, queries against a single node return responses directly instead of in a dict key.
-        
-            Example:
-                .. code-block:: python
-                
-                    # set summarize_for_single_node to True
-                    >>> agent.set_summarize_for_single_node(value=True)
-                    >>> gdf = {'strings':['hello'], 'vectors': [], 'emotives':{}}
-                    >>> agent.observe(gdf)
-                    'observed'
+        """When True, queries against a single node return responses directly
+        instead of in a dict key.
+
+        Example:
+            .. code-block:: python
+
+                # set summarize_for_single_node to True
+                >>> agent.set_summarize_for_single_node(value=True)
+                >>> gdf={'strings':['hello'], 'vectors': [], 'emotives':{}}
+                >>> agent.observe(gdf)
+                'observed'
+
+                # set summarize_for_single_node to False
+                >>> agent.set_summarize_for_single_node(value=False)
+                >>> agent.observe(gdf)
+                {'P1': 'observed'}
 
-                    # set summarize_for_single_node to False
-                    >>> agent.set_summarize_for_single_node(value=False)
-                    >>> agent.observe(gdf)
-                    {'P1': 'observed'}
-        
         """
         self.summarize_for_single_node = value
 
     def observe(self, data: Dict, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Exclusively uses the 'observe' call.
-            Will observe on nodes specified by set_ingress_nodes() unless nodes explicitly provided
+            Will observe on nodes specified by set_ingress_nodes()
+            unless nodes explicitly provided
 
             Args:
                 data (dict): the GDF data to be observed
-                nodes (list, optional): Nodes to observe data on, defaults to ingress nodes
-            
+                nodes (list, optional): Nodes to observe data on,
+                    defaults to ingress nodes
+
             Example:
                 .. code-block:: python
-                
+
                     from ia.gaius.utils import create_gdf
                     >>> gdf = create_gdf(strings=['hello'])
                     >>> agent.observe(data=gdf, nodes=["P1"])
                     'observed'
-                    
+
         """
         if nodes is None:
             nodes = self.ingress_nodes
         return self._query(self.session.post, 'observe', data=data, nodes=nodes)
 
     def _observe_event(self, data: Dict, unique_id: str = None) -> Tuple[dict, str]:
         """Exclusively uses the 'observe' call."""
         results = {}
         uid = None
         if unique_id is None:
             unique_id = str(uuid.uuid4())
         for node, node_data in data.items():
-            response, uid = self._query(self.session.post, 'observe', data=node_data, nodes=[node], unique_id=unique_id)
+            response, uid = self._query(self.session.post,
+                                        'observe',
+                                        data=node_data,
+                                        nodes=[node],
+                                        unique_id=unique_id)
             results[node] = response
         return results, uid
 
     @_ensure_connected
     def observe_classification(self, data=None, nodes: List = None):
-        """Send a classification to all nodes as a singular symbol in the last event.
+        """Send a classification to all nodes as a singular symbol in the
+        last event.
 
-        Sending the classification as a single symbol in the last event is the canonical way to classify a sequence.
+        Sending the classification as a single symbol in the last event is
+        the canonical way to classify a sequence.
         """
         if nodes is None:
             nodes = self.query_nodes
         return self._query(self.session.post, 'observe', data=data, nodes=nodes)
 
     def show_status(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Return the current status of the agent.
-        
+
         Example:
             .. code-block:: python
-            
+
                 >>> agent.show_status(nodes=['P1'])
                 {'PREDICT': True,
                 'SLEEPING': False,
                 'emotives': {},
                 'last_learned_model_name': '',
                 'models_kb': '{KB| objects: 0}',
                 'name': 'P1',
@@ -296,138 +343,143 @@
         """
         if nodes is None:
             nodes = self.all_nodes
         return self._query(self.session.get, 'status', nodes=nodes)
 
     def learn(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Return the learn results.
-        
+
         Example:
             .. code-block:: python
-            
+
                 >>> agent.learn(nodes=["P1"])
                 'MODEL|004da01b0ef40d7c3e0965a6b4fd0f413672fbff'
         """
         if nodes is None:
             nodes = self.all_nodes
         return self._query(self.session.post, 'learn', nodes=nodes)
 
     def get_wm(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Return information about Working Memory.
-        
+
         Example:
             .. code-block:: python
 
                 >>> gdf = {'strings':['hello'], 'vectors': [], 'emotives':{}}
                 >>> agent.observe(gdf, nodes=['P1'])
                 >>> agent.get_wm(nodes=['P1'])
                 [['hello']]
-                
+
         """
         if nodes is None:
             nodes = self.all_nodes
         return self._query(self.session.get, 'working-memory', nodes=nodes)
 
     def get_predictions(self, unique_id: str = None, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Return prediction result data.
-        
+
         Example:
             .. code-block:: python
-            
+
                 predictions = agent.get_predictions(nodes=["P1"])
         """
         if nodes is None:
             nodes = self.query_nodes
         return self._query(self.session.post, 'predictions', nodes=nodes, unique_id=unique_id)
 
     def clear_wm(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Clear the Working Memory of the Agent.
         Will not delete any persisted memory from the KnowledgeBase
-        
+
         Example:
             .. code-block:: python
-            
+
                 >>> agent.clear_wm(nodes=['P1'])
                 'wm-cleared'
         """
         if nodes is None:
             nodes = self.all_nodes
         return self._query(self.session.post, 'working-memory/clear', nodes=nodes)
 
-    def clear_all_memory(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
+    def clear_all_memory(self, clear_blacklist=True, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Clear both the Working Memory and persisted memory.
         Equivalent to re-initializing the nodes specified
-        
-        Example:
-            .. code-block:: python
-            
+
+        Args:
+            clear_blacklist (bool, optional): Controls if symbol blacklist is
+                also cleared or not. Defaults to False.
+            nodes (List, optional): List of nodes to call command on.
+                Defaults to None.
+
+        .. code-block:: python
+
                 >>> agent.clear_all_memory(nodes=["P1"])
                 'all-cleared'
+
+        Returns:
+            Union[dict, Tuple[dict, str]]: _description_
         """
         if nodes is None:
             nodes = self.all_nodes
-        return self._query(self.session.post, 'clear-all-memory', nodes=nodes)
+
+        data = {"clear_blacklist": clear_blacklist}
+
+        return self._query(self.session.post, 'clear-all-memory', nodes=nodes, data=data)
 
     def get_percept_data(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Return percept data.
-        
+
         Example:
             .. code-block:: python
-            
+
                 percept_data = agent.get_percept_data(nodes=["P1"])
         """
         if nodes is None:
             nodes = self.all_nodes
         return self._query(self.session.get, 'percept-data', nodes=nodes)
 
     def get_cognition_data(self, unique_id: str = None, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Return cognition data.
-        
+
         Example:
             .. code-block:: python
-            
+
                 cog_data = agent.get_cognition_data(nodes=["P1"])
         """
         if nodes is None:
             nodes = self.query_nodes
         return self._query(self.session.get, 'cognition-data', nodes=nodes, unique_id=unique_id)
-    
-    def get_all_genes(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
-        """Return cognition data."""
-        if nodes is None:
-            nodes = self.query_nodes
-        return self._query(self.session.get, 'all-genes', nodes=nodes)
 
     def get_all_genes(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Return all genes for nodes.
-        
+
         Example:
             .. code-block:: python
-            
+
                 genes = agent.get_all_genes(nodes=["P1"])
         """
         if nodes is None:
-            nodes = self.query_nodes
+            nodes = self.all_nodes
         return self._query(self.session.get, 'all-genes', nodes=nodes)
 
     @_ensure_connected
     def change_genes(self, gene_data: Dict, nodes: List = None) -> Union[dict, Any]:
         """Change the genes in *gene_data* to their associated values.
 
-        This will do live updates to an existing agent, rather than stopping an agent and starting a new one, as
-        per 'injectGenome'.
+        This will do live updates to an existing agent, rather than stopping
+        an agent and starting a new one, as per 'injectGenome'.
         gene_data of form:
 
             {gene: value}
 
         Example:
             .. code-block:: python
 
                 agent.change_genes(gene_data={"recall_threshold" : 0.15})
-                    
+
         """
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
 
         result = {}
@@ -446,541 +498,622 @@
                 return response['message']
             result[node['name']] = response['message']
         return result
 
     @_ensure_connected
     def get_gene(self, gene: str, nodes: List = None) -> Union[dict, Dict[Any, Dict[str, Any]]]:
         """Return the value for the gene *gene* on *nodes*.
-        
+
         Example:
                 .. code-block:: python
 
                     agent.get_gene(gene="recall_threshold")
-        
-        
+
         """
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
         result = {}
         for node in nodes:
             try:
-                response = self.session.get(
-                    f"{self._url}{node['id']}/gene/{gene}", verify=self._verify, headers=self._headers
-                ).json()
+                response = self.session.get(f"{self._url}{node['id']}/gene/{gene}",
+                                            verify=self._verify,
+                                            headers=self._headers
+                                            ).json()
                 if 'error' in response or response['status'] == 'failed':
                     if len(nodes) == 1 and self.summarize_for_single_node:
                         raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
                 if len(nodes) == 1 and self.summarize_for_single_node:
                     return {gene: response['message']}
                 result[node['name']] = {gene: response['message']}
             except BaseException as exception:
                 raise AgentQueryError(exception) from None
 
         return result
 
     @_ensure_connected
     def get_model(self, model_name: str, nodes: List = None) -> Union[dict, Any]:
         """Returns model with name *model_name*.
 
         Model name is unique, so it should not matter that we query all nodes, only
         one model will be found.
-        
+
+        Args:
+            model_name (str): Name of model to retrieve
+            nodes (List, optional): list of nodes to retrieve model from.
+                Defaults to None (all nodes).
+
+        Returns:
+            Union[dict, Any]: dictionary of {node_name : model} pairs
         Example:
                 .. code-block:: python
 
                     agent.get_model("MODEL|d85f28ebda228064299035bf2dbf58f5c6484108")
-        
+
         """
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
         result = {}
         for node in nodes:
             try:
-                response = self.session.get(
-                    f"{self._url}{node['id']}/model/{model_name}", headers=self._headers, verify=self._verify
-                ).json()
+                response = self.session.get(f"{self._url}{node['id']}/model/{model_name}",
+                                            headers=self._headers,
+                                            verify=self._verify
+                                            ).json()
                 if 'error' in response or response['status'] == 'failed':
                     if len(nodes) == 1 and self.summarize_for_single_node:
                         raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
                 if len(nodes) == 1 and self.summarize_for_single_node:
                     return response['message']
                 else:
                     result[node['name']] = response['message']
             except Exception as exception:
                 raise AgentQueryError(str(exception)) from None
 
         return result
-    
+
     @_ensure_connected
     def delete_model(self, model_name: str, nodes: List = None) -> Union[dict, Any]:
         """Deletes model with name *model_name*.
 
-        Model name is unique, so it should not matter that we query all nodes, 
+        Model name is unique, so it should not matter that we query all nodes,
         all its duplicates everywhere will be deleted.
         """
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
         result = {}
         for node in nodes:
             try:
-                response = self.session.delete(
-                    f"{self._url}{node['id']}/model/{model_name}", headers=self._headers, verify=self._verify
-                ).json()
+                response = self.session.delete(f"{self._url}{node['id']}/model/{model_name}",
+                                               headers=self._headers,
+                                               verify=self._verify
+                                               ).json()
                 if 'error' in response or response['status'] == 'failed':
                     if len(nodes) == 1 and self.summarize_for_single_node:
                         raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
                 if len(nodes) == 1 and self.summarize_for_single_node:
                     return response['message']
                 else:
                     result[node['name']] = response['message']
             except Exception as exception:
                 raise AgentQueryError(str(exception)) from None
 
         return result
-    
+
     @_ensure_connected
     def update_model(self, model_name: str, model: Dict, nodes: List = None) -> Union[dict, Any]:
-        """Update the model  **model_name** with the data in **model** on nodes **nodes**
-        
-        
-        .. note:: 
-
-            This function is only capable of updating the emotives corresponding to a model. In order to update the sequence corresponding to a model,
-            delete this model and reobserve the updated sequence
-            
+        """Update the model  **model_name** with the data in **model**
+        on update_model **nodes**
+
+        .. note::
+
+            This function is only capable of updating the emotives
+            corresponding to a model. In order to update the sequence
+            corresponding to a model, delete this model and reobserve
+            the updated sequence
+
         Example:
             .. code-block:: python
 
                 # retrieve a model already learned on an agent
                 model_name = 'MODEL|d85f28ebda228064299035bf2dbf58f5c6484108'
                 model = agent.get_model(model_name=model_name, nodes=['P1'])
-                
+
                 # update the emotives in the model
-                model["emotives"] = [{'utility': 500}]
+                model["emotives"] = {'utility': [150, 200, 500]}
                 agent.update_model(model_name=model_name, model=model, nodes=['P1'])
-                
-            
-            
+
         """
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
         result = {}
         for node in nodes:
             try:
-                response = self.session.put(
-                    f"{self._url}{node['id']}/model/{model_name}", headers=self._headers, verify=self._verify,
-                    json={'model': model}
-                ).json()
+                response = self.session.put(f"{self._url}{node['id']}/model/{model_name}",
+                                            headers=self._headers,
+                                            verify=self._verify,
+                                            json={'model': model}
+                                            ).json()
                 if 'error' in response or response['status'] == 'failed':
                     if len(nodes) == 1 and self.summarize_for_single_node:
                         raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
                 if len(nodes) == 1 and self.summarize_for_single_node:
                     return response['message']
                 else:
                     result[node['name']] = response['message']
             except Exception as exception:
                 raise AgentQueryError(str(exception)) from None
 
         return result
 
     @_ensure_connected
     def resolve_model(self, model_name: str, nodes: List = None) -> Union[dict, Any]:
         """Returns model with name *model_name*.
 
-        Model name is unique, so it should not matter that we query all nodes, only
-        one model will be found.
+        Model name is unique, so it should not matter that we query all nodes,
+        only one model will be found.
         """
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
         result = {}
         for node in nodes:
             try:
-                response = self.session.get(
-                    f"{self._url}{node['id']}/model/{model_name}", headers=self._headers, verify=self._verify
-                ).json()
+                response = self.session.get(f"{self._url}{node['id']}/model/{model_name}",
+                                            headers=self._headers,
+                                            verify=self._verify
+                                            ).json()
                 if 'error' in response or response['status'] == 'failed':
                     if len(nodes) == 1 and self.summarize_for_single_node:
                         raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
                 if len(nodes) == 1 and self.summarize_for_single_node:
                     return response['message']
                 else:
                     result[node['name']] = response['message']
             except Exception as exception:
                 raise AgentQueryError(str(exception)) from None
 
-        return result    
+        return result
 
     def get_name(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Return name of *nodes*.
-        
+
             Example:
                 .. code-block:: python
-                
+
                     agent.get_name(nodes=["P1", "P2"])
-        
+
         """
         if nodes is None:
             nodes = self.all_nodes
         return self._query(self.session.get, 'name', nodes=nodes)
 
     def get_time(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Return time on *nodes*.
-        
+
             Example:
                 .. code-block:: python
-                
+
                     >>> agent.get_time(nodes=['P1'])
                     '1'
         """
         if nodes is None:
             nodes = self.all_nodes
         return self._query(self.session.get, 'time', nodes=nodes)
-    
+
     @_ensure_connected
-    def get_models_with_symbols(self, symbols_list : List = None, nodes: List = None) -> Union[dict, Any]:
+    def get_models_with_symbols(self, symbols_list: List = None, nodes: List = None) -> Union[dict, Any]:
         '''
-            Function which search the kbs on the nodes for models with certain symbols.
-            All symbols must be present in model.sequence, or the model will not be returned
+            Function which search the kbs on the nodes for models with certain
+            symbols. All symbols must be present in model.sequence, or the
+            model will not be returned
         '''
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
         result = {}
         for node in nodes:
             try:
-                response = self.session.post(
-                f"{self._url}{node['id']}/get-models-with-symbols",
-                verify=self._verify,
-                headers=self._headers,
-                json={'data': symbols_list},
-            ).json()
+                response = self.session.post(f"{self._url}{node['id']}/get-models-with-symbols",
+                                             verify=self._verify,
+                                             headers=self._headers,
+                                             json={'data': symbols_list}
+                                             ).json()
                 if 'error' in response or response['status'] == 'failed':
                     if len(nodes) == 1 and self.summarize_for_single_node:
                         raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
                 if len(nodes) == 1 and self.summarize_for_single_node:
                     return response['message']
                 else:
                     result[node['name']] = response['message']
             except Exception as exception:
                 raise AgentQueryError(str(exception)) from None
         return result
-    
+
     @_ensure_connected
-    def get_models_with_patterns(self, symbols_list : List = None, nodes: List = None) -> Union[dict, Any]:
+    def get_models_with_patterns(self,
+                                 symbols_list: List = None,
+                                 nodes: List = None) -> Union[dict, Any]:
         '''
-            Function which search the kbs on the nodes for models with certain regex patterns.
-            All regex patterns must be present in model.sequence, or the model will not be returned
+            Function which search the kbs on the nodes for models with
+            certain regex patterns.
+
+            All regex patterns must be present in model.sequence, or
+            the model will not be returned
         '''
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
         result = {}
         for node in nodes:
             try:
-                response = self.session.post(
-                f"{self._url}{node['id']}/get-models-with-patterns",
-                verify=self._verify,
-                headers=self._headers,
-                json={'data': symbols_list},
-            ).json()
+                response = self.session.post(f"{self._url}{node['id']}/get-models-with-patterns",
+                                             verify=self._verify,
+                                             headers=self._headers,
+                                             json={'data': symbols_list},
+                                             ).json()
                 if 'error' in response or response['status'] == 'failed':
                     if len(nodes) == 1 and self.summarize_for_single_node:
                         raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
                 if len(nodes) == 1 and self.summarize_for_single_node:
                     return response['message']
                 else:
                     result[node['name']] = response['message']
             except Exception as exception:
                 raise AgentQueryError(str(exception)) from None
         return result
-    
+
     @_ensure_connected
-    def add_model(self, sequence : List, vector : List = None, frequency : int = 1, emotives : Dict = {}, nodes: List = None) -> Union[dict, Any]:
+    def add_model(self, sequence: List,
+                  vector: List = None,
+                  frequency: int = 1,
+                  emotives: Dict = {},
+                  metadata: List = [],
+                  nodes: List = None) -> Union[dict, Any]:
         '''
-            Function to explicitely add a model with the given sequence of symbols, frequency, and emotives.
-            Returns the hash of the generated function
+            Function to explicitely add a model with the given sequence
+            of symbols, frequency, and emotives. Returns the hash of
+            the generated function
         '''
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
         result = {}
         for node in nodes:
             try:
-                response = self.session.put(
-                f"{self._url}{node['id']}/add-model",
-                verify=self._verify,
-                headers=self._headers,
-                json={'sequence': sequence,
-                      'vector': vector,
-                     'frequency' : frequency,
-                     'emotives' : emotives},
-            ).json()
+                response = self.session.put(f"{self._url}{node['id']}/add-model",
+                                            verify=self._verify,
+                                            headers=self._headers,
+                                            json={'sequence': sequence,
+                                                  'vector': vector,
+                                                  'frequency': frequency,
+                                                  'emotives': emotives,
+                                                  "metadata": metadata},
+                                            ).json()
                 if 'error' in response or response['status'] == 'failed':
                     if len(nodes) == 1 and self.summarize_for_single_node:
                         raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
                 if len(nodes) == 1 and self.summarize_for_single_node:
                     return response['message']
                 else:
                     result[node['name']] = response['message']
             except Exception as exception:
                 raise AgentQueryError(str(exception)) from None
         return result
-    
+
     @_ensure_connected
-    def remove_symbols_from_system(self, symbols_list : List, nodes: List = None) -> Union[dict, Any]:
-        """Function which search the kbs on the nodes for models with certain symbols.
-            Symbols are removed, and the symbols are blacklisted, thus making it impossible fo them to
-            be in the working memory in the future.
+    def remove_symbols_from_system(self,
+                                   symbols_list: List,
+                                   nodes: List = None) -> Union[dict, Any]:
+        """Function which search the kbs on the nodes for models with
+        certain symbols.
+
+        Symbols are removed, and the symbols are blacklisted, thus making
+        it impossible fo them to be in the working memory in the future.
 
         Args:
             symbols_list (List): list of symbols to remove. Defaults to None.
-            nodes (List, optional): list of nodes to remove symbols from. Defaults to None (all nodes).
+            nodes (List, optional): list of nodes to remove symbols from.
+            Defaults to None (all nodes).
 
         Raises:
             AgentQueryError: Error in Cognitive Processor handling
 
         Returns:
-            Union[dict, Any]: dict showing old model hash -> new model hash (or 'deleted') pairs
+            Union[dict, Any]: dict showing old model hash -> new model hash
+            (or 'deleted') pairs
         """
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
         result = {}
         for node in nodes:
             try:
-                response = self.session.delete(
-                f"{self._url}{node['id']}/symbols/remove",
-                verify=self._verify,
-                headers=self._headers,
-                json={'data': symbols_list},
-            ).json()
+                response = self.session.delete(f"{self._url}{node['id']}/symbols/remove",
+                                               verify=self._verify,
+                                               headers=self._headers,
+                                               json={'data': symbols_list},
+                                               ).json()
                 if 'error' in response or response['status'] == 'failed':
                     if len(nodes) == 1 and self.summarize_for_single_node:
                         raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
                 if len(nodes) == 1 and self.summarize_for_single_node:
                     return response['message']
                 else:
                     result[node['name']] = response['message']
             except Exception as exception:
                 raise AgentQueryError(str(exception)) from None
         return result
-    
+
     @_ensure_connected
-    def remove_patterns_from_system(self, symbols_list : List, nodes: List = None) -> Union[dict, Any]:
-        """Function which search the kbs on the nodes for models with certain regex patterns.
-            Removed symbols that matches patterns, but does not blacklist them. So patterns may show
-            up in the future.
+    def remove_patterns_from_system(self,
+                                    symbols_list: List,
+                                    nodes: List = None) -> Union[dict, Any]:
+        """
+        Function which search the kbs on the nodes for models with
+        certain regex patterns. Removed symbols that matches patterns,
+        but does not blacklist them. So patterns may show up in the future.
 
         Args:
             symbols_list (List): list of regex symbol patterns to remove.
-            nodes (List, optional): list of nodes to remove symbols on. Defaults to None (all nodes).
+            nodes (List, optional): list of nodes to remove symbols on.
+                Defaults to None (all nodes).
 
         Raises:
             AgentQueryError: Error in Cognitive Processor handling
 
         Returns:
-            Union[dict, Any]: dict showing old model hash -> new model hash (or 'deleted') pairs
+            Union[dict, Any]: dict showing old model hash -> new model hash
+                (or 'deleted') pairs
+
+        Example:
+            .. code-block:: python
+
+                from ia.gaius.kb_ops import list_symbols
+
+                symbols_before = list_symbols(agent)
+                agent.remove_patterns_from_system(['VECTOR|.+'])
+                symbols_after = list_symbols(agent)
+
         """
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
         result = {}
         for node in nodes:
             try:
-                response = self.session.delete(
-                f"{self._url}{node['id']}/patterns/remove",
-                verify=self._verify,
-                headers=self._headers,
-                json={'data': symbols_list},
-            ).json()
+                response = self.session.delete(f"{self._url}{node['id']}/patterns/remove",
+                                               verify=self._verify,
+                                               headers=self._headers,
+                                               json={'data': symbols_list}
+                                               ).json()
                 if 'error' in response or response['status'] == 'failed':
                     if len(nodes) == 1 and self.summarize_for_single_node:
                         raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
                 if len(nodes) == 1 and self.summarize_for_single_node:
                     return response['message']
                 else:
                     result[node['name']] = response['message']
             except Exception as exception:
                 raise AgentQueryError(str(exception)) from None
         return result
 
-    def add_blacklisted_symbols(self, symbols_list: List, nodes: List = None):
-        """Add a symbol to the blacklist manually. 
+    def add_blacklisted_symbols(self,
+                                symbols_list: List,
+                                nodes: List = None):
+        """Add a symbol to the blacklist manually.
         List all symbols currently in the blacklist using :func:`list_blacklisted_symbols`.
         Symbols may be removed from this list by using :func:`remove_blacklisted_symbols`.
 
         Args:
-            symbols_list (List): list of symbols to add to the 
-            nodes (List, optional): list of nodes to add blacklisted symbols on. Defaults to None (all nodes).
+            symbols_list (List): list of symbols to add to the blacklist
+            nodes (List, optional): list of nodes to add blacklisted symbols on.
+                Defaults to None (all nodes).
 
         Raises:
             AgentQueryError: Error in Cognitive Processor handling
 
         Returns:
             dict or str: Depicting result of adding blacklisted symbols to each CP in nodes
         """
-        
+
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
         result = {}
         for node in nodes:
             try:
-                response = self.session.post(
-                f"{self._url}{node['id']}/blacklisted-symbols/add",
-                verify=self._verify,
-                headers=self._headers,
-                json={'data': symbols_list},
-            ).json()
+                response = self.session.post(f"{self._url}{node['id']}/blacklisted-symbols/add",
+                                             verify=self._verify,
+                                             headers=self._headers,
+                                             json={'data': symbols_list}
+                                             ).json()
                 if 'error' in response or response['status'] == 'failed':
                     if len(nodes) == 1 and self.summarize_for_single_node:
                         raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
                 if len(nodes) == 1 and self.summarize_for_single_node:
                     return response['message']
                 else:
                     result[node['name']] = response['message']
             except Exception as exception:
                 raise AgentQueryError(str(exception)) from None
-        return result   
+        return result
 
     def list_blacklisted_symbols(self, nodes: List = None):
-        """Display a list of all symbols currently 'blacklisted' on each node in *nodes*. 
-        Symbols enter this list by being removed from a Cognitive Processor via :func:`remove_symbols_from_system` or :func:`remove_patterns_from_system`.
-        Symbols may be removed from this list by using :func:`remove_blacklisted_symbols`.
+        """Display a list of all symbols currently 'blacklisted' on each
+        node in *nodes*.
+
+        Symbols enter this list by being removed from a Cognitive Processor
+        via :func:`remove_symbols_from_system` or
+        :func:`remove_patterns_from_system`.
+
+        Symbols may be removed from this list by using
+        :func:`remove_blacklisted_symbols`.
 
         Args:
-            nodes (List, optional): list of nodes to show blacklisted symbols on. Defaults to None (all nodes).
+            nodes (List, optional): list of nodes to show blacklisted symbols
+                on. Defaults to None (all nodes).
+
+        Example:
+            .. code-block:: python
+
+                from ia.gaius.kb_ops import list_symbols,
+                    get_models_containing_symbol
+
+                symbols_before = list_symbols(agent)
+                blacklisted_symbols = agent.list_blacklisted_symbols()
+                # ensure all blacklisted symbols do not appear in the system
+                assert all([sym not in symbols_before for sym in blacklisted_symbols])
+
+                # ensure no models contain the blacklisted symbols
+                models_containing_symbol = get_models_containing_symbol(agent, symbol_set=set(blacklisted_symbols))
+                assert all([len(val) == 0 for val in models_containing_symbol.values()])
         """
-        
+
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
         result = {}
         for node in nodes:
             try:
-                response = self.session.get(
-                f"{self._url}{node['id']}/list-blacklisted-symbols",
-                verify=self._verify,
-                headers=self._headers,
-            ).json()
+                response = self.session.get(f"{self._url}{node['id']}/list-blacklisted-symbols",
+                                            verify=self._verify,
+                                            headers=self._headers
+                                            ).json()
                 if 'error' in response or response['status'] == 'failed':
                     if len(nodes) == 1 and self.summarize_for_single_node:
                         raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
                 if len(nodes) == 1 and self.summarize_for_single_node:
                     return response['message']
                 else:
                     result[node['name']] = response['message']
             except Exception as exception:
                 raise AgentQueryError(str(exception)) from None
-        return result   
+        return result
 
-    
-    def remove_blacklisted_symbols(self, symbols_to_remove: List, nodes: List = None):
-        """Remove symbols from blacklist on each Cognitive Processor in *nodes*
+    def remove_blacklisted_symbols(self,
+                                   symbols_to_remove: List,
+                                   nodes: List = None):
+        """Remove symbols from blacklist on each Cognitive
+        Processor in *nodes*
 
         Args:
-            symbols_to_remove (List): list of symbols to remove from blacklisted symbols
-            nodes (List, optional): list of nodes to remove blacklisted symbols on. Defaults to None (all nodes).
+            symbols_to_remove (List): list of symbols to remove from
+                blacklisted symbols
+            nodes (List, optional): list of nodes to remove blacklisted
+                symbols on. Defaults to None (all nodes).
 
         Raises:
             AgentQueryError: Error in Cognitive Processor handling
 
         Returns:
-            _type_: _description_
+            str: 'removed-blacklisted-symbols' or
+            'failed-to-remove-some-symbols-from-blacklist'
         """
-        
+
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
         result = {}
         for node in nodes:
             try:
-                response = self.session.delete(
-                f"{self._url}{node['id']}/blacklisted-symbols/remove",
-                verify=self._verify,
-                headers=self._headers,
-                json={'data': symbols_to_remove},
-            ).json()
+                response = self.session.delete(f"{self._url}{node['id']}/blacklisted-symbols/remove",
+                                               verify=self._verify,
+                                               headers=self._headers,
+                                               json={'data': symbols_to_remove}
+                                               ).json()
                 if 'error' in response or response['status'] == 'failed':
                     if len(nodes) == 1 and self.summarize_for_single_node:
                         raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
                 if len(nodes) == 1 and self.summarize_for_single_node:
                     return response['message']
                 else:
                     result[node['name']] = response['message']
             except Exception as exception:
                 raise AgentQueryError(str(exception)) from None
-        return result    
+        return result
 
     @_ensure_connected
     def get_vector(self, vector_name: str, nodes: List = None) -> Union[dict, Dict[Any, Dict[str, Any]]]:
         """Return the vector with *vector_name* on *nodes* (it will be present on at most one).
-        
+
             Example:
                 .. code-block:: python
 
                     agent.get_vector(vector_name="VECTOR|0b7f2aac43ae8a0d94c58be08a5b8b0ab28079de")
-        
+
         """
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
         result = {}
         for node in nodes:
             try:
                 response = self.session.get(
                     f"{self._url}{node['id']}/vector", headers=self._headers, verify=self._verify, json={'data': vector_name}
                 ).json()
                 if 'error' in response or response['status'] == 'failed':
                     if len(nodes) == 1 and self.summarize_for_single_node:
                         raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
                 if len(nodes) == 1 and self.summarize_for_single_node:
                     return response['message']
                 else:
                     result[node['name']] = response['message']
             except Exception as exception:
                 raise AgentQueryError(str(exception)) from None
 
         return result
 
     @_ensure_connected
     def increment_recall_threshold(self, increment: float, nodes: List = None) -> Dict[Any, Dict[str, Any]]:
         """Increment recall threshold by *increment* on *nodes*.
-        
+
             Args:
                 increment (float): value by which to increment the recall threshold by
 
             Example:
                 .. code-block:: python
 
                     agent.increment_recall_threshold(increment=0.05, nodes=["P1"])
 
-            .. note:: 
+            .. note::
 
-                This command with only update the recall threshold by a specified value. 
-                In order to set the recall threshold to a specific value, 
+                This command with only update the recall threshold by a specified value.
+                In order to set the recall threshold to a specific value,
                 use :func:`change_genes` instead.
         """
         if nodes is None:
             nodes = self.all_nodes
         else:
             nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
         result = {}
@@ -991,52 +1124,56 @@
                     verify=self._verify,
                     headers=self._headers,
                     json={'increment': increment},
                 ).json()
                 if 'error' in response or response['status'] == 'failed':
                     if len(nodes) == 1 and self.summarize_for_single_node:
                         raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
                 else:
                     self.genome.primitives[node['id']]['recall_threshold'] += increment
                 if len(nodes) == 1 and self.summarize_for_single_node:
                     return {"recall_threshold": response['message']}
                 result[node['name']] = {"recall_threshold": response['message']}
             except Exception as exception:
                 raise AgentQueryError(str(exception)) from None
 
         return result
 
-    def start_sleeping(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
+    def start_sleeping(self,
+                       nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Tells *nodes* to start sleeping.
-        
+
             Example:
                     .. code-block:: python
 
                         # will disable observing new data on node P1
                         agent.start_sleeping(nodes=["P1"])
         """
         if nodes is None:
             nodes = self.all_nodes
         return self._query(self.session.post, 'sleeping/start', nodes=nodes)
 
-    def stop_sleeping(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
+    def stop_sleeping(self,
+                      nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Wakes up sleeping *nodes*.
 
             Example:
                 .. code-block:: python
 
                     # will enable observing new data on node P1
                     agent.stop_sleeping(nodes=["P1"])
-        
+
         """
         if nodes is None:
             nodes = self.all_nodes
         return self._query(self.session.post, 'sleeping/stop', nodes=nodes)
 
-    def start_predicting(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
+    def start_predicting(self,
+                         nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Tells *nodes* to start predicting.
 
             Example:
                 .. code-block:: python
 
                     # will enable prediction generation on node P1
                     agent.start_predicting(nodes=["P1"])
@@ -1045,25 +1182,25 @@
             nodes = self.all_nodes
         return self._query(self.session.post, 'predicting/start', nodes=nodes)
 
     def stop_predicting(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Tells *nodes* to stop predicting.
 
         Useful for faster training, but abstracted nodes will not learn.
-        
+
         Example:
             .. code-block:: python
 
                 # will disable prediction generation on node P1
                 agent.stop_predicting(nodes=["P1"])
         """
         if nodes is None:
             nodes = self.all_nodes
         return self._query(self.session.post, 'predicting/stop', nodes=nodes)
-    
+
     def start_autolearning(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Tells *nodes* to start predicting.
 
             Example:
                 .. code-block:: python
 
                     # will enable prediction generation on node P1
@@ -1073,332 +1210,538 @@
             nodes = self.all_nodes
         return self._query(self.session.post, 'autolearning/start', nodes=nodes)
 
     def stop_autolearning(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Tells *nodes* to stop predicting.
 
         Useful for faster training, but abstracted nodes will not learn.
-        
+
         Example:
             .. code-block:: python
 
                 # will disable prediction generation on node P1
                 agent.stop_predicting(nodes=["P1"])
         """
         if nodes is None:
             nodes = self.all_nodes
         return self._query(self.session.post, 'autolearning/stop', nodes=nodes)
 
     @_ensure_connected
     def ping(self, nodes: List = None) -> Union[dict, Any]:
         """Ping a node to ensure it's up.
-        
+
             Example:
-            
+
                 .. code-block:: python
-                                    
+
                     agent.ping(nodes=["P1"])
         """
         if nodes is None:
-            return self.session.get(f'{self._url}gaius-api/ping', headers=self._headers).json()
-        else:
-            nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
-            results = {}
-            for node in nodes:
-                response = self.session.get(f"{self._url}{node['id']}/ping", verify=self._verify, headers=self._headers).json()
-                if 'error' in response or response["status"] == 'failed':
-                    if len(nodes) == 1 and self.summarize_for_single_node:
-                        raise Exception("Request Failure:", response)
-                    print("Failure:", {node['name']: response})
+            return self.session.get(f'{self._url}gaius-api/ping',
+                                    headers=self._headers).json()
+
+        nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
+        results = {}
+        for node in nodes:
+            response = self.session.get(f"{self._url}{node['id']}/ping",
+                                        verify=self._verify,
+                                        headers=self._headers).json()
+            if 'error' in response or response["status"] == 'failed':
                 if len(nodes) == 1 and self.summarize_for_single_node:
-                    return response['message']
-                results[node['name']] = response["message"]
-            return results
-    
+                    raise AgentQueryError(response)
+                warnings.warn(response["message"], AgentQueryWarning)
+            if len(nodes) == 1 and self.summarize_for_single_node:
+                return response['message']
+            results[node['name']] = response["message"]
+        return results
+
     @_ensure_connected
-    def get_kbs(self, directory='./'):
+    def get_kbs(self, directory='./'): # pragma: no cover
         """Returns the KBs for the agent.
         This is a mongo-db and can be used to store or analyze locally.
-        Choose the directory to save in with the directory keyword. Default is in './'.
-        
+        Choose the directory to save in with the directory keyword.
+        Default is in './'.
+
         .. warning::
 
-            .. deprecated:: 12.0 (Kehl)
-            
+            .. deprecated:: 11.0 (Kehl)
+
             Use :func:`get_kbs_as_json` instead.
-        
+
         """
         _headers = self._headers
         _headers['Content-Encoding'] = 'gzip'
-        archive = self.session.get(
-                    f"{self._url}database", 
-                    headers=_headers,
-                    json={},
-                    verify=self._verify
-                )
-        archive_file = join(directory, f'{self.gaius_agent}-{self.name}-{datetime.now()}-kb.archive.gz')
+        archive = self.session.get(f"{self._url}database",
+                                   headers=_headers,
+                                   json={},
+                                   verify=self._verify
+                                   )
+        archive_file = join(directory,
+                            f'{self.gaius_agent}-{self.name}-{datetime.now()}-kb.archive.gz')
         with open(archive_file, 'wb') as f:
             f.write(archive.content)
         return f"Saved as {archive_file}"
-    
+
+
     @_ensure_connected
-    def get_kbs_as_json(self, nodes: List = None, directory='./', filename=None, separated=False, ids=True, obj=False) -> Union[List[str], dict]:
+    def _get_kbs_as_json_compressed(self,
+                                   nodes: List = None,
+                                   directory='./',
+                                   filename=None,
+                                   ids=True) -> str:
+        """Returns KBs of specified nodes in a zip file (separated by node)
+
+        """
+        field = 'name'
+        if ids:
+            field = 'id'
+        if filename is None:
+            filename = join(directory, f'{self.gaius_agent}-{self.name}-{datetime.now()}-kb.zip')
+        with ZipFile(filename, 'w', compression=ZIP_DEFLATED) as kb_zip:
+            if nodes is None:
+                nodes = self.all_nodes
+            prev_summarize_state = self.summarize_for_single_node
+
+            try:
+                self.set_summarize_for_single_node(False)
+                for node in nodes:
+                    output = self.session.get(f'{self._url}{node["id"]}/get_kb/raw', headers=self._headers)
+                    if output.status_code != 200:
+                        raise Exception(f'failed to get kb from node {node["id"]}')
+                    print(f'writing kb for node {node["name"]}')
+                    with kb_zip.open(f'{node[field]}.json', 'w', force_zip64=True) as f:
+                        f.write(output.content)
+            except Exception as e:
+                print(f'failed to get kb: {e}')
+                raise e
+            finally:
+                self.set_summarize_for_single_node(prev_summarize_state)
+
+        return filename
+
+    @_ensure_connected
+    def get_kbs_as_json(self,
+                        nodes: List = None,
+                        directory='./',
+                        filename=None,
+                        separated=False,
+                        ids=True,
+                        obj=False,
+                        compressed=False) -> Union[List[str], dict]:
         """Returns KBs of specified nodes as JSON Objects
 
         Args:
             nodes (list, optional): Defaults to None.
             directory (str, optional): Defaults to './'.
-            separated (bool, optional): store each KB separately. Defaults to False
-            ids (bool, optional): use primitive_ids as keys for knowledgebase instead of node numbers. Defaults to True
-            obj (bool, optional): whether to save the kbs to a filepath or a python object returned from the function
+            separated (bool, optional): store each KB separately.
+                Defaults to False
+            ids (bool, optional): use primitive_ids as keys for knowledgebase
+                instead of node numbers. Defaults to True
+            obj (bool, optional): whether to save the kbs to a filepath
+                or a python object returned from the function
+            compressed (bool, optional): whether to save the kbs to a zip file. Not compatible with
+                "separated" or "obj" arguments
         Returns:
-            Union[List(str), Dict]: List of files where KB is stored if obj = False, or big dictionary where KB is to be stored if obj = True
-            
+            Union[List(str), Dict]: List of files where KB is stored
+            if obj = False, or dictionary where KB is to be
+            stored if obj = True
+
 
         Example:
             .. code-block:: python
-            
+
                 # save the KBs in a specified directory, without using node IDs
                 # will use node names instead (e.g. P1, P2, P3)
                 kb_path = "../path/to/save/dir/"
                 agent.get_kbs_from_json(directory=kb_path, separated=False, ids=False)
-                
+
                 #save the KBs to the active directory, using node IDs (e.g. p46514fa2, etc.)
                 agent.get_kbs_from_json(ids=True)
-                
+
                 #save the KBs to a dictionary object, using node names
                 kb = agent.get_kbs_from_json(ids=False, obj=True)
-                
+
         """
-        
-        if obj == True and separated == True:
+
+        if obj is True and separated is True:
             print("obj == True and separated == True is not yet supported")
             return None
-        
+
+        if compressed == True:
+            return self._get_kbs_as_json_compressed(nodes=nodes, directory=directory, filename=filename, ids=ids)
+
         if nodes is None:
             nodes = self.all_nodes
         prev_summarize_state = self.summarize_for_single_node
         try:
             self.set_summarize_for_single_node(False)
             output = self._query(requests.get, 'get_kb', nodes=nodes)
         except Exception as e:
             print(f'failed to get kb: {e}')
             raise e
         finally:
             self.set_summarize_for_single_node(prev_summarize_state)
-        
+
         filenames = []
         if isinstance(output, dict):
             altered_output = {}
-            if ids == True and "metadata" not in output:
+            if ids is True and "metadata" not in output:
                 for key in output.keys():
                     node_id = [node["id"] for node in self.all_nodes if node['name'] == key][0]
                     altered_output[node_id] = output[key]
             else:
                 altered_output = output
             if separated:
-                for key, value in altered_output.items():
+                for key in altered_output.keys():
                     archive_file = join(directory, f'{self.gaius_agent}-{self.name}-{key}-{datetime.now()}-kb.json')
                     filenames.append(archive_file)
                     with open(archive_file, 'w') as f:
                         f.write(json.dumps({key: altered_output[key]}))
             else:
                 archive_file = join(directory, f'{self.gaius_agent}-{self.name}-{datetime.now()}-kb.json')
                 if filename:
                     archive_file = filename
-                    
+
                 filenames.append(archive_file)
-                
+
                 # return kb as json object
-                if obj == True:
+                if obj is True:
                     return altered_output
                 # otherwise write json file
                 with open(archive_file, 'w') as f:
                     f.write(json.dumps(altered_output))
-                
+
         return filenames
-    
+
+    def _load_compressed_kb(self, path):
+        node_dict = {}
+        for item in self.all_nodes:
+            node_dict[item['name']] = item['id']
+            node_dict[item['id']] = item['id']
+
+        with ZipFile(path, 'r') as kb_zip:
+            kb_names = kb_zip.namelist()
+            for filename in kb_names:
+                node_name = splitext(filename)[0]
+                if node_name not in node_dict:
+                    print(f'node {node_name} not found in topology, skipping')
+                    continue
+                with kb_zip.open(filename, 'r') as f:
+                    prim_id = node_dict[node_name]
+                    response = self.session.post(f'{self._url}{prim_id}/load_kb',
+                                            headers={'X-API-KEY': self._api_key,
+                                                    'content-type':'application/json'},
+                                            data=f)
+                    if response.status_code != 200:
+                        print(f'error loading kb for node {prim_id}: {response.text}')
+                        return 'failed', response.status_code
+                    response = self.session.post(f'{self._url}{prim_id}/working-memory/clear',
+                                                headers={'X-API-KEY': self._api_key})
+                    if response.status_code != 200:
+                        print(f'error loading kb for node {prim_id}: {response.text}')
+                        return 'failed', response.status_code
+
+                    print(f'loading node {prim_id} succeeded')
+        return 'success'
+
     @_ensure_connected
-    def load_kbs_from_json(self, path=None, obj=None):        
+    def load_kbs_from_json(self, path=None, obj=None):
         """Load KBs from a JSON file
 
         Args:
             path (str, optional): path to JSON file where KBs are stored.
             obj  (dict, optional): object to load KnowledgeBase from
 
         Returns:
             str: 'success' or 'failed'
-            
+
         Example:
             .. code-block:: python
-            
+
                 kb_path = "../path/to/kb.json"
                 agent.load_kbs_from_json(path=kb_path)
-        
+
         """
-        
+
         node_dict = {}
         for item in self.all_nodes:
             node_dict[item['name']] = item['id']
             node_dict[item['id']] = item['id']
-        
+
         kb = None
         if path is not None:
+            if is_zipfile(path):
+                # load_compressed_kb here
+                return self._load_compressed_kb(path)
+
             with open(path, 'r') as f:
                 kb = json.load(f)
         elif obj is not None:
             kb = obj
         else:
             raise Exception("Must specify path or obj argument")
-        
+
         # check if the kb is only for a single node (simple-topology edge case)
         if 'metadata' in kb.keys():
-            kb = {'P1' : kb}
+            kb = {'P1': kb}
 
         for key, value in kb.items():
             prim_id = key
             if prim_id in node_dict:
                 prim_id = node_dict[prim_id]
             else:
-                print(f'Warning, node {prim_id} not found in topology, skipping')
+                print(f'node {prim_id} not found in topology, skipping')
                 continue
             print(f'loading node {prim_id} from kb for {key}')
-            response = self.session.post(f'{self._url}{prim_id}/load_kb', headers={'X-API-KEY' : self._api_key}, json={'data': value})
+            response = self.session.post(f'{self._url}{prim_id}/load_kb',
+                                         headers={'X-API-KEY': self._api_key},
+                                         json={'data': value})
             if response.status_code != 200:
                 print(f'error loading kb for node {prim_id}: {response.text}')
                 return 'failed', response.status_code
             print(f'loading node {prim_id} succeeded')
-        
+
         return 'success'
-    
+
     @_ensure_connected
-    def put_kbs(self, archive_file):
+    def load_kbs_from_json_iter(self, path):
+        """Uses ijson library to load KBs more efficiently
+
+        Args:
+            path (str): path to JSON file where KBs are stored.
+
+
+        Returns:
+            str: 'success' or 'failed'
+
+        Example:
+            .. code-block:: python
+
+                kb_path = "../path/to/kb.json"
+                agent.load_kbs_from_json(path=kb_path)
+
+        """
+        import ijson
+
+        node_dict = {}
+        for item in self.all_nodes:
+            node_dict[item['name']] = item['id']
+            node_dict[item['id']] = item['id']
+
+        with open(path, 'rb') as kb_file:
+            for key, value in ijson.kvitems(kb_file, '', use_float=True):
+                prim_id = key
+                if key in ['symbols_kb', 'vectors_kb', 'models_kb', 'metadata']:
+                    raise Exception(f'use load_kbs_from_json() for a simple node')
+                if prim_id in node_dict:
+                    prim_id = node_dict[prim_id]
+                else:
+                    print(f'node {prim_id} not found in topology, skipping')
+                    continue
+                print(f'loading node {prim_id} from kb for {key}')
+                response = self.session.post(f'{self._url}{prim_id}/load_kb',
+                                                headers={'X-API-KEY': self._api_key},
+                                                json={'data': value})
+                if response.status_code != 200:
+                    print(f'error loading kb for node {prim_id}: {response.text}')
+                    return 'failed'
+                print(f'loading node {prim_id} succeeded')
+
+        return 'success'
+
+    @_ensure_connected
+    def put_kbs(self, archive_file): # pragma: no cover
         """Uploads KBs from local archive_file file.
-        
-        .. warning:: 
-        
+
+        .. warning::
+
             .. deprecated:: 12.0 (Kehl)
-            
+
             Use :func:`load_kbs_from_json` instead.
-        
+
         """
         _headers = self._headers
         _headers['Content-Encoding'] = 'gzip'
         _headers['Content-type'] = 'application/octet-stream'
         with open(archive_file, 'rb') as f:
             data = f.read()
-            response = self.session.put(f'{self._url}database', 
-                        headers=_headers,
-                        verify=self._verify,
-                        data=data)
-        return response.json()
+            response = self.session.put(f'{self._url}database',
+                                        headers=_headers,
+                                        verify=self._verify,
+                                        data=data
+                                        ).json()
+        return response
 
     def set_target_class(self, target_class: str, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Provide a target_class symbol for the searcher to look for.
 
-        The searcher will ignore all other classes. This is a symbol that is in the last event of a classification
-        sequence.
-        
+        The searcher will ignore all other classes. This is a symbol that
+        is in the last event of a classification sequence.
+
         Example:
                 .. code-block:: python
 
                     agent.set_target_class(target_class="apple", nodes=["P1"])
-                    
+
         .. note::
 
-            This will result in the nodes specified only predicting on models that include the target class
+            This will result in the nodes specified only predicting on models
+            that include the target class
         """
         if nodes is None:
             nodes = self.query_nodes
-        return self._query(self.session.post, 'set-target-class', nodes=nodes, data=target_class)
+        return self._query(self.session.post,
+                           'set-target-class',
+                           nodes=nodes,
+                           data=target_class)
 
     def clear_target_class(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
         """Clears target selection.
-        
+
             Example:
                 .. code-block:: python
 
                     agent.clear_target_class(nodes=["P1"])
         """
         if nodes is None:
             nodes = self.query_nodes
-        return self._query(self.session.post, 'clear-target-class', nodes=nodes)
+        return self._query(self.session.post,
+                           'clear-target-class',
+                           nodes=nodes)
 
     @_ensure_connected
-    def tf_attach(self, name, config):
-        return self.session.post(f'{self._url}/thinkflux/{name}/attach', data={'config' : config})
-    
-    @_ensure_connected    
-    def tf_remove(self, name):
-        return self.session.delete(f'{self._url}/thinkflux/{name}/remove')
+    def get_symbol(self, symbol_name: str, nodes: List = None) -> Union[dict, Any]:
+        """Returns symbol with name *symbol_name*.
+
+        Args:
+            symbol_name (str): Name of symbol to retrieve
+            nodes (List, optional): list of nodes to retrieve symbol information from.
+                Defaults to None (all nodes).
+
+        Returns:
+            Union[dict, Any]: dictionary of {node_name : symbol} pairs
+        Example:
+                .. code-block:: python
+
+                    agent.get_symbol("WEATHER|CLOUDY")
+
+        """
+        if nodes is None:
+            nodes = self.all_nodes
+        else:
+            nodes = [node for node in self.all_nodes if (node['name'] in nodes)]
+        result = {}
+        for node in nodes:
+            try:
+                response = self.session.get(f"{self._url}{node['id']}/symbol/{symbol_name}",
+                                            headers=self._headers,
+                                            verify=self._verify
+                                            ).json()
+                if 'error' in response or response['status'] == 'failed':
+                    if len(nodes) == 1 and self.summarize_for_single_node:
+                        raise AgentQueryError(response)
+                    warnings.warn(response["message"], AgentQueryWarning)
+                if len(nodes) == 1 and self.summarize_for_single_node:
+                    return response['message']
+                else:
+                    result[node['name']] = response['message']
+            except Exception as exception:
+                raise AgentQueryError(str(exception)) from None
+
+        return result
     
     @_ensure_connected
-    def tf_list(self):
-        return self.session.get(f'{self._url}/thinkflux/list')
-    
+    def clear_snapshots(self, nodes: List = None) -> Union[dict, Tuple[dict, str]]:
+        """Clear the WM snapshots of the Agent.
+        Will not delete any persisted memory from the KnowledgeBase
+
+        Example:
+            .. code-block:: python
+
+                >>> agent.clear_snapshots(nodes=['P1'])
+                'snapshots-cleared'
+        """
+        if nodes is None:
+            nodes = self.all_nodes
+        return self._query(self.session.post, 'snapshots/clear', nodes=nodes)
+
     @_ensure_connected
     def investigate_record(self, node, record: str) -> dict:
-        """Function for drilling down on a model recursively in a multi-node agent. Will retrieve all data "under"
-        the abstracted model, giving a complete representation of the abstracted model
+        """Function for drilling down on a model recursively in a multi-node
+        agent. Will retrieve all data "under" the abstracted model,
+        giving a complete representation of the abstracted model
 
         Args:
-            node (list or str): the node to start at/containing the model provided in `record`: e.g. ['P4'] or 'P4'
+            node (list or str): the node to start at/containing
+                the model provided in `record`: e.g. ['P4'] or 'P4'
             record (str): the model to search for
 
         Returns:
-            dict: recursive structure containing a complete representation of the abstracted model
+            dict: recursive structure containing a complete representation
+            of the abstracted model
         """
         data = {}
-        try: 
+        try:
+            prev_summarize_state = self.summarize_for_single_node
+            self.set_summarize_for_single_node(True)
             if isinstance(node, list):
                 node = node[0]
-            try:
-                # if the node passed is a primitive_id, get the name (P1, P2, etc.) of the node
+
+            # if the node passed is a primitive_id, get the name
+            # (P1, P2, etc.) of the node
+            if node in self.genome.primitives:
                 node = self.genome.primitives[node]['name']
-            except:
-                pass
-            # print(f"investigating record {record}")
-            return self.__get_model_details(model=record, node=[node], topLevel=True)
+
+            return self.__get_model_details(model=record,
+                                            node=[node],
+                                            topLevel=True)
 
         except Exception as e:
             print(str(e))
+            traceback.print_exc()
+        finally:
+            self.set_summarize_for_single_node(prev_summarize_state)
         return data
 
     @_ensure_connected
     def investigate(self, record: str) -> dict:
-        """Higher level implementation of :func:`investigate_record` that does not require a node to be entered.
-        Operates on abstracted symbols, models, etc. Useful when applying in a programatic manner, where the node
-        a symbol comes from is unknown. May throw exception if unable to identify a starting point.
-        
+        """Higher level implementation of :func:`investigate_record` that
+        does not require a node to be entered. Operates on abstracted
+        symbols, models, etc. Useful when applying in a programatic
+        manner, where the node a symbol comes from is unknown.
+        May throw exception if unable to identify a starting point.
+
         Args:
             record (str): the symbol to look for
 
         Returns:
-            dict: recursive structure containing a complete representation of the abstracted model
-            
+            dict: recursive structure containing a complete representation
+            of the abstracted model
+
         Example:
             .. code-block:: python
-            
+
                 record = 'PRIMITIVE|p124b23f9|004da01b0ef40d7c3e0965a6b4fd0f413672fbff|matches|KEY|VALUE'
                 traceback = agent.investigate(record=record)
         """
         try:
 
             split_record = str(record).split('|')
             if split_record[0] == 'PRIMITIVE':
                 if len(split_record) < 3:
                     raise Exception(f'Investigate does not know what to do with symbol: {record}')
-                    
+
                 # print(f'investigating model {split_record[2]} on node {split_record[1]}')
-                output = self.investigate_record(record=split_record[2], node=split_record[1])
-                if not output: 
+                output = self.investigate_record(record=split_record[2],
+                                                 node=split_record[1])
+                if not output:
                     return {}
                 query = {
                     'record': record,
-                    'node_id' : split_record[1],
+                    'node_id': split_record[1],
                     'name': split_record[2]
                 }
                 return {'query': query,
                         'results': output
                         }
             else:
                 prev_summarize_state = self.summarize_for_single_node
@@ -1411,109 +1754,121 @@
                     for k, v in tmp_model.items():
                         if v:
                             actual_model_dict[k] = v
                     # print(f'{actual_model_dict = }')
                     if len(actual_model_dict) == 1:
                         for k, v in actual_model_dict.items():
                             # print(f'{k = }, {v = }')
-                            output = self.investigate_record(record=v['name'], node=[k])
+                            output = self.investigate_record(record=v['name'],
+                                                             node=[k])
                             query = {
                                 'record': v['name'],
-                                'node_id' : k,
+                                'node_id': k,
                                 'name': v['name']
                             }
-                            return_data = {'query': query,
-                                    'results': output
-                            }
-                            # print(f'{return_data = }')
-                            return return_data
+
+                            return {'query': query,
+                                    'results': output}
                 except Exception as e:
                     print(f'Exception in investigate call: {e}')
                 finally:
                     self.set_summarize_for_single_node(prev_summarize_state)
         except Exception as e:
             print(f'Exception in investigate call: {e}')
         return {}
 
     @_ensure_connected
     def __get_model_details(self, model, node, topLevel=False):
-        """Recursive function to get details about a specific model on a specific node
+        """Recursive function to get details about a specific
+        model on a specific node
 
         Args:
             model (str): the model hash to look for
-            node (list(str)): The node to look for the model on (provided as a list with a single element)
-            topLevel (bool, optional): flag used to show that the function is at the top level (no recursing). Defaults to False.
+            node (list(str)): The node to look for the model on (provided as
+                a list with a single element)
+            topLevel (bool, optional): flag used to show that the function
+                is at the top level (no recursing). Defaults to False.
 
         Returns:
-            dict: recursive structure representing the data from the topLevel model
+            dict: recursive structure representing the data from the
+            topLevel model
         """
-        if model == None:
+        if model is None:
+            return None
+        p_id = self.genome.get_primitive_map().get(node[0], None)
+        if p_id is None:
             return None
-        p_id = self.genome.get_primitive_map()[node[0]]
+
+        p_name = p_id
+        if p_id in self.genome.primitives:
+            p_name = self.genome.primitives[p_id]['name']
+        # print(f'{p_id=}, {p_name=}')
         if topLevel is True:
             # top level request
-            record_data = {'record' : f"{model}",
-                        'subitems':[],
-                        'model': self.get_model(model, nodes=node),
-                        'node': p_id,
-                        'topLevel' : topLevel,
-                        'bottomLevel' : False,
-            }
-        else:            
-            record_data = {'record' : f"PRIMITIVE|{p_id}|{model['name']}",
-                        'subitems':[],
-                        'model': model,
-                        'node': p_id,
-                        'topLevel' : topLevel,
-                        'bottomLevel' : False
-            }
+            record_data = {'record': f"{model}",
+                           'subitems': [],
+                           'model': self.get_model(model, nodes=node),
+                           'node': p_name,
+                           'node_id': p_id,
+                           'topLevel': topLevel,
+                           'bottomLevel': False}
+        else:
+            record_data = {'record': f"PRIMITIVE|{p_id}|{model['name']}",
+                           'subitems': [],
+                           'model': model,
+                           'node': p_name,
+                           'node_id': p_id,
+                           'topLevel': topLevel,
+                           'bottomLevel': False}
+
         for event_list in record_data['model']['sequence']:
             event = []
             for item in event_list:
                 symbol = {}
                 split_model = item.split('|')
                 if split_model[0] == 'PRIMITIVE':
                     node_id = split_model[1]
-                    try:
+
+                    node_name = node_id
+                    if node_id in self.genome.primitives:
                         node_name = self.genome.primitives[node_id]['name']
-                    except:
-                        # node name already provided
-                        node_name = node_id
-                        pass
-                    sub_model = self.get_model(split_model[2], nodes=[node_name])
-                    symbol = self.__get_model_details(model=sub_model, node=[node_name])
+
+                    sub_model = self.get_model(split_model[2],
+                                               nodes=[node_name])
+                    symbol = self.__get_model_details(model=sub_model,
+                                                      node=[node_name])
                 elif split_model[0] == 'VECTOR':
                     symbol = {'record': item,
-                                'data'  : self.get_vector(item, nodes=node),
-                                'subitems': None,
-                                'bottomLevel': True,
-                                'topLevel' : False,
-                                'node':node[0]}
+                              'data': self.get_vector(item, nodes=node),
+                              'subitems': None,
+                              'bottomLevel': True,
+                              'topLevel': False,
+                              'node': node[0],
+                              'node_id': p_id}
                 else:
                     # print(f'reached symbol: {item}')
-                    if 'VECTOR' in item:
-                        symbol = {'record': item,
-                                    'data'  : self.get_vector(item, nodes=node),
-                                    'subitems': None,
-                                    'bottomLevel': True,
-                                    'topLevel' : False,
-                                    'node' : node[0]}
-                    else:
-                        symbol = item
+                    # if 'VECTOR' in item:
+                    #     symbol = {'record': item,
+                    #               'data': self.get_vector(item, nodes=node),
+                    #               'subitems': None,
+                    #               'bottomLevel': True,
+                    #               'topLevel': False,
+                    #               'node': node[0],
+                    #               'node_id': p_id}
+                    # else:
+                    symbol = item
                 event.append(deepcopy(symbol))
             record_data["subitems"].append(event)
         if tuple(record_data["subitems"]) == tuple(record_data["model"]["sequence"]):
             del record_data["subitems"]
-        
-        
+
         if 'subitems' in record_data:
             unique_subitems = []
             for subitem in record_data['subitems']:
                 if subitem not in unique_subitems:
                     unique_subitems.append(subitem)
-            
+
             record_data["subitems"] = tuple(unique_subitems)
         else:
             record_data['bottomLevel'] = True
 
-        
-        return record_data
+        return record_data
```

### Comparing `ia-sdk-0.3.9/ia/gaius/back_testing.py` & `ia-sdk-0.4.0/ia/gaius/back_testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 from ia.gaius.data_ops import Data
 from ia.gaius.tests import classification, utility
 
 import plotly.express as px
 from plotly.subplots import make_subplots
 import plotly.graph_objects as go
 import json 
-from math import pi, cos, sin 
+from math import pi
 import pandas as pd 
 from sklearn.metrics import accuracy_score, precision_score
-import collections 
 
 class BackTest:
     """Provides an interface for backtesting."""
     def __init__(self, **kwargs):
         """
         Pass this a configuration dictionary as the argument such as:
```

### Comparing `ia-sdk-0.3.9/ia/gaius/data_language.py` & `ia-sdk-0.4.0/ia/gaius/data_language.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.3.9/ia/gaius/data_ops.py` & `ia-sdk-0.4.0/ia/gaius/pvt/mongo_interface.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,299 +1,410 @@
-import os
 import random
-import re
 import pymongo
 import json
 from bson.objectid import ObjectId
 from copy import deepcopy
+import zipfile
 import datetime
+from traceback import print_exc
 import io
-
-def validate_data(data: dict):
-    """Validates if the data is in correct GAIuS digestible format.
-    Returns True if data validates.  Returns False if data does not validate.
-    
-    Args:
-        data (dict, required): GDF to validate
-    
-    Example: 
-        .. code-block:: python
-
-            >>> gdf = {'strings':["hello"], 'vectors': [], 'emotives': {} }
-            >>> validate_data(gdf)
-            True
-            >>> bad_gdf = {'strings': []}
-            >>> validate_data(bad_gdf)
-            Exception: Dictionary requires "vectors", "emotives", and "strings" as keys!
-            >>> bad_gdf_2 = {'strings':["hello"], 'vectors': [], 'emotives': ['utility|5'] }
-            >>> validate_data(bad_gdf_2)
-            Exception: "emotives" must be a dict of <str, float>. Dict not provided!
-            
-    """
-    if not isinstance(data, dict):
-        raise Exception("Incorrect data type.  Must be a dictionary.")
-    if "vectors" not in list(data.keys()) or "emotives" not in list(data.keys()) or "strings" not in list(
-            data.keys()):
-        raise Exception('Dictionary requires "vectors", "emotives", and "strings" as keys!')
-    for key in list(data.keys()):
-        if key not in ["vectors", "emotives", "strings", "metadata"]:
-            raise Exception("Key: %s, should not be in the data dictionary!")
-    
-    if not isinstance(data["strings"], list):
-            raise Exception('"strings" must be a list of strings.  List not provided!')
-    for item in data["strings"]:
-        if not (isinstance(item, str) or isinstance(item, str)):
-            raise Exception('"strings" must be a list of strings or unicode objects!')
-    
-    if not isinstance(data["emotives"], dict):
-        raise Exception('"emotives" must be a dict of <str, float>. Dict not provided!')
-    for item in data["emotives"]:
-        if not isinstance(item, (int, float)):
-            raise Exception('"emotives" must be a dict of <str, float>!')
-    
-    if not isinstance(data["vectors"], list):
-        raise Exception('"vectors" must be a list of arrays.  List not provided!')
-    for item in data["vectors"]:
-        if not isinstance(item, list):
-            raise Exception('"vectors" must be a list of arrays (i.e. lists)!')
-    return True
-
-def raw_in_count(filename: str):
-    return int(os.popen("sed -n '$=' '%s'" % filename).readline().split()[0])
+from ia.gaius.data_ops import validate_data
 
 
-def atoi(text: str):
-    """Attempt to convert string to int"""
-    return int(text) if text.isdigit() else text
-
-
-def natural_keys(text: str):
-    """
-    alist.sort(key=natural_keys) sorts in human order
-    http://nedbatchelder.com/blog/200712/human_sorting.html
-    (See Toothy's implementation in the comments)
-    """
-    return [atoi(c) for c in re.split(r'(\d+)', text)]
+class MongoDataRecords:
+    def __init__(self,
+                 dataset_records,
+                 DR: float,
+                 DF: float,
+                 shuffle: bool):
+        """
+        Args:
+            dataset_records (str or list, required): List of mongo
+                ObjectIds to use as data records
+            DR (float, required): fraction of total data to use for
+                testing and training. 0 < DR < 100
+            DF (float, required): fraction of the DR to use for training.
+                The rest of the DR is used for testing. 0 < DF < 100
+            shuffle (bool, required): whether to shuffle the
+                data when creating sets
 
-class DataRecords:
-    """Splits data into random sets for training and testing."""
+            After creating the class, utilize the member variables
+                `train_sequences` and `test_sequences` for the data sets
 
-    def __init__(self, original_dataset, DR: float, DF: float, shuffle: bool, folder:bool=True):
-        """
-        Args:
-            original_dataset (str or list, required): location of dataset to use for training and testing sets
-            DR (float, required): fraction of total data to use for testing and training. 0 < DR < 100
-            DF (float, required): fraction of the DR to use for training.  The rest of the DR is used for testing. 0 < DF < 100
-            shuffle (bool, required): whether to shuffle the data when creating sets
-            folder (bool, optional): set if the original dataset is a folder
-            
-        After creating the class, utilize the member variables `train_sequences` and `test_sequences` for the data sets
-        
-        :ivar train_sequences: the files to use for training
-        :ivar test_sequences: the files to use for testing
+        :ivar train_sequences: the mongo documents to use for training
+        :ivar test_sequences: the mongo documents to use for testing
         """
-        if folder:
-            original_dataset = [original_dataset + '/' + f for f in os.listdir(original_dataset) if
-                                not f.startswith('.') and not f.startswith('_')]
-            original_dataset.sort(key=natural_keys)
         DR = DR / 100
         DF = DF / 100
+        self.random = random.Random()
+
+        if DR > 1 or DF > 1:
+            raise Exception(f'Invalid value provided for DR or DF: \
+                            {DR=}, {DF=}')
+
         try:
+            if shuffle:
+                self.random.shuffle(dataset_records)
             if DR == 1 and DF == 1:
-                self.train_sequences = original_dataset
+                self.train_sequences = dataset_records
                 self.test_sequences = []
             else:
-                if shuffle:
-                    random.shuffle(original_dataset)
+                num_files = len(dataset_records)
+                # use a fraction of the whole set
+                num_use_files = int(num_files * DR)
 
-                num_files = len(original_dataset)
-                num_use_files = int(num_files * DR)  ## use a fraction of the whole set
-
-                num_train_sequences = int(num_use_files * DF)  ## train 2/3rds, test 1/3rd
+                num_train_sequences = int(num_use_files * DF)
                 num_test_sequences = num_use_files - num_train_sequences
 
-                self.train_sequences = original_dataset[:num_train_sequences]
-                self.test_sequences = original_dataset[num_train_sequences:(num_train_sequences + num_test_sequences)]
+                self.train_sequences = dataset_records[:num_train_sequences]
+                self.test_sequences = dataset_records[num_train_sequences:(
+                    num_train_sequences + num_test_sequences)]
         except Exception as exception:
-            print(f'DataRecords BROKE by {exception.args}')
+            print(f'MongoDataRecords BROKE by {exception.args}')
             raise
 
-class Data:
-    def __init__(self, data_directories=None, dataset=None):
-        """Supply either a list of data_directories, or a dataset."""
-        if data_directories is not None:
-            self.data_directories = data_directories
-            self.dataset = None
-        elif dataset is not None:
-            self.data_directories = None
-            self.dataset = dataset
-        self.train_sequences = []
-        self.test_sequences = []
-        self.train_sequences_classes = []
-        self.test_sequences_classes = []
 
-    def prep(self, percent_of_dataset_chosen:float, percent_reserved_for_training:float, shuffle:bool=False):
-        if self.data_directories:
-            data = [DataRecords(d, percent_of_dataset_chosen, percent_reserved_for_training, shuffle, folder=True) for d
-                    in self.data_directories]  ## It's a list because the user may pick several data file directories.
-        elif self.dataset:
-            data = [DataRecords(self.dataset, percent_of_dataset_chosen, percent_reserved_for_training, shuffle,
-                                folder=False)]
+def check_dataset_exists(mongo_db,
+                         dataset_collection_name: str,
+                         user_id: str,
+                         dataset_id: str):
+    """Will check if the specified dataset is found in MongoDB
 
-        self.train_sequences = []
-        self.test_sequences = []
-        for d in data:
-            self.train_sequences += d.train_sequences
-            self.test_sequences += d.test_sequences
+    Args:
+        mongo_db : MongoDB database object
+        dataset_collection_name (str): collection name where
+            master dataset record is saved
+        user_id (string): user unique identifier
+        dataset_id (string): dataset unique identifier
 
-class MongoDataRecords:
-    def __init__(self, dataset_document_list, DR: float, DF: float, shuffle: bool):
-        """
-        Args:
-            dataset_document_list (str or list, required): List of mongo ObjectIds to use as data records
-            DR (float, required): fraction of total data to use for testing and training. 0 < DR < 100
-            DF (float, required): fraction of the DR to use for training.  The rest of the DR is used for testing. 0 < DF < 100
-            shuffle (bool, required): whether to shuffle the data when creating sets
+    Returns:
+        bool: represents whether the dataset was successfully found
+    """
+    dataset_obj = {'user_id': user_id,
+                   'dataset_id': dataset_id}
 
-            After creating the class, utilize the member variables `train_sequences` and `test_sequences` for the data sets
+    # checking if dataset count != 1. If >1, something nefarious is
+    # potentially happening
+    if mongo_db[dataset_collection_name].count_documents({**dataset_obj}) != 1:
+        return False
+    return True
 
-        :ivar train_sequences: the mongo documents to use for training
-        :ivar test_sequences: the mongo documents to use for testing
-        """
-        DR = DR / 100
-        DF = DF / 100
-        
-        if DR > 1 or DF > 1:
-            raise Exception(f'Invalid value provided for DR or DF: {DR=}, {DF=}')
-        
-        try:
-            if DR == 1 and DF == 1:
-                self.train_sequences = dataset_document_list
-                self.test_sequences = []
-            else:
-                if shuffle:
-                    random.shuffle(dataset_document_list)
 
-                num_files = len(dataset_document_list)
-                num_use_files = int(num_files * DR)  ## use a fraction of the whole set
+class MongoData:
+    """
+        Analogous object to the Data class, but utilizes a MongoDB cursor
+        instead of a directory to reference data records
 
-                num_train_sequences = int(num_use_files * DF)  ## train 2/3rds, test 1/3rd
-                num_test_sequences = num_use_files - num_train_sequences
+        Start with a MongoDB document containing the name of all dataset
+        files (located separately)
 
-                self.train_sequences = dataset_document_list[:num_train_sequences]
-                self.test_sequences = dataset_document_list[num_train_sequences:(num_train_sequences + num_test_sequences)]
-        except Exception as exception:
-            print(f'MongoDataRecords BROKE by {exception.args}')
-            raise
+        Only retrieve actual data files when calling retrieveDataRecord.
+        Overloaded iterator functions to allow treating of object
+        as a list.
 
+        Example:
 
-class MongoData:
-    """
-        Analogous object to the Data class, but utilizes a MongoDB cursor instead of a directory to reference data records
-        Start with a MongoDB document containing the name of all dataset files (located separately)
-    
-        Only retrieve actual data files when calling retrieveDataRecord. Overloaded iterator functions to allow treating of object
-        as a list.
-        
-        Example: 
-        .. code-block:: python
+            .. code-block:: python
 
-            >>> mongo = pymongo.MongoClient('mongodb://mongodb:27017/')
-            >>> dataset_details = {"user_id": "ABCD1",
-                                   "dataset_id": "iris_0_0_13"}
-            >>> md = MongoData(mongo_dataset_details=dataset_details, 
-                               mongo_db=mongo_db, 
-                               data_files_collection_name='dataset_files')
-            >>> md.prep(percent_of_dataset_chosen=50, 
-                        percent_reserved_for_training=50, 
-                        shuffle=True)
-            >>> md.setIterMode('testing')
-            >>> for record in md:
+                >>> mongo = pymongo.MongoClient('mongodb://mongodb:27017/')
+                >>> mongo_db = mongo.db['main_database']
+                >>> dataset_details = {"user_id": "ABCD1",
+                                    "dataset_id": "iris_0_0_13"}
+                >>> md = MongoData(mongo_dataset_details=dataset_details,
+                                mongo_db=mongo_db,
+                                data_files_collection_name='dataset_files')
+                >>> md.prep(percent_of_dataset_chosen=50,
+                            percent_reserved_for_training=50,
+                            shuffle=True)
+                >>> md.setIterMode('testing')
+                >>> for record in md:
                 ...
-        
+
     """
-    def __init__(self, mongo_dataset_details: dict, data_files_collection_name: str, mongo_db:pymongo.MongoClient):
+
+    def __init__(self,
+                 mongo_dataset_details: dict,
+                 data_files_collection_name: str,
+                 mongo_db: pymongo.MongoClient,
+                 dataset_collection_name: str = 'datasets'):
         """Initialized dataset object from MongoDB
 
         Args:
-            mongo_dataset_details (dict): _description_
-            data_files_collection_name (str): _description_
-            mongo_db (pymongo.MongoClient): _description_
+            mongo_dataset_details (dict): contains info about the user_id
+                and dataset_id of the dataset. Used to query MongoDB
+            data_files_collection_name (str): Collection in MongoDB where
+                individual data records are stored
+            dataset_collection_name (str): Collection in MongoDB where master
+                dataset info record is stored
+            mongo_db (pymongo.MongoClient): MongoDB client object to use
+                for dataset lookups
 
         Raises:
             Exception: user_id field missing from mongo_dataset_details
             Exception: dataset_id field missing from mongo_dataset_details
-            Exception: multiple datasets found pertaining to same user_id and dataset_id field
+            Exception: multiple datasets found pertaining to same user_id
+                and dataset_id field
         """
-        if not 'user_id' in mongo_dataset_details:
-            raise Exception(f'user_id field missing from mongo_dataset_details ({mongo_dataset_details=})')
-        if not 'dataset_id' in mongo_dataset_details:
-            raise Exception(f'dataset_id field missing from mongo_dataset_details ({mongo_dataset_details=})')
-            
+        if 'user_id' not in mongo_dataset_details:
+            raise Exception(f'user_id field missing from mongo_dataset_details\
+                            ({mongo_dataset_details=})')
+        if 'dataset_id' not in mongo_dataset_details:
+            raise Exception(f'dataset_id field missing from \
+                            mongo_dataset_details ({mongo_dataset_details=})')
+
         self._mongo_dataset_details = deepcopy(mongo_dataset_details)
         self._data_files_collection_name = deepcopy(data_files_collection_name)
         self.mongo_db = mongo_db
-        
+
         # initialize iteration variables
         self._iter_mode = None
         self.__curr = None
         self.__term = None
-        
-        if not 'files' in self._mongo_dataset_details:
-            dataset_obj = {'user_id':self._mongo_dataset_details['user_id'],
-                       'dataset_id':self._mongo_dataset_details['dataset_id']}
-            
-            if mongo_db['datasets'].count_documents(dataset_obj) != 1:
-                raise Exception(f'{mongo_db["datasets"].count_documents(dataset_obj)} dataset records found for {dataset_obj=}')
-        
-            dataset = mongo_db['datasets'].find_one(dataset_obj)
-            
-        self._mongo_dataset_details['files'] = [item for item in dataset['dataset']['files']]
-        
-        
+
+        self.percent_of_dataset_chosen = None
+        self.percent_reserved_for_training = None
+        dataset_obj = {'user_id': self._mongo_dataset_details['user_id'],
+                       'dataset_id': self._mongo_dataset_details['dataset_id']}
+
+        ds_count: int = mongo_db[dataset_collection_name].count_documents(
+            dataset_obj)
+
+        if ds_count != 1:
+
+            raise Exception(f'{ds_count} \
+                            dataset records found for {dataset_obj=}')
+
+        dataset = mongo_db[dataset_collection_name].find_one(dataset_obj)
+
+        self._mongo_dataset_details['files'] = \
+            [item for item in dataset['dataset']['files']]
+
         self.train_sequences = []
         self.test_sequences = []
 
-    def prep(self, percent_of_dataset_chosen:float, percent_reserved_for_training:float, shuffle:bool=False):
-        """Prepare the dataset
+    @classmethod
+    def upload_dataset(cls, mongo_db, dataset_details: dict, filepath: str):
+        """Upload a dataset to MongoDB from a local filepath
 
         Args:
-            percent_of_dataset_chosen (float): The percent of the dataset to utilize
-            percent_reserved_for_training (float): The training/testing split for the dataset (e.g. set to 80 for 80/20 trianing/testing split)
-            shuffle (bool, optional): Whether to shuffle the data. Defaults to False.
+            mongo_db (pymongo.MongoClient): MongoDB Database object
+            dataset_details (dict): Dictionary containing details about
+            dataset (e.g. name, user_id, dataset_id, collection names, etc.)
+            filepath (str): filepath of zip folder
+                containing dataset (GDF records)
+
+        Returns:
+            _type_: _description_
+
+        Example:
+            .. code-block:: python
+
+                from ia.gaius.pvt.mongo_interface import MongoData
+                ...
+                dataset_details = {"user_id": "user-1234",
+                                   "dataset_name": "MNIST",
+                                   "dataset_id": "abba12",
+                                   "data_files_collection_name": "dataset_files",
+                                   "dataset_collection_name": "datasets"}
+                MongoData.upload_dataset(mongo_db=mongo_db,
+                                         dataset_details=dataset_details)
+
+        """
+
+        data_files_collection_name = dataset_details['data_files_collection_name']
+        dataset_collection_name = dataset_details['dataset_collection_name']
+
+        # ensure dataset details has user_id and dataset_id fields
+        if 'user_id' not in dataset_details:
+            raise Exception(
+                f'user_id field missing from dataset_details ({dataset_details=})')
+        if 'dataset_id' not in dataset_details:
+            raise Exception(
+                f'dataset_id field missing from dataset_details ({dataset_details=})')
+
+        cur_time = datetime.datetime.now().isoformat()
+        dataset_obj = {'user_id': dataset_details['user_id'],
+                       'dataset_id': dataset_details['dataset_id'],
+                       'lastModifiedDate': cur_time,
+                       'uploadedDate': cur_time,
+                       'size': None,
+                       'dataset': {'files': []}}
+
+        # retrieve dataset from filepath
+        # if anything fails along the way, try to remediate database
+        # by deleting stuff already inserted
+        try:
+            with zipfile.ZipFile(filepath, 'r') as zipObject:
+                dataset_obj['size'] = sum(
+                    [zinfo.file_size for zinfo in zipObject.filelist])
+                records = zipObject.namelist()
+                records = [(zipObject.read(item), item)
+                           for item in records if not item.endswith('/') or item.startswith('.') or item.startswith('__')]
+                records = [{'file': item[0],
+                            'filename': item[1],
+                            'user_id': dataset_obj['user_id'],
+                            'dataset_id': dataset_obj['dataset_id']}
+                           for item in records]
+
+                # upload individual records to MongoDB data_files collection
+                try:
+                    insert_result = mongo_db[data_files_collection_name].insert_many(
+                        records)
+                except Exception as e:
+                    print(f'failed to insert records: {str(e)}')
+                    try:
+                        mongo_db[data_files_collection_name].delete_many(
+                            {'dataset_id': dataset_obj['dataset_id']})
+                    except Exception as e2:
+                        print(
+                            f'failed to remediate data files collection: {str(e2)}')
+                    finally:
+                        return f'failed to insert records: {str(e)}'
+                dataset_items = insert_result.inserted_ids
+                dataset_obj['dataset']['files'] = dataset_items
+                dataset_obj['dataset']['file_count'] = len(dataset_items)
+
+                try:
+                    # upload master dataset record to MongoDB dataset_collection_name
+                    mongo_db[dataset_collection_name].insert_one(dataset_obj)
+                except Exception as e:
+                    print(f'failed to insert master record: {str(e)}')
+                    try:
+                        mongo_db[dataset_collection_name].delete_one(
+                            dataset_obj)
+                        mongo_db[data_files_collection_name].delete_many(
+                            {'dataset_id': dataset_obj['dataset_id']})
+                    except Exception as e2:
+                        print(f'failed to remediate database: {str(e2)}')
+                    finally:
+                        return f'failed to insert master dataset record: {str(e)}'
+
+        except Exception as e3:
+            print(f'failed in zipfile handling: {str(e3)}')
+            print_exc()
+            return f'failed in zipfile handling: {str(e3)}'
+
+        return 'success!!!'
+
+    @classmethod
+    def delete_dataset(cls, mongo_db, dataset_details: dict):
+        """Upload a dataset to MongoDB from a local filepath
+
+        Args:
+            mongo_db (pymongo.MongoClient): MongoDB database object
+            dataset_details (dict): Dictionary containing details about
+                dataset (e.g. name, user_id, dataset_id, collection names)
+
+        Returns:
+            str: String depicting action that was taken
+
+        Example:
+            .. code-block:: python
+
+                from ia.gaius.pvt.mongo_interface import MongoData
+                ...
+                dataset_details = {"user_id": "user-1234",
+                                   "dataset_name": "MNIST",
+                                    "dataset_id": "abba12",
+                                    "data_files_collection_name": "dataset_files",
+                                    "dataset_collection_name": "datasets"}
+                MongoData.delete_dataset(mongo_db=mongo_db,
+                                         dataset_details=dataset_details)
+
         """
-        data = [MongoDataRecords(deepcopy(self._mongo_dataset_details['files']), percent_of_dataset_chosen, percent_reserved_for_training, shuffle)]
+        data_files_collection_name = dataset_details['data_files_collection_name']
+        dataset_collection_name = dataset_details['dataset_collection_name']
+        try:
+            if not check_dataset_exists(mongo_db=mongo_db,
+                                        dataset_collection_name=dataset_collection_name,
+                                        user_id=dataset_details['user_id'],
+                                        dataset_id=dataset_details['dataset_id']):
+                return 'dataset-not-found'
+        except Exception as e:
+            print(f"error while checking if dataset exists: {str(e)}")
+            raise e
+        dataset_obj = {'user_id': dataset_details['user_id'],
+                       'dataset_id': dataset_details['dataset_id']}
+        dataset = None
+        try:
+            if mongo_db[dataset_collection_name].count_documents({**dataset_obj}) != 1:
+                raise Exception(
+                    f'found {mongo_db[dataset_collection_name].count_documents({**dataset_obj})} datasets in mongo, expecting 1')
+            dataset = mongo_db[dataset_collection_name].find_one(
+                {**dataset_obj})
+        except Exception as e:
+            print(f"error while retrieving dataset: {e}")
+            raise e
+
+        try:
+            mongo_db[data_files_collection_name].delete_many(
+                {'_id': {'$in': dataset['dataset']['files']}})
+        except Exception as e:
+            print(e)
+            raise e
+
+        mongo_db[dataset_collection_name].delete_one({**dataset_obj})
+
+        return 'deleted'
+
+    def prep(self,
+             percent_of_dataset_chosen: float,
+             percent_reserved_for_training: float,
+             shuffle: bool = False):
+        """Prepare the dataset
+
+        Args:
+            percent_of_dataset_chosen (float): The percent of the dataset
+                to utilize
+            percent_reserved_for_training (float): The training/testing
+                split for the dataset (e.g.
+                set to 80 for 80/20 training/testing split)
+            shuffle (bool, optional): Whether to shuffle the data.
+                Defaults to False.
+        """
+        self.percent_of_dataset_chosen = percent_of_dataset_chosen
+        self.percent_reserved_for_training = percent_reserved_for_training
+        
+        data = [MongoDataRecords(deepcopy(self._mongo_dataset_details['files']),
+                                 percent_of_dataset_chosen,
+                                 percent_reserved_for_training,
+                                 shuffle)]
 
         self.train_sequences = []
         self.test_sequences = []
         for d in data:
             self.train_sequences += d.train_sequences
             self.test_sequences += d.test_sequences
-            
-    
+
     def retrieveDataRecord(self, document_id: ObjectId):
-        """Retrieve a data record from MongoDB, pertaining to the ObjectId specifed
+        """Retrieve a data record from MongoDB,
+        pertaining to the ObjectId specifed
 
         Args:
-            document_id (ObjectId, required): data record to retrieve from mongo, located in the collection specified when calling :func:`__init__`
-        
+            document_id (ObjectId, required): data record to retrieve
+                from mongo, located in the collection specified when
+                calling :func:`__init__`
 
         Raises:
-            Exception: Raised when MongoDB document is not found. Shows query performed that failed
+            Exception: Raised when MongoDB document is not found.
+                Shows query performed that failed
 
         Returns:
-            str: binary string depicting data sequence stored in MongoDB Document
+            str: binary string depicting data sequence
+            stored in MongoDB Document
         """
         query_dict = {'user_id': self._mongo_dataset_details['user_id'],
                       'dataset_id': self._mongo_dataset_details['dataset_id'],
                       '_id': document_id}
-        
-        record = self.mongo_db[self._data_files_collection_name].find_one(query_dict)
+
+        record = self.mongo_db[self._data_files_collection_name].find_one(
+            query_dict)
         if record is None:
-            raise Exception(f'DataRecord {str(document_id)} not found using {query_dict=}')
+            raise Exception(
+                f'DataRecord {str(document_id)} not found using {query_dict=}')
 
         return record['file']
 
     def convertBinaryStringtoSequence(self, record):
         """Convert Binary string of multiple GDFs (delimited by newline) into a sequence of JSON objects
 
         Args:
@@ -304,179 +415,264 @@
         """
         try:
             lines = io.StringIO(record.decode('utf-8'))
             sequence = (tuple([json.loads(line.strip()) for line in lines]))
             return sequence
         except Exception as e:
             print(f'failed to retrieve record as StringIO: {e}')
-        
+
     def getSequence(self, record):
-        """Wrapper function to retrieve a record from MongoDB and convert it into a sequence
+        """Wrapper function to retrieve a record from MongoDB
+        and convert it into a sequence
 
         Args:
-            record (ObjectId): The MongoDB ObjectId of the data record to retrieve
+            record (ObjectId): The MongoDB ObjectId of the data
+                record to retrieve
 
         Returns:
             list: GDF sequence retrieved from MongoDB
         """
-        return self.convertBinaryStringtoSequence(self.retrieveDataRecord(record))
-    
-    def setIterMode(self, mode:str):
+        sequence = self.convertBinaryStringtoSequence(
+            self.retrieveDataRecord(record))
+        for gdf in sequence:
+            validate_data(gdf)
+        return sequence
+
+    def setIterMode(self, mode: str) -> None:
         """Set mode to be used for iterating across dataset
 
         Args:
-            mode (str): set to "training" or "testing" depending on what set of sequences is to be iterated across
+            mode (str): set to "training" or "testing" depending
+                on what set of sequences is to be iterated across
 
         Raises:
-            Exception: When no data is in train_sequences or test_sequences, and :func:`prep` should be called first
+            Exception: When no data is in train_sequences or
+                test_sequences, and :func:`prep` should be called first
             Exception: When invalid mode specified in mode argument
         """
         if len(self.train_sequences) == 0 and len(self.test_sequences) == 0:
-            raise Exception('no data in train_sequences or test_sequences, use prep first')
-            
+            raise Exception('no data in train_sequences or test_sequences, \
+                            use prep first')
+
         if mode == 'training':
-            
+
             self.__curr = 0
             self.__term = len(self.train_sequences)
-            
+
         elif mode == 'testing':
             self.__curr = 0
             self.__term = len(self.test_sequences)
         else:
-            raise Exception('setIterMode only supports "training" and "testing"')
-        
+            raise Exception('setIterMode only supports "training" \
+                            and "testing"')
+
         self._iter_mode = mode
         return
-    
+
     def __iter__(self):
         return self
 
     def __next__(self):
         """Iterate across range, calling :func:`retrieveDataRecord` for each item
-        """        
+        """
         if self.__curr >= self.__term:
             self.__curr = 0
             raise StopIteration()
-            
-        
+
         if self._iter_mode == 'training':
-            (cur, self.__curr) = (self.train_sequences[self.__curr], self.__curr + 1)
-        
+            (cur, self.__curr) = (
+                self.train_sequences[self.__curr], self.__curr + 1)
+
         elif self._iter_mode == 'testing':
-            (cur, self.__curr) = (self.test_sequences[self.__curr], self.__curr + 1)
-        
-        else: 
-            raise Exception('invalid iter mode: {self._iter_mode}, set using setIterMode(mode)')
+            (cur, self.__curr) = (
+                self.test_sequences[self.__curr], self.__curr + 1)
+
+        else:
+            raise Exception('invalid iter mode: {self._iter_mode}, \
+                            set using setIterMode(mode)')
 
         return self.retrieveDataRecord(cur)
 
 
 class MongoResults:
-    """Class to handle saving and linking result data inside MongoDB. Provides functions to insert single log record during training/testing,
-    save final result after test completion, and remediation/deletion function for test aborting, database cleanup
+    """Class to handle saving and linking result data inside MongoDB.
+
+    Provides functions to insert single log record during training/testing,
+    save final result after test completion, and remediation/deletion
+    function for test aborting, database cleanup
     """
-    def __init__(self, mongo_db, result_collection_name: str, log_collection_name: str, test_id:str, user_id:str, dataset_id:str, test_configuration:dict=None):
+
+    def __init__(self,
+                 mongo_db,
+                 result_collection_name: str,
+                 log_collection_name: str,
+                 test_id: str,
+                 user_id: str,
+                 dataset_id: str,
+                 test_configuration: dict = None):
         """Initialize MongoResults object
 
         Args:
-            mongo_db (pymongo.MongoClient): Database where the results are to be stored
-            result_collection_name (str): collection name to save final test results
-            log_collection_name (str): collection name to save testing log documents
+            mongo_db (pymongo.MongoClient): Database where the results
+                are to be stored
+            result_collection_name (str): collection name to save final
+                test results
+            log_collection_name (str): collection name to save testing
+                log documents
             test_id (str): unique-id for the test being conducted
             user_id (str): unique-id for the user conducting the test
-            dataset_id (str): unique-id for the dataset being used in the test
-            test_configuration (dict): object showing all of the options used for configuring pvt
+            dataset_id (str): unique-id for the dataset being used
+                in the test
+            test_configuration (dict): object showing all of the options
+                used for configuring pvt
         """
-        
+
+        self.test_id = test_id
+        self.user_id = user_id
+        self.dataset_id = dataset_id
+
         self.mongo_db = mongo_db
         self.result_collection_name = result_collection_name
         self.log_collection_name = log_collection_name
         self.result_collection = mongo_db[result_collection_name]
         self.log_collection = mongo_db[log_collection_name]
         self.test_configuration = test_configuration
         self.result_obj = {'testing_logs': [],
                            'training_logs': [],
                            'test_id': test_id,
                            'user_id': user_id,
                            'dataset_id': dataset_id,
-                           'start_time_utc' : str(datetime.datetime.utcnow()),
+                           'start_time_utc': str(datetime.datetime.utcnow()),
                            'test_configuration': self.test_configuration}
-        
+
     def reset(self):
         """Reset start time and testing/training logs in result_obj
         """
         self.result_obj.update({'testing_logs': [],
                                 'training_logs': [],
-                                'start_time_utc' : str(datetime.datetime.utcnow())})
+                                'start_time_utc': str(datetime.datetime.utcnow())})
         return
-    
-    def addLogRecord(self, type:str, record:dict):
-        """Called during the testing loop to insert a pvt status record into MongoDB
+
+    def addLogRecord(self,
+                     type: str,
+                     record: dict):
+        """Called during the testing loop to insert a pvt status
+        record into MongoDB
 
         Args:
-            type (str): Whether the record should be appended to the training or testing logs
+            type (str): Whether the record should be appended to the
+                training or testing logs
             record (dict): the record to insert
 
         Raises:
             Exception: Thrown if the type provided is not supported
         """
-        
+
         record_id = self.log_collection.insert_one(record).inserted_id
         if type == 'training':
             self.result_obj['training_logs'].append(record_id)
         elif type == 'testing':
             self.result_obj['testing_logs'].append(record_id)
         else:
-            raise Exception(f'Unsupported record type {type} for record {record}')
-        
+            raise Exception(f'Unsupported record type {type} for \
+                record {record}')
+
         return
-    
-    def saveResults(self, final_results:dict):
-        """Save a document in MongoDB, linking the result doc to the logs documents
+
+    def saveResults(self,
+                    final_results: dict):
+        """Save a document in MongoDB, linking the result doc to
+        the logs documents
 
         Args:
-            final_results (dict): Information pertaining to the results of the test, to be stored in the results object for future use
+            final_results (dict): Information pertaining to the
+                results of the test, to be stored in the results
+                object for future use
 
         Returns:
             str: string of the ObjectId saved in MongoDB
-            
-            
+
         Example:
             .. code-block:: python
-            
+
                 uid = mongo_results.saveResults(final_state)
         """
         self.result_obj['end_time_utc'] = str(datetime.datetime.utcnow())
         self.result_obj['final_results'] = final_results
-        print(f'{self.result_obj = }')
-        result_id = self.result_collection.insert_one(self.result_obj).inserted_id
-        print(f'saved test results in {self.result_collection_name} as id: {result_id}')
+        # print(f'{self.result_obj = }')
+        result_id = self.result_collection.insert_one(
+            self.result_obj).inserted_id
+        print(
+            f'saved test results in {self.result_collection_name} as id: {result_id}')
         return str(result_id)
-    
+
     def deleteResults(self):
-        """Function used to remediate database in the event of a failed/aborted test
+        """Function used to remediate database in the event of a
+        failed/aborted test
 
         Returns:
             dict: dict showing the deleted result record, if any
         """
         try:
-            delete_result = self.result_collection.find_one_and_delete({'user_id': self.result_obj['user_id'],
-                                                            'dataset_id': self.result_obj['dataset_id'],
-                                                            'test_id': self.result_obj['test_id'],
-                                                            'start_time_utc': self.result_obj['start_time_utc']
-                                                            }, {'_id': False})
-            # print(f'deleted_count = {delete_result}')
-                # print(f'log_delete_result={log_delete_result}')
-            
+            query_object = {'user_id': self.user_id,
+                            'dataset_id': self.dataset_id,
+                            'test_id': self.test_id
+                            }
+            delete_result = self.result_collection.find_one_and_delete(query_object,
+                                                                       {'_id': False})
+
         except Exception as e:
             print(f'failed to delete results: {e}')
             return None
-        
-        try:
-            for log_id in self.result_obj['training_logs']:
-                log_delete_result = self.log_collection.find_one_and_delete({'_id':log_id},{'_id': False})
-            for log_id in self.result_obj['testing_logs']:
-                log_delete_result = self.log_collection.find_one_and_delete({'_id':log_id},{'_id': False})
-        except Exception as e:
-            print(f'failed to delete log record: {e}')
-            return None
-        return {'status': 'deleted', 'record': delete_result}
+
+        if delete_result is not None:
+            try:
+                self.log_collection.delete_many(
+                    {'_id': {'$in': delete_result['training_logs']}})
+                self.log_collection.delete_many(
+                    {'_id': {'$in': delete_result['testing_logs']}})
+
+            except Exception as e:
+                print(f'failed to delete log record: {e}')
+                return None
+
+        if self.result_obj['testing_logs']:
+            self.log_collection.delete_many(
+                {'_id': {'$in': self.result_obj['testing_logs']}})
+
+        if self.result_obj['training_logs']:
+            self.log_collection.delete_many(
+                {'_id': {'$in': self.result_obj['training_logs']}})
+
+        return {'status': 'deleted', 'record': delete_result}
+
+    def retrieveResults(self):
+        """Retreive test results from MongoDB based on user_id, dataset_id,
+        and test_id
+
+        Raises:
+            Exception: If dataset master record is not found in database
+
+        Returns:
+            dict: Entire test result object
+        """
+        query_object = {'user_id': self.user_id,
+                        'dataset_id': self.dataset_id,
+                        'test_id': self.test_id
+                        }
+        self.result_obj = self.result_collection.find_one(query_object)
+
+        if self.result_obj is None:
+            raise Exception(f'Test not found based on {query_object=}')
+
+        # retrieve successful
+        training_ids = self.result_obj['training_logs']
+        testing_ids = self.result_obj['testing_logs']
+        training_logs = [item for item in self.log_collection.find(
+            {'_id': {'$in': training_ids}})]
+        testing_logs = [item for item in self.log_collection.find(
+            {'_id': {'$in': testing_ids}})]
+
+        self.result_obj['training_logs'] = training_logs
+        self.result_obj['testing_logs'] = testing_logs
+
+        return self.result_obj
```

### Comparing `ia-sdk-0.3.9/ia/gaius/genome_info.py` & `ia-sdk-0.4.0/ia/gaius/genome_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,56 @@
-try:
-    from cyjupyter import Cytoscape
-except:
-    class Cytoscape:
-        def __init__(*args, **kwargs):
-            pass
-
-
 class Genome:
+    """Wrapper class for a Genome topology, loaded from a dict
+
+    :ivar topology: the data representing a Genome
+    :ivar agent: agent data parsed from topology
+    :ivar description: Genome description field
+    :ivar primitive_map: dict of "node name" to "node id" pairings
+    """
     def __init__(self, topology: dict):
         """Initialize a genome from a GAIuS agent topology (dict)
 
         Args:
             topology (dict, required): GAIuS agent topology
         """
         self.topology = topology
         self.agent = self.topology['agent']
         self.description = self.topology['description']
-        ## Not everyone will have style information, so wrap this:
+        # Not everyone will have style information, so wrap this:
         try:
             self.style_obj = self.topology['style']
             self.style_obj[1]['style']['curve-style'] = 'bezier'
-        except:
+        except Exception:
             pass
-        #        self.agent_genome = self.topology['elements']['nodes']
         self.primitives = {}
         self.manipulatives = {}
         self.action_ids = []
         self.actions_manifests = {}
         for node in self.topology['elements']['nodes']:
             if node['data']['type'] == 'primitive':
                 self.primitives[node['data']['id']] = node['data']
             elif node['data']['type'] == 'manipulative':
                 self.manipulatives[node['data']['id']] = node['data']
-                if node['data']['name'].startswith("ACTION"):
-                    self.action_ids.append(node['data']['id'])
-                    if node['data']['primitive'] in self.actions_manifests:
-                        self.actions_manifests[node['data']['primitive']].append(node['data'])
-                    else:
-                        self.actions_manifests[node['data']['primitive']] = [node['data']]
+
         self.agent_genome = {'primitives': self.primitives, 'manipulatives': self.manipulatives}
         self.primitive_map = {x['name']: _id for _id, x in self.primitives.items()}
         self.manipulative_map = {_id: x['name'] for _id, x in self.manipulatives.items()}
-        # print(" %s total primitives" % (len(self.primitives)))
-        # print(" %s total manipulatives" % (len(self.manipulatives)))
-        # print(" %s total actions" % (len(self.actions_manifests)))
+
         return
 
     def get_nodes(self):
         """Return a tuple of :samp:`primitive node names`, :samp:`manipulative node names` from the topology"""
         return self.agent_genome['primitives'], self.agent_genome['manipulatives']
 
-    def get_actions(self):
-        """Return a list of ACTIONs in the topology
-
-        .. warning::
-            .. deprecated:: 12.0 (Kehl)
-
-                ACTIONs are not actively used in GAIuS topology creation
-        """
-        return self.action_ids
-
     def get_primitive_map(self):
         """Get a map of node names to primitive ids in the GAIuS agent topology
 
         Example:
             .. code-block:: python
-            
+
                 >>> agent = AgentClient(agent_info)
                 >>> agent.connect()
                 >>> agent.genome.get_primitive_map()
                 {'P1': 'p46b6b076c'}
         """
         return self.primitive_map
 
@@ -88,13 +69,15 @@
             p_id (str): primitive id of the node to edit
             gene_data (dict): dictionary of genes to update in the Genome's cache
         """
         for key, value in gene_data.items():
             self.agent_genome['primitives'][p_id][key] = value
         return
 
-    def display(self):
+    def display(self): # pragma: no cover
         """Display the Genome topology in Cytoscape
         """
-        return Cytoscape(data=self.topology, visual_style=self.style_obj, layout={'height': '500px'},
+        from cyjupyter import Cytoscape
+        return Cytoscape(data=self.topology,
+                         visual_style=self.style_obj,
+                         layout={'height': '500px'},
                          background='white')
-
```

### Comparing `ia-sdk-0.3.9/ia/gaius/tests/classification.py` & `ia-sdk-0.4.0/ia/gaius/tests/classification.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ia.gaius.prediction_models import prediction_ensemble_model_classification, hive_model_classification
+from ia.gaius.prediction_models import most_common_ensemble_model_classification, hive_model_classification
 
 
 class Tester:
 
     def __init__(self, **kwargs):
         self.bottle = kwargs['bottle']
         self.learning_strategy = kwargs['learning_strategy']
@@ -34,18 +34,20 @@
 
         record['node_predictions'] = {}
         predicton_error = True  ## TODO: If any of the nodes are right, then don't bother learning if on_error learning strategy is employed.
 
         ensembles = self.bottle.get_predictions()
         for node, ensemble in ensembles.items():
             # Here's where we model
-            predicted_value = prediction_ensemble_model_classification(ensemble)
+            predicted_value = most_common_ensemble_model_classification(ensemble)
             record['node_predictions'][node] = predicted_value
 
         hive_prediction = hive_model_classification(ensembles)
+        if hive_prediction is not None:
+            hive_prediction = hive_prediction.most_common(1)[0][0]
         record['node_predictions']['hive'] = hive_prediction
         if hive_prediction == historical_expecting:
             predicton_error = False
 
         if self.learning_strategy == 'continuous' or (self.learning_strategy == 'on-error' and predicton_error):
             # NOTE!: Now, we're sending the class to the EGRESS nodes for them to learn it, too.
             # Now use the last event.
```

### Comparing `ia-sdk-0.3.9/ia/gaius/tests/utility.py` & `ia-sdk-0.4.0/ia/gaius/tests/utility.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from ia.gaius.data_language import CLEAR_WM, LEARN
-from ia.gaius.prediction_models import make_modeled_emotives, hive_model_emotives
-
-
+# from ia.gaius.pvt.pvt_utils import make_modeled_emotives_
+from ia.gaius.prediction_models import prediction_ensemble_modeled_emotives
 class Tester:
 
     def __init__(self, **kwargs):
         self.bottle = kwargs['bottle']
         self.utype = kwargs['utype']  # either 'value' or 'polarity'
         self.learning_strategy = kwargs['learning_strategy']
 
@@ -28,23 +27,27 @@
         self.bottle.clear_wm()
         for data in sequence:
             self.bottle.observe(data)
 
         record['node_predictions'] = {}
         predicton_error = True  # If any of the nodes are right, then don't bother learning if on_error learning strategy is employed.
         hive_prediction = []
-        answers = self.bottle.get_predictions()
+        answer = self.bottle.get_predictions()
         # HERE IS WHERE WE MODEL OUR PREDICTIONS #######
-        for answer in answers:
-            for node, ensemble in answer.items():
-                predicted_value = make_modeled_emotives(ensemble)
-                hive_prediction.append(predicted_value)  # Add to hive model's list for later
-                record['node_predictions'][node] = predicted_value
+        utility_preds = []
+        for node, ensemble in answer.items():
+            predicted_value = prediction_ensemble_modeled_emotives(ensemble)
+            if isinstance(predicted_value, dict) and len(predicted_value) != 0:
+                predicted_value = sum(list(predicted_value.values()))/ len(predicted_value)
+            else:
+                predicted_value = 0
+            utility_preds.append(predicted_value)
+            record['node_predictions'][node] = predicted_value
 
-        hive_prediction = hive_model_emotives(hive_prediction)
+        hive_prediction = sum(utility_preds)/len(utility_preds)
         record['node_predictions']['hive'] = hive_prediction
         if hive_prediction == historical_expecting:
             predicton_error = False
 
         if self.learning_strategy == 'continuous' or (
                 self.learning_strategy == 'on-error' and predicton_error):
             # NOTE!: Unlike regular symbols for the classification tests, utilities pass through
```

### Comparing `ia-sdk-0.3.9/ia_sdk.egg-info/SOURCES.txt` & `ia-sdk-0.4.0/ia_sdk.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 README.md
 setup.cfg
 setup.py
 ia/__init__.py
 ia/gaius/__init__.py
 ia/gaius/agent_client.py
 ia/gaius/back_testing.py
+ia/gaius/comcom_client.py
 ia/gaius/data_language.py
 ia/gaius/data_ops.py
+ia/gaius/data_structures.py
 ia/gaius/genome_info.py
 ia/gaius/kb_ops.py
+ia/gaius/manager.py
 ia/gaius/prediction_models.py
-ia/gaius/pvt.py
 ia/gaius/utils.py
+ia/gaius/experimental/__init__.py
+ia/gaius/experimental/genome_optimizer.py
+ia/gaius/pvt/__init__.py
+ia/gaius/pvt/mongo_interface.py
+ia/gaius/pvt/offline_sio.py
+ia/gaius/pvt/pvt_utils.py
 ia/gaius/tests/__init__.py
 ia/gaius/tests/classification.py
-ia/gaius/tests/pvt_utils.py
 ia/gaius/tests/utility.py
+ia/scripts/__init__.py
+ia/scripts/spawn_agent.py
+ia/scripts/spawn_general.py
 ia_sdk.egg-info/PKG-INFO
 ia_sdk.egg-info/SOURCES.txt
 ia_sdk.egg-info/dependency_links.txt
 ia_sdk.egg-info/requires.txt
 ia_sdk.egg-info/top_level.txt
```

