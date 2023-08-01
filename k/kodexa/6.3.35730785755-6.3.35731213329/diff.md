# Comparing `tmp/kodexa-6.3.35730785755.tar.gz` & `tmp/kodexa-6.3.35731213329.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-6.3.35730785755.tar", max compression
+gzip compressed data, was "kodexa-6.3.35731213329.tar", max compression
```

## Comparing `kodexa-6.3.35730785755.tar` & `kodexa-6.3.35731213329.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11357 2023-08-01 19:01:48.561076 kodexa-6.3.35730785755/LICENSE
--rw-r--r--   0        0        0     2804 2023-08-01 19:01:48.561076 kodexa-6.3.35730785755/README.md
--rw-r--r--   0        0        0      847 2023-08-01 19:01:48.565076 kodexa-6.3.35730785755/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2023-08-01 19:01:48.565076 kodexa-6.3.35730785755/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    12530 2023-08-01 19:01:48.565076 kodexa-6.3.35730785755/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      297 2023-08-01 19:01:48.565076 kodexa-6.3.35730785755/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0     7722 2023-08-01 19:01:48.565076 kodexa-6.3.35730785755/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      720 2023-08-01 19:01:48.565076 kodexa-6.3.35730785755/kodexa/model/__init__.py
--rw-r--r--   0        0        0      906 2023-08-01 19:01:48.565076 kodexa-6.3.35730785755/kodexa/model/base.py
--rw-r--r--   0        0        0    97073 2023-08-01 19:01:48.565076 kodexa-6.3.35730785755/kodexa/model/model.py
--rw-r--r--   0        0        0   118371 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/model/objects.py
--rw-r--r--   0        0        0    38816 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    19505 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   111730 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/platform/client.py
--rw-r--r--   0        0        0    28342 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13499 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3698 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3735 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     2354 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       60 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7054 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       60 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    21267 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       60 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    18991 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     2738 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    34222 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      160 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/steps/__init__.py
--rw-r--r--   0        0        0     9587 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/steps/common.py
--rw-r--r--   0        0        0      159 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/testing/__init__.py
--rw-r--r--   0        0        0      932 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    13596 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 19:01:48.569076 kodexa-6.3.35730785755/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1279 2023-08-01 19:02:03.041334 kodexa-6.3.35730785755/pyproject.toml
--rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 kodexa-6.3.35730785755/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-01 19:52:07.190440 kodexa-6.3.35731213329/LICENSE
+-rw-r--r--   0        0        0     2804 2023-08-01 19:52:07.190440 kodexa-6.3.35731213329/README.md
+-rw-r--r--   0        0        0      847 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    12530 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      297 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0     7722 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      720 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      906 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/model/base.py
+-rw-r--r--   0        0        0    97073 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/model/model.py
+-rw-r--r--   0        0        0   118834 2023-08-01 19:52:07.194440 kodexa-6.3.35731213329/kodexa/model/objects.py
+-rw-r--r--   0        0        0    38816 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    19505 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   112612 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/platform/client.py
+-rw-r--r--   0        0        0    25644 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13499 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3698 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3735 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     2354 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       60 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7054 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       60 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    21267 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       60 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    18991 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     2738 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    34222 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      160 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0     9587 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/steps/common.py
+-rw-r--r--   0        0        0      159 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0      932 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    13596 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 19:52:07.198440 kodexa-6.3.35731213329/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1279 2023-08-01 19:52:24.174721 kodexa-6.3.35731213329/pyproject.toml
+-rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 kodexa-6.3.35731213329/PKG-INFO
```

### Comparing `kodexa-6.3.35730785755/LICENSE` & `kodexa-6.3.35731213329/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/README.md` & `kodexa-6.3.35731213329/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/__init__.py` & `kodexa-6.3.35731213329/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/assistant/assistant.py` & `kodexa-6.3.35731213329/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/connectors/connectors.py` & `kodexa-6.3.35731213329/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/model/__init__.py` & `kodexa-6.3.35731213329/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/model/base.py` & `kodexa-6.3.35731213329/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/model/model.py` & `kodexa-6.3.35731213329/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/model/objects.py` & `kodexa-6.3.35731213329/kodexa/model/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1912,14 +1912,27 @@
 
     number_of_elements: Optional[int] = Field(None, alias='numberOfElements')
     first: Optional[bool] = None
     last: Optional[bool] = None
     empty: Optional[bool] = None
 
 
