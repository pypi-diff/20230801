# Comparing `tmp/noteable_origami-1.0.0a2.tar.gz` & `tmp/noteable_origami-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noteable_origami-1.0.0a2.tar", max compression
+gzip compressed data, was "noteable_origami-1.0.0a3.tar", max compression
```

## Comparing `noteable_origami-1.0.0a2.tar` & `noteable_origami-1.0.0a3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1516 2023-07-26 14:03:04.509735 noteable_origami-1.0.0a2/LICENSE
--rw-r--r--   0        0        0     4615 2023-07-26 14:03:04.509735 noteable_origami-1.0.0a2/README.md
--rw-r--r--   0        0        0       82 2023-07-26 14:03:04.509735 noteable_origami-1.0.0a2/origami/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 14:03:04.509735 noteable_origami-1.0.0a2/origami/clients/__init__.py
--rw-r--r--   0        0        0    14644 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/clients/api.py
--rw-r--r--   0        0        0        0 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/clients/cache.py
--rw-r--r--   0        0        0    39670 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/clients/rtu.py
--rw-r--r--   0        0        0        0 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/__init__.py
--rw-r--r--   0        0        0      238 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/base.py
--rw-r--r--   0        0        0      649 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/datasources.py
--rw-r--r--   0        0        0      924 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/files.py
--rw-r--r--   0        0        0      659 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/outputs.py
--rw-r--r--   0        0        0      475 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/projects.py
--rw-r--r--   0        0        0      437 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/spaces.py
--rw-r--r--   0        0        0      681 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/users.py
--rw-r--r--   0        0        0        0 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/__init__.py
--rw-r--r--   0        0        0      803 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/base.py
--rw-r--r--   0        0        0      953 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_contents.py
--rw-r--r--   0        0        0     1120 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_execute.py
--rw-r--r--   0        0        0     1222 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_metadata.py
--rw-r--r--   0        0        0      703 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_output_collection.py
--rw-r--r--   0        0        0     1115 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/delta_types/nb_cells.py
--rw-r--r--   0        0        0      588 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/delta_types/nb_metadata.py
--rw-r--r--   0        0        0      850 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/discriminators.py
--rw-r--r--   0        0        0      451 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/kernels.py
--rw-r--r--   0        0        0     4010 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/notebook.py
--rw-r--r--   0        0        0        0 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/base.py
--rw-r--r--   0        0        0        0 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/channels/__init__.py
--rw-r--r--   0        0        0     7730 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/channels/files.py
--rw-r--r--   0        0        0     2508 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/channels/kernels.py
--rw-r--r--   0        0        0     2640 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/channels/system.py
--rw-r--r--   0        0        0     1210 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/discriminators.py
--rw-r--r--   0        0        0     1073 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/errors.py
--rw-r--r--   0        0        0        0 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/notebook/__init__.py
--rw-r--r--   0        0        0    11988 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/notebook/builder.py
--rw-r--r--   0        0        0     2715 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     5924 1970-01-01 00:00:00.000000 noteable_origami-1.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1516 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/LICENSE
+-rw-r--r--   0        0        0     4615 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/README.md
+-rw-r--r--   0        0        0       82 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/clients/__init__.py
+-rw-r--r--   0        0        0    14644 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/clients/api.py
+-rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/clients/cache.py
+-rw-r--r--   0        0        0    42382 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/clients/rtu.py
+-rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/__init__.py
+-rw-r--r--   0        0        0      238 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/base.py
+-rw-r--r--   0        0        0      649 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/datasources.py
+-rw-r--r--   0        0        0      924 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/files.py
+-rw-r--r--   0        0        0      659 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/outputs.py
+-rw-r--r--   0        0        0      475 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/projects.py
+-rw-r--r--   0        0        0      437 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/spaces.py
+-rw-r--r--   0        0        0      681 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/api/users.py
+-rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/__init__.py
+-rw-r--r--   0        0        0      803 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/base.py
+-rw-r--r--   0        0        0      953 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_contents.py
+-rw-r--r--   0        0        0     1120 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_execute.py
+-rw-r--r--   0        0        0     1222 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_metadata.py
+-rw-r--r--   0        0        0      703 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_output_collection.py
+-rw-r--r--   0        0        0     1115 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/delta_types/nb_cells.py
+-rw-r--r--   0        0        0      588 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/delta_types/nb_metadata.py
+-rw-r--r--   0        0        0      850 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/deltas/discriminators.py
+-rw-r--r--   0        0        0      451 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/kernels.py
+-rw-r--r--   0        0        0     5018 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/notebook.py
+-rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/__init__.py
+-rw-r--r--   0        0        0     1520 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/base.py
+-rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/channels/__init__.py
+-rw-r--r--   0        0        0     7730 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/channels/files.py
+-rw-r--r--   0        0        0     2508 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/channels/kernels.py
+-rw-r--r--   0        0        0     2640 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/channels/system.py
+-rw-r--r--   0        0        0     1210 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/discriminators.py
+-rw-r--r--   0        0        0     1073 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/models/rtu/errors.py
+-rw-r--r--   0        0        0        0 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/notebook/__init__.py
+-rw-r--r--   0        0        0    11988 2023-08-01 21:50:00.595425 noteable_origami-1.0.0a3/origami/notebook/builder.py
+-rw-r--r--   0        0        0     2715 2023-08-01 21:50:00.599425 noteable_origami-1.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     5924 1970-01-01 00:00:00.000000 noteable_origami-1.0.0a3/PKG-INFO
```

### Comparing `noteable_origami-1.0.0a2/LICENSE` & `noteable_origami-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/README.md` & `noteable_origami-1.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/clients/api.py` & `noteable_origami-1.0.0a3/origami/clients/api.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/clients/rtu.py` & `noteable_origami-1.0.0a3/origami/clients/rtu.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 RTUClient is a high-level client for establishing a websocket connection, authenticating with a jwt,
 subscribing to a file by version or last delta id, "squashing" Deltas into an in-memory Notebook
 model, and registering callbacks for incoming RTU events by event_name and channel or incoming
 Deltas by delta type and delta action.
 """
 import asyncio
 import logging
+import random
+import string
 import traceback
 import uuid
-from typing import Awaitable, Callable, Dict, List, Literal, Optional, Type, Union
+from typing import Awaitable, Callable, Dict, List, Literal, Optional, Type
 
 import orjson
 from pydantic import BaseModel, parse_obj_as
 from sending.backends.websocket import WebsocketManager
 from websockets.client import WebSocketClientProtocol
 
 from origami.models.deltas.delta_types.cell_execute import (
     CellExecute,
     CellExecuteAfter,
     CellExecuteAll,
     CellExecuteBefore,
 )
+from origami.models.deltas.delta_types.cell_metadata import CellMetadataReplace, CellMetadataUpdate
 from origami.models.deltas.delta_types.nb_cells import (
     NBCellsAdd,
     NBCellsAddProperties,
     NBCellsDelete,
 )
 from origami.models.deltas.discriminators import FileDelta
 from origami.models.notebook import CodeCell, NotebookCell
@@ -730,79 +733,142 @@
         Raises errors if the Delta was rejected for any reason.
         """
         req = DeltaRequestCallbackManager(client=self, delta=delta)
         return await req.result
 
     async def add_cell(
         self,
+        source: str = '',
         cell: Optional[NotebookCell] = None,
         before_id: Optional[str] = None,
         after_id: Optional[str] = None,
     ) -> NotebookCell:
         """
-        Adds a Cell to the Notebook. If before_id and after_id are unspecified, then it will add
-        the new cell at the bottom of the notebook.
+        Adds a Cell to the Notebook.
+         - if a cell is passed in, will use that or otherwise make a CodeCell from source value
+         - If before_id and after_id are unspecified, then it will add the new cell at the bottom of
+            the notebook.
         """
         if not cell:
-            cell = CodeCell()
+            cell = CodeCell(source=source)
         # Default behavior: add cell to end of Notebook. Guard against a Notebook with no cells
         if not before_id and not after_id and self.cell_ids:
             after_id = self.cell_ids[-1]
         props = NBCellsAddProperties(cell=cell, before_id=before_id, after_id=after_id, id=cell.id)
         delta = NBCellsAdd(file_id=self.file_id, properties=props)
         await self.new_delta_request(delta)
+        # grab newly-squashed cell
+        _, cell = self.builder.get_cell(cell.id)
         return cell
 
-    async def delete_cell(self, cell_id: str) -> None:
+    async def delete_cell(self, cell_id: str) -> NBCellsDelete:
         delta = NBCellsDelete(file_id=self.file_id, properties={'id': cell_id})
-        await self.new_delta_request(delta)
+        return await self.new_delta_request(delta)
+
+    async def change_cell_type(
+        self,
+        cell_id: str,
+        cell_type: Literal['code', 'markdown', 'sql'],
+        code_language: str = 'python',
+        db_connection: str = '@noteable',
+        assign_results_to: Optional[str] = None,
+    ) -> NotebookCell:
+        """
+        Switch a cell between code, markdown, or SQL cell.
+         - code_language only relevant when switching to code cell
+         - db_connection and assign_results_to only relevant when switching to SQL cell
+        """
+        self.builder.get_cell(cell_id)  # Raise CellNotFound if it doesn't exist
+        if cell_type == 'code':
+            delta = CellMetadataReplace(
+                file_id=self.file_id,
+                resource_id=cell_id,
+                properties={'language': code_language, 'type': 'code'},
+            )
+            await self.new_delta_request(delta)
+        elif cell_type == 'markdown':
+            delta = CellMetadataReplace(
+                file_id=self.file_id,
+                resource_id=cell_id,
+                properties={'language': 'markdown', 'type': 'markdown'},
+            )
+            await self.new_delta_request(delta)
+        elif cell_type == 'sql':
+            delta = CellMetadataReplace(
+                file_id=self.file_id,
+                resource_id=cell_id,
+                properties={'language': 'sql', 'type': 'code'},
+            )
+            await self.new_delta_request(delta)
+
+            if not assign_results_to:
+                name_suffix = "".join(random.choices(string.ascii_lowercase, k=4))
+                assign_results_to = 'df_' + name_suffix
+            delta = CellMetadataUpdate(
+                file_id=self.file_id,
+                resource_id=cell_id,
+                properties={
+                    'path': ['metadata', 'noteable'],
+                    'value': {
+                        'cell_type': 'sql',
+                        'db_connection': db_connection,
+                        'assign_results_to': assign_results_to,
+                    },
+                },
+            )
+            await self.new_delta_request(delta)
+        else:
+            raise ValueError(f"Unknown cell type {cell_type}")
+        # Grab updated cell post-squashing
+        _, cell = self.builder.get_cell(cell_id)
+        return cell
 
     async def queue_execution(
         self,
         cell_id: Optional[str] = None,
         before_id: Optional[str] = None,
         after_id: Optional[str] = None,
         run_all: bool = False,
-    ) -> Union[asyncio.Future[CodeCell], List[asyncio.Future[CodeCell]]]:
+    ) -> Dict[asyncio.Future[CodeCell], str]:
         """
-        Execute an individual cell or multiple cells in the Notebook. The return value is a single
-        Future or list of Futures that will resolve to the CodeCell executed when the cell has
-        finished running.
+        Execute an individual cell or multiple cells in the Notebook. The return value is a dict of
+        {future: cell_id}, even in the case of executing a single cell.
+
          - Only code Cells can be executed. When running multiple cells with before / after / all
            non-code cells will be excluded automatically
-         - Outputs should be available from the cell.output_collection_id property.
+         - Code cells with no source are not executed on Noteable backend, so they'll be skipped
+         - Outputs should be available from the cell.output_collection_id property
+
+        Use:
+        queued_execute = await rtu_client.queue_execution(run_all=True)
+        done, pending = await asyncio.wait(*queued_execute, timeout=5)
+
+        still_running_cell_ids = [queued_execute[f] for f in pending]
         """
