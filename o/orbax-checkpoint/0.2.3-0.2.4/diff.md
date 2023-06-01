# Comparing `tmp/orbax-checkpoint-0.2.3.tar.gz` & `tmp/orbax_checkpoint-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbax-checkpoint-0.2.3.tar", last modified: Fri May 12 16:00:53 2023, max compression
+gzip compressed data, was "orbax_checkpoint-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `orbax-checkpoint-0.2.3.tar` & `orbax_checkpoint-0.2.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/LICENSE
--rw-r--r--   0        0        0      699 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/README.md
--rw-r--r--   0        0        0     2564 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/orbax/checkpoint/__init__.py
--rw-r--r--   0        0        0     2599 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/orbax/checkpoint/abstract_checkpointer.py
--rw-r--r--   0        0        0     2629 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/orbax/checkpoint/aggregate_handlers.py
--rw-r--r--   0        0        0     5348 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/orbax/checkpoint/array_checkpoint_handler.py
--rw-r--r--   0        0        0     1440 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/orbax/checkpoint/async_checkpoint_handler.py
--rw-r--r--   0        0        0     4744 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/orbax/checkpoint/async_checkpointer.py
--rw-r--r--   0        0        0     2119 2023-05-12 16:00:14.403023 orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_handler.py
--rw-r--r--   0        0        0    34823 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_manager.py
--rw-r--r--   0        0        0     9920 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_utils.py
--rw-r--r--   0        0        0     7190 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_utils_test.py
--rw-r--r--   0        0        0     4022 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/checkpointer.py
--rw-r--r--   0        0        0      740 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/conftest.py
--rw-r--r--   0        0        0     1465 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/future.py
--rw-r--r--   0        0        0     2103 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/json_checkpoint_handler.py
--rw-r--r--   0        0        0     1821 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/json_checkpoint_handler_test.py
--rw-r--r--   0        0        0     2002 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/lazy_utils.py
--rw-r--r--   0        0        0     7672 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/msgpack_utils.py
--rw-r--r--   0        0        0     1129 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/msgpack_utils_test.py
--rw-r--r--   0        0        0    45137 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/orbax_checkpoint.ipynb
--rw-r--r--   0        0        0    22114 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/pytree_checkpoint_handler.py
--rw-r--r--   0        0        0     5234 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/test_utils.py
--rw-r--r--   0        0        0     9406 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/transform_utils.py
--rw-r--r--   0        0        0    13488 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/transform_utils_test.py
--rw-r--r--   0        0        0    23003 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/type_handlers.py
--rw-r--r--   0        0        0    21387 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/utils.py
--rw-r--r--   0        0        0     7444 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/orbax/checkpoint/utils_test.py
--rw-r--r--   0        0        0     1172 2023-05-12 16:00:14.407023 orbax-checkpoint-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1841 1970-01-01 00:00:00.000000 orbax-checkpoint-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-01 15:35:33.579835 orbax_checkpoint-0.2.4/LICENSE
+-rw-r--r--   0        0        0      834 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/README.md
+-rw-r--r--   0        0        0     2666 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/__init__.py
+-rw-r--r--   0        0        0     2599 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/abstract_checkpointer.py
+-rw-r--r--   0        0        0     2629 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/aggregate_handlers.py
+-rw-r--r--   0        0        0     5348 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/array_checkpoint_handler.py
+-rw-r--r--   0        0        0     1440 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/async_checkpoint_handler.py
+-rw-r--r--   0        0        0     4744 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/async_checkpointer.py
+-rw-r--r--   0        0        0     2119 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_handler.py
+-rw-r--r--   0        0        0    35205 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_manager.py
+-rw-r--r--   0        0        0     9920 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_utils.py
+-rw-r--r--   0        0        0     7190 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_utils_test.py
+-rw-r--r--   0        0        0     4022 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/checkpointer.py
+-rw-r--r--   0        0        0      740 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/conftest.py
+-rw-r--r--   0        0        0     1465 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/future.py
+-rw-r--r--   0        0        0     2103 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/json_checkpoint_handler.py
+-rw-r--r--   0        0        0     1821 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/json_checkpoint_handler_test.py
+-rw-r--r--   0        0        0     2002 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/lazy_utils.py
+-rw-r--r--   0        0        0     7672 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/msgpack_utils.py
+-rw-r--r--   0        0        0     1129 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/msgpack_utils_test.py
+-rw-r--r--   0        0        0    45137 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/orbax_checkpoint.ipynb
+-rw-r--r--   0        0        0    22735 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/pytree_checkpoint_handler.py
+-rw-r--r--   0        0        0     5333 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/test_utils.py
+-rw-r--r--   0        0        0    10077 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/transform_utils.py
+-rw-r--r--   0        0        0    15155 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/transform_utils_test.py
+-rw-r--r--   0        0        0    23039 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/type_handlers.py
+-rw-r--r--   0        0        0    21981 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/utils.py
+-rw-r--r--   0        0        0     7465 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/orbax/checkpoint/utils_test.py
+-rw-r--r--   0        0        0     1172 2023-06-01 15:35:33.587835 orbax_checkpoint-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 orbax_checkpoint-0.2.4/PKG-INFO
```

### Comparing `orbax-checkpoint-0.2.3/LICENSE` & `orbax_checkpoint-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/README.md` & `orbax_checkpoint-0.2.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Orbax Checkpointing
 
