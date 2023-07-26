# Comparing `tmp/torchmanager-1.1.5.tar.gz` & `tmp/torchmanager-1.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager-1.1.5.tar", max compression
+gzip compressed data, was "torchmanager-1.2b1.tar", last modified: Wed Jul 26 18:17:49 2023, max compression
```

## Comparing `torchmanager-1.1.5.tar` & `torchmanager-1.2b1.tar`

### file list

```diff
@@ -1,44 +1,72 @@
--rw-r--r--   0        0        0     1318 2023-07-13 17:22:38.863844 torchmanager-1.1.5/LICENSE
--rw-r--r--   0        0        0      616 2023-07-24 18:20:42.158872 torchmanager-1.1.5/pyproject.toml
--rw-r--r--   0        0        0      281 2023-07-24 18:20:29.306791 torchmanager-1.1.5/torchmanager/__init__.py
--rw-r--r--   0        0        0    11076 2023-07-24 18:20:29.307075 torchmanager-1.1.5/torchmanager/basic.py
--rw-r--r--   0        0        0      659 2023-07-24 18:20:29.307303 torchmanager-1.1.5/torchmanager/callbacks/__init__.py
--rw-r--r--   0        0        0     4248 2023-07-24 18:20:29.307524 torchmanager-1.1.5/torchmanager/callbacks/callback.py
--rw-r--r--   0        0        0     4686 2023-07-24 18:20:29.307738 torchmanager-1.1.5/torchmanager/callbacks/ckpt.py
--rw-r--r--   0        0        0     3522 2023-07-19 18:01:53.901655 torchmanager-1.1.5/torchmanager/callbacks/dynamic.py
--rw-r--r--   0        0        0     1984 2023-07-24 18:20:29.307933 torchmanager-1.1.5/torchmanager/callbacks/early_stop.py
--rw-r--r--   0        0        0     4854 2023-07-24 18:20:29.308143 torchmanager-1.1.5/torchmanager/callbacks/experiment.py
--rw-r--r--   0        0        0     2238 2023-07-24 18:20:29.308326 torchmanager-1.1.5/torchmanager/callbacks/lr.py
--rw-r--r--   0        0        0     2454 2023-07-24 18:20:29.308508 torchmanager-1.1.5/torchmanager/callbacks/tensorboard.py
--rw-r--r--   0        0        0      963 2023-07-24 18:20:29.308686 torchmanager-1.1.5/torchmanager/compatibility.py
--rw-r--r--   0        0        0       85 2023-07-19 18:01:53.902732 torchmanager-1.1.5/torchmanager/data/__init__.py
--rw-r--r--   0        0        0     6962 2023-07-24 18:20:29.308901 torchmanager-1.1.5/torchmanager/data/dataset.py
--rw-r--r--   0        0        0     2236 2023-07-24 18:20:29.309114 torchmanager-1.1.5/torchmanager/data/sliding.py
--rw-r--r--   0        0        0      195 2023-07-24 18:20:42.159166 torchmanager-1.1.5/torchmanager/losses/__init__.py
--rw-r--r--   0        0        0     5386 2023-07-24 18:20:29.309487 torchmanager-1.1.5/torchmanager/losses/cross_entropy.py
--rw-r--r--   0        0        0     1351 2023-07-24 18:20:42.159410 torchmanager-1.1.5/torchmanager/losses/dice.py
--rw-r--r--   0        0        0     7177 2023-07-24 18:20:42.159624 torchmanager-1.1.5/torchmanager/losses/loss.py
--rw-r--r--   0        0        0     2381 2023-07-24 18:20:29.310038 torchmanager-1.1.5/torchmanager/losses/mse.py
--rw-r--r--   0        0        0      234 2023-07-24 18:20:29.310249 torchmanager-1.1.5/torchmanager/metrics/__init__.py
--rw-r--r--   0        0        0     3272 2023-07-24 18:20:29.310449 torchmanager-1.1.5/torchmanager/metrics/accuracy.py
--rw-r--r--   0        0        0     2546 2023-07-24 18:20:29.310667 torchmanager-1.1.5/torchmanager/metrics/conf_met.py
--rw-r--r--   0        0        0     2635 2023-07-24 18:20:42.159953 torchmanager-1.1.5/torchmanager/metrics/iou.py
--rw-r--r--   0        0        0     4000 2023-07-24 18:20:29.311079 torchmanager-1.1.5/torchmanager/metrics/metric.py
--rw-r--r--   0        0        0     9401 2023-07-24 18:20:29.311297 torchmanager-1.1.5/torchmanager/testing.py
--rw-r--r--   0        0        0      191 2023-07-24 18:20:29.311471 torchmanager-1.1.5/torchmanager/train/__init__.py
--rw-r--r--   0        0        0     4986 2023-07-24 18:20:29.311709 torchmanager-1.1.5/torchmanager/train/checkpoint.py
--rw-r--r--   0        0        0     2037 2023-07-24 18:20:29.311938 torchmanager-1.1.5/torchmanager/train/learning_rate.py
--rw-r--r--   0        0        0    14893 2023-07-24 18:20:29.312204 torchmanager-1.1.5/torchmanager/training.py
--rw-r--r--   0        0        0      443 2023-07-24 18:20:29.312496 torchmanager-1.1.5/torchmanager_core/__init__.py
--rw-r--r--   0        0        0      114 2023-07-24 18:20:29.312713 torchmanager-1.1.5/torchmanager_core/devices/__init__.py
--rw-r--r--   0        0        0     5587 2023-07-24 18:20:29.312937 torchmanager-1.1.5/torchmanager_core/devices/device.py
--rw-r--r--   0        0        0      264 2023-07-19 18:01:53.907517 torchmanager-1.1.5/torchmanager_core/devices/protocols.py
--rw-r--r--   0        0        0      153 2023-07-24 18:20:29.313320 torchmanager-1.1.5/torchmanager_core/errors/__init__.py
--rw-r--r--   0        0        0      350 2023-07-24 18:20:29.313473 torchmanager-1.1.5/torchmanager_core/errors/runtime.py
--rw-r--r--   0        0        0      669 2023-07-19 18:01:53.907838 torchmanager-1.1.5/torchmanager_core/errors/train.py
--rw-r--r--   0        0        0     2728 2023-07-24 18:20:29.313655 torchmanager-1.1.5/torchmanager_core/protocols.py
--rw-r--r--   0        0        0      204 2023-07-19 18:01:53.908282 torchmanager-1.1.5/torchmanager_core/typing.py
--rw-r--r--   0        0        0     7356 2023-07-24 18:20:42.160278 torchmanager-1.1.5/torchmanager_core/version.py
--rw-r--r--   0        0        0      163 2023-07-24 18:20:29.314043 torchmanager-1.1.5/torchmanager_core/view/__init__.py
--rw-r--r--   0        0        0      313 2023-07-19 18:01:53.908597 torchmanager-1.1.5/torchmanager_core/view/protocols.py
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 torchmanager-1.1.5/PKG-INFO
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:17:49.645224 torchmanager-1.2b1/
+-rw-r--r--   0 kisonho    (501) staff       (20)     1318 2023-07-13 17:22:38.000000 torchmanager-1.2b1/LICENSE
+-rw-r--r--   0 kisonho    (501) staff       (20)     2109 2023-07-26 18:17:49.645107 torchmanager-1.2b1/PKG-INFO
+-rw-r--r--   0 kisonho    (501) staff       (20)     1806 2023-07-26 18:16:57.000000 torchmanager-1.2b1/README.md
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:17:49.639243 torchmanager-1.2b1/core/
+-rw-r--r--   0 kisonho    (501) staff       (20)      450 2023-07-26 18:16:57.000000 torchmanager-1.2b1/core/__init__.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:17:49.639606 torchmanager-1.2b1/core/devices/
+-rw-r--r--   0 kisonho    (501) staff       (20)      109 2023-07-26 18:16:57.000000 torchmanager-1.2b1/core/devices/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4870 2023-07-26 18:16:57.000000 torchmanager-1.2b1/core/devices/device.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      264 2023-07-26 18:16:57.000000 torchmanager-1.2b1/core/devices/protocols.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:17:49.639979 torchmanager-1.2b1/core/errors/
+-rw-r--r--   0 kisonho    (501) staff       (20)      153 2023-07-26 18:16:57.000000 torchmanager-1.2b1/core/errors/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      350 2023-07-26 18:16:57.000000 torchmanager-1.2b1/core/errors/runtime.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      669 2023-07-26 18:16:57.000000 torchmanager-1.2b1/core/errors/train.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2728 2023-07-26 18:16:57.000000 torchmanager-1.2b1/core/protocols.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:17:49.640230 torchmanager-1.2b1/core/random/
+-rw-r--r--   0 kisonho    (501) staff       (20)       44 2023-07-26 18:16:57.000000 torchmanager-1.2b1/core/random/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      876 2023-07-26 18:16:57.000000 torchmanager-1.2b1/core/random/seed.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      204 2023-07-26 18:16:57.000000 torchmanager-1.2b1/core/typing.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     1305 2023-07-26 18:16:57.000000 torchmanager-1.2b1/core/version.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:17:49.640470 torchmanager-1.2b1/core/view/
+-rw-r--r--   0 kisonho    (501) staff       (20)      439 2023-07-26 18:16:57.000000 torchmanager-1.2b1/core/view/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      313 2023-07-26 18:16:57.000000 torchmanager-1.2b1/core/view/protocols.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:17:49.641031 torchmanager-1.2b1/lib/
+-rw-r--r--   0 kisonho    (501) staff       (20)      290 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)    10805 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/basic.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:17:49.642164 torchmanager-1.2b1/lib/callbacks/
+-rw-r--r--   0 kisonho    (501) staff       (20)      476 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/callbacks/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4255 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/callbacks/callback.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4542 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/callbacks/ckpt.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     3523 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/callbacks/dynamic.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     1608 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/callbacks/early_stop.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4611 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/callbacks/experiment.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2224 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/callbacks/lr.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2440 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/callbacks/tensorboard.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      810 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/compatibility.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:17:49.642392 torchmanager-1.2b1/lib/configs/
+-rw-r--r--   0 kisonho    (501) staff       (20)       26 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/configs/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2836 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/configs/basic.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:17:49.642612 torchmanager-1.2b1/lib/data/
+-rw-r--r--   0 kisonho    (501) staff       (20)       69 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/data/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     6866 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/data/dataset.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:17:49.642821 torchmanager-1.2b1/lib/data/utils/
+-rw-r--r--   0 kisonho    (501) staff       (20)       35 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/data/utils/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2483 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/data/utils/sliding.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:17:49.643370 torchmanager-1.2b1/lib/losses/
+-rw-r--r--   0 kisonho    (501) staff       (20)      156 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/losses/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     5386 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/losses/cross_entropy.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     1044 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/losses/dice.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     5757 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/losses/loss.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     3108 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/losses/mse.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:17:49.643994 torchmanager-1.2b1/lib/metrics/
+-rw-r--r--   0 kisonho    (501) staff       (20)      238 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/metrics/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     3056 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/metrics/accuracy.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2126 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/metrics/conf_met.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4185 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/metrics/fid.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     2182 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/metrics/iou.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4000 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/metrics/metric.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     9413 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/testing.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:17:49.644354 torchmanager-1.2b1/lib/train/
+-rw-r--r--   0 kisonho    (501) staff       (20)      164 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/train/__init__.py
+-rw-r--r--   0 kisonho    (501) staff       (20)     4964 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/train/checkpoint.py
+-rw-r--r--   0 kisonho    (501) staff       (20)      694 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/train/learning_rate.py
+-rw-r--r--   0 kisonho    (501) staff       (20)    14905 2023-07-26 18:16:57.000000 torchmanager-1.2b1/lib/training.py
+-rw-r--r--   0 kisonho    (501) staff       (20)       38 2023-07-26 18:17:49.645262 torchmanager-1.2b1/setup.cfg
+-rw-r--r--   0 kisonho    (501) staff       (20)     1638 2023-07-26 18:17:17.000000 torchmanager-1.2b1/setup.py
+drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:17:49.644947 torchmanager-1.2b1/torchmanager.egg-info/
+-rw-r--r--   0 kisonho    (501) staff       (20)     2109 2023-07-26 18:17:49.000000 torchmanager-1.2b1/torchmanager.egg-info/PKG-INFO
+-rw-r--r--   0 kisonho    (501) staff       (20)     1238 2023-07-26 18:17:49.000000 torchmanager-1.2b1/torchmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 kisonho    (501) staff       (20)        1 2023-07-26 18:17:49.000000 torchmanager-1.2b1/torchmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 kisonho    (501) staff       (20)       11 2023-07-26 18:17:49.000000 torchmanager-1.2b1/torchmanager.egg-info/requires.txt
+-rw-r--r--   0 kisonho    (501) staff       (20)       31 2023-07-26 18:17:49.000000 torchmanager-1.2b1/torchmanager.egg-info/top_level.txt
```

### Comparing `torchmanager-1.1.5/LICENSE` & `torchmanager-1.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.5/torchmanager/basic.py` & `torchmanager-1.2b1/lib/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from torchmanager_core import torch, Version, _raise, API_VERSION, VERSION as CURRENT_VERSION
+from torchmanager_core import torch, _raise, API_VERSION, VERSION as CURRENT_VERSION
 from torchmanager_core.typing import Any, Collection, Dict, Generic, Module, Optional, OrderedDict, Self, Tuple, Union
 
 from .compatibility import convert
