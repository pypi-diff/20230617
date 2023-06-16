# Comparing `tmp/orbax_checkpoint-0.2.5.tar.gz` & `tmp/orbax_checkpoint-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbax_checkpoint-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "orbax_checkpoint-0.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orbax_checkpoint-0.2.5.tar` & `orbax_checkpoint-0.2.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/LICENSE
--rw-r--r--   0        0        0      834 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/README.md
--rw-r--r--   0        0        0     2666 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/__init__.py
--rw-r--r--   0        0        0     2599 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/abstract_checkpointer.py
--rw-r--r--   0        0        0     2629 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/aggregate_handlers.py
--rw-r--r--   0        0        0     5348 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/array_checkpoint_handler.py
--rw-r--r--   0        0        0     1440 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/async_checkpoint_handler.py
--rw-r--r--   0        0        0     4744 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/async_checkpointer.py
--rw-r--r--   0        0        0     2119 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_handler.py
--rw-r--r--   0        0        0    35838 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_manager.py
--rw-r--r--   0        0        0     9920 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_utils.py
--rw-r--r--   0        0        0     7190 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_utils_test.py
--rw-r--r--   0        0        0     4022 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/checkpointer.py
--rw-r--r--   0        0        0      740 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/conftest.py
--rw-r--r--   0        0        0     1465 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/future.py
--rw-r--r--   0        0        0     2103 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/json_checkpoint_handler.py
--rw-r--r--   0        0        0     1821 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/json_checkpoint_handler_test.py
--rw-r--r--   0        0        0     2002 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/lazy_utils.py
--rw-r--r--   0        0        0     7672 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/msgpack_utils.py
--rw-r--r--   0        0        0     1129 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/msgpack_utils_test.py
--rw-r--r--   0        0        0    45137 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/orbax_checkpoint.ipynb
--rw-r--r--   0        0        0    23131 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/pytree_checkpoint_handler.py
--rw-r--r--   0        0        0     5333 2023-06-09 17:35:07.026293 orbax_checkpoint-0.2.5/orbax/checkpoint/test_utils.py
--rw-r--r--   0        0        0    10077 2023-06-09 17:35:07.030293 orbax_checkpoint-0.2.5/orbax/checkpoint/transform_utils.py
--rw-r--r--   0        0        0    15155 2023-06-09 17:35:07.030293 orbax_checkpoint-0.2.5/orbax/checkpoint/transform_utils_test.py
--rw-r--r--   0        0        0    23039 2023-06-09 17:35:07.030293 orbax_checkpoint-0.2.5/orbax/checkpoint/type_handlers.py
--rw-r--r--   0        0        0    22307 2023-06-09 17:35:07.030293 orbax_checkpoint-0.2.5/orbax/checkpoint/utils.py
--rw-r--r--   0        0        0     7465 2023-06-09 17:35:07.030293 orbax_checkpoint-0.2.5/orbax/checkpoint/utils_test.py
--rw-r--r--   0        0        0     1172 2023-06-09 17:35:07.030293 orbax_checkpoint-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 orbax_checkpoint-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 23:05:04.046330 orbax_checkpoint-0.2.6/LICENSE
+-rw-r--r--   0        0        0      834 2023-06-16 23:05:04.046330 orbax_checkpoint-0.2.6/README.md
+-rw-r--r--   0        0        0     2666 2023-06-16 23:05:04.046330 orbax_checkpoint-0.2.6/orbax/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2599 2023-06-16 23:05:04.046330 orbax_checkpoint-0.2.6/orbax/checkpoint/abstract_checkpointer.py
+-rw-r--r--   0        0        0     3106 2023-06-16 23:05:04.046330 orbax_checkpoint-0.2.6/orbax/checkpoint/aggregate_handlers.py
+-rw-r--r--   0        0        0     5727 2023-06-16 23:05:04.046330 orbax_checkpoint-0.2.6/orbax/checkpoint/array_checkpoint_handler.py
+-rw-r--r--   0        0        0     1440 2023-06-16 23:05:04.046330 orbax_checkpoint-0.2.6/orbax/checkpoint/async_checkpoint_handler.py
+-rw-r--r--   0        0        0     4744 2023-06-16 23:05:04.046330 orbax_checkpoint-0.2.6/orbax/checkpoint/async_checkpointer.py
+-rw-r--r--   0        0        0     2119 2023-06-16 23:05:04.046330 orbax_checkpoint-0.2.6/orbax/checkpoint/checkpoint_handler.py
+-rw-r--r--   0        0        0    36142 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/checkpoint_manager.py
+-rw-r--r--   0        0        0    12622 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/checkpoint_utils.py
+-rw-r--r--   0        0        0     8143 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/checkpoint_utils_test.py
+-rw-r--r--   0        0        0     4022 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/checkpointer.py
+-rw-r--r--   0        0        0      740 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/conftest.py
+-rw-r--r--   0        0        0     1576 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/future.py
+-rw-r--r--   0        0        0     2103 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/json_checkpoint_handler.py
+-rw-r--r--   0        0        0     1821 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/json_checkpoint_handler_test.py
+-rw-r--r--   0        0        0     2002 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/lazy_utils.py
+-rw-r--r--   0        0        0     7672 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/msgpack_utils.py
+-rw-r--r--   0        0        0     1129 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/msgpack_utils_test.py
+-rw-r--r--   0        0        0    45137 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/orbax_checkpoint.ipynb
+-rw-r--r--   0        0        0    24056 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/pytree_checkpoint_handler.py
+-rw-r--r--   0        0        0     5333 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/test_utils.py
+-rw-r--r--   0        0        0    10232 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/transform_utils.py
+-rw-r--r--   0        0        0    15155 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/transform_utils_test.py
+-rw-r--r--   0        0        0    23190 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/type_handlers.py
+-rw-r--r--   0        0        0    22603 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/utils.py
+-rw-r--r--   0        0        0     7465 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/orbax/checkpoint/utils_test.py
+-rw-r--r--   0        0        0     1172 2023-06-16 23:05:04.050330 orbax_checkpoint-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 orbax_checkpoint-0.2.6/PKG-INFO
```

### Comparing `orbax_checkpoint-0.2.5/LICENSE` & `orbax_checkpoint-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/README.md` & `orbax_checkpoint-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/__init__.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,8 @@
 # Convenient shorthand where instead of the following:
 #   `checkpointer = Checkpointer(PyTreeCheckpointer())`
 # we can just use:
 #   `checkpointer = PyTreeCheckpointer()`
 PyTreeCheckpointer = functools.partial(Checkpointer, PyTreeCheckpointHandler())
 
 # A new PyPI release will be pushed everytime `__version__` is increased.