-`pip install orbax-checkpoint`
+`pip install orbax-checkpoint` (latest PyPi release) OR
+
+`pip install 'git+https://github.com/google/orbax/#subdirectory=checkpoint'` (from this repository, at HEAD)
 
 `import orbax.checkpoint`
 
 Orbax includes a checkpointing library oriented towards JAX users, supporting a
 variety of different features required by different frameworks, including
 asynchronous checkpointing, various types, and various storage formats.
 We aim to provide a highly customizable and composable API which maximizes
```

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/__init__.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import functools
 
 from orbax.checkpoint import aggregate_handlers
 from orbax.checkpoint import checkpoint_utils
 from orbax.checkpoint import lazy_utils
 from orbax.checkpoint import msgpack_utils
 from orbax.checkpoint import test_utils
+from orbax.checkpoint import transform_utils
 from orbax.checkpoint import type_handlers
 from orbax.checkpoint import utils
 from orbax.checkpoint.abstract_checkpointer import AbstractCheckpointer
 from orbax.checkpoint.array_checkpoint_handler import ArrayCheckpointHandler
 from orbax.checkpoint.async_checkpoint_handler import AsyncCheckpointHandler
 from orbax.checkpoint.async_checkpointer import AsyncCheckpointer
 from orbax.checkpoint.checkpoint_handler import CheckpointHandler
@@ -34,14 +35,15 @@
 from orbax.checkpoint.future import Future
 from orbax.checkpoint.json_checkpoint_handler import JsonCheckpointHandler
 from orbax.checkpoint.pytree_checkpoint_handler import ArrayRestoreArgs
 from orbax.checkpoint.pytree_checkpoint_handler import PyTreeCheckpointHandler
 from orbax.checkpoint.pytree_checkpoint_handler import RestoreArgs
 from orbax.checkpoint.pytree_checkpoint_handler import SaveArgs
 from orbax.checkpoint.transform_utils import apply_transformations
+from orbax.checkpoint.transform_utils import merge_trees
 from orbax.checkpoint.transform_utils import Transform
 
 try:
   __IPYTHON__
   _in_ipython_session = True
 except NameError:
   _in_ipython_session = False
@@ -52,8 +54,8 @@
 # Convenient shorthand where instead of the following:
 #   `checkpointer = Checkpointer(PyTreeCheckpointer())`
 # we can just use:
 #   `checkpointer = PyTreeCheckpointer()`
 PyTreeCheckpointer = functools.partial(Checkpointer, PyTreeCheckpointHandler())
 
 # A new PyPI release will be pushed everytime `__version__` is increased.
-__version__ = '0.2.3'
+__version__ = '0.2.4'
```

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/abstract_checkpointer.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/abstract_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/aggregate_handlers.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/aggregate_handlers.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/array_checkpoint_handler.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/array_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/async_checkpoint_handler.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/async_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/async_checkpointer.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/async_checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_handler.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_manager.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 
 """CheckpointManager, a sync implementation of AbstractCheckpointManager."""
 
 import asyncio
 import dataclasses
 import datetime
 import threading
-import time
-from typing import Any, Callable, List, Mapping, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Container, List, Mapping, Optional, Sequence, Tuple, Union
 import uuid
 
 from absl import logging
 from etils import epath
 import jax
 from jax.experimental import multihost_utils
 from jax.experimental.array_serialization import serialization
