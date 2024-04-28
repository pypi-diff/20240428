# Comparing `tmp/gym_jiminy_rllib-1.8.4-py3-none-any.whl.zip` & `tmp/gym_jiminy_rllib-1.8.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 25592 bytes, number of entries: 10
--rw-r--r--  2.0 unx      264 b- defN 24-Apr-19 21:51 gym_jiminy/rllib/__init__.py
--rw-r--r--  2.0 unx     3162 b- defN 24-Apr-19 21:51 gym_jiminy/rllib/callbacks.py
--rw-r--r--  2.0 unx    12290 b- defN 24-Apr-19 21:51 gym_jiminy/rllib/curriculum.py
--rw-r--r--  2.0 unx    28076 b- defN 24-Apr-19 21:51 gym_jiminy/rllib/ppo.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 21:51 gym_jiminy/rllib/py.typed
--rw-r--r--  2.0 unx    46328 b- defN 24-Apr-19 21:51 gym_jiminy/rllib/utilities.py
--rw-r--r--  2.0 unx      954 b- defN 24-Apr-19 21:52 gym_jiminy_rllib-1.8.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 21:52 gym_jiminy_rllib-1.8.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-19 21:52 gym_jiminy_rllib-1.8.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      838 b- defN 24-Apr-19 21:52 gym_jiminy_rllib-1.8.4.dist-info/RECORD
-10 files, 92015 bytes uncompressed, 24154 bytes compressed:  73.7%
+Zip file size: 25704 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      264 b- defN 24-Apr-28 20:51 gym_jiminy/rllib/__init__.py
+-rw-r--r--  2.0 unx     3162 b- defN 24-Apr-28 20:51 gym_jiminy/rllib/callbacks.py
+-rw-r--r--  2.0 unx    12290 b- defN 24-Apr-28 20:51 gym_jiminy/rllib/curriculum.py
+-rw-r--r--  2.0 unx    28124 b- defN 24-Apr-28 20:51 gym_jiminy/rllib/ppo.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-28 20:51 gym_jiminy/rllib/py.typed
+-rw-r--r--  2.0 unx    46565 b- defN 24-Apr-28 20:51 gym_jiminy/rllib/utilities.py
+-rw-r--r--  2.0 unx      954 b- defN 24-Apr-28 20:52 gym_jiminy_rllib-1.8.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-28 20:52 gym_jiminy_rllib-1.8.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-28 20:52 gym_jiminy_rllib-1.8.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      838 b- defN 24-Apr-28 20:52 gym_jiminy_rllib-1.8.5.dist-info/RECORD
+10 files, 92300 bytes uncompressed, 24266 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: gym_jiminy/rllib/py.typed
 Comment: 
 
 Filename: gym_jiminy/rllib/utilities.py
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.4.dist-info/METADATA
+Filename: gym_jiminy_rllib-1.8.5.dist-info/METADATA
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.4.dist-info/WHEEL
+Filename: gym_jiminy_rllib-1.8.5.dist-info/WHEEL
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.4.dist-info/top_level.txt
+Filename: gym_jiminy_rllib-1.8.5.dist-info/top_level.txt
 Comment: 
 
-Filename: gym_jiminy_rllib-1.8.4.dist-info/RECORD
+Filename: gym_jiminy_rllib-1.8.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gym_jiminy/rllib/ppo.py

```diff
@@ -157,14 +157,15 @@
     """
     def _update_flattened_slice(data: torch.Tensor,
                                 shape: Tuple[int, ...],
                                 mirror_mat: torch.Tensor) -> torch.Tensor:
         """Mirror an array of flattened tensor using provided transformation
         matrix.
         """
+        mirror_mat = mirror_mat.to(data.device)
         if len(shape) > 1:
             assert len(shape) == 2, "shape > 2 is not supported for now."
             data = data.reshape(
                 (-1, *shape)).swapaxes(1, 0).reshape((shape[0], -1))
             data_mirrored = mirror_mat @ data
             return data_mirrored.reshape(
                 (shape[0], -1, shape[1])).swapaxes(1, 0).reshape((-1, *shape))
```

## gym_jiminy/rllib/utilities.py

```diff
@@ -35,14 +35,15 @@
 from ray._private.test_utils import monitor_memory_usage
 from ray._raylet import GcsClientOptions  # type: ignore[attr-defined]
 from ray.exceptions import RayTaskError
 from ray.tune.logger import Logger
 from ray.tune.result import TRAINING_ITERATION, TIME_TOTAL_S, TIMESTEPS_TOTAL
 from ray.tune.utils import flatten_dict
 from ray.tune.utils.util import SafeFallbackEncoder
+from ray.train._internal.session import _TrainingResult
 from ray.rllib.connectors.connector import Connector, ConnectorContext
 from ray.rllib.connectors.registry import register_connector
 from ray.rllib.connectors.util import (
     get_agent_connectors_from_config, get_action_connectors_from_config)
 from ray.rllib.algorithms.algorithm import Algorithm
 from ray.rllib.algorithms.algorithm_config import AlgorithmConfig
 from ray.rllib.models import ModelCatalog
@@ -364,15 +365,15 @@
 def train(algo: Algorithm,
           max_timesteps: int = 0,
           max_iters: int = 0,
           logger_cls: type = TBXLogger,
           logdir: Optional[Logger] = None,
           checkpoint_period: int = 0,
           verbose: bool = True,
-          debug: bool = False) -> str:
+          debug: bool = False) -> _TrainingResult:
     """Train a model on a specific environment using a given algorithm.
 
     The algorithm is associated with a given reinforcement learning algorithm,
     instantiated for a specific environment and policy model. Thus, it already
     wraps all the required information to actually perform training.
 
     .. note::
@@ -392,16 +393,18 @@
                               Optional: Disabled by default.
     :param verbose: Whether to print high-level information after each training
                     iteration.
                     Optional: True by default.
     :param debug: Whether to monitor memory allocation to debug memory leaks.
                   Optional: Disabled by default.
 
-    :returns: Fullpath of algorithm's final state dump. This includes the
-              trained policy model.
+    :returns: Ray-specific `_TrainingResult` object, which are named tuple
+    (checkpoint: ray.train.Checkpoint, metrics: Dict[str, Any]). The fullpath
+    of algorithm's final state dump can be retrieve via `.checkpoint.path`. The
+    latter includes the trained policy model.
     """
     # Get environment's reward threshold, if any
     assert isinstance(algo.workers, WorkerSet)
     env_spec, *_ = chain(*algo.workers.foreach_env(attrgetter('spec')))
     if env_spec is None or env_spec.reward_threshold is None:
         reward_threshold = float('inf')
     else:
```

## Comparing `gym_jiminy_rllib-1.8.4.dist-info/METADATA` & `gym_jiminy_rllib-1.8.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-jiminy-rllib
-Version: 1.8.4
+Version: 1.8.5
 Summary: Specialized Reinforcement learning toolbox based on Ray RLlib for Gym Jiminy.
 Author: Alexis Duburcq
 Author-email: alexis.duburcq@gmail.com
 Maintainer: Alexis Duburcq
 License: MIT
 Keywords: reinforcement-learning robotics gym jiminy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,12 +13,12 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8,<3.12
-Requires-Dist: gym-jiminy ~=1.8.4
+Requires-Dist: gym-jiminy ~=1.8.5
 Requires-Dist: ray[rllib] ~=2.9.0
 Requires-Dist: tensorboardX
 Requires-Dist: plotext >=5.0.0
```