-__version__ = '0.2.5'
+__version__ = '0.2.6'
```

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/abstract_checkpointer.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/abstract_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/aggregate_handlers.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/aggregate_handlers.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,29 +11,34 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Provides definitions for AggregateHandler and implementations."""
 
 import abc
+from concurrent import futures
+import functools
 from typing import Any
 
 from etils import epath
 import jax
+from orbax.checkpoint import future as orbax_future
 from orbax.checkpoint import msgpack_utils
 from orbax.checkpoint import utils
 
 PyTree = Any
 
 
 class AggregateHandler(abc.ABC):
   """Interface for reading and writing a PyTree using a specific format."""
 
   @abc.abstractmethod
-  async def serialize(self, path: epath.Path, item: PyTree):
+  async def serialize(
+      self, path: epath.Path, item: PyTree
+  ) -> orbax_future.Future:
     """Serializes and writes `item` to a given `path`.
 
     The function is compatible with a multihost setting, but does not include
     extra logic to ensure atomicity.
 
     Args:
       path: the folder to which the item should be written.
@@ -47,20 +52,32 @@
     pass
 
 
 class MsgpackHandler(AggregateHandler):
   """An implementation of AggregateHandler that uses msgpack to store the tree.
   """
 
-  async def serialize(self, path: epath.Path, item: PyTree):
+  def __init__(self):
+    self._executor = futures.ThreadPoolExecutor(max_workers=1)
+
+  async def serialize(
+      self, path: epath.Path, item: PyTree
+  ) -> orbax_future.Future:
     """See superclass documentation."""
-    if jax.process_index() == 0:
-      serializable_dict = utils.serialize_tree(item, keep_empty_nodes=True)
-      msgpack = msgpack_utils.msgpack_serialize(serializable_dict)
-      await utils.async_write_bytes(path, msgpack)
+
+    def _serialize_fn(x):
+      if jax.process_index() == 0:
+        serializable_dict = utils.serialize_tree(x, keep_empty_nodes=True)
+        msgpack = msgpack_utils.msgpack_serialize(serializable_dict)
+        # Explicit "copy" phase is not needed because msgpack only contains
+        # basic types and numpy arrays.
+        return path.write_bytes(msgpack)
+      return 0
+
+    return self._executor.submit(functools.partial(_serialize_fn, item))
 
   def deserialize(self, path: epath.Path) -> PyTree:
     """See superclass documentation."""
     if path.exists():
       msgpack = path.read_bytes()
       return msgpack_utils.msgpack_restore(msgpack)
     else:
```

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/array_checkpoint_handler.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/array_checkpoint_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,14 +134,22 @@
 
     if (directory / self._checkpoint_name).is_file():
       aggregate_handler = aggregate_handlers.get_aggregate_handler()
       result = aggregate_handler.deserialize(directory / self._checkpoint_name)
       result = result[_ELEMENT_KEY]
       if not self._is_supported_type(result):
         raise TypeError(f'Unsupported type: {type(result)}.')
+      if isinstance(restore_args, type_handlers.ArrayRestoreArgs):
+        result = result.reshape(restore_args.global_shape)
+        sharding = restore_args.sharding or jax.sharding.NamedSharding(
+            restore_args.mesh, restore_args.mesh_axes
+        )
+        result = jax.make_array_from_callback(
+            result.shape, sharding, lambda idx: result[idx]
+        )
     else:
       info = type_handlers.ParamInfo(
           name=self._checkpoint_name,
           path=directory / self._checkpoint_name,
           aggregate=False,
       )
       type_handler = type_handlers.get_type_handler(restore_args.restore_type)
