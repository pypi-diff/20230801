# Comparing `tmp/orbax_checkpoint-0.3.1.tar.gz` & `tmp/orbax_checkpoint-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbax_checkpoint-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orbax_checkpoint-0.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orbax_checkpoint-0.3.1.tar` & `orbax_checkpoint-0.3.2.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0    11357 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/LICENSE
--rw-r--r--   0        0        0      834 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/README.md
--rw-r--r--   0        0        0     2920 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/__init__.py
--rw-r--r--   0        0        0     2663 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/abstract_checkpointer.py
--rw-r--r--   0        0        0     2832 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/aggregate_handlers.py
--rw-r--r--   0        0        0     5803 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/array_checkpoint_handler.py
--rw-r--r--   0        0        0     1440 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/async_checkpoint_handler.py
--rw-r--r--   0        0        0     5692 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/async_checkpointer.py
--rw-r--r--   0        0        0     2188 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_handler.py
--rw-r--r--   0        0        0    37385 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_manager.py
--rw-r--r--   0        0        0    15252 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_utils.py
--rw-r--r--   0        0        0    11915 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_utils_test.py
--rw-r--r--   0        0        0     4839 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/checkpointer.py
--rw-r--r--   0        0        0      740 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/conftest.py
--rw-r--r--   0        0        0     1576 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/future.py
--rw-r--r--   0        0        0     2103 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/json_checkpoint_handler.py
--rw-r--r--   0        0        0     1821 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/json_checkpoint_handler_test.py
--rw-r--r--   0        0        0     7672 2023-07-27 17:40:45.285375 orbax_checkpoint-0.3.1/orbax/checkpoint/msgpack_utils.py
--rw-r--r--   0        0        0     1129 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/msgpack_utils_test.py
--rw-r--r--   0        0        0    45194 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/orbax_checkpoint.ipynb
--rw-r--r--   0        0        0      757 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/proto/__init__.py
--rw-r--r--   0        0        0      757 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/proto/testing/__init__.py
--rw-r--r--   0        0        0      136 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/proto/testing/foo.proto
--rw-r--r--   0        0        0     1549 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/proto/testing/foo_pb2.py
--rw-r--r--   0        0        0     3055 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/proto_checkpoint_handler.py
--rw-r--r--   0        0        0     2108 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/proto_checkpoint_handler_test.py
--rw-r--r--   0        0        0    30479 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/pytree_checkpoint_handler.py
--rw-r--r--   0        0        0     5109 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/test_utils.py
--rw-r--r--   0        0        0    11807 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/transform_utils.py
--rw-r--r--   0        0        0    15155 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/transform_utils_test.py
--rw-r--r--   0        0        0    25970 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/type_handlers.py
--rw-r--r--   0        0        0    24135 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/utils.py
--rw-r--r--   0        0        0     8158 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/orbax/checkpoint/utils_test.py
--rw-r--r--   0        0        0     1153 2023-07-27 17:40:45.289375 orbax_checkpoint-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 orbax_checkpoint-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/LICENSE
+-rw-r--r--   0        0        0      834 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/README.md
+-rw-r--r--   0        0        0     2964 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/__init__.py
+-rw-r--r--   0        0        0     3017 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/abstract_checkpointer.py
+-rw-r--r--   0        0        0     2832 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/aggregate_handlers.py
+-rw-r--r--   0        0        0     5940 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/array_checkpoint_handler.py
+-rw-r--r--   0        0        0     1440 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/async_checkpoint_handler.py
+-rw-r--r--   0        0        0     5692 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/async_checkpointer.py
+-rw-r--r--   0        0        0     2169 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/checkpoint_handler.py
+-rw-r--r--   0        0        0    36798 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/checkpoint_manager.py
+-rw-r--r--   0        0        0    13010 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/checkpoint_utils.py
+-rw-r--r--   0        0        0     9758 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/checkpoint_utils_test.py
+-rw-r--r--   0        0        0     4781 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/checkpointer.py
+-rw-r--r--   0        0        0      740 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/conftest.py
+-rw-r--r--   0        0        0     1576 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/future.py
+-rw-r--r--   0        0        0     2103 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/json_checkpoint_handler.py
+-rw-r--r--   0        0        0     1821 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/json_checkpoint_handler_test.py
+-rw-r--r--   0        0        0     7672 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/msgpack_utils.py
+-rw-r--r--   0        0        0     1129 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/msgpack_utils_test.py
+-rw-r--r--   0        0        0    45718 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/orbax_checkpoint.ipynb
+-rw-r--r--   0        0        0      757 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/proto/__init__.py
+-rw-r--r--   0        0        0      757 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/proto/testing/__init__.py
+-rw-r--r--   0        0        0      136 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/proto/testing/foo.proto
+-rw-r--r--   0        0        0     3055 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/proto_checkpoint_handler.py
+-rw-r--r--   0        0        0    41333 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/pytree_checkpoint_handler.py
+-rw-r--r--   0        0        0     5109 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/test_utils.py
+-rw-r--r--   0        0        0    11807 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/transform_utils.py
+-rw-r--r--   0        0        0    15155 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/transform_utils_test.py
+-rw-r--r--   0        0        0    31759 2023-08-01 19:07:05.566309 orbax_checkpoint-0.3.2/orbax/checkpoint/type_handlers.py
+-rw-r--r--   0        0        0    24312 2023-08-01 19:07:05.570309 orbax_checkpoint-0.3.2/orbax/checkpoint/utils.py
+-rw-r--r--   0        0        0     8158 2023-08-01 19:07:05.570309 orbax_checkpoint-0.3.2/orbax/checkpoint/utils_test.py
+-rw-r--r--   0        0        0     1981 2023-08-01 19:07:05.570309 orbax_checkpoint-0.3.2/orbax/checkpoint/value_metadata.py
+-rw-r--r--   0        0        0     1153 2023-08-01 19:07:05.570309 orbax_checkpoint-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 orbax_checkpoint-0.3.2/PKG-INFO
```

### Comparing `orbax_checkpoint-0.3.1/LICENSE` & `orbax_checkpoint-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/README.md` & `orbax_checkpoint-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/__init__.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from orbax.checkpoint import aggregate_handlers
 from orbax.checkpoint import checkpoint_utils
 from orbax.checkpoint import msgpack_utils
 from orbax.checkpoint import test_utils
 from orbax.checkpoint import transform_utils
 from orbax.checkpoint import type_handlers
 from orbax.checkpoint import utils
+from orbax.checkpoint import value_metadata
 from orbax.checkpoint.abstract_checkpointer import AbstractCheckpointer
 from orbax.checkpoint.array_checkpoint_handler import ArrayCheckpointHandler
 from orbax.checkpoint.async_checkpoint_handler import AsyncCheckpointHandler
 from orbax.checkpoint.async_checkpointer import async_checkpointer_context
 from orbax.checkpoint.async_checkpointer import AsyncCheckpointer
 from orbax.checkpoint.checkpoint_handler import CheckpointHandler
 from orbax.checkpoint.checkpoint_manager import checkpoint_manager_context
@@ -59,8 +60,8 @@
 # Convenient shorthand where instead of the following:
 #   `checkpointer = Checkpointer(PyTreeCheckpointer())`
 # we can just use:
 #   `checkpointer = PyTreeCheckpointer()`
 PyTreeCheckpointer = functools.partial(Checkpointer, PyTreeCheckpointHandler())
 
 # A new PyPI release will be pushed everytime `__version__` is increased.
-__version__ = '0.3.1'
+__version__ = '0.3.2'
```

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/abstract_checkpointer.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/abstract_checkpointer.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,25 +61,40 @@
         restore method.
 
     Returns:
       a restored object
     """
     pass
 
-  @abc.abstractmethod
   def structure(self, directory: epath.PathLike) -> Optional[Any]:
-    """The structure of the saved object at `directory`.
+    """DEPRECATED.
+
+    The structure of the saved object at `directory`.
 
     Delegates to underlying handler.
 
     Args:
       directory: a path to a saved checkpoint.
 
     Returns:
       the object structure or None, if the underlying handler does not implement
       `structure`.
     """
     pass
 
+  def metadata(self, directory: epath.PathLike) -> Optional[Any]:
+    """Returns metadata about the saved item.
+
+    Ideally, this is a cheap way to collect information about the checkpoint
+    without requiring a full restoration.
+
+    Args:
+      directory: the directory where the checkpoint is located.
+
+    Returns:
+      item metadata
+    """
+    pass
+
   def close(self):
     """Closes the Checkpointer."""
     pass
```

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/aggregate_handlers.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/aggregate_handlers.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/array_checkpoint_handler.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/array_checkpoint_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,18 @@
         )
     else:
       info = type_handlers.ParamInfo(
           name=self._checkpoint_name,
           path=directory / self._checkpoint_name,
           skip_deserialize=False,
       )
-      type_handler = type_handlers.get_type_handler(restore_args.restore_type)
+      restore_type = restore_args.restore_type
+      if restore_type is None:
+        restore_type = type_handlers.default_restore_type(restore_args)
+      type_handler = type_handlers.get_type_handler(restore_type)
       result = asyncio.run(
           type_handler.deserialize([info], args=[restore_args])
       )[0]
 
     utils.sync_global_devices('ArrayCheckpointHandler:restore')
     return result
```

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/async_checkpoint_handler.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/async_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/async_checkpointer.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/async_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_handler.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/checkpoint_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,25 +53,24 @@
       **kwargs: additional arguments for restore.
 
     Returns:
       The restored item.
     """
     pass
 
-  @abc.abstractmethod
-  def structure(self, directory: epath.Path) -> Any:
-    """Returns the structure of the item.
+  def metadata(self, directory: epath.Path) -> Optional[Any]:
+    """Returns metadata about the saved item.
 
-    This should represent the checkpointed item format without needing to fully
-    restore the entire item and all its values.
+    Ideally, this is a cheap way to collect information about the checkpoint
+    without requiring a full restoration.
 
     Args:
       directory: the directory where the checkpoint is located.
 
     Returns:
-      item structure
+      item metadata
     """
     pass
 
   def close(self):
     """Closes the CheckpointHandler."""
     pass
```

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_manager.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/checkpoint_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,18 +330,15 @@
     _, sorted_checkpoints = self._sort_checkpoints_by_metrics(self._checkpoints)
     if not sorted_checkpoints:
       return None
     return sorted_checkpoints[-1].step
 
   def reached_preemption(self, step: int) -> bool:
     """Returns True if a preemption sync point has been reached."""
-    return (
-        jax.config.jax_coordination_service
-        and multihost_utils.reached_preemption_sync_point(step)
-    )
+    return multihost_utils.reached_preemption_sync_point(step)
 
   def should_save(self, step: int) -> bool:
     """Returns True if a checkpoint should be saved for the current step.
 
     This depends the previous step and save interval.
 
     Args:
@@ -629,50 +626,41 @@
       item = items.get(item_name, None)
       kwargs = restore_kwargs.get(item_name, {})
       restored[item_name] = self._checkpointers[item_name].restore(
           path, item=item, **kwargs)
 
     return restored
 
-  def structure(self) -> Union[Any, Mapping[str, Any]]:
-    """For all Checkpointers, returns the saved structure.
+  def item_metadata(self, step: int) -> Union[Any, Mapping[str, Optional[Any]]]:
+    """For all Checkpointers, returns any metadata associated with the item.
+
+    Calls the `metadata` method for each Checkpointer and returns a
+    mapping of each item name to the restored metadata. If the manager only
+    manages a single item, a single metadata will be returned instead.
 
-    Calls the `structure` method for each Checkpointer and returns a
-    mapping of each item name to the restored structure. If the manager only
-    manages a single item, a single structure will be returned instead.
-
-    Note that any items for which the corresponding Checkpointer does not
-    have an implemented `structure` method, these items will simply not be
-    contained in the result. If, in this case, there is also only a single item
-    managed, None will be returned.
+    Metadata may be None for an individual item.
+
+    Args:
+      step: Step for which to retrieve metadata.
 
     Returns:
-      A dictionary mapping name to item structure, or a single item structure.
+      A dictionary mapping name to item metadata, or a single item metadata.
     """
     result = {}