-from .losses import Loss, MultiLosses, MultiOutputsLosses, ParallelLoss
+from .losses import Loss, MultiLosses, ParallelLoss
 from .metrics import Metric
 from .train import Checkpoint
 
 
 class BaseManager(Generic[Module]):
     """
     The basic manager
@@ -43,15 +43,15 @@
         - raw_model: A non-paralleled target `torch.nn.Module` model
     """
     # properties
     loss_fn: Optional[Union[Loss, ParallelLoss]]
     metric_fns: Dict[str, Metric]
     model: Module
     optimizer: Optional[torch.optim.Optimizer]
-    version: Version
+    version: str
 
     @property
     def compiled(self) -> bool:
         return True if self.loss_fn is not None and self.optimizer is not None else False
 
     @property
     def raw_loss_fn(self) -> Optional[Loss]:
@@ -93,33 +93,30 @@
 
         - Parameters:
             - loss_fn: An optional `Loss` object to calculate the loss for single loss or a `dict` of losses in `Loss` with their names in `str` to calculate multiple losses
             - metrics: An optional `dict` of metrics with a name in `str` and a `Metric` object to calculate the metric
             - optimizer: An optional `torch.optim.Optimizer` to train the model
         """
         # initialize loss
-        if isinstance(loss_fn, MultiOutputsLosses) and len(loss_fn.losses) > 1:
-            loss_fn_mapping: Dict[str, Loss] = {f"{name}_loss": fn for name, fn in loss_fn.losses.items()}  # type: ignore
-            self.metric_fns.update(loss_fn_mapping)
-        elif isinstance(loss_fn, dict):
+        if isinstance(loss_fn, dict):
             loss_fn_mapping: Dict[str, Loss] = {f"{name}_loss": fn for name, fn in loss_fn.items()}
             self.metric_fns.update(loss_fn_mapping)
             loss_fn = MultiLosses([l for l in loss_fn_mapping.values()])
         self.loss_fn = loss_fn
 
         # initialize metrics
         for name, fn in metrics.items():
             self.metric_fns[name] = fn
 
         # initialize optimizer
         self.optimizer = optimizer
 
     def compile(self, optimizer: torch.optim.Optimizer, loss_fn: Union[Loss, Dict[str, Loss]], metrics: Dict[str, Metric] = {}) -> None:
         """