```

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/async_checkpoint_handler.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/async_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/async_checkpointer.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/async_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_handler.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_manager.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/checkpoint_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from orbax.checkpoint.checkpointer import Checkpointer
 from orbax.checkpoint.json_checkpoint_handler import JsonCheckpointHandler
 
 PyTree = Any
 CheckpointDirs = Tuple[str, str]
 SaveParams = Mapping[str, Any]
 RestoreParams = SaveParams
+CheckpointersDict = Mapping[str, AbstractCheckpointer]
 
 DEFAULT_ITEM_NAME = 'default'
 DESCRIPTOR_ITEM_NAME = 'descriptor'
 METRIC_ITEM_NAME = 'metrics'
 METADATA_ITEM_NAME = 'metadata'
 
 RESERVED_ITEM_NAMES = [DESCRIPTOR_ITEM_NAME, METRIC_ITEM_NAME]
@@ -81,49 +82,61 @@
     return checkpointer.save(*args, **kwargs)
 
 
 @dataclasses.dataclass
 class CheckpointManagerOptions:
   """Optional arguments for CheckpointManager.
 
-  save_interval_steps: the interval at which checkpoints should be saved.
-  Ensures checkpoints will only be saved every n steps. Defaults to 1.
-  max_to_keep: if provided, specifies the maximum number of checkpoints to
+  save_interval_steps:
+    The interval at which checkpoints should be saved.
+    Ensures checkpoints will only be saved every n steps. Defaults to 1.
+  max_to_keep:
+    If provided, specifies the maximum number of checkpoints to
     keep. Older checkpoints are removed. By default, does not remove any old
     checkpoints. Must be None or non-negative. When set, checkpoints
     may be considered for deletion when there are more than `max_to_keep`
     checkpoints present. Checkpoints are kept if they meet any of the conditions
     below, such as `keep_time_interval`, `keep_period`, etc. Any remaining
     checkpoints that do not meet these conditions are garbage-collected.
-  keep_time_interval: When more than max_to_keep checkpoints are present,
+  keep_time_interval:
+    When more than max_to_keep checkpoints are present,
     an older checkpoint that would ordinarily be deleted will be preserved if it
     has been at least `keep_time_interval` since the previous preserved
     checkpoint. The default setting of `None` does not preserve any checkpoints
     in this way. For example, this may be used to ensure checkpoints are
     retained at a frequency of approximately than one per hour.
-  keep_period: If set, will not delete any checkpoint where checkpoint_step %
+  keep_period:
+    If set, will not delete any checkpoint where checkpoint_step %
     keep_period == 0.
-  best_fn: if set, maintains checkpoints based on the quality of given
+  best_fn:
+    If set, maintains checkpoints based on the quality of given
     metrics rather than recency. The function should accept a PyTree of metrics,
     and return a scalar value that can be used to determine the quality score
     of the checkpoint. If `max_to_keep` is also set, then the retained
     checkpoints will be kept based on their quality, as measured by this
     function.
-  best_mode: one of ['max', 'min']. The best metric is determine on the basis of
-    this value.
-  keep_checkpoints_without_metrics: If False, checkpoints with metrics present
+  best_mode:
+    One of ['max', 'min']. The best metric is determine on the basis of this
+    value.
+  keep_checkpoints_without_metrics:
+    If False, checkpoints with metrics present
     are eligible for cleanup. Otherwise, they will never be deleted.
-  step_prefix: if provided, step directories will take the form
+  step_prefix:
+    If provided, step directories will take the form
     f'{step_prefix}_<step>'. Otherwise, they will simply be an integer <step>.
-  step_format_fixed_length: If set, formats step with n digits (leading zeros).
+  step_format_fixed_length:
+    If set, formats step with n digits (leading zeros).
     This makes sorting steps easier. Otherwise, step has no leading zeros.
-  create: if True, creates the top-level directory if it does not already exist.
-  cleanup_tmp_directories: if True, cleans up any existing temporary directories
+  create:
+    If True, creates the top-level directory if it does not already exist.
+  cleanup_tmp_directories:
+    If True, cleans up any existing temporary directories
     on CheckpointManager creation.
-  save_on_steps: Optional set of steps at which checkpoints should be saved.
+  save_on_steps:
+    Optional set of steps at which checkpoints should be saved.
     Useful to save checkpoints on a fixed set of steps that are not multiple of
     `save_interval_steps`.
   """
   save_interval_steps: int = 1
   max_to_keep: Optional[int] = None
   keep_time_interval: Optional[datetime.timedelta] = None
   keep_period: Optional[int] = None
@@ -161,56 +174,56 @@
 
 
 class CheckpointManager:
   """A generic, synchronous CheckpointManager implementation.
 
   Allows a user to save and restore objects for which a Checkpointer
   implementation exists (e.g. PyTreeCheckpointer for PyTrees). The class
-  keeps track of multiple checkpointable objects in the following structure:
+  keeps track of multiple checkpointable objects in the following structure::
 
-  path/to/directory/    (top-level directory)
-    0/    (step)
-      params/    (first saveable)
+    path/to/directory/    (top-level directory)
+      0/    (step)
+        params/    (first saveable)
+          ...
+        metadata/    (second saveable)
+          ...
+      1/    (step)
         ...
-      metadata/    (second saveable)
+      2/    (step)
         ...
-    1/    (step)
       ...
-    2/    (step)
-      ...
-    ...
   """
 
   def __init__(
       self,
       directory: epath.PathLike,
-      checkpointers: Union[AbstractCheckpointer, Mapping[str,
-                                                         AbstractCheckpointer]],
+      checkpointers: Union[AbstractCheckpointer, CheckpointersDict],
       options: Optional[CheckpointManagerOptions] = None,
       metadata: Optional[Mapping[str, Any]] = None,
   ):
     """CheckpointManager constructor.
 
-    Ex:
-    CheckpointManager(
+    Example::
+
+      CheckpointManager(
         'path/to/dir/',
         # Multiple items.
         checkpointers = {
             'train_state': AsyncCheckpointer(PyTreeCheckpointHandler()),
-            'dataset': Checkpointer(CustomTFDatasetCheckpointHandler())
+            'dataset': Checkpointer(CustomTFDatasetCheckpointHandler()),
         },
         metadata={'version': 1.1, 'lang': 'en'},
-    )
+      )
 
-    CheckpointManager(
+      CheckpointManager(
         'path/to/dir/',
         # Single item.
         checkpointers = AsyncCheckpointer(PyTreeCheckpointHandler()),
         options = CheckpointManagerOptions(max_to_keep=5, ...),
-    )
+      )
 
     Args:
       directory: the top level directory in which to save all files.
       checkpointers: a mapping of object name to Checkpointer object. For
         example, `items` provided to `save` below should have keys matching the
         keys in this argument. Alternatively, a single Checkpointer may be
         provided, in which case `save` and `restore` should always be called
@@ -394,30 +407,32 @@
     This method should be called by all hosts - process synchronization and
     actions that need to be performed on only one host are managed internally.
 
     Items and save_kwargs must have a top-level structure matching that of
     self._checkpointers, meaning that for every key in items and save_kwargs, a
     corresponding key must be present in self._checkpointers.
 
-    Items takes a form similar to the following:
-    {
-      'params': PyTree(),
-      'metadata': <nested k/v>,
-      ...
-    }
-    Similarly, save_kwargs takes the form:
-    {
-      'params': {
-        <kwargs for PyTreeCheckpointHandler.save>
-      },
-      'metadata': {
-        <kwargs for JsonCheckpointHandler.save>
+    Items takes a form similar to the following::
+
+      {
+        'params': PyTree(),
+        'metadata': <nested k/v>,
+        ...
       }
-      ...
-    }
+      Similarly, save_kwargs takes the form:
+      {
+        'params': {
+          <kwargs for PyTreeCheckpointHandler.save>
+        },
+        'metadata': {
+          <kwargs for JsonCheckpointHandler.save>
+        }
+        ...
+      }
+
     The kwargs under 'params' correspond to PyTreeCheckpointHandler.save. If a
     key is not present in save_kwargs, it is assumed that no kwargs are needed
     for saving that item. If not provided at all, it is assumed that no items
     need extra kwargs for saving.
 
     Note that if a single Checkpointer was provided at construction time,
     `items` must be a singular saveable object, and `save_kwargs` must be the
@@ -511,37 +526,41 @@
     actions that need to be performed on only one host are managed internally.
 
     Items and restore_kwargs must have a top-level structure matching that of
     self._checkpointers, meaning that for every key in items and restore_kwargs,
     a
     corresponding key must be present in self._checkpointers.
 
-    Items takes a form similar to the following:
-    {
-      'params': PyTree(),
-      'metadata': <nested k/v>,
-      ...
-    }
+    Items takes a form similar to the following::
+
+      {
+        'params': PyTree(),
+        'metadata': <nested k/v>,
+        ...
+      }
+
     Items may not be provided at all, in which case it the items restored are
     those specified in self._checkpointers, and item=None is provided to
     Checkpointer.restore. Similarly, an item may be omitted from `items`,
     in
     which case item=None will be provided to Checkpointer.restore.
 
-    Similarly, restore_kwargs takes the form:
-    {
-      'params': {
-        'meshes': PyTree(),
-        'mesh_axes': PyTree(),
-      },
-      'metadata': {
-        <kwargs for JsonCheckpointHandler.save>
+    Similarly, restore_kwargs takes the form::
+
+      {
+        'params': {
+          'meshes': PyTree(),
+          'mesh_axes': PyTree(),
+        },
+        'metadata': {
+          <kwargs for JsonCheckpointHandler.save>
+        }
+        ...
       }
-      ...
-    }
+
     The kwargs under 'params' correspond to PyTreeCheckpointHandler.restore. If
     a key is not present in restore_kwargs, it is assumed that no kwargs are
     needed for restoring that item. If not provided at all, it is assumed that
     no items need extra kwargs for restoring.
 
     Note that if a single Checkpointer was provided at construction time,
     `items` must be a singular saveable object, and `restore_kwargs` must be the
@@ -805,14 +824,19 @@
     else:
       all_checkpoints = checkpoints_without_metrics + sorted_checkpoints
       maybe_delete = all_checkpoints[:-keep] if keep > 0 else sorted_checkpoints
       active_checkpoints = all_checkpoints[-keep:] if keep > 0 else []
 
     kept_checkpoints = []
     for info in maybe_delete:
+      if utils.is_locked(self.directory, info.step):
+        logging.info(
+            'Preserving %s: (Reason: checkpoint is locked).',
+            info,
+        )
       if (
           self._options.keep_time_interval is not None
           and self._interval_preserved_checkpoints
       ):
         if info in self._interval_preserved_checkpoints:
           logging.info(
               'Preserving %s: (Reason: older falling on keep_time_interval).',
```

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_utils.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/checkpoint_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,69 +9,137 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """High-level checkpoint utils provided for user convenience."""
+import contextlib
 import time
-from typing import Any, Iterator, Optional
+from typing import Any, Callable, Iterator, Optional
 
 from absl import logging
 from etils import epath
 import jax
 from jax.experimental import multihost_utils
-from jax.sharding import Mesh
 import numpy as np
 from orbax.checkpoint import type_handlers
 from orbax.checkpoint import utils
 
 
 PyTree = Any
 
 