-    step = self.latest_step()
-    if step is None:
-      raise ValueError(
-          'No existing checkpoint; structure cannot be determined.')
     for name, checkpointer in self._checkpointers.items():
       path = self._get_save_directory(step, self.directory, name)
       if name == METRIC_ITEM_NAME:
         assert self._track_best
         # No metrics file present: not an error.
         if not _metrics_file_exists(path):
           logging.warning('Missing metrics for step %d', step)
           continue
-      structure = checkpointer.structure(path)
-      # If None, then the item has no defined structure, and should be excluded.
-      # May be empty, which would simply represent a valid, but empty structure.
-      if structure is not None:
-        result[name] = structure
+      metadata = checkpointer.metadata(path)
+      result[name] = metadata
     if self._single_item:
-      if DEFAULT_ITEM_NAME not in result:
-        return None
       return result[DEFAULT_ITEM_NAME]
     return result
 
   @property
   def _track_best(self):
     """Returns true if we should track the best checkpoints by given metric."""
     return self._options.best_fn is not None
```

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_utils.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/checkpoint_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -304,81 +304,14 @@
       checkpoint_step = new_checkpoint_step
       yield checkpoint_step
     time_to_next_eval = start + min_interval_secs - time.time()
     if time_to_next_eval > 0:
       time.sleep(time_to_next_eval)
 
 
-# TODO(b/274813763): Remove this function when no longer depended on by Flax.
-def restore_args_from_target(
-    mesh: jax.sharding.Mesh, target: PyTree, axes_tree: PyTree
-) -> PyTree:
-  """DEPRECATED, DO NOT USE.
-
-  Creates restore_args given a target PyTree.
-
-  This method should be used in conjunction with a CheckpointManager or
-  Checkpointer that wraps a PyTreeCheckpointHandler.
-
-  For example:
-
-  mngr = CheckpointManager(path, Checkpointer(PyTreeCheckpointHandler()))
-  restore_args = restore_args_from_target(mesh, train_state, train_state_axes)
-  restore_kwargs = {'restore_args': restore_args}
-  mngr.restore(..., restore_kwargs=restore_kwargs)
-
-  OR
-
-  mngr = CheckpointManager(path, {
-      'train_state': Checkpointer(PyTreeCheckpointHandler())
-  })
-  restore_args = restore_args_from_target(mesh, train_state, train_state_axes)
-  restore_kwargs = {'train_state': {'restore_args': restore_args} }
-  mngr.restore(..., restore_kwargs=restore_kwargs)
-
-  OR
-
-  ckptr = Checkpointer(PyTreeCheckpointHandler())
-  restore_args = restore_args_from_target(mesh, train_state, train_state_axes)
-  ckptr.restore(..., restore_args=restore_args)
-
-  If a leaf in target does is a np.ndarray, or int, or string, for example, a
-  corresponding value for that leaf must be provided in axes_tree, but will be
-  ignored.
-
-  Args:
-    mesh: jax.sharding.Mesh to shard arrays with.
-    target: The returned value will match the structure of `target`, will be
-      used to set the desired dtype and restoration shape.
-    axes_tree: A PyTree matching `target` which will be used to set the
-      restoration sharding.
-
-  Returns:
-    A PyTree matching target of RestoreArgs (or ArrayRestoreArgs) objects.
-  """
-
-  def _restore_args(value, axes):
-    restore_type = type(value)
-    dtype = None
-    if hasattr(value, 'dtype'):
-      dtype = value.dtype
-    if isinstance(value, jax.Array):
-      return type_handlers.ArrayRestoreArgs(
-          restore_type=restore_type,
-          mesh=mesh,
-          mesh_axes=axes,
-          global_shape=value.shape,
-          dtype=value.dtype,
-      )
-    else:
-      return type_handlers.RestoreArgs(restore_type=restore_type, dtype=dtype)
-
-  return jax.tree_util.tree_map(_restore_args, target, axes_tree)
-
-
 def construct_restore_args(
     target: PyTree, sharding_tree: PyTree, set_global_shape: bool = True
 ) -> PyTree:
   """Creates restore_args given a target PyTree.
 
   This method should be used in conjunction with a CheckpointManager or
   Checkpointer that wraps a PyTreeCheckpointHandler.
```

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/checkpoint_utils_test.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/checkpoint_utils_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,76 +24,14 @@
 from orbax.checkpoint import checkpoint_utils
 from orbax.checkpoint import test_utils
 from orbax.checkpoint import utils
 
 
 class CheckpointUtilsTest(absltest.TestCase):
 