-        Compiles the manager
+        Recompiles the manager with optimizer loss function and metrics
 
         - Parameters:
             - loss_fn: A `Loss` object to calculate the loss for single loss or a `dict` of losses in `Loss` with their names in `str` to calculate multiple losses
             - metrics: A `dict` of metrics with a name in `str` and a `Metric` object to calculate the metric
             - optimizer: A `torch.optim.Optimizer` to train the model
         """
         self._compile(optimizer, loss_fn, metrics)
@@ -215,19 +212,19 @@
         Convert the current manager to a checkpoint
 
         - Returns: A `Checkpoint` with its model as the current manager
         """
         ckpt = Checkpoint(self)
         return ckpt
 
-    def unpack_data(self, data: Collection[Any]) -> Tuple[Any, Any]:
+    def unpack_data(self, data: Collection) -> Tuple[Any, Any]:
         """
         Unpacks data to input and target
 
         - Parameters:
-            - data: A `Collection` of `Any` kind of data objects
+            - data: `Any` kind of data object
         - Returns: A `tuple` of `Any` kind of input and `Any` kind of target
         """
         if len(data) >= 2:
             return tuple(data)
         else:
             return NotImplemented
```

### Comparing `torchmanager-1.1.5/torchmanager/callbacks/callback.py` & `torchmanager-1.2b1/lib/callbacks/callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from torchmanager_core import abc, torch
 from torchmanager_core.protocols import Frequency
 from torchmanager_core.typing import Any, Dict, Optional
 
-
 class Callback:
     """An empty basic training callback"""
 
     def on_batch_end(self, batch: int, summary: Dict[str, float] = {}) -> None:
         """
         The callback when batch ends
 
@@ -125,14 +124,14 @@
             self._update(result)
             self.current_step += 1
 
     @abc.abstractmethod
     def step(self, summary: Dict[str, float], val_summary: Optional[Dict[str, float]] = None) -> Any:
         """
         Abstract method to step the callback
-
+        
         - Parameters:
             - summary: A `dict` of training summary with name in `str` and value in `float`
             - val_summary: An optional `dict` of validation summary with name in `str` and value in `float`
         - Returns: An `Any` type of result for the new step
         """
         return NotImplemented
```

### Comparing `torchmanager-1.1.5/torchmanager/callbacks/ckpt.py` & `torchmanager-1.2b1/lib/callbacks/ckpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,84 +3,76 @@
 from torchmanager_core.typing import Any, Dict, Generic, Optional, TypeVar
 
 from ..train import Checkpoint as Ckpt
 from .callback import Callback
 
 T = TypeVar('T', bound=StateDictLoadable)
 
-
 class _Checkpoint(Callback, Generic[T]):
     """
     The callback to save the last checkpoint during training
 
     * extends: `.Callback
 
     - Properties:
         - ckpt_path: A `str` of checkpoint path
     """
     __ckpt_path: str
-    __checkpoint: Ckpt[T]
+    _checkpoint: Ckpt[T]
 
     @property
     def ckpt_path(self) -> str:
         return self.__ckpt_path
 
     @ckpt_path.setter
     def ckpt_path(self, p: str) -> None:
         self.__ckpt_path = os.path.normpath(p)
 
-    @property
-    def checkpoint(self) -> Ckpt[T]:
-        return self.__checkpoint
-
     def __init__(self, model: T, ckpt_path: str, **kwargs: Any) -> None:
         """
         Constructor
 
         - Parameters:
             - model: Any type of model to be saved
             - ckpt_path: A `str` of the checkpoint path
             - **kwargs: Other arguments in `Checkpoint` constructor
         """
         super().__init__()
-        self.__checkpoint = Ckpt(model, **kwargs)
+        self._checkpoint = Ckpt(model, **kwargs)
         self.ckpt_path = os.path.normpath(ckpt_path)
 
     def on_epoch_end(self, epoch: int, summary: Dict[str, float] = ..., val_summary: Optional[Dict[str, float]] = ...) -> None:
-        self.checkpoint.save(epoch, self.ckpt_path)
-
+        self._checkpoint.save(epoch, self.ckpt_path)
 
 class LastCheckpoint(_Checkpoint[T]):
     """
     Last checkpoint with frequency control support
 
     * extends: `_Checkpoint`
-
+    
     - Properties:
         - freq: An `int` of checkpoint epoch frequency
     """
     __freq: int
 
     @property
     def freq(self) -> int:
         return self.__freq
-
+    
     @freq.setter
     def freq(self, f: int) -> None:
         assert f > 0, _raise(ValueError(f"Frequency must be a positive number, got {f}. "))
         self.__freq = f
 
     def __init__(self, model: T, ckpt_path: str, freq: int = 1, **kwargs: Any) -> None:
         super().__init__(model, ckpt_path, **kwargs)
         self.freq = freq
 
     def on_epoch_end(self, epoch: int, summary: Dict[str, float] = ..., val_summary: Optional[Dict[str, float]] = ...) -> None:
-        if epoch % self.freq == 0:
-            super().on_epoch_end(epoch, summary, val_summary)
-
+        if epoch % self.freq == 0: super().on_epoch_end(epoch, summary, val_summary)
 
 class BestCheckpoint(_Checkpoint[T]):
     """
     The callback to save the latest checkpoint for each epoch
 
     * extends: `_Checkpoint`
 
@@ -91,15 +83,15 @@
     """
     # properties
     best_score: float
     load_best: bool
     monitor: str
     monitor_type: MonitorType
 
-    def __init__(self, monitor: str, model: T, ckpt_path: str, load_best: bool = False, monitor_type: MonitorType = MonitorType.MAX, **kwargs: Any) -> None:
+    def __init__(self, monitor: str, model: T, ckpt_path: str, load_best: bool = False, monitor_type: MonitorType=MonitorType.MAX, **kwargs: Any) -> None:
         """
         Constructor
 
         - Parameters:
             - monitor: A `str` of monitored metric
             - monitor_type: A `MonitorType` of either `MIN` of `MAX` mode for the best model
         """
@@ -126,13 +118,10 @@
         if self.load_best:
             # load checkpoint
             best_ckpt: Ckpt[StateDictLoadable] = Ckpt.from_saved(self.ckpt_path)
 
             # load to model
             if isinstance(best_ckpt.model, ModelContainer):
                 ckpt_model = best_ckpt.model.model
-            else:
-                ckpt_model = best_ckpt.model
-            try:
-                model.load_state_dict(ckpt_model.state_dict())
-            except:
-                raise TypeError(f"Reload best checkpoint to model failed: supposed to have {type(model)} in checkpoint, got {type(ckpt_model)}.")
+            else: ckpt_model = best_ckpt.model
+            try: model.load_state_dict(ckpt_model.state_dict())
+            except: raise TypeError(f"Reload best checkpoint to model failed: supposed to have {type(model)} in checkpoint, got {type(ckpt_model)}.")
```