+def _lock_checkpoint(checkpoint_dir: epath.Path, step: int) -> bool:
+  """Locks a checkpoint by writing a LOCKED directory."""
+  lockdir = utils.lockdir(checkpoint_dir, step)
+  try:
+    lockdir.mkdir(parents=False, exist_ok=True)
+    return True
+  except FileNotFoundError:
+    logging.info(
+        'Checkpoint step: %d was cleaned up while attempting to lock.', step
+    )
+    return False
+
+
+def _unlock_checkpoint(checkpoint_dir: epath.Path, step: int):
+  """Removes a LOCKED directory to indicate unlocking."""
+  utils.lockdir(checkpoint_dir, step).rmdir()
+
+
+def _unlock_existing_checkpoints(checkpoint_dir: epath.Path):
+  """Removes LOCKED file for all existing steps, if present."""
+  steps = utils.checkpoint_steps(checkpoint_dir)
+  for step in steps:
+    if utils.is_locked(checkpoint_dir, step):
+      _unlock_checkpoint(checkpoint_dir, step)
+
+
 def _wait_for_new_checkpoint(
     checkpoint_dir: epath.Path,
     last_checkpoint_step: Optional[int],
     seconds_to_sleep: int = 1,
     timeout: Optional[int] = None,
-) -> Optional[int]:
+) -> int:
   """Waits until a new checkpoint file is found.
 
   Args:
     checkpoint_dir: The directory in which checkpoints are saved.
     last_checkpoint_step: The last checkpoint step used or `None` if we're
       expecting a checkpoint for the first time.
     seconds_to_sleep: The number of seconds to sleep for before looking for a
       new checkpoint.
     timeout: The maximum number of seconds to wait. If left as `None`, then the
       process will wait indefinitely.
 
   Returns:
-    a new checkpoint step, or None if the timeout was reached.
+    a new checkpoint step, or -1 if the timeout was reached.
   """
   logging.info('Waiting for new checkpoint at %s', checkpoint_dir)
-  stop_time = time.time() + timeout if timeout is not None else None
-  while True:
-    steps = utils.checkpoint_steps(checkpoint_dir)
-    checkpoint_step = max(steps) if steps else None
-    if checkpoint_step is None or checkpoint_step == last_checkpoint_step:
-      if stop_time is not None and time.time() + seconds_to_sleep > stop_time:
-        return None
-      time.sleep(seconds_to_sleep)
-    else:
-      logging.info('Found new checkpoint step: %d', checkpoint_step)
-      return checkpoint_step
+  result = -1
+  if jax.process_index() == 0:
+    stop_time = time.time() + timeout if timeout is not None else None
+    while True:
+      steps = utils.checkpoint_steps(checkpoint_dir)
+      checkpoint_step = max(steps) if steps else None
+      if checkpoint_step is None or checkpoint_step == last_checkpoint_step:
+        if stop_time is not None and time.time() + seconds_to_sleep > stop_time:
+          break
+        time.sleep(seconds_to_sleep)
+      else:
+        if not _lock_checkpoint(checkpoint_dir, checkpoint_step):
+          continue
+        logging.info('Found new checkpoint step: %d', checkpoint_step)
+        result = checkpoint_step
+        break
+  return multihost_utils.broadcast_one_to_all(np.int32(result))
+
+
+@contextlib.contextmanager
+def wait_for_new_checkpoint(
+    checkpoint_dir: epath.Path,
+    last_checkpoint_step: Optional[int],
+    seconds_to_sleep: int = 1,
+    timeout: Optional[int] = None,
+):
+  """Waits until a new checkpoint file is found.
+
+  Automatically locks any checkpoint that is returned, and unlocks the
+  checkpoint when execution returns to this function.
+
+  Args:
+    checkpoint_dir: The directory in which checkpoints are saved.
+    last_checkpoint_step: The last checkpoint step used or `None` if we're
+      expecting a checkpoint for the first time.
+    seconds_to_sleep: The number of seconds to sleep for before looking for a
+      new checkpoint.
+    timeout: The maximum number of seconds to wait. If left as `None`, then the
+      process will wait indefinitely.
+
+  Yields:
+    a new checkpoint step, or -1 if the timeout was reached.
+  """
+  step = _wait_for_new_checkpoint(
+      checkpoint_dir, last_checkpoint_step, seconds_to_sleep, timeout
+  )
+  try:
+    yield step
+  finally:
+    # Release lock on the checkpoint step.
+    if step != -1:
+      _unlock_checkpoint(checkpoint_dir, step)
 
 
 def checkpoints_iterator(
     checkpoint_dir: epath.PathLike,
-    min_interval_secs=0,
-    timeout=None,
-    timeout_fn=None,
+    min_interval_secs: int = 0,
+    timeout: Optional[int] = None,
+    timeout_fn: Optional[Callable[[], bool]] = None,
+    unlock_existing_checkpoints: bool = True,
 ) -> Iterator[int]:
   """Continuously yield new checkpoint files as they appear.
 
   Based on the equivalent TF method.
 
   The iterator only checks for new checkpoints when control flow has been
   reverted to it. This means it can miss checkpoints if your code takes longer
@@ -106,53 +174,58 @@
     min_interval_secs: The minimum number of seconds between yielding
       checkpoints.
     timeout: The maximum number of seconds to wait between checkpoints. If left
       as `None`, then the process will wait indefinitely.
     timeout_fn: Optional function to call after a timeout.  If the function
       returns True, then it means that no new checkpoints will be generated and
       the iterator will exit.  The function is called with no arguments.
+    unlock_existing_checkpoints: If True, marks any existing checkpoints as
+      "unlocked", since these were most likely created by a failure during a
+      previous run, which left some checkpoints as "locked", despite not being
+      in use.
 
   Yields:
     Integer step numbers of the latest checkpoints as they arrive.
   """
   checkpoint_dir = epath.Path(checkpoint_dir)
+  if unlock_existing_checkpoints:
+    try:
+      _unlock_existing_checkpoints(checkpoint_dir)
+    except FileNotFoundError as e:
+      logging.warning(
+          'Encountered error while unlocking existing checkpoints. Some'
+          ' checkpoints may still be locked. %s.',
+          e,
+      )
   checkpoint_step = None
   while True:
-    new_checkpoint_step = 0
-    if jax.process_index() == 0:
-      new_checkpoint_step = (
-          _wait_for_new_checkpoint(
-              checkpoint_dir, checkpoint_step, timeout=timeout
-          )
-          or -1
-      )
-    new_checkpoint_step = multihost_utils.broadcast_one_to_all(
-        np.int32(new_checkpoint_step)
-    )
-    if new_checkpoint_step == -1:
-      if not timeout_fn:
-        logging.info('Timed-out waiting for a checkpoint.')
-        return
-      if timeout_fn():
-        # The timeout_fn indicated that we are truly done.
-        return
-      else:
-        # The timeout_fn indicated that more checkpoints may come.
-        continue
-    start = time.time()
-    checkpoint_step = new_checkpoint_step
-    yield checkpoint_step
+    with wait_for_new_checkpoint(
+        checkpoint_dir, checkpoint_step, timeout=timeout
+    ) as new_checkpoint_step:
+      if new_checkpoint_step == -1:
+        if not timeout_fn:
+          logging.info('Timed-out waiting for a checkpoint.')
+          return
+        if timeout_fn():
+          # The timeout_fn indicated that we are truly done.
+          return
+        else:
+          # The timeout_fn indicated that more checkpoints may come.
+          continue
+      start = time.time()
+      checkpoint_step = new_checkpoint_step
+      yield checkpoint_step
     time_to_next_eval = start + min_interval_secs - time.time()
     if time_to_next_eval > 0:
       time.sleep(time_to_next_eval)
 
 
 # TODO(b/274813763): Remove this function when no longer depended on by Flax.
 def restore_args_from_target(
-    mesh: Mesh, target: PyTree, axes_tree: PyTree
+    mesh: jax.sharding.Mesh, target: PyTree, axes_tree: PyTree
 ) -> PyTree:
   """DEPRECATED, DO NOT USE.
 
   Creates restore_args given a target PyTree.
 
   This method should be used in conjunction with a CheckpointManager or
   Checkpointer that wraps a PyTreeCheckpointHandler.
@@ -180,15 +253,15 @@
   ckptr.restore(..., restore_args=restore_args)
 
   If a leaf in target does is a np.ndarray, or int, or string, for example, a
   corresponding value for that leaf must be provided in axes_tree, but will be
   ignored.
 
   Args:
-    mesh: Mesh to shard arrays with.
+    mesh: jax.sharding.Mesh to shard arrays with.
     target: The returned value will match the structure of `target`, will be
       used to set the desired dtype and restoration shape.
     axes_tree: A PyTree matching `target` which will be used to set the
       restoration sharding.
 
   Returns:
     A PyTree matching target of RestoreArgs (or ArrayRestoreArgs) objects.
@@ -215,35 +288,35 @@
 
 def construct_restore_args(target: PyTree, sharding_tree: PyTree) -> PyTree:
   """Creates restore_args given a target PyTree.
 
   This method should be used in conjunction with a CheckpointManager or
   Checkpointer that wraps a PyTreeCheckpointHandler.
 
-  For example:
-
-  mngr = CheckpointManager(path, Checkpointer(PyTreeCheckpointHandler()))
-  restore_args = construct_restore_args(train_state, train_state_sharding)
-  restore_kwargs = {'restore_args': restore_args}
-  mngr.restore(..., restore_kwargs=restore_kwargs)
-
-  OR
+  For example::
 
-  mngr = CheckpointManager(path, {
-      'train_state': Checkpointer(PyTreeCheckpointHandler())
-  })
-  restore_args = construct_restore_args(train_state, train_state_sharding)
-  restore_kwargs = {'train_state': {'restore_args': restore_args} }
-  mngr.restore(..., restore_kwargs=restore_kwargs)
-
-  OR
-
-  ckptr = Checkpointer(PyTreeCheckpointHandler())
-  restore_args = construct_restore_args(train_state, train_state_sharding)
-  ckptr.restore(..., restore_args=restore_args)
+    mngr = CheckpointManager(path, Checkpointer(PyTreeCheckpointHandler()))
+    restore_args = construct_restore_args(train_state, train_state_sharding)
+    restore_kwargs = {'restore_args': restore_args}
+    mngr.restore(..., restore_kwargs=restore_kwargs)
+
+  OR::
+
+    mngr = CheckpointManager(path, {
+        'train_state': Checkpointer(PyTreeCheckpointHandler())
+    })
+    restore_args = construct_restore_args(train_state, train_state_sharding)
+    restore_kwargs = {'train_state': {'restore_args': restore_args} }
+    mngr.restore(..., restore_kwargs=restore_kwargs)
+
+  OR::
+
+    ckptr = Checkpointer(PyTreeCheckpointHandler())
+    restore_args = construct_restore_args(train_state, train_state_sharding)
+    ckptr.restore(..., restore_args=restore_args)
 
   If a leaf in target does is a np.ndarray, or int, or string, for example, a
   corresponding value for that leaf must be provided in axes_tree, but will be
   ignored.
 
   Args:
     target: The returned value will match the structure of `target`, will be
```

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/checkpoint_utils_test.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/checkpoint_utils_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -211,10 +211,38 @@
         checkpoint_utils.checkpoints_iterator(
             self.directory, timeout=0.1, timeout_fn=timeout_fn
         )
     )
     self.assertEqual([], results)
     self.assertEqual(4, timeout_fn_calls[0])
 
+  def test_locking(self):
+    max_step = 5
+    self.manager.save(0, self.items)
+    previous_step = None
+    for step in checkpoint_utils.checkpoints_iterator(
+        self.directory, timeout=0
+    ):
+      if previous_step is not None:
+        self.assertFalse(utils.is_locked(self.directory, previous_step))
+      self.assertTrue(utils.is_locked(self.directory, step))
+      previous_step = step
+
+      if step + 1 < max_step:
+        self.manager.save(step + 1, self.items)
+
+  def test_unlock_existing(self):
+    self.manager.save(0, self.items)
+    self.manager.save(1, self.items)
+
+    checkpoint_utils._lock_checkpoint(self.directory, 0)
+    self.assertTrue(utils.is_locked(self.directory, 0))
+    self.assertFalse(utils.is_locked(self.directory, 1))
+
+    for _ in checkpoint_utils.checkpoints_iterator(self.directory):
+      break
+    self.assertFalse(utils.is_locked(self.directory, 0))
+    self.assertFalse(utils.is_locked(self.directory, 1))
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/checkpointer.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/conftest.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/conftest.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/future.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/future.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,7 +30,14 @@
   completes. Importantly, calling `result` should not *start* execution of the
   future, but merely wait for an ongoing operation to complete.
   """
 
   def result(self, timeout: Optional[int] = None) -> Any:
     """Waits for the future to complete its operation."""
     ...
+
+
+class NoopFuture:
+
+  def result(self, timeout: Optional[int] = None) -> Any:
+    del timeout
+    return None
```

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/json_checkpoint_handler.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/json_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/json_checkpoint_handler_test.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/json_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/lazy_utils.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/lazy_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/msgpack_utils.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/msgpack_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/msgpack_utils_test.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/msgpack_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/orbax_checkpoint.ipynb` & `orbax_checkpoint-0.2.6/orbax/checkpoint/orbax_checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/pytree_checkpoint_handler.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/pytree_checkpoint_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,59 +309,74 @@
     self._concurrent_gb = concurrent_gb
     self._use_ocdbt = use_ocdbt
 
   def _get_param_names(self, item: PyTree) -> PyTree:
     """Gets parameter names for PyTree elements."""
     return _get_param_names(item)
 
-  def _get_param_infos(self, item: PyTree, directory: epath.Path,
-                       save_args: PyTree) -> PyTree:
+  def _get_param_infos(
+      self, item: PyTree, directory: epath.Path, save_args: PyTree
+  ) -> Tuple[PyTree, bool]:
     """Returns parameter information for elements in `item`.
 
     At minimum, this method should extract the names of each parameter for
     saving/restoring.
 
     Args:
       item: a PyTree to extract information from.
       directory: a directory where checkpoint files are located.
       save_args: PyTree matching item containing SaveArgs.
 
     Returns:
-      A PyTree matching `item` of ParamInfo.
+      A PyTree matching `item` of ParamInfo, and a bool indicating whether all
+      parameters were aggregated. The bool can enable us to skip some steps
+      later, potentially saving time.
     """
     if not item:
       raise ValueError('Found empty item')
     names = self._get_param_names(item)