@@ -41,15 +40,15 @@
 DEFAULT_ITEM_NAME = 'default'
 DESCRIPTOR_ITEM_NAME = 'descriptor'
 METRIC_ITEM_NAME = 'metrics'
 METADATA_ITEM_NAME = 'metadata'
 
 RESERVED_ITEM_NAMES = [DESCRIPTOR_ITEM_NAME, METRIC_ITEM_NAME]
 
-_INIT_TIME = time.time()
+_INIT_TIME = datetime.datetime.now(tz=datetime.timezone.utc)
 
 
 def _metrics_file_exists(metrics_item_path: epath.Path) -> bool:
   """True if item directory AND actual file both exist."""
   return (
       metrics_item_path.exists()
       and (metrics_item_path / METRIC_ITEM_NAME).exists()
@@ -112,34 +111,37 @@
   step_prefix: if provided, step directories will take the form
     f'{step_prefix}_<step>'. Otherwise, they will simply be an integer <step>.
   step_format_fixed_length: If set, formats step with n digits (leading zeros).
     This makes sorting steps easier. Otherwise, step has no leading zeros.
   create: if True, creates the top-level directory if it does not already exist.
   cleanup_tmp_directories: if True, cleans up any existing temporary directories
     on CheckpointManager creation.
-  enable_descriptor: if True, logs a Descriptor proto that contains lineage
-    information about a directory.
+  save_on_steps: Optional set of steps at which checkpoints should be saved.
+    Useful to save checkpoints on a fixed set of steps that are not multiple of
+    `save_interval_steps`.
   """
   save_interval_steps: int = 1
   max_to_keep: Optional[int] = None
   keep_time_interval: Optional[datetime.timedelta] = None
   keep_period: Optional[int] = None
   best_fn: Optional[Callable[[PyTree], float]] = None
   best_mode: str = 'max'
   keep_checkpoints_without_metrics: bool = True
   step_prefix: Optional[str] = None
   step_format_fixed_length: Optional[int] = None
   create: bool = True
   cleanup_tmp_directories: bool = False
+  save_on_steps: Optional[Container[int]] = None
 
   def __post_init__(self):
     if self.best_mode not in ('min', 'max'):
       msg = ("`CheckpointManagerOptions.best_mode` must be one of None, 'min' "
              "or 'max'. Got {self.dtype}.")
       raise ValueError(msg)
+    self.save_on_steps = frozenset(self.save_on_steps or ())
 
 
 @dataclasses.dataclass
 class CheckpointInfo:
   """Metadata about a checkpoint."""
   step: int
   time: datetime.datetime
@@ -333,15 +335,16 @@
     # save interval). The `last_checkpoint_step` may not be initialized, in
     # which case we should save. Otherwise, step must fall on the specified
     # save interval. This condition accounts for the possibility of saving
     # on preemption, in which case we want to maintain the same save period as
     # if preemption had not happened.
     return last_checkpoint_step is None or (
         last_checkpoint_step < step and
-        step % self._options.save_interval_steps == 0)
+        (step % self._options.save_interval_steps == 0 or
+         step in self._options.save_on_steps))
 
   def _get_save_directory(
       self,
       step: int,
       directory: epath.Path,
       key_name: Optional[str] = None,
       tmp_directory: Optional[epath.Path] = None,
@@ -434,14 +437,16 @@
       ValueError: directory creation failed.
       ValueError: if an item is provided for which no `Checkpointer` is
       found.
       ValueError: if the checkpoint already exists.
     """
     if not force and not self.should_save(step):
       return False
+    if self.reached_preemption(step):
+      logging.info('Saving checkpoint at step %d due to preemption.', step)
 
     # Wait for ongoing saves to complete. Only applicable if some of the
     # checkpointers are AsyncCheckpointers.
     self.wait_until_finished()
 
     if step in self.all_steps():
       raise ValueError(f'Checkpoint for step {step} already exists.')
```

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_utils.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/checkpoint_utils_test.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/checkpoint_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/checkpointer.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/checkpointer.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/conftest.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/conftest.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/future.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/future.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/json_checkpoint_handler.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/json_checkpoint_handler.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/json_checkpoint_handler_test.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/json_checkpoint_handler_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/lazy_utils.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/lazy_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/msgpack_utils.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/msgpack_utils.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/msgpack_utils_test.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/msgpack_utils_test.py`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/orbax_checkpoint.ipynb` & `orbax_checkpoint-0.2.4/orbax/checkpoint/orbax_checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/pytree_checkpoint_handler.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/pytree_checkpoint_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,17 +131,28 @@
 
   return jax.tree_util.tree_map(_get_param_info, names, structure)
 
 
 def _get_tree_for_aggregation(param_infos, save_args, item):
   """Get tree for aggregated checkpoint."""
 
+  # TODO(b/283164080): These type checks result in logic from the lower layer
+  # (TypeHandler/AggregateHandler) leaking into the upper layer
+  # (CheckpointHandler). Ideally, AggregateHandler could define its own
+  # supported values and error conditions.
   def _get_leaf_for_aggregation(param_info, arg, value):
     if arg.aggregate:  # Param was aggregated, return value after cast.
+      if isinstance(value, jax.Array) and not value.is_fully_replicated:
+        raise ValueError(
+            'jax.Array must be fully replicated to be saved in aggregate file.'
+        )
       if not utils.is_supported_aggregation_type(value):
+        # Not an error because users' training states often have a bunch of
+        # random unserializable objects in them (empty states, optimizer
+        # objects, etc.).
         value = None
       return _try_array_cast(value, arg.dtype)
     else:  # Placeholder string for non-aggregated value.
       return utils.leaf_placeholder(param_info.name)
 
   return jax.tree_util.tree_map(
       _get_leaf_for_aggregation, param_infos, save_args, item
@@ -171,15 +182,15 @@
     if transforms is not None:
       msg = ('If providing `transforms`, must provide `item` matching structure'
              ' of expected result.')
       raise ValueError(msg)
     item = restored
   else:
     if transforms is None:
-      item = utils.deserialize_tree(item, restored)
+      item = utils.deserialize_tree(restored, item)
     else:
       transforms = _construct_lazy_transform_wrappers(transforms)
       item = transform_utils.apply_transformations(
           restored, transforms, item, transforms_default_to_original)
   return item
```

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/test_utils.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/test_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utils for orbax tests."""
 
+import functools
 from typing import List, Optional
 
 from etils import epath
 import jax
 from jax import sharding
 from jax.experimental import pjit
 import jax.numpy as jnp
-from jax.sharding import Mesh
 import numpy as np
 from orbax.checkpoint import lazy_utils
 from orbax.checkpoint import pytree_checkpoint_handler
 from orbax.checkpoint import utils
 
 
 def save_fake_tmp_dir(
@@ -48,15 +48,15 @@
       (item_tmp_dir / sub).mkdir(parents=True)
   utils.sync_global_devices('save_fake_tmp_dir')
   return item_tmp_dir
 
 
 def replicate_sharded_array(arr: jax.Array):
   """Returns the input array, but replicated across all devices."""
-  mesh = Mesh(np.asarray(jax.devices()), ('x',))
+  mesh = jax.sharding.Mesh(np.asarray(jax.devices()), ('x',))
   replicated_sharding = sharding.NamedSharding(
       mesh,
       jax.sharding.PartitionSpec(
           None,
       ),
   )
   return pjit.pjit(lambda x: x, out_axis_resources=replicated_sharding)(arr)
@@ -75,39 +75,44 @@
 
   def f(arr):
     return pjit.pjit(function)(arr)
 
   return jax.tree_util.tree_map(f, tree)
 
 
-def assert_tree_equal(testclass, expected, actual):
-  """Asserts that two PyTrees are equal."""
+def assert_array_equal(testclass, v_expected, v_actual):
+  """Asserts that two arrays are equal."""
+  if isinstance(v_expected, lazy_utils.LazyValue):
+    testclass.assertIsInstance(v_actual, lazy_utils.LazyValue)
+    v_expected = v_expected.get()
+    v_actual = v_actual.get()
+
+  testclass.assertIsInstance(v_actual, type(v_expected))
+  if isinstance(v_expected, jax.Array):
+    testclass.assertEqual(
+        len(v_expected.addressable_shards), len(v_actual.addressable_shards)
+    )
+    for shard_expected, shard_actual in zip(
+        v_expected.addressable_shards, v_actual.addressable_shards
+    ):
+      np.testing.assert_array_equal(shard_expected.data, shard_actual.data)
+  elif isinstance(v_expected, (np.ndarray, jnp.ndarray)):
+    np.testing.assert_array_equal(v_expected, v_actual)
+  else:
+    testclass.assertEqual(v_expected, v_actual)
 
-  def assert_array_equal(v_expected, v_actual):
-    if isinstance(v_expected, lazy_utils.LazyValue):
-      testclass.assertIsInstance(v_actual, lazy_utils.LazyValue)
-      v_expected = v_expected.get()
-      v_actual = v_actual.get()
-
-    testclass.assertIsInstance(v_actual, type(v_expected))
-    if isinstance(v_expected, jax.Array):
-      testclass.assertEqual(
-          len(v_expected.addressable_shards), len(v_actual.addressable_shards))
-      for shard_expected, shard_actual in zip(v_expected.addressable_shards,
-                                              v_actual.addressable_shards):
-        np.testing.assert_array_equal(shard_expected.data, shard_actual.data)
-    elif isinstance(v_expected, (np.ndarray, jnp.ndarray)):
-      np.testing.assert_array_equal(v_expected, v_actual)
-    else:
-      testclass.assertEqual(v_expected, v_actual)
 
+def assert_tree_equal(testclass, expected, actual):
+  """Asserts that two PyTrees are equal."""
   expected_flat = utils.to_flat_dict(expected)
   actual_flat = utils.to_flat_dict(actual)
   testclass.assertSameElements(expected_flat.keys(), actual_flat.keys())
-  jax.tree_util.tree_map(assert_array_equal, expected, actual)
+  jax.tree_util.tree_map(
+      functools.partial(assert_array_equal, testclass), expected, actual
+  )
 
 
 def setup_pytree(add: int = 0):
   """Creates a numpy PyTree for testing."""
   pytree = {
       'a': np.arange(8) * 1,
       'b': np.arange(16) * 2,
@@ -120,19 +125,21 @@
   return pytree
 
 
 def setup_sharded_pytree():
   """Creates a PyTree of sharded arrays for testing."""
   devices = np.asarray(jax.devices())
 
-  mesh_2d = Mesh(devices.reshape((2, len(devices) // 2)), ('x', 'y'))
+  mesh_2d = jax.sharding.Mesh(
+      devices.reshape((2, len(devices) // 2)), ('x', 'y')
+  )
   mesh_axes_2d = jax.sharding.PartitionSpec('x', 'y')
-  mesh_1d = Mesh(devices, ('x',))
+  mesh_1d = jax.sharding.Mesh(devices, ('x',))
   mesh_axes_1d = jax.sharding.PartitionSpec('x',)
-  mesh_0d = Mesh(devices, ('x',))
+  mesh_0d = jax.sharding.Mesh(devices, ('x',))
   mesh_axes_0d = jax.sharding.PartitionSpec(None,)
 
   pytree = setup_pytree()
   mesh_tree = {
       'a': mesh_0d,
       'b': mesh_1d,
       'c': {
@@ -153,15 +160,15 @@
       create_sharded_array, pytree, mesh_tree, axes_tree, is_leaf=is_leaf)
   return pytree, mesh_tree, axes_tree
 
 
 def is_leaf(x):
   return (
       isinstance(x, np.ndarray)
-      or isinstance(x, Mesh)
+      or isinstance(x, jax.sharding.Mesh)
       or isinstance(x, jax.sharding.PartitionSpec)
       or isinstance(x, pytree_checkpoint_handler.ParamInfo)
   )
 
 
 def create_sharded_array(arr, mesh, mesh_axes):
   """Create sharded jax.Array."""
```

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/transform_utils.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/transform_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Provides utils for transforming PyTrees from one version to another."""
 
 import dataclasses
+import functools
+import operator
 import re
-from typing import Any, Callable, Dict, Optional, Tuple, Union
+from typing import Any, Callable, Dict, Optional, Sequence, Tuple, Union
 
 from absl import logging
 from orbax.checkpoint import utils
 
 PyTree = Any
 ValueFn = Callable[[Any], Any]
 MultiValueFn = Callable[[str, PyTree], Any]
@@ -247,8 +249,29 @@
         unmatched_new_keys.append(key)
 
   if unmatched_new_keys:
     logging.info('The following keys are not loaded from the original tree '
                  'after applying specified transforms: %s',
                  ', '.join(unmatched_new_keys))
 
-  return utils.from_flat_dict(new_tree, new, sep='/')
+  return utils.from_flat_dict(new, target=new_tree, sep='/')
+
+
+def merge_trees(
+    *trees: Sequence[PyTree], target: Optional[PyTree] = None
+) -> PyTree:
+  """Merges the provided PyTrees into a single result.
+
+  If trees have overlapping keys, the key of the last tree in the list will take
+  precedence.
+
+  Args:
+    *trees: PyTrees to merge.
+    target: A PyTree to provide structure for the returned value. If not
+      provided, the result will take the form of a dictionary.
+
+  Returns:
+    A single merged PyTree.
+  """
+  trees = [utils.to_flat_dict(t) for t in trees]
+  merged = functools.reduce(operator.ior, trees, {})
+  return utils.from_flat_dict(merged, target=target)
```

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/transform_utils_test.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/transform_utils_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -428,15 +428,15 @@
         expected_flat_dict[k] = old_flat_dict[k.replace('Dense_2', 'Dense_1')]
       elif 'Dense_' in k:  # layers in new, but not old.
         expected_flat_dict[k] = v
       else:  # extra keys in both, expected is the old value
         expected_flat_dict[k] = old_flat_dict[k]
 
     expected_state = utils.from_flat_dict(
-        new_state, expected_flat_dict, sep='/'
+        expected_flat_dict, target=new_state, sep='/'
     )
     test_utils.assert_tree_equal(self, expected_state, restored_state)
 
   def test_flax_train_state_default_new(self):
 
     class Model(nn.Module):
 
@@ -470,14 +470,109 @@
     for k, v in new_flat_dict.items():
       if 'Dense_1' in k:
         expected_flat_dict[k] = old_flat_dict[k]
       else:
         expected_flat_dict[k] = v
 
     expected_state = utils.from_flat_dict(
-        new_state, expected_flat_dict, sep='/'
+        expected_flat_dict, target=new_state, sep='/'
     )
     test_utils.assert_tree_equal(self, expected_state, restored_state)
 
+  def test_merge_trees(self):
+    one = {
+        'a': 1,
+        'b': {
+            'c': 2,
+            'd': 3,
+        },
+    }
+    two = {
+        'a': 2,
+        'b': {
+            'c': 4,
+            'e': 6,
+        },
+    }
+    three = {}
+    four = {
+        'f': 7,
+        'g': 8,
+    }
+    expected = {
+        'a': 2,
+        'b': {
+            'c': 4,
+            'd': 3,
+            'e': 6,
+        },
+        'f': 7,
+        'g': 8,
+    }
+    self.assertDictEqual(
+        expected, transform_utils.merge_trees(one, two, three, four)
+    )
+
+  def test_merge_trees_target(self):
+    one = {
+        'a': 1,
+        'b': {
+            'c': 2,
+            'd': 3,
+        },
+    }
+    two = {
+        'a': 2,
+        'b': {
+            'c': 4,
+            'e': 6,
+        },
+    }
+    three = {}
+    four = {
+        'f': 7,
+        'g': 8,
+    }
+
+    @flax.struct.dataclass
+    class Expected:
+      a: int
+      b: Mapping[str, int]
+      f: int
+      g: int
+
+      def __eq__(self, other):
+        return (
+            self.a == other.a
+            and self.b == other.b
+            and self.f == other.f
+            and self.g == other.g
+        )
+
+    expected = Expected(
+        a=2,
+        b={
+            'c': 4,
+            'd': 3,
+            'e': 6,
+        },
+        f=7,
+        g=8,
+    )
+
+    self.assertEqual(
+        expected,
+        transform_utils.merge_trees(
+            one,
+            two,
+            three,
+            four,
+            target=jax.tree_util.tree_map(lambda x: 0, expected),
+        ),
+    )
+
+  def test_merge_trees_empty(self):
+    self.assertDictEqual({}, transform_utils.merge_trees({}, {}))
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/type_handlers.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/type_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -487,15 +487,16 @@
     if (
         isinstance(value, jax.Array)
         and jax.process_count() > 1
         and value.is_fully_addressable
     ):
       raise ValueError(
           'Cannot serialize host local arrays. Arrays like this are typically'
-          ' obtained using pmap. Consider using host_local_to_global_array in'
+          ' obtained using pmap. Consider using'
+          ' fully_replicated_host_local_array_to_global_array in'
           ' orbax/checkpoint/utils.py to convert your arrays into serializable'
           ' objects.'
       )
     args = args or SaveArgs()
     tspec = self._get_json_tspec_write(info, value, use_ocdbt=self._use_ocdbt)
     tspec = _get_cast_tspec_serialize(tspec, value, args)
     commit_futures = []
```

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/utils.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 import time
 from typing import Any, List, Optional, Tuple, Union
 
 from absl import logging
 from etils import epath
 import jax
 from jax.experimental import multihost_utils
-import jax.numpy as jnp
 import numpy as np
 
 TMP_DIR_SUFFIX = '.orbax-checkpoint-tmp-'
 # prefix_1000.orbax-checkpoint-tmp-1010101
 # OR
 # 1000.orbax-checkpoint-tmp-1010101
 TMP_DIR_STEP_PATTERN = r'.*?_*?(\d+)\.orbax-checkpoint-tmp-\d+'
@@ -202,14 +201,15 @@
   # (keypath tuple), first key in keypath (outermost key in the PyTree).
   outerkey = flat_with_keys[0][0][0]
   if _is_dict_key(outerkey):
     result = {}
   elif _is_sequence_key(outerkey):
     result = []
   else:
+    result = None
     _raise_unsupported_key_error(outerkey)
 
   for keypath, value in flat_with_keys:
     subtree = result
     for i, key in enumerate(keypath):
       if i == 0:
         assert isinstance(key, type(outerkey))
@@ -224,14 +224,15 @@
       else:
         nextkey = keypath[i + 1]
         if _is_dict_key(nextkey):
           nextvalue = {}
         elif _is_sequence_key(nextkey):
           nextvalue = []
         else:
+          nextvalue = None
           _raise_unsupported_key_error(nextkey)
 
         if _is_dict_key(key):
           assert isinstance(subtree, dict)
           name = get_key_name(key)
           if name not in subtree:
             subtree[name] = nextvalue
@@ -244,15 +245,15 @@
         else:
           _raise_unsupported_key_error(key)
 
   return result
 
 
 def deserialize_tree(
-    target: PyTree, serialized: PyTree, keep_empty_nodes: bool = False
+    serialized: PyTree, target: PyTree, keep_empty_nodes: bool = False
 ) -> PyTree:
   """Deserializes a PyTree to the same structure as `target`."""
 
   def _reconstruct_from_keypath(keypath, _):
     result = serialized
     for key in keypath:
       key_name = get_key_name(key)
@@ -266,33 +267,52 @@
       _reconstruct_from_keypath,
       target,
       is_leaf=is_empty_or_leaf if keep_empty_nodes else None,
   )
 
 
 def from_flat_dict(
-    tree: PyTree, flat_dict: PyTree, sep: Optional[str] = None
+    flat_dict: PyTree,
+    target: Optional[PyTree] = None,
+    sep: Optional[str] = None,
 ) -> PyTree:
   """Reconstructs the original tree object from a flattened dictionary.
 
   Args:
-    tree: A reference PyTree. The returned value will conform to this structure.
     flat_dict: A dictionary conforming to the return value of `to_flat_dict`.
+    target: A reference PyTree. The returned value will conform to this
+      structure. If not provided, an unflattened dict will be returned with the
+      inferred structure of the original tree, without necessarily matching it
+      exactly.
     sep: separator used for nested keys in `flat_dict`.
 
   Returns:
     A dict matching the structure of `tree` with the values of `flat_dict`.
   """
-  flat_structure = to_flat_dict(tree, sep=sep)
-  # Ensure that the ordering of `flat_dict` keys matches that of `tree`.
-  # Necessary for later unflattening.
-  flat_dict = {k: flat_dict[k] for k in flat_structure.keys()}
-  return jax.tree_util.tree_unflatten(
-      jax.tree_util.tree_structure(tree), flat_dict.values()
-  )
+  if target is None:
+    result = {}
+    for k, v in flat_dict.items():
+      subtree = result
+      for i, name in enumerate(k):
+        if i == len(k) - 1:
+          assert name not in subtree
+          subtree[name] = v
+        else:
+          if name not in subtree:
+            subtree[name] = {}
+          subtree = subtree[name]
+    return result
+  else:
+    flat_structure = to_flat_dict(target, sep=sep)
+    # Ensure that the ordering of `flat_dict` keys matches that of `target`.
+    # Necessary for later unflattening.
+    flat_dict = {k: flat_dict[k] for k in flat_structure.keys()}
+    return jax.tree_util.tree_unflatten(
+        jax.tree_util.tree_structure(target), flat_dict.values()
+    )
 
 
 def leaf_is_placeholder(leaf: Any) -> bool:
   """Determines if `leaf` represents a placeholder for a non-aggregated value.
   """
   return isinstance(leaf, str) and (leaf.startswith(_PLACEHOLDER_PREFIX) or
                                     leaf.startswith(_AGGREGATED_PREFIX))
@@ -322,15 +342,15 @@
   return isinstance(value, (dict, list, type(None))) and not value
 
 
 def is_supported_aggregation_type(value: Any) -> bool:
   """Determines if the value is supported for aggregation."""
   return isinstance(
       value,
-      (str, int, float, np.number, np.ndarray, jnp.ndarray, bytes),
+      (str, int, float, np.number, np.ndarray, bytes, jax.Array),
   ) or is_supported_empty_aggregation_type(value)
 
 
 def pytree_structure(directory: epath.PathLike) -> PyTree:
   """Reconstruct state dict from saved model format in `directory`."""
   directory = epath.Path(directory)
```

### Comparing `orbax-checkpoint-0.2.3/orbax/checkpoint/utils_test.py` & `orbax_checkpoint-0.2.4/orbax/checkpoint/utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,17 @@
   @parameterized.parameters(
       ({'a': 1, 'b': {'d': 2}}, {('a',): 1, ('b', 'd'): 2}),
       ({'x': ['foo', 'bar']}, {('x', '0'): 'foo', ('x', '1'): 'bar'}),
       ({'a': 1, 'b': 2}, {('b',): 2, ('a',): 1}),
   )
   def test_from_flat_dict(self, expected, flat_dict):
     empty = jax.tree_util.tree_map(lambda _: 0, expected)
-    self.assertDictEqual(expected, utils.from_flat_dict(empty, flat_dict))
+    self.assertDictEqual(
+        expected, utils.from_flat_dict(flat_dict, target=empty)
+    )
 
   def test_serialize(self):
     tree = {'a': 1, 'b': {'c': {'d': 2}}, 'e': [1, {'x': 5, 'y': 7}, [9, 10]]}
     serialized = utils.serialize_tree(tree, keep_empty_nodes=True)
     self.assertDictEqual(tree, serialized)
 
   def test_serialize_list(self):
```

### Comparing `orbax-checkpoint-0.2.3/pyproject.toml` & `orbax_checkpoint-0.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "orbax-checkpoint"
 description = "Orbax Checkpoint"
 readme = 'README.md'
 license = {file = 'LICENSE'}
-requires-python = '>=3.8'
+requires-python = '>=3.9'
 authors = [{name = 'Orbax Authors', email='orbax-dev@google.com'}]
 classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python',
```

### Comparing `orbax-checkpoint-0.2.3/PKG-INFO` & `orbax_checkpoint-0.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: orbax-checkpoint
-Version: 0.2.3
+Version: 0.2.4
 Summary: Orbax Checkpoint
 Keywords: JAX machine learning,checkpoint,training
 Author-email: Orbax Authors <orbax-dev@google.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -29,15 +29,17 @@
 Requires-Dist: pytest-xdist ; extra == "dev"
 Project-URL: homepage, http://github.com/google/orbax
 Project-URL: repository, http://github.com/google/orbax
 Provides-Extra: dev
 
 # Orbax Checkpointing
 
-`pip install orbax-checkpoint`
+`pip install orbax-checkpoint` (latest PyPi release) OR
+
+`pip install 'git+https://github.com/google/orbax/#subdirectory=checkpoint'` (from this repository, at HEAD)
 
 `import orbax.checkpoint`
 
 Orbax includes a checkpointing library oriented towards JAX users, supporting a
 variety of different features required by different frameworks, including
 asynchronous checkpointing, various types, and various storage formats.
 We aim to provide a highly customizable and composable API which maximizes
```