-        # Single cell flow, return a single Future
+        if not cell_id and not before_id and not after_id and not run_all:
+            raise ValueError("One of cell_id, before_id, after_id, or run_all must be set.")
+
         if cell_id:
-            idx, cell = self.builder.get_cell(cell_id)  # can raise CellNotFound
-            if cell.cell_type != 'code':
-                raise ValueError("Can only queue execute on code cells")
-            future = asyncio.Future()
-            self._execute_cell_events[cell_id] = future
+            cell_ids = [cell_id]
             delta = CellExecute(file_id=self.file_id, resource_id=cell_id)
-            await self.new_delta_request(delta)
-            return future
-
-        # Multiple cell flow
-        if not before_id and not after_id and not run_all:
-            raise ValueError("One of cell_id, before_id, after_id, or run_all must be set.")
-        if before_id:
+        elif before_id:
             idx, cell = self.builder.get_cell(before_id)  # can raise CellNotFound
             cell_ids = self.cell_ids[: idx + 1]  # inclusive of the "before_id" cell
             delta = CellExecuteBefore(file_id=self.file_id, resource_id=before_id)
         elif after_id:
             idx, cell = self.builder.get_cell(after_id)  # can raise CellNotFound
             cell_ids = self.cell_ids[idx:]  # inclusive of the "after_id" cell
             delta = CellExecuteAfter(file_id=self.file_id, resource_id=after_id)
         else:
             cell_ids = self.cell_ids[:]
             delta = CellExecuteAll(file_id=self.file_id)