### Comparing `torchmanager-1.1.5/torchmanager/callbacks/dynamic.py` & `torchmanager-1.2b1/lib/callbacks/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from torchmanager_core.protocols import Frequency, SummaryWriteble, Weighted
 from torchmanager_core.typing import Any, Callable, Generic, Optional, SupportsFloat, TypeVar
 
 from .callback import FrequencyCallback
 
 W = TypeVar('W', bound=Weighted)
 
-
 class DynamicWeight(FrequencyCallback, abc.ABC, Generic[W]):
     '''
     An abstract dynamic weight callback that set weight dynamically
 
     * extends: `.callback.FrequencyCallback`
     * abstract class that needs implementation of `step` method
     '''
@@ -55,19 +54,18 @@
             w = self._weighted.weight
             result = {'train': w}
             self._writer.add_scalars(self._key, result, epoch)
 
         # update
         super().on_epoch_end(epoch, *args, **kwargs)
 
-
 class LambdaDynamicWeight(DynamicWeight[W], Generic[W]):
     '''
     A dynamic weight callback that set weight dynamically with lambda function
-
+    
     * extends: `DynamicWeight`
 
     Targeting to any object that performs to `.protocol.Weighted` protocol:
     >>> from torchmanager import losses
     >>> loss_fn = losses.Loss(...) # where `torchmanager.losses.Loss` performs to `.protocols.Weighted` protocol
 
     Passing defined functions into the `DynamicWeight` callback:
@@ -89,8 +87,8 @@
     def _lambda_fn(self) -> Callable[[int], Any]: return self.__lambda_fn
 
     def __init__(self, fn: Callable[[int], Any], weighted: W, freq: Frequency = Frequency.EPOCH, writer: Optional[SummaryWriteble] = None, name: Optional[str] = None) -> None:
         super().__init__(weighted, freq, writer, name)
         self.__lambda_fn = fn
 
     def step(self, *args: Any, **kwargs: Any) -> Any:
-        return self._lambda_fn(self.current_step)
+        return self._lambda_fn(self.current_step)
```

### Comparing `torchmanager-1.1.5/torchmanager/callbacks/early_stop.py` & `torchmanager-1.2b1/lib/callbacks/early_stop.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from torchmanager_core import errors, sys
 from torchmanager_core.typing import Dict, List, Optional
 
 from .ckpt import Callback, MonitorType
 
-
 class EarlyStop(Callback):
     '''
     The early stop callback that raises `StopTraining` error during the training if monitored metric not improved for several steps
 
     - Properties:
         - monitor: A `str` of monitored metric
         - monitor_type: A `MonitorType` of either `MIN` of `MAX` mode for the best model
@@ -27,21 +26,15 @@
         self.__metrics = [sys.float_info.min if monitor_type == MonitorType.MAX else sys.float_info.max]
         self.monitor = monitor
         self.monitor_type = monitor_type
         self.steps = steps
 
     def on_epoch_end(self, epoch: int, summary: Dict[str, float] = ..., val_summary: Optional[Dict[str, float]] = None) -> None:
         # load monitoring value
-        summary = val_summary if val_summary is not None else summary
+        if val_summary is not None: summary = val_summary
         monitoring_value = summary[self.monitor]
 
         # compare with recorded metrics
-        value = self._metrics[0]
-        if self.monitor_type == MonitorType.MAX and monitoring_value <= value and len(self._metrics) > self.steps:
-            raise errors.StopTraining(epoch)
-        elif self.monitor_type == MonitorType.MAX and monitoring_value > value:
-            self._metrics.clear()
-        elif self.monitor_type == MonitorType.MIN and monitoring_value >= value and len(self._metrics) > self.steps:
-            raise errors.StopTraining(epoch)
-        elif self.monitor_type == MonitorType.MIN and monitoring_value < value:
-            self._metrics.clear()
-        self._metrics.append(monitoring_value)
+        max_value = max(self.__metrics)
+        if monitoring_value < max_value and len(self._metrics) >= self.steps: raise errors.StopTraining(epoch)
+        elif len(self._metrics) >= self.steps: self._metrics.pop()
+        self._metrics.insert(0, monitoring_value)
```

### Comparing `torchmanager-1.1.5/torchmanager/callbacks/experiment.py` & `torchmanager-1.2b1/lib/callbacks/experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from torchmanager_core import os
+from torchmanager_core import os, view
 from torchmanager_core.typing import Any, Dict, Generic, List, TypeVar, Union
 from torchmanager_core.protocols import MonitorType, StateDictLoadable
-from torchmanager_core.view import logging
 
 from .callback import Callback
 from .ckpt import BestCheckpoint, LastCheckpoint
 from .tensorboard import TensorBoard
 
 T = TypeVar('T', bound=StateDictLoadable)
 
-
 class Experiment(Callback, Generic[T]):
     """
     The tensorboard callback that wraps last and best checkpoints in `checkpoints` folder by `last.model` and `best_*.model` with tensorboard logs in `data` folder together into a wrapped *.exp file
 
     * extends: `.callback.Callback`
     * requires: `tensorboard` package
 
@@ -22,33 +20,32 @@
         - last_ckpt: A `.ckpt.LastCheckpoint` callback that records the last checkpoint
         - tensorboard: A `.ckpt.TensorBoard` callback that records data to tensorboard
     """
     best_ckpts: List[BestCheckpoint[T]]
     last_ckpt: LastCheckpoint[T]
     tensorboard: TensorBoard
 