+    all_params_aggregated = True
 
     def _param_info(name, args):
+      nonlocal all_params_aggregated
+      all_params_aggregated &= args.aggregate
       return ParamInfo(
           name=name, path=(directory / name), aggregate=args.aggregate)
 
-    return jax.tree_util.tree_map(_param_info, names, save_args)
+    return (
+        jax.tree_util.tree_map(_param_info, names, save_args),
+        all_params_aggregated,
+    )
 
-  async def _write_aggregate_file(self, directory: epath.Path, item: PyTree,
-                                  param_infos: PyTree, save_args: PyTree):
+  async def _write_aggregate_file(
+      self,
+      directory: epath.Path,
+      item: PyTree,
+      param_infos: PyTree,
+      save_args: PyTree,
+  ) -> Future:
     ser_item = _get_tree_for_aggregation(param_infos, save_args, item)
-    await self._aggregate_handler.serialize(
-        directory / self._aggregate_filename, ser_item)
+    return await self._aggregate_handler.serialize(
+        directory / self._aggregate_filename, ser_item
+    )
 
   async def async_save(
       self,
       directory: epath.Path,
       item: PyTree,
       save_args: Optional[PyTree] = None) -> Optional[List[Future]]:
     """Saves a PyTree from a given training step.
 
     This operation is compatible with a multi-host, multi-device setting. Tree
     leaf values must be supported by type_handlers. Standard supported types
     include scalars, np.ndarray, jax.Array, string.
 
-    After saving, all files will be located in directory/
+    After saving, all files will be located in "directory/".
 
-    Saves an additional file to directory/checkpoint on host 0 which
+    Saves an additional file to "directory/checkpoint" on host 0 which
     contains the serialized structure of `item`, along with any parameters that
     request aggregation.
 
     Args:
       directory: save location directory.
       item: a PyTree to be saved.
       save_args: a PyTree matching `item` which consists of SaveArgs objects as
@@ -377,16 +392,18 @@
     # all necessary arguments. These should be filled in with default args.
     save_args = jax.tree_util.tree_map(
         _maybe_set_default_save_args,
         item,
         item if save_args is None else save_args,
         is_leaf=utils.is_empty_or_leaf,
     )
-    param_infos = self._get_param_infos(item, directory, save_args)
-    if not self._use_ocdbt:
+    param_infos, all_params_aggregated = self._get_param_infos(
+        item, directory, save_args
+    )
+    if not self._use_ocdbt and not all_params_aggregated:
       # Create directories in parallel.
       await asyncio.gather(
           *jax.tree_util.tree_flatten(
               jax.tree_util.tree_map(
                   _create_param_save_dir, param_infos, save_args
               )
           )[0]
@@ -397,24 +414,34 @@
 
     async def serialize(value, info, args):
       if args.aggregate:
         return  # skip serialize now, include in aggregated file
       handler = type_handlers.get_type_handler(type(value))
       return await handler.serialize(value, info, args)
 
-    future_tree = jax.tree_util.tree_map(
-        serialize, item, param_infos, save_args, is_leaf=utils.is_empty_or_leaf
+    if all_params_aggregated:
+      commit_futures = []
+    else:
+      future_tree = jax.tree_util.tree_map(
+          serialize,
+          item,
+          param_infos,
+          save_args,
+          is_leaf=utils.is_empty_or_leaf,
+      )
+      copy_futures, _ = jax.tree_util.tree_flatten(future_tree)
+      assert isinstance(copy_futures, list)
+      # Await copy futures.
+      commit_futures = await asyncio.gather(*copy_futures)
+      commit_futures, _ = jax.tree_util.tree_flatten(commit_futures)
+
+    aggregate_commit_future = await self._write_aggregate_file(
+        directory, item, param_infos, save_args
     )
-    copy_futures, _ = jax.tree_util.tree_flatten(future_tree)
-    assert isinstance(copy_futures, list)
-    # Await copy futures.
-    commit_futures = await asyncio.gather(*copy_futures)
-    commit_futures, _ = jax.tree_util.tree_flatten(commit_futures)
-    await self._write_aggregate_file(directory, item, param_infos, save_args)
-    return commit_futures
+    return commit_futures + [aggregate_commit_future]
 
   def save(self, directory: epath.Path, item: Any, *args, **kwargs):
     """Saves the provided item.
 
     Blocks until both copy and commit complete.
 
     See async_save.
@@ -453,15 +480,24 @@
         info.aggregate is False.
 
     Returns:
       A LazyValue.
     """
 
     async def _maybe_cast(val: Any, args: RestoreArgs) -> Any:
-      return _try_array_cast(val, args.dtype)
+      val = _try_array_cast(val, args.dtype)
+      if isinstance(args, ArrayRestoreArgs):
+        val = val.reshape(args.global_shape)
+        sharding = args.sharding or jax.sharding.NamedSharding(
+            args.mesh, args.mesh_axes
+        )
+        val = jax.make_array_from_callback(
+            val.shape, sharding, lambda idx: val[idx]
+        )
+      return val
 
     async def _deserialize(info: ParamInfo, args: RestoreArgs) -> Any:
       handler = type_handlers.get_type_handler(args.restore_type)
       return await handler.deserialize(info, args)
 
     if param_info.aggregate:  # Already restored from AggregateHandler.
       get_fn = functools.partial(_maybe_cast, val=value)
```

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/test_utils.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/test_utils.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/transform_utils.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/transform_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,51 +29,56 @@
 
 
 @dataclasses.dataclass
 class Transform:
   r"""A representation of a transformation applied to pytree keys/values.
 
   See `apply_transformations` for usage examples. Transform represents an
-  operation on a single key/value pair. For example, the following mapping:
+  operation on a single key/value pair. For example, the following mapping::
 
-  {'a': Transform(original_key='b')}
+    {'a': Transform(original_key='b')}
 
   This denotes that the original key was named 'b', but we are changing it to
-  'a'. A regex can also be used as follows:
+  'a'. A regex can also be used as follows::
 