-        futures = []
+        futures = {}
         for cell_id in cell_ids:
-            # Only create futures for Code cells
+            # Only create futures for Code cells that have something in source. Otherwise the cell
+            # will never get executed by PA/Kernel, so we'd never see cell status and resolve future
             future = asyncio.Future()
             idx, cell = self.builder.get_cell(cell_id)
-            if cell.cell_type == 'code':
+            if cell.cell_type == 'code' and cell.source.strip():
                 self._execute_cell_events[cell_id] = future
-                futures.append(future)
+                futures[future] = cell_id
         await self.new_delta_request(delta)
         return futures
```

### Comparing `noteable_origami-1.0.0a2/origami/models/api/datasources.py` & `noteable_origami-1.0.0a3/origami/models/api/datasources.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/api/files.py` & `noteable_origami-1.0.0a3/origami/models/api/files.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/api/outputs.py` & `noteable_origami-1.0.0a3/origami/models/api/outputs.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/api/users.py` & `noteable_origami-1.0.0a3/origami/models/api/users.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/deltas/base.py` & `noteable_origami-1.0.0a3/origami/models/deltas/base.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_contents.py` & `noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_contents.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_execute.py` & `noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_execute.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_metadata.py` & `noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_metadata.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_output_collection.py` & `noteable_origami-1.0.0a3/origami/models/deltas/delta_types/cell_output_collection.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/deltas/delta_types/nb_cells.py` & `noteable_origami-1.0.0a3/origami/models/deltas/delta_types/nb_cells.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/deltas/delta_types/nb_metadata.py` & `noteable_origami-1.0.0a3/origami/models/deltas/delta_types/nb_metadata.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/deltas/discriminators.py` & `noteable_origami-1.0.0a3/origami/models/deltas/discriminators.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/notebook.py` & `noteable_origami-1.0.0a3/origami/models/notebook.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 collection id, which is a Noteable-specific cell output context.
 
 See https://nbformat.readthedocs.io/en/latest/format_description.html# for Notebook model spec.
 
 Devs: as usual with Pydantic modeling, the top-level model (Notebook) is at the bottom of this file,
 read from bottom up for most clarity.
 """
+import random
+import string
 import uuid
 from typing import Any, Dict, List, Literal, Optional, Union
 
 from pydantic import BaseModel, Field, validator
 from typing_extensions import Annotated  # for 3.8 compatibility
 
 
@@ -93,14 +95,42 @@
         return self.metadata.get("noteable", {}).get("cell_type") == "sql"
 
     @property
     def output_collection_id(self) -> Optional[Union[str, uuid.UUID]]:
         return self.metadata.get("noteable", {}).get("output_collection_id")
 
 
+def make_sql_cell(
+    cell_id: Optional[str] = None,
+    source: str = '',
+    db_connection: str = '@noteable',
+    assign_results_to: Optional[str] = None,
+) -> CodeCell:
+    cell_id = cell_id or str(uuid.uuid4())
+    # Remove first line of source if it starts with %%sql. That is the right syntax for regular
+    # code cells with sql magic support, but Noteable SQL cells should have just the sql source
+    if source.startswith('%%sql'):
+        lines = source.splitlines()
+        source = '\n'.join(lines[1:])
+
+    if not assign_results_to:
+        name_suffix = "".join(random.choices(string.ascii_lowercase, k=4))
+        assign_results_to = 'df_' + name_suffix
+    metadata = {
+        'language': 'sql',
+        'type': 'code',
+        'noteable': {
+            'cell_type': 'sql',
+            'db_connection': db_connection,
+            'assign_results_to': assign_results_to,
+        },
+    }
+    return CodeCell(cell_id=cell_id, source=source, metadata=metadata)
+
+
 class MarkdownCell(CellBase):
     cell_type: Literal["markdown"] = "markdown"
 
 
 class RawCell(CellBase):
     cell_type: Literal["raw"] = "raw"
```

### Comparing `noteable_origami-1.0.0a2/origami/models/rtu/base.py` & `noteable_origami-1.0.0a3/origami/models/rtu/base.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/rtu/channels/files.py` & `noteable_origami-1.0.0a3/origami/models/rtu/channels/files.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/rtu/channels/kernels.py` & `noteable_origami-1.0.0a3/origami/models/rtu/channels/kernels.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/rtu/channels/system.py` & `noteable_origami-1.0.0a3/origami/models/rtu/channels/system.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/rtu/discriminators.py` & `noteable_origami-1.0.0a3/origami/models/rtu/discriminators.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/models/rtu/errors.py` & `noteable_origami-1.0.0a3/origami/models/rtu/errors.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/origami/notebook/builder.py` & `noteable_origami-1.0.0a3/origami/notebook/builder.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a2/pyproject.toml` & `noteable_origami-1.0.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.poetry]
 name = "noteable-origami"
-version = "1.0.0-alpha.2"
+version = "1.0.0-alpha.3"
 description = "The Noteable API interface"
 authors = ["Matt Seal <matt@noteable.io>"]
 maintainers = ["Matt Seal <matt@noteable.io>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/noteable-io/origami"
 # old setup.cfg had a bdist_wheel option.
```

### Comparing `noteable_origami-1.0.0a2/PKG-INFO` & `noteable_origami-1.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noteable-origami
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: The Noteable API interface
 Home-page: https://github.com/noteable-io/origami
 License: BSD-3-Clause
 Keywords: notebook,api,noteable
 Author: Matt Seal
 Author-email: matt@noteable.io
 Maintainer: Matt Seal
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: noteable-origami Version: 1.0.0a2 Summary: The
+Metadata-Version: 2.1 Name: noteable-origami Version: 1.0.0a3 Summary: The
 Noteable API interface Home-page: https://github.com/noteable-io/origami
 License: BSD-3-Clause Keywords: notebook,api,noteable Author: Matt Seal Author-
 email: matt@noteable.io Maintainer: Matt Seal Maintainer-email:
 matt@noteable.io Requires-Python: >=3.8,<4.0 Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