+class PageAssistant(KodexaBaseModel):
+    total_pages: Optional[int] = Field(None, alias='totalPages')
+    total_elements: Optional[int] = Field(None, alias='totalElements')
+    size: Optional[int] = None
+    content: Optional[List[Assistant]] = None
+    number: Optional[int] = None
+
+    number_of_elements: Optional[int] = Field(None, alias='numberOfElements')
+    first: Optional[bool] = None
+    last: Optional[bool] = None
+    empty: Optional[bool] = None
+
+
 class PageWorkspace(KodexaBaseModel):
     total_pages: Optional[int] = Field(None, alias='totalPages')
     total_elements: Optional[int] = Field(None, alias='totalElements')
     size: Optional[int] = None
     content: Optional[List[Workspace]] = None
     number: Optional[int] = None
```

### Comparing `kodexa-6.3.35730785755/kodexa/model/persistence.py` & `kodexa-6.3.35731213329/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/pipeline/pipeline.py` & `kodexa-6.3.35731213329/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/platform/client.py` & `kodexa-6.3.35731213329/kodexa/platform/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -560,14 +560,22 @@
     """Represents a page project endpoint"""
 
     def get_type(self) -> Optional[str]:
         """Get the type of the endpoint"""
         return "project"
 
 
+class PageAssistantEndpoint(PageAssistant, PageEndpoint):
+    """Represents a page assistant endpoint"""
+
+    def get_type(self) -> Optional[str]:
+        """Get the type of the endpoint"""
+        return "assistant"
+
+
 class PageWorkspaceEndpoint(PageWorkspace, PageEndpoint):
     """Represents a page workspace endpoints"""
 
     def get_type(self) -> Optional[str]:
         """Get the type of the endpoint"""
         return "workspace"
 
@@ -1082,14 +1090,30 @@
         return WorkspaceEndpoint
 
     def get_page_class(self, object_dict=None):
         """Get the page class of the endpoint"""
         return PageWorkspaceEndpoint
 
 
+class AssistantsEndpoint(EntitiesEndpoint):
+    """Represents a assistants endpoint"""
+
+    def get_type(self) -> str:
+        """Get the type of the endpoint"""
+        return f"assistants"
+
+    def get_instance_class(self, object_dict=None):
+        """Get the instance class of the endpoint"""
+        return AssistantEndpoint
+
+    def get_page_class(self, object_dict=None):
+        """Get the page class of the endpoint"""
+        return PageAssistantEndpoint
+
+
 class ProjectsEndpoint(EntitiesEndpoint):
     """Represents a projects endpoint"""
 
     def get_type(self) -> str:
         """Get the type of the endpoint"""
         return f"projects"
 