-    def __init__(self, experiment: str, model: T, monitors: Union[Dict[str, MonitorType], List[str]] = {}, show_verbose: bool = True) -> None:
+    def __init__(self, experiment: str, model: T, monitors: Union[Dict[str, MonitorType], List[str]]={}, show_verbose: bool = True) -> None:
         """
         Constructor
 
         - Parameters:
             - experiment: A `str` of target folder for the experiment
             - model: A target model to be tracked during experiment in `T`
             - monitors: A `list` of metric name if all monitors are using `MonitorType.MAX` to track, or `dict` of metric name to be tracked for the best checkpoint in `str` and the `.ckpt.MonitorType` to track as values
             - show_verbose: A `bool` flag of if showing loggins in console
         """
         # call super constructor
         experiment = os.path.normpath(experiment)
-        if not experiment.endswith(".exp"):
-            experiment += ".exp"
+        if not experiment.endswith(".exp"): experiment += ".exp"
         experiment_dir = os.path.join("experiments", experiment)
         os.makedirs(experiment_dir, exist_ok=True)
         log_dir = os.path.join(experiment_dir, "data")
         ckpt_path = os.path.join(experiment_dir, "checkpoints")
-
+        
         # initial checkpoints
         self.best_ckpts = []
         last_ckpt_path = os.path.join(ckpt_path, "last.model")
         self.last_ckpt = LastCheckpoint(model, last_ckpt_path)
         self.tensorboard = TensorBoard(log_dir)
 
         # initialize best checkpoints according to monitors
@@ -57,28 +54,23 @@
             best_ckpt_path = os.path.join(ckpt_path, f"best_{m}.model")
             best_ckpt = BestCheckpoint(m, model, best_ckpt_path, monitor_type=mode)
             self.best_ckpts.append(best_ckpt)
 
         # initialize logging
         log_file = os.path.basename(experiment.replace(".exp", ".log"))
         log_path = os.path.join(experiment_dir, log_file)
-        logger = logging.getLogger("torchmanager")
-        logger.handlers.clear()
-        logger.setLevel(logging.INFO)
-        file_handler = logging.FileHandler(log_path)
-        formatter = logging.Formatter("%(message)s")
-        file_handler.setFormatter(formatter)
-        logger.addHandler(file_handler)
+        os.makedirs(experiment_dir, exist_ok=True)
+        formatter = view.set_log_path(log_path)
 
         # initialize console
         if show_verbose:
-            console = logging.StreamHandler()
-            console.setLevel(logging.INFO)
+            console = view.logging.StreamHandler()
+            console.setLevel(view.logging.INFO)
             console.setFormatter(formatter)
-            logger.addHandler(console)
+            view.logger.addHandler(console)
 
     def on_train_start(self, initial_epoch: int = 0) -> None:
         for best_ckpt in self.best_ckpts:
             best_ckpt.on_batch_start(initial_epoch)
         self.last_ckpt.on_train_start(initial_epoch)
         self.tensorboard.on_train_start(initial_epoch)
 
@@ -100,8 +92,8 @@
         self.last_ckpt.on_epoch_end(*args, **kwargs)
         self.tensorboard.on_epoch_end(*args, **kwargs)
 
     def on_epoch_start(self, *args: Any, **kwargs: Any) -> None:
         for best_ckpt in self.best_ckpts:
             best_ckpt.on_epoch_start(*args, **kwargs)
         self.last_ckpt.on_epoch_start(*args, **kwargs)
-        self.tensorboard.on_epoch_start(*args, **kwargs)
+        self.tensorboard.on_epoch_start(*args, **kwargs)
```

### Comparing `torchmanager-1.1.5/torchmanager/callbacks/lr.py` & `torchmanager-1.2b1/lib/callbacks/lr.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from torchmanager_core.typing import Any, Dict, Generic, Optional, TypeVar
 
 from .callback import FrequencyCallback
 
 Scheduler = TypeVar("Scheduler", bound=torch.optim.lr_scheduler._LRScheduler)
 Writer = TypeVar("Writer", bound=SummaryWriteble)
 
-
 class LrSchedueler(FrequencyCallback, Generic[Scheduler]):
     """
     The callback to step learning rate scheduler
 
     * extends: `FrequencyCallback`
 
     - Parameters:
@@ -45,24 +44,23 @@
     def on_epoch_end(self, epoch: int, summary: Dict[str, float], val_summary: Optional[Dict[str, Any]] = None) -> None:
         # get lr summary
         lr_summary = {}
         lr_list = self._scheduler.get_last_lr()
         if len(lr_list) > 1:
             for i, lr in enumerate(lr_list):
                 lr_summary[f'{self._name}_{i}'] = lr
-        else:
-            lr_summary[self._name] = lr_list[0]
+        else: lr_summary[self._name] = lr_list[0]
 
         # write results to Tensorboard
         if self._writer is not None:
             # record summary
             for key in lr_summary.keys():
                 result: Dict[str, float] = {}
                 result["train"] = lr_summary[key]
                 self._writer.add_scalars(key, result, epoch)
 
         # update lr scheduler
         summary.update(lr_summary)
         super().on_epoch_end(epoch, summary, val_summary)
 
     def step(self, *args: Any, **kwargs: Any) -> Any:
-        self._scheduler.step()
+        self._scheduler.step()
```

### Comparing `torchmanager-1.1.5/torchmanager/callbacks/tensorboard.py` & `torchmanager-1.2b1/lib/callbacks/tensorboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from torchmanager_core import tensorboard, torch
 from torchmanager_core.typing import Dict, Optional, Set, Tuple
 from torchmanager_core.protocols import Frequency
 
 from .callback import FrequencyCallback
 
-
 class TensorBoard(FrequencyCallback):
     """
     The callback to record summary to tensorboard for each epoch
 
     * extends: `.callback.FrequencyCallback`
     * requires: `tensorboard` package
 
@@ -56,11 +55,10 @@
             if val_summary is not None and key in val_summary:
                 r["val"] = val_summary[key]
             self.writer.add_scalars(key, r, self.current_step + 1)
 
     def step(self, summary: Dict[str, float], val_summary: Optional[Dict[str, float]] = None) -> Tuple[Set[str], Dict[str, float], Optional[Dict[str, float]]]:
         # fetch keys
         keys = list(summary.keys())
-        if val_summary is not None:
-            keys += list(val_summary.keys())
+        if val_summary is not None: keys += list(val_summary.keys())
         keys = set(keys)
-        return keys, summary, val_summary
+        return keys, summary, val_summary
```

### Comparing `torchmanager-1.1.5/torchmanager/compatibility.py` & `torchmanager-1.2b1/lib/compatibility.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,21 @@
-from torchmanager_core import Version
 from torchmanager_core.typing import Any, Optional, TypeVar
 
 from .losses import KLDiv
 from .metrics import Accuracy, MAE, Reduction
 
 T = TypeVar("T")
 
 
-def convert(obj: T, from_version: Optional[Any] = None) -> T:
+def convert(obj: T, from_version: Optional[str] = None) -> T:
     """
     Convert an object from old version of torchmanager to the latest one.
     """