-  {r'(.*)a(.*)': Transform(original_key=r'\1b\2'}
+    {r'(.*)a(.*)': Transform(original_key=r'\1b\2'}
 
   This denotes that the key 'b' should be renamed to 'a'. This may apply to
   multiple different keys at different levels of nesting. The '/' character
   denotes a successive level of nesting.
 
-  We also have the following example:
+  We also have the following example::
 
-  {'a': Transform(multi_value_fn=lambda kv: kv['b'] * 2)}
+    {'a': Transform(multi_value_fn=lambda kv: kv['b'] * 2)}
 
   This signifies that the new key 'a' is the old key 'b' multiplied by two.
 
-  original_key: Denotes the original name of the key. Represented as a string
+  original_key:
+    Denotes the original name of the key. Represented as a string
     with '/' denoting successive levels of nesting. If the key corresponding to
     this Transform is a regex, backreferences (such as \1) will be replaced with
     the appropriate matched group in the regex. Note: not needed if
     multi_value_fn is provided.
-  use_fallback: if True, takes the value from the fallback tree. If
+  use_fallback:
+    If True, takes the value from the fallback tree. If
     `default_to_original=True` in `apply_transformations`, the fallback tree is
     `new_tree`. If `default_to_original=False` in `apply_transformations`, the
     fallback tree is `original_tree`.
-  value_fn: A function accepting a single value and returning a single value.
+  value_fn:
+    A function accepting a single value and returning a single value.
     The value provided as an argument is the value of the transformation key in
     the original PyTree.
-  multi_value_fn: A function accepting a string and PyTree and returning any
+  multi_value_fn:
+    A function accepting a string and PyTree and returning any
     value. The string is the result key associated with the returned value, so
     the function implementation can know for which key it is supposed to return
     a value for. The PyTree argument will be the original PyTree, and the
     function should return the value of the key in the new PyTree.
-  multi_value_fn_input_args: A dict of key name (in the original tree) to
+  multi_value_fn_input_args:
+    A dict of key name (in the original tree) to
     required input arguments (typically `RestoreArgs` - see
     `PyTreeCheckpointHandler`). These arguments are not used directly in
     `apply_transformations`, but are necessary when applying transformations
     when restoring from a checkpoint in `PyTreeCheckpointHandler`. These
     arguments identify "dependencies" in the original tree (the checkpoint)
     which are needed as inputs by the function, and provides additional
     information needed for restoration. IMPORTANT: using multi_value_fn during
@@ -115,77 +120,78 @@
                           transformations: PyTree,
                           new_tree: PyTree,
                           default_to_original: Optional[bool] = True) -> PyTree:
   r"""Applies transformations to a pytree.
 
   Also uses `transformations` to provide structure to the output tree.
 
-  Example:
+  Example::
 
-  original_tree = {
-    'a': 1,
-    'b': {
-      'c': 5,
-      'd': [0, 1, 2, 3]
-    },
-    'f': 2,
-    'b1': {
-      'c': 2,
-    },
-    'b2': {
-      'c': 3,
-    },
-  }
-  transformations = {
-    'a1': Transform(original_key='a'),  # rename
-    'a1': Transform(multi_value_fn=lambda kv: kv['a']),  # another way of doing
-    above
-    'b': {
-      'c': Transform(multi_value_fn=lambda kv: kv['b']['c'] * 2)  # doubled
-      original
-      # drop b/d
-    },
-     # Copy original into multiple new keys
-    'c1': Transform(original_key='b/c'),
-    'c2': Transform(original_key='b/c'),
-    # one to many mapping
-    'x': Transform(multi_value_fn=lambda kv: kv['b']['d'][0]),
-    'y': Transform(multi_value_fn=lambda kv: kv['b']['d'][1:]),
-    # many to one mapping
-    'z': Transform(multi_value_fn=lambda kv: kv['a'] * 2 + sum(kv['b']['d'])),
-    r'x(\d.*)': Transform(original_key=r'b\1')
-  }
-
-  # defines the structure of the result
-  new_tree = {
-    'a1': ...,
-    'a1': ...,
-    'b': {
-      'c': ...,
-    },
-    'c1': ...,
-    'c2': ...,
-    'x': ...,
-    'y': ...,
-    'z': ...,
-    # defined in original_tree and new_tree, but not in transforms. Value
-    carried over from original_tree.
-    'f': ...,
-    # This value matters since it is not present in original_tree or
-    transformations, so the value here will simply be preserved in the result.
-    'g': 5,
-    # These are just 'b1', 'b2', but renamed to 'x1', 'x2', with all values
-    copied over.
-    'x1': {
-      'c': 2,
+    original_tree = {
+      'a': 1,
+      'b': {
+        'c': 5,
+        'd': [0, 1, 2, 3]
+      },
+      'f': 2,
+      'b1': {
+        'c': 2,
+      },
+      'b2': {
+        'c': 3,
+      },
     }
-    'x2': {
-      'c': 3,
+    transformations = {
+      'a1': Transform(original_key='a'),  # rename
+      'a1': Transform(multi_value_fn=lambda kv: kv['a']),  # another way of
+      doing
+      above
+      'b': {
+        'c': Transform(multi_value_fn=lambda kv: kv['b']['c'] * 2)  # doubled
+        original
+        # drop b/d
+      },
+      # Copy original into multiple new keys
+      'c1': Transform(original_key='b/c'),
+      'c2': Transform(original_key='b/c'),
+      # one to many mapping
+      'x': Transform(multi_value_fn=lambda kv: kv['b']['d'][0]),
+      'y': Transform(multi_value_fn=lambda kv: kv['b']['d'][1:]),
+      # many to one mapping
+      'z': Transform(multi_value_fn=lambda kv: kv['a'] * 2 + sum(kv['b']['d'])),
+      r'x(\d.*)': Transform(original_key=r'b\1')
+    }
+
+    # defines the structure of the result
+    new_tree = {
+      'a1': ...,
+      'a1': ...,
+      'b': {
+        'c': ...,
+      },
+      'c1': ...,
+      'c2': ...,
+      'x': ...,
+      'y': ...,
+      'z': ...,
+      # defined in original_tree and new_tree, but not in transforms. Value
+      carried over from original_tree.
+      'f': ...,
+      # This value matters since it is not present in original_tree or
+      transformations, so the value here will simply be preserved in the result.
+      'g': 5,
+      # These are just 'b1', 'b2', but renamed to 'x1', 'x2', with all values
+      copied over.
+      'x1': {
+        'c': 2,
+      }
+      'x2': {
+        'c': 3,
+      }
     }
-  }
 
   Args:
     original_tree: a PyTree to be transformed.
     transformations: a PyTree of Transform objects.
     new_tree: a PyTree defining the structure of the output. A leaf value is
       only relevant if the key is not present in transformations or
       original_tree. Note: values in the provided tree must not be None, or they
```

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/transform_utils_test.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/transform_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/type_handlers.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/type_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,24 +52,26 @@
   """Creates OCDBT coordinator and Tensorstore context.
 
   This function must be called at the start of the program across all processes
   in order to initialize the OCDBT coordinator service. The coordinator object
   should be kept alive for the life of the program, while the returned
   ts.Context should be provided when saving or restoring using Tensorstore.
 
-  Example usage:
-  ```
-  ocdbt_context, coordinator_server = (
-      orbax.checkpoint.type_handlers.create_coordinator_server_and_context()
-  )
-  orbax.checkpoint.type_handlers.register_standard_handlers_with_options(
-      use_ocdbt=True, ts_context=ocdbt_context
-  )
-  orbax.checkpoint.utils.sync_global_devices('init_ocdbt_server')
-  ```
+  Example usage::
+
+    ocdbt_context, coordinator_server = (
+        orbax.checkpoint.type_handlers.create_coordinator_server_and_context()
+    )
+    orbax.checkpoint.type_handlers.register_standard_handlers_with_options(
+        use_ocdbt=True, ts_context=ocdbt_context
+    )
+    orbax.checkpoint.utils.sync_global_devices('init_ocdbt_server')
+
+  Later, when creating the `PyTreeCheckpointHandler`, initialize with
+  `use_ocdbt=True`.
 
   Returns:
     Tuple of ts.Context and OCDBT coordinator server object.
   """
   jax_global_state = jax._src.distributed.global_state  # pylint: disable=protected-access
   ocdbt_address = _get_coordinator_address_without_port(
       jax_global_state.coordinator_address
@@ -126,54 +128,64 @@
 class ParamInfo:
   """Information describing a parameter in a PyTree.
 
   Note that ParamInfo is distinct from SaveArgs and RestoreArgs in that in
   represents information not provided by a user, and should be computed
   internally.
 
-  name: name of the parameter.
-  path: A path providing a location where file(s) should be saved. The path is
+  name:
+    Name of the parameter.
+  path:
+    A path providing a location where file(s) should be saved. The path is
     assumed to be a directory.
-  aggregate: whether the parameter should be / was aggregated.
-  byte_limiter: object to limit the number of bytes that can be read in
+  aggregate:
+    Whether the parameter should be / was aggregated.
+  byte_limiter:
+    Object to limit the number of bytes that can be read in
     parallel.
-  is_ocdbt_checkpoint: indicates whether the checkpoint path uses OCDBT format
+  is_ocdbt_checkpoint:
+    Indicates whether the checkpoint path uses OCDBT format
     or not. Only used for restoration.
   """
   name: Optional[str] = None
   path: Optional[epath.Path] = None
   aggregate: Optional[bool] = None
   byte_limiter: Optional[serialization._LimitInFlightBytes] = None  # pylint: disable=protected-access
   is_ocdbt_checkpoint: Optional[bool] = None
 
 
 @dataclasses.dataclass
 class SaveArgs:
   """Extra arguments that can be provided for saving.
 
-  aggregate: if true, saves the given parameter in an aggregated tree format
+  aggregate:
+    If true, saves the given parameter in an aggregated tree format
     rather than individually. See AggregateHandler.
-  dtype: if provided, casts the parameter to the given dtype before saving.
+  dtype:
+    If provided, casts the parameter to the given dtype before saving.
     Note that the parameter must be compatible with the given type (e.g.
     jnp.bfloat16 is not compatible with np.ndarray).
   """
   aggregate: bool = False
   dtype: Optional[jnp.dtype] = None
 
 
 @dataclasses.dataclass
 class RestoreArgs:
   """Extra arguments that can be provided for restoration.
 
-  lazy: if True, restores using LazyArray. The actual read operation will not be
+  lazy:
+    If True, restores using LazyArray. The actual read operation will not be
     performed until `get` is called for the restored LazyArray.
-  restore_type: Specifies the object type of the restored parameter. The type
+  restore_type:
+    Specifies the object type of the restored parameter. The type
     must have a corresponding TypeHandler for restoration. Ignored if the
     parameter is restored from an aggregated checkpoint file.
-  dtype: if provided, casts the parameter to the given dtype after restoring.
+  dtype:
+    If provided, casts the parameter to the given dtype after restoring.
     Note that the parameter must be compatible with the given type (e.g.
     jnp.bfloat16 is not compatible with np.ndarray).
   """
   lazy: bool = False
   # TODO(b/253238305) Consider deprecating this in favor of saving type
   # information in checkpoint metadata.
   restore_type: Any = np.ndarray
@@ -396,20 +408,24 @@
     return result.item()
 
 
 @dataclasses.dataclass
 class ArrayRestoreArgs(RestoreArgs):
   """Arguments used when restoring with ArrayHandler.
 
-  mesh: the device mesh that the array should be restored as. Cannot be None.
-  mesh_axes: the mesh_axes that the array should be restored as. Cannot be None.
-  sharding: jax.sharding.Sharding object which takes precedence over mesh and
+  mesh:
+    The device mesh that the array should be restored as. Cannot be None.
+  mesh_axes:
+    The mesh_axes that the array should be restored as. Cannot be None.
+  sharding:
+    jax.sharding.Sharding object which takes precedence over mesh and
     mesh_axes if provided. Otherwise, mesh and mesh_axes will be used to
     construct a NamedSharding object.
-  global_shapes: the global shape that the array should be restored into. If not
+  global_shapes:
+    The global shape that the array should be restored into. If not
     provided, the shape will be restored as written. Presently, arbitrary shape
     transformations are not supported (for example, reshaping to different
     dimensions). Padding and truncating are supported. When the global_shape is
     greater than that of the saved array, 0's will be appended. If the
     global_shape is shorter than that of the saved array, excess elements will
     be dropped from the end of the array.
   """
```

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/utils.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 # individually. Typically, this may indicate an array that was written using
 # Tensorstore rather than its value being directly stored in the msgpack file.
 # To avoid duplication, we replace the value with a placeholder prefix and other
 # relevant information (see functions below).
 _PLACEHOLDER_PREFIX = 'PLACEHOLDER://'
 _COMMIT_SUCCESS_FILE = 'commit_success.txt'
 _GCS_PATH_PREFIX = 'gs://'
+_LOCK_ITEM_NAME = 'LOCKED'
 _LAST_CHECKPOINT_WRITE_TIME = time.time()
 CheckpointDirs = Tuple[str, str]
 PyTree = Any
 
 
 
 
@@ -613,24 +614,26 @@
       return step_from_checkpoint_name(s.name)
   return None
 
 
 def is_checkpoint_finalized(path: epath.PathLike) -> bool:
   """Determines if the given path represents a finalized checkpoint.
 
-   Path takes the form:
-  path/to/my/dir/<name>.orbax-checkpoint-tmp-<timestamp>/  # not finalized
-  path/to/my/dir/<name>/  # finalized
-
-  Alternatively:
-  gs://path/to/my/dir/<name>/  # finalized
-    commit_success.txt
-    ...
-  gs://<path/to/my/dir/<name>/  # not finalized
-    ...
+  Path takes the form::
+
+    path/to/my/dir/<name>.orbax-checkpoint-tmp-<timestamp>/  # not finalized
+    path/to/my/dir/<name>/  # finalized
+
+  Alternatively::
+
+    gs://path/to/my/dir/<name>/  # finalized
+      commit_success.txt
+      ...
+    gs://<path/to/my/dir/<name>/  # not finalized
+      ...
 
   Args:
     path: Directory.
 
   Returns:
     True if the checkpoint is finalized.
 
@@ -690,7 +693,15 @@
   sharding = jax.sharding.NamedSharding(
       jax.sharding.Mesh(np.array(jax.devices()), axis_names=('x',)),
       jax.sharding.PartitionSpec(None),
   )
   # pmap-produced Array has a "scrambled" device order.
   dbs = sorted(arr.device_buffers, key=lambda x: x.device().id)
   return jax.make_array_from_single_device_arrays(global_shape, sharding, dbs)
+
+
+def lockdir(checkpoint_dir: epath.Path, step: int) -> epath.Path:
+  return get_save_directory(step, checkpoint_dir, name=_LOCK_ITEM_NAME)
+
+
+def is_locked(checkpoint_dir: epath.Path, step: int) -> bool:
+  return lockdir(checkpoint_dir, step).exists()
```

### Comparing `orbax_checkpoint-0.2.5/orbax/checkpoint/utils_test.py` & `orbax_checkpoint-0.2.6/orbax/checkpoint/utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/pyproject.toml` & `orbax_checkpoint-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orbax_checkpoint-0.2.5/PKG-INFO` & `orbax_checkpoint-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbax-checkpoint
-Version: 0.2.5
+Version: 0.2.6
 Summary: Orbax Checkpoint
 Keywords: JAX machine learning,checkpoint,training
 Author-email: Orbax Authors <orbax-dev@google.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