-  def test_restore_args_from_target(self):
-    devices = np.asarray(jax.devices())
-    mesh = jax.sharding.Mesh(devices, ('x',))
-    axes_tree = {
-        'a': jax.sharding.PartitionSpec(
-            'x',
-        ),
-        'x': None,
-        'y': None,
-    }
-    pytree = {
-        'a': test_utils.create_sharded_array(
-            np.arange(16, dtype=np.int32) * 1,
-            mesh,
-            jax.sharding.PartitionSpec(
-                'x',
-            ),
-        ),
-        'x': np.ones(8, dtype=np.float64),
-        'y': 1,
-    }
-
-    expected_restore_args = {
-        'a': orbax.checkpoint.ArrayRestoreArgs(
-            restore_type=jax.Array,
-            mesh=mesh,
-            mesh_axes=jax.sharding.PartitionSpec(
-                'x',
-            ),
-            global_shape=(16,),
-            dtype=np.int32,
-        ),
-        'x': orbax.checkpoint.RestoreArgs(
-            restore_type=np.ndarray, dtype=np.float64
-        ),
-        'y': orbax.checkpoint.RestoreArgs(restore_type=int),
-    }
-    restore_args = checkpoint_utils.restore_args_from_target(
-        mesh, pytree, axes_tree
-    )
-
-    self.assertSameElements(expected_restore_args.keys(), restore_args.keys())
-
-    def _check_restore_args(expected, actual):
-      self.assertIsInstance(actual, orbax.checkpoint.RestoreArgs)
-      self.assertEqual(expected.restore_type, actual.restore_type)
-      self.assertEqual(expected.dtype, actual.dtype)
-
-    def _check_array_restore_args(expected, actual):
-      self.assertIsInstance(actual, orbax.checkpoint.ArrayRestoreArgs)
-      self.assertEqual(expected.restore_type, jax.Array)
-      self.assertEqual(expected.mesh, actual.mesh)
-      self.assertEqual(expected.mesh_axes, actual.mesh_axes)
-      self.assertEqual(expected.global_shape, actual.global_shape)
-      self.assertEqual(expected.dtype, actual.dtype)
-
-    with self.subTest(name='array_restore_args'):
-      _check_array_restore_args(expected_restore_args['a'], restore_args['a'])
-    with self.subTest(name='restore_args'):
-      _check_restore_args(expected_restore_args['x'], restore_args['x'])
-      _check_restore_args(expected_restore_args['y'], restore_args['y'])
-
   def test_construct_restore_args(self):
     devices = np.asarray(jax.devices())
     mesh = jax.sharding.Mesh(devices, ('x',))
     sharding_tree = {
         'a': jax.sharding.NamedSharding(
             mesh,
             jax.sharding.PartitionSpec(
```

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/checkpointer.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/checkpointer.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,21 +98,18 @@
     if not utils.is_checkpoint_finalized(directory):
       raise ValueError(f'Found incomplete checkpoint at {directory}.')
     logging.info('Restoring item from %s.', directory)
     restored = self._handler.restore(directory, *args, item=item, **kwargs)
     logging.info('Finished restoring checkpoint from %s.', directory)
     return restored
 
-  def structure(self, directory: epath.PathLike) -> Optional[Any]:
+  def metadata(self, directory: epath.PathLike) -> Optional[Any]:
     """See superclass documentation."""
     directory = epath.Path(directory)
-    try:
-      return self._handler.structure(directory)
-    except NotImplementedError:
-      return
+    return self._handler.metadata(directory)
 
   def close(self):
     """Closes the underlying CheckpointHandler."""
     self._handler.close()
 
 
 @contextlib.contextmanager
```

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/conftest.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/conftest.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/future.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/future.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/json_checkpoint_handler.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/json_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/json_checkpoint_handler_test.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/json_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/msgpack_utils.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/msgpack_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/msgpack_utils_test.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/msgpack_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/orbax_checkpoint.ipynb` & `orbax_checkpoint-0.3.2/orbax/checkpoint/orbax_checkpoint.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999612369337979%*

 * *Differences: {"'cells'": "{46: {'source': ['As shown in this example, this object may be useful for restoring a "*

 * *            "pre-existing checkpoint without requiring a `CheckpointManager`.']}, 61: {'source': "*

 * *            "{insert: [(0, 'from orbax.checkpoint.value_metadata import Metadata\\n'), (1, 'from "*

 * *            "orbax.checkpoint.type_handlers import ParamInfo\\n'), (2, 'from typing import Any, "*

 * *            "Tuple\\n'), (3, '\\n'), (5, '\\n'), (6, '  def typestr(self) -> str:\\n'), (7, "*

 * *            '"    ret […]*

```diff
@@ -690,15 +690,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "i-JTtxeNtO95"
             },
             "source": [
-                "As shown in this example, this object may be useful for restoring a pre-exisiting checkpoint without requiring a `CheckpointManager`."
+                "As shown in this example, this object may be useful for restoring a pre-existing checkpoint without requiring a `CheckpointManager`."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "M-_hqQoTtrAK"
             },
@@ -943,29 +943,44 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "id": "dlhtm54F-wAP"
             },
             "outputs": [],
             "source": [
+                "from orbax.checkpoint.value_metadata import Metadata\n",
+                "from orbax.checkpoint.type_handlers import ParamInfo\n",
+                "from typing import Any, Tuple\n",
+                "\n",
                 "class FooHandler(orbax.checkpoint.type_handlers.TypeHandler):\n",
                 "\n",
+                "  def typestr(self) -> str:\n",
+                "    return 'foo'\n",
+                "\n",
+                "  def metadata(self, value: Foo) -> Metadata:\n",
+                "    return Metadata()\n",
+                "\n",
+                "  async def open(self, info: ParamInfo) -> Tuple[Metadata, Any]:\n",
+                "    return Metadata(), None\n",
+                "\n",
                 "  async def serialize(\n",
                 "      self,\n",
                 "      value: Foo,\n",
-                "      info: orbax.checkpoint.type_handlers.ParamInfo,\n",
+                "      info: ParamInfo,\n",
                 "      args: Optional[orbax.checkpoint.SaveArgs] = None) -> List[orbax.checkpoint.future.Future]:\n",
                 "    # A more sophisticated implementation would make this write asynchronous.\n",
                 "    (info.path / 'data.txt').write_text(str(value))\n",
                 "    return []\n",
                 "\n",
                 "  async def deserialize(\n",
                 "      self,\n",
-                "      info: orbax.checkpoint.type_handlers.ParamInfo,\n",
+                "      file: Any,\n",
+                "      info: ParamInfo,\n",
                 "      args: Optional[orbax.checkpoint.RestoreArgs] = None) -> Foo:\n",
+                "    del file\n",
                 "    entries = (info.path / 'data.txt').read_text().split(';')\n",
                 "    assert len(entries) == 3\n",
                 "    return Foo(*entries)"
             ]
         },
         {
             "cell_type": "code",
@@ -1023,15 +1038,15 @@
                 "id": "0rRnvnVaag00"
             },
             "source": [
                 "A key component of the Orbax checkpointing library is PyTree [transformations](https://github.com/google/orbax/tree/main/orbax/checkpoint/transform_utils.py). While this functionality is designed to be as flexible as possible, it can be used to support:\n",
                 "\n",
                 "\n",
                 "*   Partial restoration of checkpoints where some keys can be dropped and replaced with randomly initialized values.\n",
-                "*   Checkpoint version compatiblity where newer checkpoints may have different structures than old ones.\n",
+                "*   Checkpoint version compatibility where newer checkpoints may have different structures than old ones.\n",
                 "*   Mappings over keys, including one-to-one, many-to-one, one-to-many, and many-to-many transformations.\n",
                 "\n",
                 "The transformations library is discussed in detail [here](https://github.com/google/orbax/blob/main/docs/checkpoint.md#transformations), so we will avoid discussing all possible features and will instead focus on concrete examples.\n",
                 "\n"
             ]
         },
         {
```

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/proto/__init__.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/proto/testing/__init__.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/proto/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/proto_checkpoint_handler.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/proto_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/pytree_checkpoint_handler.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/pytree_checkpoint_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,50 +14,147 @@
 
 """PyTreeCheckpointHandler class.
 
 Implementation of CheckpointHandler interface.
 """
 
 import asyncio
+import collections
 import dataclasses
+import enum
 import re
 import typing
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from absl import logging
 from etils import epath
 import jax
 from jax.experimental.array_serialization import serialization
 import numpy as np
 from orbax.checkpoint import aggregate_handlers
+from orbax.checkpoint import json_checkpoint_handler
 from orbax.checkpoint import transform_utils
 from orbax.checkpoint import type_handlers
 from orbax.checkpoint import utils
+from orbax.checkpoint import value_metadata
 from orbax.checkpoint.async_checkpoint_handler import AsyncCheckpointHandler
 from orbax.checkpoint.future import Future
-import tensorstore as ts
 
 
 PyTree = Any
 TupleKey = Tuple[str, ...]
 RestoreArgs = type_handlers.RestoreArgs
 ArrayRestoreArgs = type_handlers.ArrayRestoreArgs
 SaveArgs = type_handlers.SaveArgs
 ParamInfo = type_handlers.ParamInfo
 TypeHandler = type_handlers.TypeHandler
 AggregateHandler = aggregate_handlers.AggregateHandler
 MsgpackHandler = aggregate_handlers.MsgpackHandler
 TransformFn = Callable[[PyTree, PyTree, PyTree], Tuple[PyTree, PyTree]]
 Transform = transform_utils.Transform
 RestoreTransform = transform_utils.RestoreTransform
+JsonCheckpointHandler = json_checkpoint_handler.JsonCheckpointHandler
 
-_TYPE_METADATA_FILE = 'type_metadata'
+
+_METADATA_FILE = '_METADATA'
 _CHECKPOINT_FILE = 'checkpoint'
 
 
+### Metadata utils
+_KEY_NAME = 'key'
+_KEY_TYPE = 'key_type'
+_VALUE_TYPE = 'value_type'
+_SKIP_DESERIALIZE = 'skip_deserialize'
+
+_TREE_METADATA_KEY = 'tree_metadata'
+_KEY_METADATA_KEY = 'key_metadata'
+_VALUE_METADATA_KEY = 'value_metadata'
+
+
+class KeyType(enum.Enum):
+  """Enum representing PyTree key type."""
+
+  SEQUENCE = 1
+  DICT = 2
+
+  def to_json(self) -> int:
+    return self.value
+
+  @classmethod
+  def from_json(cls, value: int) -> 'KeyType':
+    return cls(value)
+
+
+def _get_key_metadata_type(key: Any) -> KeyType:
+  """Translates the JAX key class into a proto enum."""
+  if utils.is_sequence_key(key):
+    return KeyType.SEQUENCE
+  elif utils.is_dict_key(key):
+    return KeyType.DICT
+  else:
+    raise ValueError(f'Unsupported KeyEntry: {type(key)}: "{key}"')
+
+
+def _keypath_from_key_type(key_name: str, key_type: KeyType) -> Any:
+  """Converts from Key in TreeMetadata to JAX keypath class."""
+  if key_type == KeyType.SEQUENCE:
+    return jax.tree_util.SequenceKey(int(key_name))
+  elif key_type == KeyType.DICT:
+    return jax.tree_util.DictKey(key_name)
+  else:
+    raise ValueError(f'Unsupported KeyEntry: {key_type}')
+
+
+def _get_keypath_metadata(keypath: Any) -> Tuple[Dict[str, Any]]:
+  """Gets JSON metadata for a JAX keypath."""
+  keypath_serialized = []
+  for k in keypath:
+    keypath_serialized.append({
+        _KEY_NAME: str(utils.get_key_name(k)),
+        _KEY_TYPE: _get_key_metadata_type(k).to_json(),
+    })
+  return tuple(keypath_serialized)
+
+
+def _keypath_from_metadata(keypath_serialized: Tuple[Dict[str, Any]]) -> Any:
+  """Creates a JAX keypath from JSON metadata."""
+  keypath = []
+  for k in keypath_serialized:
+    keypath.append(
+        _keypath_from_key_type(k[_KEY_NAME], KeyType.from_json(k[_KEY_TYPE]))
+    )
+  return tuple(keypath)
+
+
+def _get_value_metadata(value: Any, save_arg: SaveArgs) -> Dict[str, Any]:
+  """Gets JSON metadata for a given value."""
+  if utils.is_supported_empty_aggregation_type(value):
+    typestr = type_handlers.get_empty_value_typestr(value)
+    skip_deserialize = True
+  else:
+    try:
+      handler = type_handlers.get_type_handler(type(value))
+      typestr = handler.typestr()
+      skip_deserialize = save_arg.aggregate
+    except ValueError:
+      # Not an error because users' training states often have a bunch of
+      # random unserializable objects in them (empty states, optimizer
+      # objects, etc.). An error occurring due to a missing TypeHandler
+      # will be surfaced elsewhere.
+      typestr = 'None'
+      skip_deserialize = True
+  return {
+      _VALUE_TYPE: typestr,
+      _SKIP_DESERIALIZE: skip_deserialize,
+  }
+
+
+### End metadata utils
+
+
 async def _create_param_save_dir(param_info: ParamInfo, args: SaveArgs):
   # Directory will be unused.
   path = param_info.path
   if path is None or args.aggregate:
     return
   if jax.process_index() == 0:
     # TODO(b/273803615): Note that keys with slashes ('/', generated by Haiku,
@@ -102,14 +199,15 @@
         value.shape, sharding, lambda idx: value[idx]
     )
   return value
 
 
 def _get_param_names(item: PyTree) -> PyTree:
   """Gets parameter names for PyTree elements."""
+
   def _param_name_from_keypath(keypath: Tuple[Any, ...]) -> str:
     return '.'.join([str(utils.get_key_name(k)) for k in keypath])
 
   return jax.tree_util.tree_map_with_path(
       lambda kp, _: _param_name_from_keypath(kp),
       item,
       is_leaf=utils.is_empty_or_leaf,
@@ -123,21 +221,21 @@
 def _find_matching_input_args(
     input_key: TupleKey,
     flat_item: Dict[TupleKey, Any],
     flat_transforms: Dict[TupleKey, Transform],
     flat_restore_args: Dict[TupleKey, RestoreArgs],
 ) -> Optional[RestoreArgs]:
   """Given an input_key, tries to find matching RestoreArgs for the input.
-  
+
   Args:
     input_key: A key in the input tree.
     flat_item: The flattened, user-provided item.
     flat_transforms: Flattened transformations dict.
     flat_restore_args: Flattened tree of RestoreArgs, relative to item.
-    
+
   Returns:
     RestoreArgs that match the given input_key, according to the
     transformations, or None if no match is found.
   """
   for transform_key, transform in flat_transforms.items():
     if transform.multi_value_fn is not None:
       if not isinstance(transform, RestoreTransform):
@@ -182,14 +280,21 @@
   for transform_key, transform in flat_transforms.items():
     match = re.fullmatch(_keystr(transform_key), _keystr(input_key))
     if match and transform.use_fallback:
       result = True
   return result
 
 
+@dataclasses.dataclass
+class _InternalValueMetadata:
+  restore_type: Optional[str]
+  skip_deserialize: bool = False
+  aggregate_value: Optional[Any] = None
+
+
 def _get_restore_parameters(
     directory: epath.Path,
     item: Optional[PyTree],
     structure: PyTree,
     transforms: Optional[PyTree],
     restore_args: Optional[PyTree],
     byte_limiter: Optional[serialization._LimitInFlightBytes] = None,
@@ -237,58 +342,49 @@
   if restore_args is None:
     restore_args = jax.tree_util.tree_map(lambda x: RestoreArgs(), structure)
   flat_restore_args = utils.to_flat_dict(restore_args, keep_empty_nodes=True)
   flat_param_infos = {}
   flat_input_restore_args = {}
   is_ocdbt_checkpoint = type_handlers.is_ocdbt_checkpoint(directory)
 
-  def _get_param_info(nested_name: Tuple[str, ...], leaf: Any) -> ParamInfo:
-    if utils.leaf_is_placeholder(leaf):
-      # Leaf is a param name.
-      path = directory / utils.name_from_leaf_placeholder(leaf)
-    # The following is kept for backwards compatibility.
-    elif isinstance(leaf, ts.Spec):
-      tspec = leaf.to_json()  # pytype: disable=attribute-error
-      # Skip '.', since we need special regex handling for this char.
-      pattern = r'\.' + utils.TMP_DIR_SUFFIX[1:] + r'\d+'
-      path = re.sub(pattern, '', tspec['kvstore']['path'])
-    elif utils.is_supported_empty_aggregation_type(leaf):
-      return leaf  # Empty node, ParamInfo should not be returned.
-    elif utils.is_supported_aggregation_type(leaf):
-      # Value already restored, do not need ts.Spec.
-      path = None
-    else:
-      raise ValueError(f'Unsupported type: {type(leaf)}')
+  def _get_param_info(
+      nested_name: Tuple[str, ...],
+      meta: _InternalValueMetadata,
+  ) -> Union[ParamInfo, Any]:
+    if utils.is_supported_empty_aggregation_type(meta):
+      # Empty node, ParamInfo should not be returned.
+      return meta
+    name = '.'.join(nested_name)
     return ParamInfo(
-        name='.'.join(nested_name),
-        path=path,
-        skip_deserialize=(path is None),
+        name=name,
+        path=directory / name,
+        skip_deserialize=meta.skip_deserialize,
         is_ocdbt_checkpoint=is_ocdbt_checkpoint,
         byte_limiter=byte_limiter,
     )
 
   if transforms is None:
-    for key, value in flat_structure.items():
-      flat_param_infos[key] = _get_param_info(key, value)
+    for key, meta in flat_structure.items():
+      flat_param_infos[key] = _get_param_info(key, meta)
     restore_args = utils.serialize_tree(restore_args, keep_empty_nodes=True)
   else:
     if item is None:
       raise ValueError(
           'If providing `transforms`, must provide `item` matching structure'
           ' of expected result.'
       )
     flat_item = utils.to_flat_dict(item, keep_empty_nodes=True)
     flat_transforms = utils.to_flat_dict(transforms)
 
-    for input_key, value in flat_structure.items():
+    for input_key, meta in flat_structure.items():
       maybe_input_args = _find_matching_input_args(
           input_key, flat_item, flat_transforms, flat_restore_args
       )
       if maybe_input_args:
-        flat_param_infos[input_key] = _get_param_info(input_key, value)
+        flat_param_infos[input_key] = _get_param_info(input_key, meta)
         flat_input_restore_args[input_key] = maybe_input_args
       elif input_key in flat_item and input_key in flat_structure:
         # Key is present in both input and output.
         if _has_use_fallback_transform(input_key, flat_transforms):
           # Indicates that a `use_fallback` transformation was specified.
           if transforms_default_to_original:
             # Specified `use_fallback`, but key was also present in the
@@ -296,21 +392,21 @@
             # overridden with a new value.
             flat_param_infos[input_key] = ParamInfo(skip_deserialize=True)
             flat_input_restore_args[input_key] = RestoreArgs()
           else:
             # Specified `use_fallback`, but `transforms_default_to_original`
             # is False. This means we draw the value from the user-provided
             # `item`.
-            flat_param_infos[input_key] = _get_param_info(input_key, value)
+            flat_param_infos[input_key] = _get_param_info(input_key, meta)
             flat_input_restore_args[input_key] = flat_restore_args[input_key]
         else:
           # Transform not specified.
           if transforms_default_to_original:
             # Key/value is carried over from the original unchanged.
-            flat_param_infos[input_key] = _get_param_info(input_key, value)
+            flat_param_infos[input_key] = _get_param_info(input_key, meta)
             flat_input_restore_args[input_key] = flat_restore_args[input_key]
           else:
             # Take the value from the user-provided `item`, ignoring any value
             # in the checkpoint.
             flat_param_infos[input_key] = ParamInfo(skip_deserialize=True)
             flat_input_restore_args[input_key] = RestoreArgs()
       else:
@@ -355,35 +451,43 @@
       _get_leaf_for_aggregation, param_infos, save_args, item
   )
 
 
 @dataclasses.dataclass
 class _BatchRequest:
   """Represents a a request for batched serialization or deserialization."""
+
   handler: TypeHandler
   values: List[Any]
   infos: List[ParamInfo]
   args: List[Union[SaveArgs, RestoreArgs]]
 
 
 def _batched_serialization_requests(
     tree: PyTree, param_infos: PyTree, args: PyTree
 ) -> List[_BatchRequest]:
   """Gets a list of batched serialization or deserialization requests."""
-  result = []
   grouped = {}
 
-  def _group_value(info, value, arg):
-    nonlocal result
+  def _group_value(
+      info: ParamInfo,
+      value: Union[Any, _InternalValueMetadata],
+      arg: RestoreArgs,
+  ):
     nonlocal grouped
     # Exclude from serialize/deserialize with TypeHandler if aggregated.
     if info.skip_deserialize:
       return
     if isinstance(arg, RestoreArgs):
-      handler = type_handlers.get_type_handler(arg.restore_type)
+      assert isinstance(value, _InternalValueMetadata)
+      restore_type = value.restore_type
+      if arg.restore_type is not None:
+        # Give user the chance to override restore_type if they want.
+        restore_type = arg.restore_type
+      handler = type_handlers.get_type_handler(restore_type)
     else:
       handler = type_handlers.get_type_handler(type(value))
     if handler not in grouped:
       grouped[handler] = _BatchRequest(handler, [], [], [])
     request = grouped[handler]
     grouped[handler] = dataclasses.replace(
         request,
@@ -394,15 +498,15 @@
 
   jax.tree_util.tree_map(
       _group_value,
       param_infos,
       tree,
       args,
   )
-  return result + list(grouped.values())
+  return list(grouped.values())
 
 
 def _multi_value_fns_with_args(
     transforms: PyTree, restore_args: PyTree
 ) -> PyTree:
   """Constructs a wrapper for multi_value_fn including RestoreArgs."""
   flat_restore_args = utils.to_flat_dict(restore_args, sep='/')
@@ -419,15 +523,15 @@
       return Transform(multi_value_fn=_multi_value_fn_with_args)
     else:
       return transform
 
   return jax.tree_util.tree_map(_maybe_wrap_transform, transforms)
 
 
-def _transform_structure(
+def _transform_checkpoint(
     item: PyTree,
     restored: PyTree,
     restore_args: Optional[PyTree],
     transforms: Optional[PyTree],
     transforms_default_to_original: bool,
 ) -> PyTree:
   """Optionally transforms the restored PyTree to the structure of `item`.
@@ -441,30 +545,33 @@
     transforms_default_to_original: See transform_utils.
 
   Returns:
     A transformed PyTree.
   """
   if item is None:
     if transforms is not None:
-      msg = ('If providing `transforms`, must provide `item` matching structure'
-             ' of expected result.')
+      msg = (
+          'If providing `transforms`, must provide `item` matching structure'
+          ' of expected result.'
+      )
       raise ValueError(msg)
     item = restored
   else:
     if transforms is None:
       item = utils.deserialize_tree(restored, item)
     else:
       if restore_args is None:
         raise ValueError(
             'If providing `transforms`, must provide `restore_args` matching'
             ' structure of expected result.'
         )
       transforms = _multi_value_fns_with_args(transforms, restore_args)
       item = transform_utils.apply_transformations(
-          restored, transforms, item, transforms_default_to_original)
+          restored, transforms, item, transforms_default_to_original
+      )
   return item
 
 
 class PyTreeCheckpointHandler(AsyncCheckpointHandler):
   """A CheckpointHandler implementation for any PyTree structure.
 
   The PyTree is assumed to be a nested dictionary with array values represented
@@ -474,35 +581,44 @@
 
   def __init__(
       self,
       aggregate_filename: Optional[str] = None,
       concurrent_gb: int = 96,
       use_ocdbt: bool = False,
       restore_with_serialized_types: bool = True,
+      write_tree_metadata: bool = False,
   ):
     """Creates PyTreeCheckpointHandler.
 
     Args:
       aggregate_filename: name that the aggregated checkpoint should be saved
         as.
       concurrent_gb: max concurrent GB that are allowed to be read.
       use_ocdbt: enables Tensorstore OCDBT driver.
       restore_with_serialized_types: If True, the values with unspecified
         restore types will be restored using the typing information in the
         checkpoint. Otherwise, arrays will be restored as either np.ndarray or
         jax.Array, and will ignore any typing information present in the
         checkpoint.
+      write_tree_metadata: Experimental feature. Writes tree metadata in JSON
+        format.
     """
     self._aggregate_handler = MsgpackHandler()
     if aggregate_filename is None:
       aggregate_filename = _CHECKPOINT_FILE
     self._aggregate_filename = aggregate_filename
     self._concurrent_gb = concurrent_gb
     self._use_ocdbt = use_ocdbt
     self._restore_with_serialized_types = restore_with_serialized_types
+    self._write_tree_metadata = write_tree_metadata
+    self._metadata = None
+    self._metadata_handler = JsonCheckpointHandler(_METADATA_FILE)
+
+    if self._use_ocdbt:
+      type_handlers.start_coordinator_server_and_create_context()
 
   def _get_param_names(self, item: PyTree) -> PyTree:
     """Gets parameter names for PyTree elements."""
     return _get_param_names(item)
 
   def _get_param_infos(
       self, item: PyTree, directory: epath.Path, save_args: PyTree
@@ -535,31 +651,20 @@
       )
 
     return (
         jax.tree_util.tree_map(_param_info, names, save_args),
         all_params_aggregated,
     )
 
-  async def _write_aggregate_file(
-      self,
-      directory: epath.Path,
-      item: PyTree,
-      param_infos: PyTree,
-      save_args: PyTree,
-  ) -> Future:
-    ser_item = _get_tree_for_aggregation(param_infos, save_args, item)
-    return await self._aggregate_handler.serialize(
-        directory / self._aggregate_filename, ser_item
-    )
-
   async def async_save(
       self,
       directory: epath.Path,
       item: PyTree,
-      save_args: Optional[PyTree] = None) -> Optional[List[Future]]:
+      save_args: Optional[PyTree] = None,
+  ) -> Optional[List[Future]]:
     """Saves a PyTree from a given training step.
 
     This operation is compatible with a multi-host, multi-device setting. Tree
     leaf values must be supported by type_handlers. Standard supported types
     include scalars, np.ndarray, jax.Array, string.
 
     After saving, all files will be located in "directory/".
@@ -615,14 +720,16 @@
                 request.values, request.infos, request.args
             )
         ]
       # Await copy futures. Returns list of lists.
       commit_futures = await asyncio.gather(*serialize_ops)
       commit_futures, _ = jax.tree_util.tree_flatten(commit_futures)
 
+    # TODO(b/285888834): Allow this to be asynchronous.
+    self._write_metadata_file(directory, item, save_args)
     aggregate_commit_future = await self._write_aggregate_file(
         directory, item, param_infos, save_args
     )
     return commit_futures + [aggregate_commit_future]
 
   def save(self, directory: epath.Path, item: Any, *args, **kwargs):
     """Saves the provided item.
@@ -651,42 +758,49 @@
 
   async def _maybe_deserialize(
       self, structure: PyTree, param_infos: PyTree, restore_args: PyTree
   ) -> PyTree:
     """Deserializes values or gets them from the aggregate file."""
 
     # Handle parameters from aggregate file.
-    def _process_aggregated_value(info, value, args):
+    def _process_aggregated_value(info, meta, args):
+      value = meta.aggregate_value
       if info.skip_deserialize:
         value = _try_array_cast(value, args.dtype)
         value = _maybe_shard_array(value, args)
       return value
 
-    structure = jax.tree_util.tree_map(
-        _process_aggregated_value, param_infos, structure, restore_args
+    flat_aggregate = utils.to_flat_dict(
+        jax.tree_util.tree_map(
+            _process_aggregated_value, param_infos, structure, restore_args
+        ),
+        sep='.',
     )
 
     batch_requests = _batched_serialization_requests(
         structure, param_infos, restore_args
     )
     deserialized_batches = []
     deserialized_batches_ops = []
     for request in batch_requests:
       deserialized_batches_ops.append(
           request.handler.deserialize(request.infos, request.args)
       )
     deserialized_batches += await asyncio.gather(*deserialized_batches_ops)
 
-    flat_restored = utils.to_flat_dict(structure, sep='.')
+    flat_restored = {}
     for request, deserialized in zip(batch_requests, deserialized_batches):
       for info, value in zip(request.infos, deserialized):
+        assert not info.skip_deserialize
         flat_restored[info.name] = value
-
-    restored = utils.from_flat_dict(flat_restored, target=structure, sep='.')
-    return restored
+    # Add in any values which were not deserialized, coming from aggregate file.
+    for key in flat_aggregate.keys():
+      if key not in flat_restored:
+        flat_restored[key] = flat_aggregate[key]
+    return utils.from_flat_dict(flat_restored, target=structure, sep='.')
 
   def restore(
       self,
       directory: epath.Path,
       item: Optional[PyTree] = None,
       restore_args: Optional[PyTree] = None,
       transforms: Optional[PyTree] = None,
@@ -724,27 +838,28 @@
     Raises:
       FileNotFoundError: `directory` does not exist or is missing required files
       ValueError: `transforms` is provided without `item`.
       ValueError: `transforms` contains elements with `multi_value_fn`.
     """
     if not directory.exists():
       raise FileNotFoundError(
-          f'Requested directory for restore does not exist at {directory}')
+          f'Requested directory for restore does not exist at {directory}'
+      )
 
     async def _create_byte_limiter():
       # Wrap creation in async function to avoid issues on python<=3.9.
       concurrent_bytes = self._concurrent_gb * 10**9
       # Construction must take place here so that it is within the same async
       # method, to prevent errors resulting from different event loops, and
       # cannot be created below this level because there must be a single object
       # for the entire restore call.
       return serialization._LimitInFlightBytes(concurrent_bytes)  # pylint: disable=protected-access
 
     byte_limiter = asyncio.run(_create_byte_limiter())
-    structure = self.structure(directory)
+    structure = self._get_internal_metadata(directory)
     # `checkpoint_restore_args` has a structure relative to the checkpoint,
     # while `restore_args` remains structured relative to the output.
     param_infos, checkpoint_restore_args = _get_restore_parameters(
         directory,
         item,
         structure,
         transforms,
@@ -757,55 +872,279 @@
       raise ValueError('Cannot provide both `transforms` and `transform_fn`.')
     if transform_fn is not None:
       structure, param_infos = transform_fn(item, structure, param_infos)
       if restore_args is None:
         restore_args = jax.tree_util.tree_map(lambda x: RestoreArgs(), item)
       checkpoint_restore_args = restore_args
 
+    def _maybe_set_default_restore_types(
+        meta: _InternalValueMetadata, arg: RestoreArgs
+    ):
+      if not meta.skip_deserialize and meta.restore_type is None:
+        return dataclasses.replace(
+            meta, restore_type=type_handlers.default_restore_type(arg)
+        )
+      return meta
+
+    # If metadata file was missing in the checkpoint, we need to decide
+    # restore_type based on RestoreArgs.
+    structure = jax.tree_util.tree_map(
+        _maybe_set_default_restore_types, structure, checkpoint_restore_args
+    )
+
     restored_item = asyncio.run(
         self._maybe_deserialize(structure, param_infos, checkpoint_restore_args)
     )
 
     if not transform_fn:
-      restored_item = _transform_structure(
+      restored_item = _transform_checkpoint(
           item,
           restored_item,
           restore_args,
           transforms,
           transforms_default_to_original,
       )
     utils.sync_global_devices('PyTreeCheckpointHandler:restore')
     return restored_item
 
-  def structure(self, directory: epath.Path) -> PyTree:
-    """Restores the saved PyTree structure without regard for its leaf values.
+  async def _write_aggregate_file(
+      self,
+      directory: epath.Path,
+      item: PyTree,
+      param_infos: PyTree,
+      save_args: PyTree,
+  ) -> Future:
+    ser_item = _get_tree_for_aggregation(param_infos, save_args, item)
+    return await self._aggregate_handler.serialize(
+        directory / self._aggregate_filename, ser_item
+    )
+
+  def _read_aggregate_file(self, directory: epath.Path) -> PyTree:
+    """Restores the aggregate file representing PyTree structure."""
+    checkpoint_path = directory / self._aggregate_filename
+    if checkpoint_path.exists():
+      return self._aggregate_handler.deserialize(checkpoint_path)
+    elif self._use_ocdbt:
+      raise ValueError(
+          f'Checkpoint structure file does not exist at {directory}.'
+      )
+    else:
+      return utils.pytree_structure(directory)
+
+  def _write_metadata_file(
+      self, directory: epath.Path, item: PyTree, save_args: PyTree
+  ):
+    """Write PyTree metadata.
+
+    Uses JSON format:
+
+    {
+        _TREE_METADATA_KEY: {
+          "(top_level_key, lower_level_key)": {
+              _KEY_METADATA_KEY: (
+                  {_KEY_NAME: "top_level_key", _KEY_TYPE: <KeyType (int)>},
+                  {_KEY_NAME: "lower_level_key", _KEY_TYPE: <KeyType (int)>},
+              )
+              _VALUE_METADATA_KEY: {
+                  _VALUE_TYPE: "jax.Array",
+                  _SKIP_DESERIALIZE: True/False,
+              }
+          }
+          ...
+      }
+    }
+
+    Args:
+      directory: directory
+      item: item to save
+      save_args: save_args
+
+    Returns:
+      None
+    """
+    if not self._write_tree_metadata:
+      return []
+
+    flat_with_keys, _ = jax.tree_util.tree_flatten_with_path(
+        item, is_leaf=utils.is_empty_or_leaf
+    )
+    flat_save_args_with_keys, _ = jax.tree_util.tree_flatten_with_path(
+        save_args, is_leaf=utils.is_empty_or_leaf
+    )
+
+    flat_metadata_with_keys = {}
+    for (keypath, value), (_, save_arg) in zip(
+        flat_with_keys, flat_save_args_with_keys
+    ):
+      tuple_keypath = str(tuple([str(utils.get_key_name(k)) for k in keypath]))
+      flat_metadata_with_keys[tuple_keypath] = {
+          _KEY_METADATA_KEY: _get_keypath_metadata(keypath),
+          _VALUE_METADATA_KEY: _get_value_metadata(value, save_arg),
+      }
+
+    metadata = {_TREE_METADATA_KEY: flat_metadata_with_keys}
+    self._metadata_handler.save(directory, metadata)
+
+  def _read_metadata_file(self, directory: epath.Path) -> PyTree:
+    """Reads metadata file and returns a tree of restore types.
 
     Args:
-      directory: the directory to restore from.
+      directory: directory
 
     Returns:
-      The structure of the checkpointed PyTree. Leaves may be of any type.
+      Tree with _InternalValueMetadata as values.
 
     Raises:
-      FileNotFoundError: if the checkpoint is not found.
+      FileNotFoundError: if the metadata file is not found.
     """
-    checkpoint_path = directory / self._aggregate_filename
-    if checkpoint_path.exists():
-      return self._aggregate_handler.deserialize(checkpoint_path)
-    else:
-      if self._use_ocdbt:
-        raise ValueError(
-            f'Checkpoint structure file does not exist at {directory}.'
-        )
+    path = directory / _METADATA_FILE
+    if not path.exists():
+      raise FileNotFoundError(
+          f'Metadata file (named {_METADATA_FILE}) does not exist at'
+          f' {directory}.'
+      )
+
+    tree_metadata = typing.cast(
+        Dict[Any, Any], self._metadata_handler.restore(directory)
+    )[_TREE_METADATA_KEY]
+    flat_tree_metadata = []
+    for metadata in tree_metadata.values():
+      keypath = _keypath_from_metadata(metadata[_KEY_METADATA_KEY])
+      value_meta = metadata[_VALUE_METADATA_KEY]
+      value_meta = _InternalValueMetadata(
+          value_meta[_VALUE_TYPE],
+          skip_deserialize=value_meta[_SKIP_DESERIALIZE],
+      )
+      flat_tree_metadata.append((keypath, value_meta))
+
+    return utils.from_flattened_with_keypath(flat_tree_metadata)
+
+  def _get_internal_metadata(self, directory: epath.Path) -> PyTree:
+    """Gets limited information needed to fully restore the checkpoint.
+
+    This information just consists of the restore type for each leaf, as well
+    as the aggregated value (from the msgpack file) if present, and determines
+    whether we need to deserialize the parameter using TypeHandler later.
+
+    Args:
+      directory: directory
+
+    Returns:
+      A PyTree of _InternalValueMetadata with the tree structure of the
+      checkpoint.
+    """
+    aggregate_tree = self._read_aggregate_file(directory)
+    flat_aggregate = utils.to_flat_dict(aggregate_tree, keep_empty_nodes=True)
+    try:
+      metadata_tree = self._read_metadata_file(directory)
+      flat_metadata = utils.to_flat_dict(metadata_tree, keep_empty_nodes=True)
+    except FileNotFoundError:
+      metadata_tree = None
+      flat_metadata = None
+    if flat_metadata is None:
+      flat_metadata = jax.tree_util.tree_map(
+          lambda _: None, flat_aggregate, is_leaf=utils.is_empty_or_leaf
+      )
+
+    def _get_internal_value_metadata(value_meta, value):
+      if value_meta is None:
+        if utils.is_supported_empty_aggregation_type(value):
+          return value
+        restore_type = None
+        skip_deserialize = not utils.leaf_is_placeholder(value)
       else:
-        logging.error(
-            (
-                'Checkpoint structure file does not exist at %s.'
-                ' Attempting to assume an implicit tree structure.'
-            ),
-            directory,
+        if type_handlers.is_empty_typestr(value_meta.restore_type):
+          return type_handlers.get_empty_value_from_typestr(
+              value_meta.restore_type
+          )
+        restore_type, skip_deserialize = (
+            value_meta.restore_type,
+            value_meta.skip_deserialize,
         )
-        return utils.pytree_structure(directory)
+      return _InternalValueMetadata(
+          restore_type=restore_type,
+          skip_deserialize=skip_deserialize,
+          aggregate_value=value,
+      )
+
+    result = {}
+    for tuple_key in flat_metadata.keys():
+      result[tuple_key] = _get_internal_value_metadata(
+          flat_metadata[tuple_key], flat_aggregate[tuple_key]
+      )
+    target = metadata_tree if metadata_tree is not None else aggregate_tree
+    return utils.from_flat_dict(result, target=target)
+
+  def _get_user_metadata(self, directory: epath.Path) -> PyTree:
+    """Reads metadata file and constructs user-friendly metadata.
+
+    This will involve more file reads than are necessary for internal metadata.
+    Typically, we will need to perform extra reads in order to get metadata
+    about individual arrays.
+
+    Args:
+      directory: directory
+
+    Returns:
+      A PyTree of value_metadata.Metadata matching the checkpoint tree
+      structure.
+    """
+    is_ocdbt_checkpoint = type_handlers.is_ocdbt_checkpoint(directory)
+
+    flat_param_infos = {}
+    flat_restore_types = {}
+    metadata = self._read_metadata_file(directory)
+    for keypath, value_meta in utils.to_flat_dict(
+        metadata, keep_empty_nodes=True
+    ).items():
+      param_name = '.'.join(keypath)
+      restore_type, skip_deserialize = (
+          value_meta.restore_type,
+          value_meta.skip_deserialize,
+      )
+      flat_param_infos[keypath] = ParamInfo(
+          name=param_name,
+          path=directory / param_name,
+          skip_deserialize=skip_deserialize,
+          is_ocdbt_checkpoint=is_ocdbt_checkpoint,
+      )
+      flat_restore_types[keypath] = restore_type
+
+    flat_metadatas = {}
+    batched_param_infos = collections.defaultdict(list)
+    batched_keypaths = collections.defaultdict(list)
+    for keypath in flat_param_infos:
+      param_info = flat_param_infos[keypath]
+      restore_type = flat_restore_types[keypath]
+      if param_info.skip_deserialize:
+        flat_metadatas[keypath] = value_metadata.Metadata()
+      else:
+        batched_keypaths[restore_type].append(keypath)
+        batched_param_infos[restore_type].append(param_info)
+
+    metadata_ops = []
+    for restore_type, param_infos in batched_param_infos.items():
+      handler = type_handlers.get_type_handler(restore_type)
+      metadata_ops.append(handler.metadata(param_infos))
+
+    async def _get_metadata():
+      return await asyncio.gather(*metadata_ops)
+
+    batched_metadatas = asyncio.run(_get_metadata())
+    for keypath_batch, metadata_batch in zip(
+        batched_keypaths.values(), batched_metadatas
+    ):
+      for keypath, value in zip(keypath_batch, metadata_batch):
+        flat_metadatas[keypath] = value
+    return utils.from_flat_dict(flat_metadatas, target=metadata)
+
+  def metadata(self, directory: epath.Path) -> Optional[PyTree]:
+    if self._metadata is None:
+      try:
+        self._metadata = self._get_user_metadata(directory)
+      except FileNotFoundError as e:
+        logging.warning(e)
+    return self._metadata
 
   def close(self):
     """See superclass documentation."""
     self._aggregate_handler.close()
```

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/test_utils.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/test_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/transform_utils.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/transform_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/transform_utils_test.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/type_handlers.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/type_handlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,107 +15,143 @@
 """Provides utils for PytreeCheckpointHandler."""
 
 import abc
 import asyncio
 import dataclasses
 import json
 import os
+import typing
 from typing import Any, Callable, Dict, Optional, Sequence, Tuple, Union, cast
+import warnings
 
 from absl import logging
 from etils import epath
 import jax
 from jax.experimental.array_serialization import serialization
 from jax.experimental.array_serialization.serialization import get_tensorstore_spec
 import jax.numpy as jnp
 from jax.sharding import Mesh
 import numpy as np
 from orbax.checkpoint import utils
+from orbax.checkpoint import value_metadata
 from orbax.checkpoint.future import Future
 import tensorstore as ts
 
 
 Scalar = Union[int, float, np.number]
+Metadata = value_metadata.Metadata
+ScalarMetadata = value_metadata.ScalarMetadata
+ArrayMetadata = value_metadata.ArrayMetadata
+StringMetadata = value_metadata.StringMetadata
 _OCDBT_MANIFEST_FILE = 'manifest.ocdbt'
 _COORDINATOR_SETUP_TIMEOUT_SECS = 30
+_OCDBT_TS_CONTEXT = None
+_OCDBT_COORDINATOR_SERVER = None
 
 
 def _get_coordinator_address_without_port(coordinator_address: str) -> str:
   """Returns JAX coordinator address stripped of port number."""
   return coordinator_address.split(':')[0]
 
 
-def create_coordinator_server_and_context() -> (
-    Tuple[ts.Context, Optional[ts.ocdbt.DistributedCoordinatorServer]]
-):
-  """Creates OCDBT coordinator and Tensorstore context.
+def _enable_ocdbt_for_handlers():
+  # TODO(b/293331479) remove this once OCDBT is enabled by default
+  global _TYPESTR_REGISTRY
+  if _OCDBT_TS_CONTEXT is not None:
+    for _, handler in _TYPE_REGISTRY:
+      if hasattr(handler, 'enable_ocdbt') and callable(handler.enable_ocdbt):
+        handler.enable_ocdbt(_OCDBT_TS_CONTEXT)
+    _TYPESTR_REGISTRY = _make_typestr_registry(_TYPE_REGISTRY)
 
-  This function must be called at the start of the program across all processes
-  in order to initialize the OCDBT coordinator service. The coordinator object
-  should be kept alive for the life of the program, while the returned
-  ts.Context should be provided when saving or restoring using Tensorstore.
 
-  Example usage::
+def create_coordinator_server_and_context() -> None:
+  # TODO(b/293331479) remove this once OCDBT is enabled by default
+  warnings.warn('This function has been deprecated.  Do not use.')
 
-    ocdbt_context, coordinator_server = (
-        orbax.checkpoint.type_handlers.create_coordinator_server_and_context()
-    )
-    orbax.checkpoint.type_handlers.register_standard_handlers_with_options(
-        use_ocdbt=True, ts_context=ocdbt_context
-    )
-    orbax.checkpoint.utils.sync_global_devices('init_ocdbt_server')
 
-  Later, when creating the `PyTreeCheckpointHandler`, initialize with
-  `use_ocdbt=True`.
+def start_coordinator_server_and_create_context() -> None:
+  """Start a OCDBT coordinator and create a Tensorstore context.
+
+  This function is only for Orbax internal use.
+
+  The following function starts a coordinator_server and update type handlers
+  with enable_ocdbt() defined.
+
+  The context and server will be stored as global variables in _OCDBT_TS_CONTEXT
+  and _OCDBT_COORDINATOR_SERVER.  They will be preserved for the life of the
+  program.  Succeeding calls to this function will not try to start the
+  coordinator server again.
+
+  For testing purpose, if one needs to restart the coordinator server, set
+  _OCDBT_TS_CONTEXT and _OCDBT_COORDINATOR_SERVER to None and call this function
+  again.
 
   Returns:
-    Tuple of ts.Context and OCDBT coordinator server object.
+    None
   """
-  jax_global_state = jax._src.distributed.global_state  # pylint: disable=protected-access
-  if not jax_global_state.coordinator_address:
-    ts_context = {
-        # Provide cache pool for B-tree nodes to avoid repeated reads.
-        # 100MB limit.
-        'cache_pool#ocdbt': {'total_bytes_limit': 100000000},
-    }
-    return (
-        ts.Context(ts_context, parent=serialization.TS_CONTEXT),
-        None,
-    )
+  global _OCDBT_TS_CONTEXT, _OCDBT_COORDINATOR_SERVER
 
-  ocdbt_address = _get_coordinator_address_without_port(
-      jax_global_state.coordinator_address
-  )
-
-  coordinator_server = None
-  if jax_global_state.process_id == 0:
-    bind_address = f'{ocdbt_address}:0'
-    logging.info('Starting DistributedCoordinatorServer at: %s', bind_address)
-    coordinator_server = ts.ocdbt.DistributedCoordinatorServer({
-        'bind_addresses': [bind_address],
-    })
-    jax_global_state.client.key_value_set(
-        'ocdbt_coordinator', f'{ocdbt_address}:{coordinator_server.port}'
-    )
+  if _OCDBT_TS_CONTEXT is not None:
+    # OCDBT ts_context is already set, return
+    return
 
-  ocdbt_address = jax_global_state.client.blocking_key_value_get(
-      'ocdbt_coordinator', _COORDINATOR_SETUP_TIMEOUT_SECS * 1000
-  )
   ts_context = {
-      'ocdbt_coordinator': {
-          'address': ocdbt_address,
-      },
       # Provide cache pool for B-tree nodes to avoid repeated reads.
       # 100MB limit.
       'cache_pool#ocdbt': {'total_bytes_limit': 100000000},
   }
-  return (
-      ts.Context(ts_context, parent=serialization.TS_CONTEXT),
-      coordinator_server,
-  )
+
+  jax_global_state = jax._src.distributed.global_state  # pylint: disable=protected-access
+  if (
+      jax_global_state.coordinator_address
+      and jax_global_state.num_processes > 1
+  ):
+    ocdbt_address = _get_coordinator_address_without_port(
+        jax_global_state.coordinator_address
+    )
+
+    if jax_global_state.process_id == 0:
+      bind_address = f'{ocdbt_address}:0'
+      _OCDBT_COORDINATOR_SERVER = ts.ocdbt.DistributedCoordinatorServer(
+          {
+              'bind_addresses': [bind_address],
+          }
+      )
+      ocdbt_coordinator = f'{ocdbt_address}:{_OCDBT_COORDINATOR_SERVER.port}'
+      logging.info(
+          'Started OCDBT DistributedCoordinatorServer at: %s', ocdbt_coordinator
+      )
+      jax_global_state.client.key_value_set(
+          'ocdbt_coordinator', ocdbt_coordinator
+      )
+
+    ocdbt_address = jax_global_state.client.blocking_key_value_get(
+        'ocdbt_coordinator', _COORDINATOR_SETUP_TIMEOUT_SECS * 1000
+    )
+
+    # add ocdbt_coordinator spec into ts_context
+    ts_context['ocdbt_coordinator'] = {
+        'address': ocdbt_address,
+    }
+
+  _OCDBT_TS_CONTEXT = ts.Context(ts_context, parent=serialization.TS_CONTEXT)
+  _enable_ocdbt_for_handlers()
+  logging.info('OCDBT is initialized successfully.')
+
+
+def _use_ocdbt_for_restore(
+    maybe_use_ocdbt: bool, checkpoint_is_ocdbt: bool
+) -> bool:
+  """Determines whether the checkpoint should be restored using OCDBT."""
+  if not maybe_use_ocdbt and checkpoint_is_ocdbt:
+    raise ValueError(
+        'TypeHandler is not configured to allow OCDBT restoration, but found'
+        ' OCDBT checkpoint.'
+    )
+  return maybe_use_ocdbt and checkpoint_is_ocdbt
 
 
 async def _assert_parameter_files_exist(
     param_dir: epath.Path, metadata_key: Optional[str]
 ):
   """Checks for existence of parameter subdir and .zarray file."""
   exists = await utils.async_exists(param_dir)
@@ -130,14 +166,42 @@
   if not exists:
     raise FileNotFoundError(
         f'File not found: {metadata_path}. In many cases, this results from'
         ' copying a checkpoint without using the `-a` flag.'
     )
 
 
+def get_empty_value_typestr(value: Any) -> str:
+  if not utils.is_supported_empty_aggregation_type(value):
+    raise ValueError(f'{value} is not a supported empty aggregation type.')
+  if isinstance(value, list):
+    return 'List'
+  elif isinstance(value, dict):
+    return 'Dict'
+  elif isinstance(value, type(None)):
+    return 'None'
+  else:
+    raise ValueError(f'Unrecognized empty type: {value}.')
+
+
+def is_empty_typestr(typestr: str) -> bool:
+  return typestr == 'List' or typestr == 'Dict' or typestr == 'None'
+
+
+def get_empty_value_from_typestr(typestr: str) -> Any:
+  if typestr == 'List':
+    return []
+  elif typestr == 'Dict':
+    return {}
+  elif typestr == 'None':
+    return None
+  else:
+    raise ValueError(f'Unrecognized typestr: {typestr}.')
+
+
 @dataclasses.dataclass
 class ParamInfo:
   """Information describing a parameter in a PyTree.
 
   Note that ParamInfo is distinct from SaveArgs and RestoreArgs in that in
   represents information not provided by a user, and should be computed
   internally.
@@ -147,26 +211,30 @@
   path:
     A path providing a location where file(s) should be saved. The path is
     assumed to be a directory.
   skip_deserialize:
     If specified, skips deserialization of the given parameter using the
     TypeHandler. This may be for multiple different reasons, including that the
     parameter may have been aggregated, or it will be unneeded after
-    transformations.
+    transformations. Note: this parameter is handled by PyTreeCheckpointHandler,
+    so it is unnecessary for TypeHandler implementations to deal with it.
   byte_limiter:
     Object to limit the number of bytes that can be read in
     parallel.
   is_ocdbt_checkpoint:
     Indicates whether the checkpoint path uses OCDBT format
     or not. Only used for restoration.
   """
+
   name: Optional[str] = None
   path: Optional[epath.Path] = None
   skip_deserialize: Optional[bool] = None
-  byte_limiter: Optional[serialization._LimitInFlightBytes] = None  # pylint: disable=protected-access
+  byte_limiter: Optional[serialization._LimitInFlightBytes] = (
+      None  # pylint: disable=protected-access
+  )
   is_ocdbt_checkpoint: Optional[bool] = None
 
 
 @dataclasses.dataclass
 class SaveArgs:
   """Extra arguments that can be provided for saving.
 
@@ -174,14 +242,15 @@
     If true, saves the given parameter in an aggregated tree format
     rather than individually. See AggregateHandler.
   dtype:
     If provided, casts the parameter to the given dtype before saving.
     Note that the parameter must be compatible with the given type (e.g.
     jnp.bfloat16 is not compatible with np.ndarray).
   """
+
   aggregate: bool = False
   dtype: Optional[jnp.dtype] = None
 
 
 @dataclasses.dataclass
 class RestoreArgs:
   """Extra arguments that can be provided for restoration.
@@ -191,24 +260,46 @@
     must have a corresponding TypeHandler for restoration. Ignored if the
     parameter is restored from an aggregated checkpoint file.
   dtype:
     If provided, casts the parameter to the given dtype after restoring.
     Note that the parameter must be compatible with the given type (e.g.
     jnp.bfloat16 is not compatible with np.ndarray).
   """
-  # TODO(b/253238305) Consider deprecating this in favor of saving type
-  # information in checkpoint metadata.
-  restore_type: Any = np.ndarray
+
+  restore_type: Optional[Any] = None
   dtype: Optional[jnp.dtype] = None
 
 
 class TypeHandler(abc.ABC):
   """Interface for reading and writing a PyTree leaf."""
 
   @abc.abstractmethod
+  def typestr(self) -> str:
+    """A string representation of the type.
+
+    Cannot conflict with other types.
+
+    Returns:
+      The type as a string.
+    """
+    pass
+
+  @abc.abstractmethod
+  async def metadata(self, infos: Sequence[ParamInfo]) -> Sequence[Metadata]:
+    """Constructs object metadata from a stored parameter location.
+
+    Args:
+      infos: sequence of ParamInfo
+
+    Returns:
+      Sequence of Metadata for each provided ParamInfo.
+    """
+    pass
+
+  @abc.abstractmethod
   async def serialize(
       self,
       values: Sequence[Any],
       infos: Sequence[ParamInfo],
       args: Optional[Sequence[SaveArgs]] = None,
   ) -> Sequence[Future]:
     """Writes the parameter to a storage location.
@@ -312,14 +403,28 @@
       'max_inline_value_bytes': 1024,
       # Large value allows a single root node to support faster traversal.
       'max_decoded_node_bytes': 100000000,
   }
   return tspec
 
 
+def _array_metadata_from_tensorstore(t: Any) -> ArrayMetadata:
+  if t.chunk_layout.read_chunk.shape is None:
+    shards = None
+  else:
+    shards = tuple(
+        [int(s / c) for s, c in zip(t.shape, t.chunk_layout.read_chunk.shape)]
+    )
+  return ArrayMetadata(
+      shape=t.shape,
+      dtype=jnp.dtype(t.dtype.name),
+      shards=shards,
+  )
+
+
 class NumpyHandler(TypeHandler):
   """Provides an implementation of TypeHandler for replicated numpy arrays."""
 
   def __init__(
       self,
       metadata_key: Optional[str] = None,
       use_ocdbt: bool = False,
@@ -339,14 +444,18 @@
           'Must provide a ts.Context if use_ocdbt is True. Ensure that the'
           ' context contains a coordinator address.'
       )
     self._ts_context = ts_context or ts.Context(
         {'file_io_concurrency': {'limit': 128}}
     )
 
+  def enable_ocdbt(self, ts_context: ts.Context) -> None:
+    self._use_ocdbt = True
+    self._ts_context = ts_context
+
   def _get_json_tspec(
       self,
       info: ParamInfo,
       use_ocdbt: bool = False,
   ) -> Dict[str, Any]:
     """Gets Tensorstore spec in JSON format."""
     if info.path is None:
@@ -356,36 +465,51 @@
     if self._metadata_key is not None:
       tspec['metadata_key'] = self._metadata_key
     if use_ocdbt:
       tspec = _add_base_tspec_ocdbt_options(tspec)
     return tspec
 
   def _get_json_tspec_write(
-      self, info: ParamInfo, value: Any, use_ocdbt: bool = False
+      self, info: ParamInfo, value: np.ndarray, use_ocdbt: bool = False
   ) -> Dict[str, Any]:
     """Gets Tensorstore spec for writing."""
     tspec = self._get_json_tspec(info, use_ocdbt=use_ocdbt)
     tspec['metadata'] = {
-        'compressor': {
-            'id': 'zstd'
-        },
+        'compressor': {'id': 'zstd'},
     }
-    if value is not None:
-      tspec['metadata']['shape'] = value.shape
-      tspec['metadata']['chunks'] = value.shape
+    tspec['metadata']['shape'] = value.shape
+    tspec['metadata']['chunks'] = value.shape
     if use_ocdbt:
       tspec = _add_write_tspec_ocdbt_options(tspec)
     return tspec
 
   def _get_json_tspec_read(
       self, info: ParamInfo, use_ocdbt: bool = False
   ) -> Dict[str, Any]:
     """Gets Tensorstore spec for reading."""
     return self._get_json_tspec(info, use_ocdbt=use_ocdbt)
 
+  def typestr(self) -> str:
+    return 'np.ndarray'
+
+  async def metadata(self, infos: Sequence[ParamInfo]) -> Sequence[Metadata]:
+    open_ops = []
+    for info in infos:
+      # Using OCDBT, but existing checkpoint may be stored in old format.
+      use_ocdbt = _use_ocdbt_for_restore(
+          self._use_ocdbt, info.is_ocdbt_checkpoint
+      )
+      tspec = self._get_json_tspec_read(info, use_ocdbt=use_ocdbt)
+      open_ops.append(
+          ts.open(ts.Spec(tspec), open=True, context=self._ts_context)
+      )
+
+    tensorstores = await asyncio.gather(*open_ops)
+    return [_array_metadata_from_tensorstore(t) for t in tensorstores]
+
   async def serialize(
       self,
       values: Sequence[np.ndarray],
       infos: Sequence[ParamInfo],
       args: Optional[Sequence[SaveArgs]] = None,
   ) -> Sequence[Future]:
     """Uses Tensorstore to serialize a numpy array."""
@@ -424,28 +548,39 @@
     args = args or [RestoreArgs()] * len(infos)
     _check_input_arguments(infos, args)
     open_futures = []
     for info, arg in zip(infos, args):
       if not info.is_ocdbt_checkpoint:
         await _assert_parameter_files_exist(info.path, self._metadata_key)
       # Using OCDBT, but existing checkpoint may be stored in old format.
-      use_ocdbt = self._use_ocdbt and info.is_ocdbt_checkpoint
+      use_ocdbt = _use_ocdbt_for_restore(
+          self._use_ocdbt, info.is_ocdbt_checkpoint
+      )
       tspec = self._get_json_tspec_read(info, use_ocdbt=use_ocdbt)
       tspec = _get_cast_tspec_deserialize(tspec, arg)
       open_futures += [
           ts.open(ts.Spec(tspec), open=True, context=self._ts_context)
       ]
     tensorstores = await asyncio.gather(*open_futures)
     read_ops = [t.read() for t in tensorstores]
     return await asyncio.gather(*read_ops)
 
 
 class ScalarHandler(NumpyHandler):
-  """A wrapper around NumpyHandler to deal with scalar types (int, float, etc.).
-  """
+  """A wrapper around NumpyHandler to deal with scalar types (int, float, etc.)."""
+
+  def typestr(self) -> str:
+    return 'scalar'
+
+  async def metadata(self, infos: Sequence[ParamInfo]) -> Sequence[Metadata]:
+    metadatas = await super().metadata(infos)
+    return [
+        ScalarMetadata(dtype=typing.cast(ArrayMetadata, m).dtype)
+        for m in metadatas
+    ]
 
   async def serialize(
       self,
       values: Sequence[Scalar],  # pytype: disable=signature-mismatch
       infos: Sequence[ParamInfo],
       args: Optional[Sequence[SaveArgs]] = None,
   ) -> Sequence[Future]:
@@ -483,15 +618,15 @@
     provided, the shape will be restored as written. Presently, arbitrary shape
     transformations are not supported (for example, reshaping to different
     dimensions). Padding and truncating are supported. When the global_shape is
     greater than that of the saved array, 0's will be appended. If the
     global_shape is shorter than that of the saved array, excess elements will
     be dropped from the end of the array.
   """
-  restore_type: Any = jax.Array
+
   mesh: Optional[Mesh] = None
   mesh_axes: Optional[jax.sharding.PartitionSpec] = None
   sharding: Optional[jax.sharding.Sharding] = None
   global_shape: Optional[Tuple[int]] = None
 
 
 class ArrayHandler(TypeHandler):
@@ -517,14 +652,18 @@
           'Must provide a ts.Context if use_ocdbt is True. Ensure that the'
           ' context contains a coordinator address.'
       )
     self._ts_context = ts_context or ts.Context(
         {'file_io_concurrency': {'limit': 128}}
     )
 
+  def enable_ocdbt(self, ts_context: ts.Context) -> None:
+    self._use_ocdbt = True
+    self._ts_context = ts_context
+
   def _get_json_tspec(
       self,
       info: ParamInfo,
       use_ocdbt: bool = False,
   ) -> Dict[str, Any]:
     """Gets Tensorstore spec in JSON format."""
     if info.path is None:
@@ -550,14 +689,32 @@
 
   def _get_json_tspec_read(
       self, info: ParamInfo, use_ocdbt: bool = False
   ) -> Dict[str, Any]:
     """Gets Tensorstore spec for reading."""
     return self._get_json_tspec(info, use_ocdbt=use_ocdbt)
 
+  def typestr(self) -> str:
+    return 'jax.Array'
+
+  async def metadata(self, infos: Sequence[ParamInfo]) -> Sequence[Metadata]:
+    open_ops = []
+    for info in infos:
+      # Using OCDBT, but existing checkpoint may be stored in old format.
+      use_ocdbt = _use_ocdbt_for_restore(
+          self._use_ocdbt, info.is_ocdbt_checkpoint
+      )
+      tspec = self._get_json_tspec_read(info, use_ocdbt=use_ocdbt)
+      open_ops.append(
+          ts.open(ts.Spec(tspec), open=True, context=self._ts_context)
+      )
+
+    tensorstores = await asyncio.gather(*open_ops)
+    return [_array_metadata_from_tensorstore(t) for t in tensorstores]
+
   async def serialize(
       self,
       values: Sequence[jax.Array],
       infos: Sequence[ParamInfo],
       args: Optional[Sequence[SaveArgs]] = None,
   ) -> Sequence[Future]:
     """See superclass documentation."""
@@ -625,35 +782,44 @@
       if arg.sharding is None:
         sharding = jax.sharding.NamedSharding(arg.mesh, arg.mesh_axes)
       else:
         sharding = arg.sharding
       if not info.is_ocdbt_checkpoint:
         await _assert_parameter_files_exist(info.path, self._metadata_key)
       # Using OCDBT, but existing checkpoint may be stored in old format.
-      use_ocdbt = self._use_ocdbt and info.is_ocdbt_checkpoint
+      use_ocdbt = _use_ocdbt_for_restore(
+          self._use_ocdbt, info.is_ocdbt_checkpoint
+      )
       tspec = self._get_json_tspec_read(info, use_ocdbt=use_ocdbt)
       tspec = _get_cast_tspec_deserialize(tspec, arg)
       deserialize_ops += [
           serialization.async_deserialize(
               sharding,
               tspec,
               global_shape=arg.global_shape,
               byte_limiter=info.byte_limiter,
               context=self._ts_context,
           )
       ]
     return await asyncio.gather(*deserialize_ops)
 
 
+# TODO(b/285888834) Consider using Tensorstore JSON driver.
 class StringHandler(TypeHandler):
   """TypeHandler for strings."""
 
   def __init__(self, filename: Optional[str] = None):
     self._filename = filename or '_strings.json'
 
+  def typestr(self) -> str:
+    return 'string'
+
+  async def metadata(self, infos: Sequence[ParamInfo]) -> Sequence[Metadata]:
+    return [StringMetadata()] * len(infos)
+
   async def serialize(
       self,
       values: Sequence[str],
       infos: Sequence[ParamInfo],
       args: Optional[Sequence[SaveArgs]] = None,
   ) -> Sequence[Future]:
     """See superclass documentation."""
@@ -689,31 +855,40 @@
     (lambda ty: issubclass(ty, np.number), ScalarHandler()),
     (lambda ty: issubclass(ty, np.ndarray), NumpyHandler()),
     (lambda ty: issubclass(ty, jax.Array), ArrayHandler()),
     (lambda ty: issubclass(ty, str), StringHandler()),
 ]
 
 
-def register_type_handler(ty: Any,
-                          handler: TypeHandler,
-                          func: Optional[Callable[[Any], bool]] = None,
-                          override: bool = False):
+def _make_typestr_registry(type_registry: Any) -> Dict[str, TypeHandler]:
+  return {h.typestr(): h for _, h in type_registry}
+
+
+_TYPESTR_REGISTRY = _make_typestr_registry(_TYPE_REGISTRY)
+
+
+def register_type_handler(
+    ty: Any,
+    handler: TypeHandler,
+    func: Optional[Callable[[Any], bool]] = None,
+    override: bool = False,
+):
   """Registers a type for serialization/deserialization with a given handler.
 
   Note that it is possible for a type to match multiple different entries in
   the registry, each with a different handler. In this case, only the first
   match is used.
 
   Args:
     ty: A type to register.
     handler: a TypeHandler capable of reading and writing parameters of type
       `ty`.
     func: A function that accepts a type and returns True if the type should be
-      handled by the provided TypeHandler. If not specified, defaults to
-      `lambda t: issubclass(t, ty)`.
+      handled by the provided TypeHandler. If this parameter is not specified,
+      defaults to `lambda t: issubclass(t, ty)`.
     override: if True, will override an existing mapping of type to handler.
 
   Raises:
     ValueError if a type is already registered and override is False.
   """
   if func is None:
     func = lambda t: issubclass(t, ty)
@@ -723,36 +898,47 @@
     if f(ty):
       existing_handler_idx = i
       # Ignore the possibility for subsequent matches, as these will not be used
       # anyway.
       break
 
   if existing_handler_idx is None:
+    if handler.typestr() in _TYPESTR_REGISTRY:
+      raise ValueError(
+          f'Type "{ty}" has a `typestr` ("{handler.typestr()}") which collides'
+          ' with that of an existing TypeHandler.'
+      )
     _TYPE_REGISTRY.append((func, handler))
+    _TYPESTR_REGISTRY[handler.typestr()] = handler
   elif override:
     _TYPE_REGISTRY[existing_handler_idx] = (func, handler)
+    _TYPESTR_REGISTRY[handler.typestr()] = handler
   else:
     raise ValueError(f'A TypeHandler for "{ty}" is already registered.')
 
 
 def get_type_handler(ty: Any) -> TypeHandler:
   """Returns the handler registered for a given type, if available.
 
   Args:
-    ty: an object type.
+    ty: an object type (or string representation of the type.)
 
   Returns:
     The TypeHandler that is registered for the given type.
 
   Raises:
     ValueError if the given type has no registered handler.
   """
-  for func, handler in _TYPE_REGISTRY:
-    if func(ty):
-      return handler
+  if isinstance(ty, str):
+    if ty in _TYPESTR_REGISTRY:
+      return _TYPESTR_REGISTRY[ty]
+  else:
+    for func, handler in _TYPE_REGISTRY:
+      if func(ty):
+        return handler
   raise ValueError(f'Unknown type: "{ty}". Must register a TypeHandler.')
 
 
 def has_type_handler(ty: Any) -> bool:
   try:
     get_type_handler(ty)
     return True
@@ -775,7 +961,17 @@
       override=True,
   )
   register_type_handler(
       jax.Array,
       ArrayHandler(**kwargs),
       override=True,
   )
+
+
+# TODO(b/253238305) Deprecate when all checkpoints have saved types.
+def default_restore_type(args: RestoreArgs) -> Any:
+  if isinstance(args, ArrayRestoreArgs):
+    return jax.Array
+  elif isinstance(args, RestoreArgs):
+    return np.ndarray
+  else:
+    raise ValueError(f'Unsupported restore_args type: {type(args)}')
```

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/utils.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,19 +123,19 @@
     return key.name
   elif isinstance(key, jax.tree_util.FlattenedIndexKey):
     return key.key
   else:
     raise ValueError(f'Unsupported KeyEntry: {type(key)}: "{key}"')
 
 
-def _is_dict_key(key) -> bool:
+def is_dict_key(key) -> bool:
   return isinstance(key, (jax.tree_util.DictKey, jax.tree_util.GetAttrKey))
 
 
-def _is_sequence_key(key) -> bool:
+def is_sequence_key(key) -> bool:
   return isinstance(
       key, (jax.tree_util.FlattenedIndexKey, jax.tree_util.SequenceKey)
   )
 
 
 def _raise_unsupported_key_error(key):
   raise ValueError(f'Unsupported KeyEntry: {key}.')
@@ -144,14 +144,67 @@
 def _extend_list(ls, idx, nextvalue):
   assert idx <= len(ls)
   if idx == len(ls):
     ls.append(nextvalue)
   return ls
 
 
+def from_flattened_with_keypath(flat_with_keys: PyTree) -> PyTree:
+  """Reconstructs a tree given the a flat dict with keypaths."""
+  # Accesses the first path element (arbitrary), first tuple element
+  # (keypath tuple), first key in keypath (outermost key in the PyTree).
+  outerkey = flat_with_keys[0][0][0]
+  if is_dict_key(outerkey):
+    result = {}
+  elif is_sequence_key(outerkey):
+    result = []
+  else:
+    result = None
+    _raise_unsupported_key_error(outerkey)
+
+  for keypath, value in flat_with_keys:
+    subtree = result
+    for i, key in enumerate(keypath):
+      if i == 0:
+        assert isinstance(key, type(outerkey))
+      if i == len(keypath) - 1:
+        if is_dict_key(key):
+          assert isinstance(subtree, dict)
+          subtree[get_key_name(key)] = value
+        elif is_sequence_key(key):
+          assert isinstance(subtree, list)
+          idx = get_key_name(key)
+          subtree = _extend_list(subtree, idx, value)
+      else:
+        nextkey = keypath[i + 1]
+        if is_dict_key(nextkey):
+          nextvalue = {}
+        elif is_sequence_key(nextkey):
+          nextvalue = []
+        else:
+          nextvalue = None
+          _raise_unsupported_key_error(nextkey)
+
+        if is_dict_key(key):
+          assert isinstance(subtree, dict)
+          name = get_key_name(key)
+          if name not in subtree:
+            subtree[name] = nextvalue
+          subtree = subtree[name]
+        elif is_sequence_key(key):
+          assert isinstance(subtree, list)
+          idx = get_key_name(key)
+          subtree = _extend_list(subtree, idx, nextvalue)
+          subtree = subtree[idx]
+        else:
+          _raise_unsupported_key_error(key)
+
+  return result
+
+
 def to_flat_dict(
     tree: PyTree, sep: Optional[str] = None, keep_empty_nodes: bool = False
 ) -> PyTree:
   """Converts a tree into a flattened dictionary.
 
   The nested keys are flattened to a tuple.
 
@@ -195,63 +248,15 @@
 
   Returns:
     The serialized PyTree.
   """
   flat_with_keys, _ = jax.tree_util.tree_flatten_with_path(
       tree, is_leaf=is_empty_or_leaf if keep_empty_nodes else None
   )
-  # Accesses the first path element (arbitrary), first tuple element
-  # (keypath tuple), first key in keypath (outermost key in the PyTree).
-  outerkey = flat_with_keys[0][0][0]
-  if _is_dict_key(outerkey):
-    result = {}
-  elif _is_sequence_key(outerkey):
-    result = []
-  else:
-    result = None
-    _raise_unsupported_key_error(outerkey)
-
-  for keypath, value in flat_with_keys:
-    subtree = result
-    for i, key in enumerate(keypath):
-      if i == 0:
-        assert isinstance(key, type(outerkey))
-      if i == len(keypath) - 1:
-        if _is_dict_key(key):
-          assert isinstance(subtree, dict)
-          subtree[get_key_name(key)] = value
-        elif _is_sequence_key(key):
-          assert isinstance(subtree, list)
-          idx = get_key_name(key)
-          subtree = _extend_list(subtree, idx, value)
-      else:
-        nextkey = keypath[i + 1]
-        if _is_dict_key(nextkey):
-          nextvalue = {}
-        elif _is_sequence_key(nextkey):
-          nextvalue = []
-        else:
-          nextvalue = None
-          _raise_unsupported_key_error(nextkey)
-
-        if _is_dict_key(key):
-          assert isinstance(subtree, dict)
-          name = get_key_name(key)
-          if name not in subtree:
-            subtree[name] = nextvalue
-          subtree = subtree[name]
-        elif _is_sequence_key(key):
-          assert isinstance(subtree, list)
-          idx = get_key_name(key)
-          subtree = _extend_list(subtree, idx, nextvalue)
-          subtree = subtree[idx]
-        else:
-          _raise_unsupported_key_error(key)
-
-  return result
+  return from_flattened_with_keypath(flat_with_keys)
 
 
 def deserialize_tree(
     serialized: PyTree, target: PyTree, keep_empty_nodes: bool = False
 ) -> PyTree:
   """Deserializes a PyTree to the same structure as `target`."""
```

### Comparing `orbax_checkpoint-0.3.1/orbax/checkpoint/utils_test.py` & `orbax_checkpoint-0.3.2/orbax/checkpoint/utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/pyproject.toml` & `orbax_checkpoint-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.3.1/PKG-INFO` & `orbax_checkpoint-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbax-checkpoint
-Version: 0.3.1
+Version: 0.3.2
 Summary: Orbax Checkpoint
 Keywords: JAX machine learning,checkpoint,training
 Author-email: Orbax Authors <orbax-dev@google.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