-    # format version
-    v = Version(from_version) if from_version is not None else Version("v1.0")
-
-    # Return if None
-    if obj is None:
-        return obj
-
-    if v < Version("v1.1"): # convert from 1.0
+    # convert from 1.0 (from_version = None)
+    if from_version is None and obj is not None:
         # convert KLDiv
         if isinstance(obj, KLDiv) and not hasattr(obj, "replace_nan"):
             obj.replace_nan = False
         elif isinstance(obj, KLDiv) and not hasattr(obj, "_t"):
             obj._t = None
 
         # convert Accuracy and MAE
```

### Comparing `torchmanager-1.1.5/torchmanager/data/dataset.py` & `torchmanager-1.2b1/lib/data/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     * Used as a combination of `torch.utils.data.Dataset` and `torch.utils.data.DataLoader`
 
     >>> from torchmanager import Manager
     >>> class SomeDataset(Dataset):
     ...    @property
     ...    def unbatched_size(self) -> int: ...
     ...
+    ...    def __init__(self, ...,  batch_size: int, device: torch.device = devices.CPU) -> None: ...
     ...    def __getitem__(self, index: Any) -> Any: ...
     >>> dataset = SomeDataset(..., batch_size)
     >>> manager = Manager(...)
     >>> manager.fit(dataset, ...)
 
     - Properties:
         - batch_size: An `int` of batch size for the current dataset
@@ -96,17 +97,18 @@
         return NotImplemented
 
     def __iter__(self) -> Iterator[T]:
         # initialize devices
         cpu_count = os.cpu_count()
         if cpu_count is None:
             cpu_count = 0
+        device = self.device
 
         # initialize loader
-        if self.device != devices.CPU:
+        if device != devices.CPU:
             data_loader = DataLoader(self, batch_size=self.batch_size, drop_last=self.drop_last, shuffle=self.shuffle, num_workers=cpu_count, pin_memory=True, pin_memory_device=str(self.device))
         else:
             data_loader = DataLoader(self, batch_size=self.batch_size, drop_last=self.drop_last, shuffle=self.shuffle, num_workers=cpu_count)
 
         # yield data
         for data in data_loader:
             yield self.unpack_data(data)
@@ -120,20 +122,18 @@
         """
         Unpacks a single data into inputs and targets
 
         - Parameters:
             - data: `Any` kind of single data
         - Returns: `Any` kind of inputs with type `T`
         """
-        if isinstance(data, torch.Tensor) or isinstance(data, dict):
-            return data, data  # type: ignore # suppose for unsupervised reconstruction or a dictionary of packed data
-        if isinstance(data, Sequence) and len(data) == 2:
-            return data[0], data[1]  # type: ignore # suppose for supervised
+        if isinstance(data, Sequence):
+            return data[0], data[1] if len(data) >= 2 else NotImplemented # type: ignore
         else:
-            return NotImplemented  # unknown type of dataset
+            return NotImplemented
 
 
 def batched(fn: Callable[..., _Dataset]):
     """
     Wrap a loading PyTorch dataset function into a loading dataset function
 
     Use as decorator with a function:
```

### Comparing `torchmanager-1.1.5/torchmanager/data/sliding.py` & `torchmanager-1.2b1/lib/data/utils/sliding.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 from itertools import product
 from torchmanager_core import torch, _raise
 from torchmanager_core.typing import List, Tuple
 
-
 def sliding_window(image: torch.Tensor, window_size: Tuple[int, ...], stride: Tuple[int, ...]) -> torch.Tensor:
     """
-    Extract sliding windows from a multi-dimensional `torch.Tensor`.
+    Extract sliding windows from a multi-dimensional PyTorch tensor.
 
     - Parameters:
         - image: The input image `torch.Tensor`. Can have any number of dimensions.
         - window_size: A `tuple` of the size of the sliding window in `int` to extract from the image, must have the same number of dimensions as the input image tensor.
         - stride: A `tuple` of the stride of the sliding window in `int`, must have the same number of dimensions as the input image tensor.
-    Returns: A `list` of `torch.Tensor`, where each tensor corresponds to a sliding window extracted from the input image tensor.
-    Raises: `ValueError` if the window size or stride are not valid for the input image tensor.
+
+    Returns: A list of PyTorch tensors, where each tensor corresponds to a
+            sliding window extracted from the input image tensor.
+
+    Raises: ValueError: If the window size or stride are not valid for the input image tensor.
 
     Example:
     ```
     >>> image = torch.randn(3, 224, 224)
     >>> window_size = (64, 64)
     >>> stride = (32, 32)
     >>> windows = sliding_window(image, window_size, stride)
     >>> windows.shape[0]
-    36
+    49
     ```
     """
-    # initialize
-    assert len(window_size) == len(stride), _raise(ValueError(f"Window size dimension ({len(window_size)}) and stride dimension ({stride}) must be the same."))
-    stride_dims: List[int] = []
-    windows: List[torch.Tensor] = []
-    window_dims: List[int] = []
+    # check inputs
+    assert len(window_size) == len(image.shape) == len(image.shape), _raise(ValueError(f"Window size dimension ({len(window_size)}) and stride dimension ({stride}) must be the same of image ({len(image.shape)})."))
 
     # Calculate number of windows in each dimension
-    for dim_size, window_dim, stride_dim in zip(image.shape[1:], window_size, stride):
+    window_dims: List[int] = []
+    stride_dims: List[int] = []
+    for dim_size, window_dim, stride_dim in zip(image.shape, window_size, stride):
         num_windows = (dim_size - window_dim) // stride_dim + 1
         window_dims.append(num_windows)
         stride_dims.append(stride_dim)
-
+    
+    # Create a list to hold the windows
+    windows: List[torch.Tensor] = []
+    
     # Iterate over each window
     window_starts = product(*[range(num_windows) for num_windows in window_dims])
-    for indices in window_starts:
+    for starts in window_starts:
         # Calculate the starting coordinates of the window
-        indices = (slice(None),) + tuple(slice(i, i+ws) for i, ws in zip(indices, window_size))
-
+        starts = torch.tensor(starts)
+        window_starts = starts * torch.tensor(stride_dims)
+        window_ends = window_starts + torch.tensor(window_size)
+        
         # Extract the window from the image
-        window = image[indices]
-
+        window = image[tuple(slice(s, e) for s, e in zip(window_starts, window_ends))]
+        
         # Add the window to the list
         windows.append(window.unsqueeze(0))
-    return torch.cat(windows)
+    return torch.cat(windows)
```

### Comparing `torchmanager-1.1.5/torchmanager/losses/cross_entropy.py` & `torchmanager-1.2b1/lib/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.5/torchmanager/losses/dice.py` & `torchmanager-1.2b1/lib/losses/dice.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,36 +6,30 @@
 
 class Dice(Loss):
     """
     The dice loss
 
     * extends: `.loss.Loss`
     """
-    _dim: int
-    _smooth: float
+    _smooth: int
     _softmax_input: bool
 
-    def __init__(self, dim: int = 1, smooth: float = 1e-6, softmax_input: bool = True, **kwargs: Any) -> None:
+    def __init__(self, smooth: int = 1, softmax_input: bool = True, **kwargs: Any) -> None:
         """
         Constructor
 
         - Parameters:
-            - dim: An `int` of class dimension
-            - smooth: An `float` of smooth value to avoid dividing zero
+            - smooth: An `int` of smooth value to avoid dividing zero
             - softmax_input: A `bool` flag of if softmax the input
         """
         super().__init__(**kwargs)
-        self._dim = dim
         self._smooth = smooth
         self._softmax_input = softmax_input
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         # softmax activation
-        num_classes = input.shape[self._dim]
-        input = input.softmax(self._dim).view(-1) if self._softmax_input else input.view(-1)
-        target = F.one_hot(target.view(-1), num_classes)
-        assert isinstance(target, torch.Tensor), "Target is not a valid `torch.Tensor`."
+        input = F.softmax(input).view(-1) if self._softmax_input else input.view(-1)
         target = target.view(-1)
 
         # calculate dice
         intersection = input * target
         return (2 * intersection.sum() + self._smooth) / (input.sum() + target.sum() + self._smooth)
```

### Comparing `torchmanager-1.1.5/torchmanager/losses/loss.py` & `torchmanager-1.2b1/lib/losses/loss.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from torchmanager_core import torch, _raise, deprecated
+from torchmanager_core import torch, _raise
 from torchmanager_core.typing import Any, Callable, Dict, List, Optional
 
 from ..metrics import Metric, Reduction
 
 
 class Loss(Metric):
     """
@@ -51,15 +51,14 @@
         """
         super().__init__(loss_fn, target=target)
         self.weight = weight
 
     def __call__(self, input: Any, target: Any) -> torch.Tensor:
         m: torch.Tensor = super().__call__(input, target) * self.weight
         self._results[-1] *= self.weight
-        assert m.numel() == 1, _raise(TypeError(f"The returned loss must be a scalar tensor, got shape {m.shape}"))
         return m
 
     def forward(self, input: Any, target: Any) -> torch.Tensor:
         return super().forward(input, target)
 
 
 class MultiLosses(Loss):
@@ -114,52 +113,14 @@
     def reset(self) -> None:
         for fn in self.losses:
             assert isinstance(fn, Loss), _raise(TypeError(f"Function {fn} is not a Loss object."))
             fn.reset()
         return super().reset()
 
 
-class MultiOutputsLosses(Loss):
-    """
-    A loss with multiple losses for multiple outputs
-
-    * extends: `.Loss`
-    * [Depreciation Warning]: `MultiOutputsLosses` has been deprecated in v1.1.0 and will be removed in v1.2.0, use `MultiLosses` along with `target` parameter for each loss instead.
-
-    - Properties:
-        - losses: A `dict` of loss metrics in `Metric`
-    """
-
-    __losses: torch.nn.ModuleDict
-
-    @property
-    def losses(self) -> torch.nn.ModuleDict:
-        return self.__losses
-
-    @deprecated("v1.1.0", "v1.2.0")
-    def __init__(self, loss_fns: Dict[str, Loss]) -> None:
-        super().__init__()
-        assert len(loss_fns) > 0, "The loss dictionary should not be empty."
-        self.__losses = torch.nn.ModuleDict(loss_fns)
-
-    def forward(self, input: Dict[str, torch.Tensor], target: Dict[str, torch.Tensor]) -> torch.Tensor:
-        # initilaize
-        loss = 0
-
-        # loop for losses
-        for k, fn in self.losses.items():
-            assert isinstance(fn, Loss), _raise(TypeError(f"Function {fn} is not a Loss object."))
-            l = fn(input[k], target[k])
-            loss += l
-
-        # return loss
-        assert isinstance(loss, torch.Tensor), _raise(TypeError("The total loss is not a valid `torch.Tensor`."))
-        return loss
-
-
 class ParallelLoss(Loss):
     """
     A data parallel loss function
 
     * extends: `torch.nn.parallel.DataParallel`
     * implements: `torchmanager_core.protocols.Resulting`
```

### Comparing `torchmanager-1.1.5/torchmanager/losses/mse.py` & `torchmanager-1.2b1/lib/losses/mse.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,32 @@
             return loss.mean()
         elif self.reduction == Reduction.SUM:
             return loss.sum()
         else:
             return loss
 
 
+class MAE(_ReductableLoss):
+    """
+    The MSE loss
+    """
+    def __init__(self, reduction: Reduction = Reduction.MEAN, replace_nan: bool = False, target: Optional[str] = None, weight: float = 1) -> None:
+        """
+        Constructor
+
+        - Parameters:
+            - reduction: A `.loss.Reduction` of reduction method
+            - replace_nan: A `boolean` flag of if replacing nan results to zeros
+            - target: An optional `str` of target name in `input` and `target` during direct calling
+            - weight: A `float` of the loss weight
+        """
+        l1 = torch.nn.L1Loss(reduction="none")
+        super().__init__(l1, reduction=reduction, replace_nan=replace_nan, target=target, weight=weight)
+
+
 class MSE(_ReductableLoss):
     """
     The MSE loss
     """
     def __init__(self, reduction: Reduction = Reduction.MEAN, replace_nan: bool = False, target: Optional[str] = None, weight: float = 1) -> None:
         """
         Constructor
```

### Comparing `torchmanager-1.1.5/torchmanager/metrics/accuracy.py` & `torchmanager-1.2b1/lib/metrics/accuracy.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,24 +34,14 @@
 
     - Properties:
         - dim: An `int` of the probability dim index for the input
     """
 
     _dim: int
 
-    @property
-    @deprecated("v1.1.0", "v1.2.0")
-    def dim(self) -> int:
-        return self._dim
-
-    @dim.setter
-    @deprecated("v1.1.0", "v1.2.0")
-    def dim(self, dim: int) -> None:
-        self._dim = dim
-
     def __init__(self, dim: int = -1, target: Optional[str] = None) -> None:
         """
         Constructor
 
         - Parameters:
             - dim: An `int` of the classification dimension
             - target: A `str` of target name in `input` and `target` during direct calling
```

### Comparing `torchmanager-1.1.5/torchmanager/metrics/iou.py` & `torchmanager-1.2b1/lib/metrics/iou.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from torchmanager_core import torch, _raise, deprecated
+from torchmanager_core import torch, _raise
 from torchmanager_core.typing import Optional
-from torchmanager_core.view import warnings
 
 from .conf_met import ConfusionMetrics
 from .metric import Metric
 
 
 class InstanceIoU(ConfusionMetrics):
     """
@@ -14,15 +13,19 @@
     """
 
     def __init__(self, num_classes: int, target: Optional[str] = None) -> None:
         super().__init__(num_classes, target=target)
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         # argmax for input
-        iou = torch.diag(input) / (input.sum(1) + input.sum(0) - torch.diag(input))
+        input = input.argmax(1).to(target.dtype)
+
+        # calculate mean IoU
+        hist = super().forward(input, target)
+        iou = torch.diag(hist) / (hist.sum(1) + hist.sum(0) - torch.diag(hist))
         return iou.nanmean()
 
 
 class MeanIoU(Metric):
     """
     The mIoU metric for segmentation
 