@@ -2501,14 +2525,21 @@
         "plural": "pipelines",
         "type": PipelineEndpoint,
         "endpoint": PipelinesEndpoint
     },
     "assistants": {
         "name": "assistant",
         "plural": "assistants",
+        "type": AssistantEndpoint,
+        "endpoint": AssistantsEndpoint,
+        "global": True
+    },
+    "assistantDefinitions": {
+        "name": "assistant",
+        "plural": "assistants",
         "type": AssistantDefinitionEndpoint,
         "endpoint": AssistantDefinitionsEndpoint
     },
     "actions": {
         "name": "action",
         "plural": "actions",
         "type": ActionEndpoint,
```

### Comparing `kodexa-6.3.35730785755/kodexa/platform/kodexa.py` & `kodexa-6.3.35731213329/kodexa/platform/kodexa.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,26 @@
 from __future__ import annotations
 
 import errno
 import io
 import json
 import logging
 import os
-import sys
 import time
 from json import JSONDecodeError
 
 import requests
 from addict import Dict
 from appdirs import AppDirs
 
 from kodexa.connectors import get_source
 from kodexa.connectors.connectors import get_caller_dir, FolderConnector
-from kodexa.model import Document, ExtensionPack
-from kodexa.model.objects import AssistantDefinition, Action, Taxonomy, ModelRuntime, CredentialDefinition, \
-    ExecutionEvent, \
-    ContentObject, AssistantEvent, ContentEvent, ScheduledEvent, Project, Execution, ProjectTemplate, Membership, \
-    DataForm, DocumentFamilyEvent, ChannelEvent, DataObjectEvent
+from kodexa.model import Document
+from kodexa.model.objects import ExecutionEvent, \
+    ContentObject, AssistantEvent, ContentEvent, ScheduledEvent, DocumentFamilyEvent, ChannelEvent, DataObjectEvent
 from kodexa.pipeline import PipelineContext, Pipeline, PipelineStatistics
 from kodexa.platform.client import DocumentStoreEndpoint, KodexaClient
 
 logger = logging.getLogger()
 
 dirs = AppDirs("Kodexa", "Kodexa")
 
@@ -77,120 +74,14 @@
         except OSError as exc:  # Guard against race condition
             if exc.errno != errno.EEXIST:
                 raise
     with open(path, 'w') as outfile:
         json.dump(config_obj, outfile)
 
 
-OBJECT_TYPES = {
-    "extensionPacks": {
-        "name": "extension pack",
-        "plural": "extension packs",
-        "type": ExtensionPack
-    },
-    "pipelines": {
-        "name": "pipeline",
-        "plural": "pipelines",
-        "type": Pipeline
-    },
-    "assistants": {
-        "name": "assistant",
-        "plural": "assistants",
-        "type": AssistantDefinition
-    },
-    "actions": {
-        "name": "action",
-        "plural": "actions",
-        "type": Action
-    },
-    "modelRuntimes": {
-        "name": "modelRuntime",
-        "plural": "modelRuntimes",
-        "type": ModelRuntime
-    },
-    "credentialDefinitions": {
-        "name": "credential definition",
-        "plural": "credential definitions",
-        "type": CredentialDefinition
-    },
-    "dataForms": {
-        "name": "dataForm",
-        "plural": "dataForms",
-        "type": DataForm
-    },
-    "taxonomies": {
-        "name": "taxonomy",
-        "plural": "taxonomies",
-        "type": Taxonomy
-    },
-    "stores": {
-        "name": "store",
-        "plural": "stores"
-    },
-    "projects": {
-        "name": "project",
-        "plural": "projects",
-        "type": Project,
-        "global": True
-    },
-    "projectTemplates": {
-        "name": "project template",
-        "plural": "project templates",
-        "type": ProjectTemplate
-    },
-    "executions": {
-        "name": "execution",
-        "plural": "executions",
-        "type": Execution,
-        "global": True,
-        "sort": "startDate:desc"
-    },
-    "memberships": {
-        "name": "membership",
-        "plural": "memberships",
-        "type": Membership,
-        "global": True
-    }
-}
-
-
-def resolve_object_type(obj_type):
-    """Takes part of an object type (ie. pipeline) and then resolves the object type (pipelines)
-
-    Args:
-      obj_type: part of the object type
-
-    Returns:
-      The object type dict (if found)
-
-    """
-    hits = []
-    keys = []
-
-    if not isinstance(obj_type, str):
-        obj_type = str(obj_type).lower()
-    else:
-        obj_type = obj_type.lower()
-
-    for target_type in OBJECT_TYPES.keys():
-        if obj_type in target_type.lower():
-            hits.append(OBJECT_TYPES[target_type])
-            keys.append(target_type)
-
-    if len(hits) == 1:
-        return keys[0], hits[0]
-
-    if len(hits) == 0:
-        print(f":exclaimation: Unable to find object type {obj_type}")
-        sys.exit(1)
-    else:
-        print(f":exclaimation: To many potential matches for object type ({','.join(keys)}")
-        sys.exit(1)
-
-
 class KodexaPlatform:
     """
     The KodexaPlatform object allows you to work with an instance of the Kodexa platform, allow you to list, view and deploy
     components
 
     Note it also can be used to get your access token and Kodexa platform URL using:
```

### Comparing `kodexa-6.3.35730785755/kodexa/selectors/ast.py` & `kodexa-6.3.35731213329/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/selectors/core.py` & `kodexa-6.3.35731213329/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/selectors/lexrules.py` & `kodexa-6.3.35731213329/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/selectors/lextab.py` & `kodexa-6.3.35731213329/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/selectors/parserules.py` & `kodexa-6.3.35731213329/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/selectors/parsetab.py` & `kodexa-6.3.35731213329/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/spatial/azure_models.py` & `kodexa-6.3.35731213329/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/spatial/bbox_common.py` & `kodexa-6.3.35731213329/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/spatial/table_form_common.py` & `kodexa-6.3.35731213329/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/steps/common.py` & `kodexa-6.3.35731213329/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/testing/test_components.py` & `kodexa-6.3.35731213329/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/kodexa/testing/test_utils.py` & `kodexa-6.3.35731213329/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.3.35730785755/pyproject.toml` & `kodexa-6.3.35731213329/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "6.3.35730785755"
+version = "6.3.35731213329"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-6.3.35730785755/PKG-INFO` & `kodexa-6.3.35731213329/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 6.3.35730785755
+Version: 6.3.35731213329
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