@@ -36,31 +39,22 @@
     def __init__(self, dim: int = 1, smooth: float = 1e-4, threshold: float = 0, target: Optional[str] = None) -> None:
         """
         Constructor
 
         - Parameters:
             - dim: An `int` of class dimension
             - smooth: A `float` of smooth value to avoid zero devision
-            - threshold: A `float` of min mIoU threshold
-            - target: A `str` of target name in `input` and `target` during direct calling
         """
         super().__init__(target=target)
         assert dim > 0, _raise(ValueError(f"The dimension must be a positive number, got {dim}."))
         assert threshold >= 0 and threshold <= 1, _raise(ValueError(f"The threshold must be in range [0,1], got {threshold}."))
         self._dim = dim
         self._smooth = smooth
         self._threshold = threshold
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
-        input = input.argmax(self._dim) if input.shape[self._dim] > 1 else input > 0.5
+        input = input.argmax(self._dim)
         intersection = (input & target).float().sum()
         union = (input | target).float().sum()
         iou = (intersection + self._smooth) / (union + self._smooth)
         thresholded = torch.clamp(10 / (1 - self._threshold) * (iou - self._threshold), 0, 10).ceil() / 10
         return thresholded
-
-
-@deprecated("v1.1.0", "v1.2.0")
-class MIoU(InstanceIoU):
-    def __init__(self, num_classes: int, target: Optional[str] = None) -> None:
-        super().__init__(num_classes, target)
-        warnings.warn("The class `MIoU` has been renamed to `InstanceIoU` in v1.1.0, and will be removed in v1.2.0.", DeprecationWarning)
```

### Comparing `torchmanager-1.1.5/torchmanager/metrics/metric.py` & `torchmanager-1.2b1/lib/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.5/torchmanager/testing.py` & `torchmanager-1.2b1/lib/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from torch.utils.data import DataLoader
-from torchmanager_core import devices, errors, torch, view, _raise
+from torchmanager_core import devices, errors, torch, view, _raise, deprecated
 from torchmanager_core.protocols import Resulting
 from torchmanager_core.typing import Any, Collection, Dict, List, Module, Optional, Union
 
 from .basic import BaseManager
 from .data import Dataset
 from .losses import Loss, ParallelLoss
```

### Comparing `torchmanager-1.1.5/torchmanager/train/checkpoint.py` & `torchmanager-1.2b1/lib/train/checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,25 +56,25 @@
         # load checkpint dictionary
         ckpt: Dict[str, Any] = torch.load(ckpt_path, map_location=map_location)
 
         # load model
         if ckpt["save_weights_only"] is True:
             assert model is not None, _raise(TypeError("Model must be given to load this checkpoint because `save_weights_only` was set to be `True`."))
             state_dict: OrderedDict[str, Any] = ckpt["model"]
-            model.load_state_dict(state_dict=state_dict)
+            model.load_state_dict(state_dict)
             ckpt["model"] = model
         else:
             # remove data parallel wrap
             if isinstance(ckpt["model"], torch.nn.parallel.DataParallel):
                 ckpt["model"] = ckpt["model"].module
 
             # load model structure with checkpoint weights
             if model is not None:
                 saved_model: StateDictLoadable = ckpt["model"]  # type: ignore
-                model.load_state_dict(state_dict=OrderedDict(saved_model.state_dict()))
+                model.load_state_dict(OrderedDict(saved_model.state_dict()))
                 ckpt["model"] = model
         return cls(**ckpt)
 
     def save(self, epoch: int, ckpt_path: str) -> None:
         """
         Saves current checkpoint
```

### Comparing `torchmanager-1.1.5/torchmanager/training.py` & `torchmanager-1.2b1/lib/training.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from torch.utils.data import DataLoader
-from torchmanager_core import devices, errors, math, torch, view
+from torchmanager_core import devices, errors, math, torch, view, deprecated
 from torchmanager_core.protocols import Resulting
 from torchmanager_core.typing import Any, Collection, Dict, List, Module, Optional, Self, Union
 
 from .callbacks import Callback
 from .data import Dataset
 from .losses import Loss, ParallelLoss
 from .metrics import Metric
```

### Comparing `torchmanager-1.1.5/torchmanager_core/devices/device.py` & `torchmanager-1.2b1/core/devices/device.py`

 * *Files 16% similar despite different names*

```diff
@@ -48,31 +48,14 @@
         warnings.warn(f"CUDA is not available, unable to use multi-GPUs.", ResourceWarning)
         return raw_model, False
 
 def empty_cache() -> None:
     """Empty CUDA cache"""
     if GPU is not NotImplemented: torch.cuda.empty_cache()
 
-def find(specified: Optional[torch.device] = None) -> Tuple[torch.device, torch.device]:
-    """
-    Find available devices
-
-    - Pameters:
-        - specified: An optional `torch.device` of specified
-    - Returns: A `tuple` of CPU in `torch.device` and available device in `torch.device`
-    """
-    warnings.warn("This has been deprecated from v1.1.0 and will be removed in v1.2.0, use `torchmanager_core.devices.search` instead.", PendingDeprecationWarning)
-    if specified is None and GPU is not NotImplemented:
-        return (CPU, GPU)
-    elif specified is None and METAL is not NotImplemented:
-        return (CPU, METAL)
-    elif specified is None:
-        return (CPU, CPU)
-    else: return CPU, specified
-
 def search(specified: Optional[Union[torch.device, List[torch.device]]] = None) -> Tuple[torch.device, torch.device, List[torch.device]]:
     """
     Find available devices
 
     - Pameters:
         - specified: An optional `torch.device` of specified
     - Returns: A `tuple` of CPU in `torch.device`, available device in `torch.device` and `list` of specified devices in `torch.device`
@@ -88,16 +71,16 @@
         specified = [specified]
     elif len(specified) > 0:
         # set default device
         device = torch.device(specified[0].type)
 
         # check for each device
         for d in specified:
-            if d.type != specified[0].type: raise SystemError("All devices in the specified list must have the same device type.")
-            if d.index is None: raise SystemError("All devices in the specified list must have a device index.")
+            if d.type != GPU.type: raise SystemError("All devices in the specified list must have the same device type with GPU type")
+            if d.index is None: raise SystemError("All devices in the specified list must have a device index")
     else: raise SystemError("Specified device list must not be empty")
     return CPU, device, specified
 
 def move_to_device(target: Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]], device: torch.device, recursive: bool = False) -> Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]]:
     """
     Recurrently move a target variable to device if elements perform to `DeviceMovable` protocol
```

### Comparing `torchmanager-1.1.5/torchmanager_core/errors/train.py` & `torchmanager-1.2b1/core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.5/torchmanager_core/protocols.py` & `torchmanager-1.2b1/core/protocols.py`

 * *Files identical despite different names*

