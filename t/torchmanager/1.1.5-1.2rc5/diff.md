# Comparing `tmp/torchmanager-1.1.5.tar.gz` & `tmp/torchmanager-1.2rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager-1.1.5.tar", max compression
+gzip compressed data, was "torchmanager-1.2rc5.tar", max compression
```

## Comparing `torchmanager-1.1.5.tar` & `torchmanager-1.2rc5.tar`

### file list

```diff
@@ -1,44 +1,53 @@
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
+-rw-r--r--   0        0        0     1318 2023-07-13 17:22:38.863844 torchmanager-1.2rc5/LICENSE
+-rw-r--r--   0        0        0     2819 2023-07-26 18:32:35.452909 torchmanager-1.2rc5/README.md
+-rw-r--r--   0        0        0      667 2023-07-26 18:32:04.123531 torchmanager-1.2rc5/pyproject.toml
+-rw-r--r--   0        0        0      283 2023-07-26 18:31:11.263223 torchmanager-1.2rc5/torchmanager/__init__.py
+-rw-r--r--   0        0        0    13736 2023-07-26 18:31:11.263600 torchmanager-1.2rc5/torchmanager/basic.py
+-rw-r--r--   0        0        0      639 2023-07-26 18:31:11.263841 torchmanager-1.2rc5/torchmanager/callbacks/__init__.py
+-rw-r--r--   0        0        0     4437 2023-07-26 18:31:11.264067 torchmanager-1.2rc5/torchmanager/callbacks/callback.py
+-rw-r--r--   0        0        0     4707 2023-07-26 18:31:11.264304 torchmanager-1.2rc5/torchmanager/callbacks/ckpt.py
+-rw-r--r--   0        0        0     3522 2023-07-26 18:31:11.264516 torchmanager-1.2rc5/torchmanager/callbacks/dynamic.py
+-rw-r--r--   0        0        0     1984 2023-07-26 18:31:11.264711 torchmanager-1.2rc5/torchmanager/callbacks/early_stop.py
+-rw-r--r--   0        0        0     4649 2023-07-26 18:31:11.264954 torchmanager-1.2rc5/torchmanager/callbacks/experiment.py
+-rw-r--r--   0        0        0     2356 2023-07-26 18:31:11.265173 torchmanager-1.2rc5/torchmanager/callbacks/lr.py
+-rw-r--r--   0        0        0     2613 2023-07-26 18:31:11.265380 torchmanager-1.2rc5/torchmanager/callbacks/tensorboard.py
+-rw-r--r--   0        0        0      544 2023-07-26 18:31:11.265583 torchmanager-1.2rc5/torchmanager/compatibility.py
+-rw-r--r--   0        0        0       26 2023-07-26 18:24:39.705242 torchmanager-1.2rc5/torchmanager/configs/__init__.py
+-rw-r--r--   0        0        0     4799 2023-07-26 18:31:11.265883 torchmanager-1.2rc5/torchmanager/configs/basic.py
+-rw-r--r--   0        0        0       85 2023-07-26 18:24:39.705531 torchmanager-1.2rc5/torchmanager/data/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-26 18:31:11.266133 torchmanager-1.2rc5/torchmanager/data/dataset.py
+-rw-r--r--   0        0        0     2238 2023-07-26 18:24:39.706045 torchmanager-1.2rc5/torchmanager/data/sliding.py
+-rw-r--r--   0        0        0      180 2023-07-26 18:31:11.266555 torchmanager-1.2rc5/torchmanager/losses/__init__.py
+-rw-r--r--   0        0        0     5557 2023-07-26 18:31:11.266829 torchmanager-1.2rc5/torchmanager/losses/cross_entropy.py
+-rw-r--r--   0        0        0     1354 2023-07-26 18:31:11.267250 torchmanager-1.2rc5/torchmanager/losses/dice.py
+-rw-r--r--   0        0        0     5856 2023-07-26 18:31:11.267490 torchmanager-1.2rc5/torchmanager/losses/loss.py
+-rw-r--r--   0        0        0     3156 2023-07-26 18:31:11.267721 torchmanager-1.2rc5/torchmanager/losses/mse.py
+-rw-r--r--   0        0        0      370 2023-07-26 18:31:11.268275 torchmanager-1.2rc5/torchmanager/metrics/__init__.py
+-rw-r--r--   0        0        0     5577 2023-07-26 18:31:11.268680 torchmanager-1.2rc5/torchmanager/metrics/accuracy.py
+-rw-r--r--   0        0        0     4801 2023-07-26 18:31:11.269233 torchmanager-1.2rc5/torchmanager/metrics/conf_met.py
+-rw-r--r--   0        0        0     5139 2023-07-26 18:26:46.436791 torchmanager-1.2rc5/torchmanager/metrics/extractor.py
+-rw-r--r--   0        0        0     2265 2023-07-26 18:31:11.269466 torchmanager-1.2rc5/torchmanager/metrics/iou.py
+-rw-r--r--   0        0        0     4062 2023-07-26 18:31:11.269695 torchmanager-1.2rc5/torchmanager/metrics/metric.py
+-rw-r--r--   0        0        0     2307 2023-07-26 18:31:11.269842 torchmanager-1.2rc5/torchmanager/metrics/similarity.py
+-rw-r--r--   0        0        0     8779 2023-07-26 18:31:11.270140 torchmanager-1.2rc5/torchmanager/testing.py
+-rw-r--r--   0        0        0      286 2023-07-26 18:31:11.270354 torchmanager-1.2rc5/torchmanager/train/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-26 18:31:11.270550 torchmanager-1.2rc5/torchmanager/train/checkpoint.py
+-rw-r--r--   0        0        0      763 2023-07-26 18:31:11.270740 torchmanager-1.2rc5/torchmanager/train/learning_rate.py
+-rw-r--r--   0        0        0    13195 2023-07-26 18:31:11.271263 torchmanager-1.2rc5/torchmanager/training.py
+-rw-r--r--   0        0        0      641 2023-07-26 18:31:11.271487 torchmanager-1.2rc5/torchmanager_core/__init__.py
+-rw-r--r--   0        0        0       52 2023-07-26 18:31:11.271589 torchmanager-1.2rc5/torchmanager_core/checkpoint/__init__.py
+-rw-r--r--   0        0        0     5015 2023-07-26 18:31:11.271720 torchmanager-1.2rc5/torchmanager_core/checkpoint/ckpt.py
+-rw-r--r--   0        0        0      109 2023-07-26 18:24:39.708665 torchmanager-1.2rc5/torchmanager_core/devices/__init__.py
+-rw-r--r--   0        0        0     4935 2023-07-26 18:31:11.271937 torchmanager-1.2rc5/torchmanager_core/devices/device.py
+-rw-r--r--   0        0        0      264 2023-07-26 18:24:39.708914 torchmanager-1.2rc5/torchmanager_core/devices/protocols.py
+-rw-r--r--   0        0        0      153 2023-07-26 18:26:46.439298 torchmanager-1.2rc5/torchmanager_core/errors/__init__.py
+-rw-r--r--   0        0        0      351 2023-07-26 18:31:11.272112 torchmanager-1.2rc5/torchmanager_core/errors/runtime.py
+-rw-r--r--   0        0        0      669 2023-07-26 18:24:39.709333 torchmanager-1.2rc5/torchmanager_core/errors/train.py
+-rw-r--r--   0        0        0     3394 2023-07-26 18:31:11.272296 torchmanager-1.2rc5/torchmanager_core/protocols.py
+-rw-r--r--   0        0        0       44 2023-07-26 18:24:39.709561 torchmanager-1.2rc5/torchmanager_core/random/__init__.py
+-rw-r--r--   0        0        0     1029 2023-07-26 18:24:39.709656 torchmanager-1.2rc5/torchmanager_core/random/seed.py
+-rw-r--r--   0        0        0      204 2023-07-26 18:24:39.709751 torchmanager-1.2rc5/torchmanager_core/typing.py
+-rw-r--r--   0        0        0     7694 2023-07-26 18:31:11.272673 torchmanager-1.2rc5/torchmanager_core/version.py
+-rw-r--r--   0        0        0      476 2023-07-26 18:31:11.272848 torchmanager-1.2rc5/torchmanager_core/view/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-26 18:24:39.710122 torchmanager-1.2rc5/torchmanager_core/view/protocols.py
+-rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 torchmanager-1.2rc5/PKG-INFO
```

### Comparing `torchmanager-1.1.5/LICENSE` & `torchmanager-1.2rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.5/pyproject.toml` & `torchmanager-1.2rc5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "torchmanager"
-version = "1.1.5"
-description = "PyTorch Training Manager v1.1.5"
+version = "1.2rc5"
+description = "PyTorch Training Manager v1.2rc5"
 authors = ["Qisheng He <Qisheng.He@wayne.edu>"]
 repository = "https://github.com/kisonho/torchmanager.git"
 packages = [
     { include = "torchmanager" },
     { include = "torchmanager_core" },
 ]
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 torch = "*"
 tqdm = "*"
 
 [tool.poetry.optional-dependencies]
-scipy = "*"
-tensorboard = "*"
+scipy = { version = "*" }
+tensorboard = { version = "*" }
 
 [tool.poetry.extras]
 scipy = ["scipy"]
 tensorboard = ["tensorboard"]
 all = ["scipy", "tensorboard"]
 
 [build-system]
```

### Comparing `torchmanager-1.1.5/torchmanager/basic.py` & `torchmanager-1.2rc5/torchmanager/basic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from torchmanager_core import torch, Version, _raise, API_VERSION, VERSION as CURRENT_VERSION
-from torchmanager_core.typing import Any, Collection, Dict, Generic, Module, Optional, OrderedDict, Self, Tuple, Union
+from torchmanager_core import devices, errors, torch, Version, deprecated, API_VERSION, VERSION as CURRENT_VERSION
+from torchmanager_core.checkpoint import Checkpoint
+from torchmanager_core.protocols import Resulting
+from torchmanager_core.typing import Any, Collection, Dict, Generic, List, Module, Optional, OrderedDict, Self, Tuple, Union
 
-from .compatibility import convert
-from .losses import Loss, MultiLosses, MultiOutputsLosses, ParallelLoss
+from .losses import Loss, MultiLosses, ParallelLoss
 from .metrics import Metric
-from .train import Checkpoint
 
 
 class BaseManager(Generic[Module]):
     """
     The basic manager
 
     * Implements: `torchmanager_core.devices.DeviceMovable`, `.callbacks.protocols.ModelContainer`
@@ -39,39 +39,44 @@
         - metrics: A `dict` of metrics with a name in `str` as keys and a `Metric` as values
         - model: A target `torch.nn.Module` to be trained
         - optimizer: A `torch.optim.Optimizer` to train the model
         - raw_loss_fn: An optional `Loss` of the non-paralleled loss function
         - raw_model: A non-paralleled target `torch.nn.Module` model
     """
     # properties
-    loss_fn: Optional[Union[Loss, ParallelLoss]]
-    metric_fns: Dict[str, Metric]
-    model: Module
+    loss_fn: Optional[Resulting]
+    """The optional main loss function in `Resulting`"""
+    metric_fns: Dict[str, Resulting]
+    """A `dict` of the metric functions with names as keys in `str` and metric functions as values in `torch.metrics.Metric`"""
+    model: Union[Module, torch.nn.DataParallel]
     optimizer: Optional[torch.optim.Optimizer]
     version: Version
 
     @property
     def compiled(self) -> bool:
+        """The `bool` flag of if this manager has been compiled"""
         return True if self.loss_fn is not None and self.optimizer is not None else False
 
     @property
-    def raw_loss_fn(self) -> Optional[Loss]:
+    def raw_loss_fn(self) -> Optional[Resulting]:
+        """The `torchmanager.losses.Loss` controlled by this manager without `torch.nn.DataParallel` wrap"""
         if self.loss_fn is None:
             return self.loss_fn
         elif isinstance(self.loss_fn, ParallelLoss):
             return self.loss_fn.module
         elif isinstance(self.loss_fn._metric_fn, torch.nn.parallel.DataParallel):
             self.loss_fn._metric_fn = self.loss_fn._metric_fn.module
             return self.loss_fn
         else:
             return self.loss_fn
 
     @property
     def raw_model(self) -> Module:
-        return self.model.module if isinstance(self.model, torch.nn.parallel.DataParallel) else self.model
+        """The `Module` controlled by this manager without `torch.nn.DataParallel` wrap"""
+        return self.model.module if isinstance(self.model, torch.nn.DataParallel) else self.model  # type: ignore
 
     def __init__(self, model: Module, optimizer: Optional[torch.optim.Optimizer] = None, loss_fn: Optional[Union[Loss, Dict[str, Loss]]] = None, metrics: Dict[str, Metric] = {}) -> None:
         """
         Constructor
 
         - Parameters:
             - loss_fn: An optional `Loss` object to calculate the loss for single loss or a `dict` of losses in `Loss` with their names in `str` to calculate multiple losses
@@ -80,54 +85,102 @@
             - optimizer: An optional `torch.optim.Optimizer` to train the model
         """
         # initialize
         self.metric_fns = {}
         self.model = model
         self.version = CURRENT_VERSION
 
-        # compile
-        self._compile(optimizer, loss_fn, metrics)
+        # initialize loss
+        if isinstance(loss_fn, dict):
+            loss_fn_mapping: Dict[str, Loss] = {f"{name}_loss": fn for name, fn in loss_fn.items()}
+            self.metric_fns.update(loss_fn_mapping)
+            loss_fn = MultiLosses([l for l in loss_fn_mapping.values()])
+        self.loss_fn = loss_fn
 
+        # initialize metrics
+        for name, fn in metrics.items():
+            self.metric_fns[name] = fn
+
+        # initialize optimizer
+        self.optimizer = optimizer
+
+    @deprecated('v1.3', 'v1.4')
     def _compile(self, optimizer: Optional[torch.optim.Optimizer] = None, loss_fn: Optional[Union[Loss, Dict[str, Loss]]] = None, metrics: Dict[str, Metric] = {}) -> None:
         """
         Compiles the manager
 
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
 
+    @deprecated('v1.3', 'v1.4')
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
 
+    def convert(self, from_version: Version) -> None:
+        """
+        Convert from a version to current version
+
+        - Parameters:
+            - from_version: A `torchmanager.version.Version` to convert from
+        """
+        # check manager version
+        if from_version < API_VERSION:
+            # convert loss version
+            if self.raw_loss_fn is not None:
+                self.raw_loss_fn.convert(from_version)
+        
+            # convert metrics version
+            for m in self.metric_fns.values():
+                m.convert(from_version)
+
+            # set version
+            self.version = API_VERSION
+
+    def data_parallel(self, target_devices: List[torch.device]) -> bool:
+        """
+        Data parallel all available models
+
+        - Parameters:
+            - target_devices: The target multiple devices for data parallel
+        - Returns: A `bool` flag of if use multi GPUs
+        """
+        # multi gpus support for loss
+        assert isinstance(self.raw_loss_fn, Loss), errors._raise(TypeError("The loss function is not a valid `Loss` object."))
+        paralleled_loss_fn, use_multi_gpus = devices.data_parallel(self.raw_loss_fn, devices=target_devices, parallel_type=ParallelLoss)
+        assert isinstance(paralleled_loss_fn, ParallelLoss) or isinstance(paralleled_loss_fn, Loss), errors._raise(TypeError("Paralleled function is not a valid `ParallelLoss` or `Loss` after parallel."))
+        self.loss_fn = paralleled_loss_fn
+
+        # multi gpus support for model
+        self.model, use_multi_gpus = devices.data_parallel(self.raw_model, devices=target_devices)
+        return use_multi_gpus
+
     @classmethod
     def from_checkpoint(cls, ckpt: Union[Checkpoint[Any], str], map_location: Optional[torch.device] = None):
         """
         Method to load a manager from a saved `Checkpoint`. The manager will not be compiled with a loss function and its metrics.
 
         - Parameters:
             - ckpt: Either a `Checkpoint` of `Any` object or a `str` of checkpoint path
@@ -143,55 +196,63 @@
             manager = cls(ckpt.model, ckpt.optimizer, loss_fn=ckpt.loss_fn, metrics=ckpt.metrics)  # type: ignore
         elif isinstance(ckpt.model, BaseManager):
             manager = ckpt.model
             if isinstance(manager.model, torch.nn.parallel.DataParallel):
                 manager.model = manager.model.module
             if manager.loss_fn is not None and hasattr(manager.loss_fn, "_metric_fn"):
                 if isinstance(manager.loss_fn._metric_fn, torch.nn.parallel.DataParallel):
-                    assert isinstance(manager.loss_fn._metric_fn.module, Loss), _raise(TypeError("Loss function is not a valid `Loss`."))
+                    assert isinstance(manager.loss_fn._metric_fn.module, Loss), errors._raise(TypeError("Loss function is not a valid `Loss`."))
                     manager.loss_fn = manager.loss_fn._metric_fn.module
             else:
                 manager.loss_fn = None
         else:
             raise TypeError(f"The saved checkpoint contains a model with type of {type(ckpt.model)} that cannot be recoverred to a `Manager`.")
         
-        # convert manager version
+        # initialize manager version
         if not hasattr(manager, "version"):
-            manager.loss_fn = convert(manager.loss_fn)
-            for k in manager.metric_fns:
-                manager.metric_fns[k] = convert(manager.metric_fns[k])
-        elif manager.version < API_VERSION:
-            manager.loss_fn = convert(manager.loss_fn, from_version=manager.version)
-            for k in manager.metric_fns:
-                manager.metric_fns[k] = convert(manager.metric_fns[k], from_version=manager.version)
+            manager.version = Version("v1.0")
+
+        # convert to current version
+        manager.convert(manager.version)
         return manager
 
     def load_state_dict(self, state_dict: OrderedDict[str, Any], strict: bool = True) -> None:
         # load state dict elements
-        assert "model" in state_dict, _raise(KeyError("The given dictionary does not have 'model' element."))
-        assert "optimizer" in state_dict, _raise(KeyError("The given dictionary does not have 'optimizer' element."))
-        assert "loss_fn" in state_dict, _raise(KeyError("The given dictionary does not have 'loss_fn' element."))
-        assert "metrics" in state_dict, _raise(KeyError("The given dictionary does not have 'metrics' element."))
+        assert "model" in state_dict, errors._raise(KeyError("The given dictionary does not have 'model' element."))
+        assert "optimizer" in state_dict, errors._raise(KeyError("The given dictionary does not have 'optimizer' element."))
+        assert "loss_fn" in state_dict, errors._raise(KeyError("The given dictionary does not have 'loss_fn' element."))
+        assert "metrics" in state_dict, errors._raise(KeyError("The given dictionary does not have 'metrics' element."))
         model: OrderedDict[str, Any] = state_dict["model"]
         optimizer: Optional[Dict[str, Any]] = state_dict["optimizer"]
         loss_fn: Optional[OrderedDict[str, Any]] = state_dict["loss_fn"]
         metrics: Dict[str, OrderedDict[str, Any]] = state_dict["metrics"]
 
         # load state dict to current model, optimizer, loss_fn, and metrics
         self.model.load_state_dict(model, strict=strict)  # type: ignore
         if optimizer is not None:
-            assert self.optimizer is not None, _raise(ValueError("The manager has not been compiled with 'optimizer' given."))
+            assert self.optimizer is not None, errors._raise(ValueError("The manager has not been compiled with 'optimizer' given."))
             self.optimizer.load_state_dict(optimizer)
         if loss_fn is not None:
-            assert self.loss_fn is not None, _raise(ValueError("The manager has not been compiled with 'loss_fn' given."))
-            self.loss_fn.load_state_dict(loss_fn)
-        assert metrics is not None, _raise(ValueError("The given dictionary must have 'metrics' element not to be None."))
+            assert self.loss_fn is not None, errors._raise(ValueError("The manager has not been compiled with 'loss_fn' given."))
+            self.loss_fn.load_state_dict(state_dict=loss_fn)
+        assert metrics is not None, errors._raise(ValueError("The given dictionary must have 'metrics' element not to be None."))
         for k, m in metrics.items():
-            assert k in self.metric_fns, _raise(KeyError(f"The manager does not have a metric named '{k}'."))
-            self.metric_fns[k].load_state_dict(m)
+            assert k in self.metric_fns, errors._raise(KeyError(f"The manager does not have a metric named '{k}'."))
+            self.metric_fns[k].load_state_dict(state_dict=m)
+
+    def reset(self, cpu: torch.device = devices.CPU) -> None:
+        """
+        Reset model and loss functions, move all to CPU and empty device cache
+
+        - Parameters:
+            - cpu: The CPU in `torch.device`
+        """
+        self.model = self.raw_model.to(cpu)
+        self.loss_fn = self.raw_loss_fn.to(cpu) if self.raw_loss_fn is not None else self.raw_loss_fn
+        devices.empty_cache()
 
     def state_dict(self, prefix: str = '', keep_vars: bool = False) -> OrderedDict[str, Any]:
         return OrderedDict({
             "model": self.model.state_dict(prefix=prefix, keep_vars=keep_vars),
             "optimizer": self.optimizer.state_dict() if self.optimizer is not None else None,
             "loss_fn": self.loss_fn.state_dict(keep_vars=keep_vars) if self.loss_fn is not None else None,
             "metrics": {k: m.state_dict(keep_vars=keep_vars) for k, m in self.metric_fns.items()}
@@ -200,14 +261,15 @@
     def to(self, device: torch.device) -> None:
         """
         Move the elements in the manager to a target device
 
         - Parameters:
             - device: A target `torch.device`
         """
+        # Move to device
         self.model = self.model.to(device)
         if self.loss_fn is not None:
             self.loss_fn = self.loss_fn.to(device)
         for k, m in self.metric_fns.items():
             self.metric_fns[k] = m.to(device)
 
     def to_checkpoint(self) -> Checkpoint[Self]:
```

### Comparing `torchmanager-1.1.5/torchmanager/callbacks/__init__.py` & `torchmanager-1.2rc5/torchmanager/callbacks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,11 +8,9 @@
 
 try:
     from .experiment import Experiment
     from .tensorboard import TensorBoard
 except:
     from torchmanager_core import view
     view.warnings.warn("Tensorboard dependency is not installed, install it to use `Experiment` and `TensorBoard` callbacks.", ImportWarning)
-
-    Experiment = NotImplemented
-    TensorBoard = NotImplemented
+    Experiment = TensorBoard = NotImplemented
     pass
```

### Comparing `torchmanager-1.1.5/torchmanager/callbacks/callback.py` & `torchmanager-1.2rc5/torchmanager/callbacks/callback.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,25 +112,31 @@
     def on_batch_end(self, batch: int, summary: Dict[str, float] = {}) -> None:
         if self.freq == Frequency.BATCH:
             result = self.step(summary)
             self._update(result)
             self.current_step += 1
 
     def on_train_start(self, initial_epoch: int = 0) -> None:
-        if self.freq == Frequency.EPOCH:
+        if self.freq == Frequency.EPOCH or self.freq == Frequency.EPOCH_START:
             self.current_step = initial_epoch
 
     def on_epoch_end(self, epoch: int, summary: Dict[str, float] = {}, val_summary: Optional[Dict[str, float]] = None) -> None:
         if self.freq == Frequency.EPOCH:
             result = self.step(summary, val_summary)
             self._update(result)
             self.current_step += 1
 
+    def on_epoch_start(self, epoch: int) -> None:
+        if self.freq == Frequency.EPOCH_START:
+            result = self.step()
+            self._update(result)
+            self.current_step += 1
+
     @abc.abstractmethod
-    def step(self, summary: Dict[str, float], val_summary: Optional[Dict[str, float]] = None) -> Any:
+    def step(self, *args: Any, **kwargs: Any) -> Any:
         """
         Abstract method to step the callback
 
         - Parameters:
             - summary: A `dict` of training summary with name in `str` and value in `float`
             - val_summary: An optional `dict` of validation summary with name in `str` and value in `float`
         - Returns: An `Any` type of result for the new step
```

### Comparing `torchmanager-1.1.5/torchmanager/callbacks/ckpt.py` & `torchmanager-1.2rc5/torchmanager/callbacks/ckpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from torchmanager_core import os, torch, _raise
+from torchmanager_core.checkpoint import Checkpoint as Ckpt
 from torchmanager_core.protocols import ModelContainer, MonitorType, StateDictLoadable
 from torchmanager_core.typing import Any, Dict, Generic, Optional, TypeVar
 
-from ..train import Checkpoint as Ckpt
 from .callback import Callback
 
 T = TypeVar('T', bound=StateDictLoadable)
 
 
 class _Checkpoint(Callback, Generic[T]):
     """
```

### Comparing `torchmanager-1.1.5/torchmanager/callbacks/dynamic.py` & `torchmanager-1.2rc5/torchmanager/callbacks/dynamic.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.5/torchmanager/callbacks/early_stop.py` & `torchmanager-1.2rc5/torchmanager/callbacks/early_stop.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.5/torchmanager/callbacks/experiment.py` & `torchmanager-1.2rc5/torchmanager/callbacks/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from torchmanager_core import os
+from torchmanager.callbacks import Callback
+from torchmanager.callbacks import BestCheckpoint, LastCheckpoint
+from torchmanager_core import os, view
 from torchmanager_core.typing import Any, Dict, Generic, List, TypeVar, Union
 from torchmanager_core.protocols import MonitorType, StateDictLoadable
-from torchmanager_core.view import logging
 
-from .callback import Callback
-from .ckpt import BestCheckpoint, LastCheckpoint
 from .tensorboard import TensorBoard
 
 T = TypeVar('T', bound=StateDictLoadable)
 
 
 class Experiment(Callback, Generic[T]):
     """
@@ -57,28 +56,23 @@
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
```

### Comparing `torchmanager-1.1.5/torchmanager/callbacks/lr.py` & `torchmanager-1.2rc5/torchmanager/callbacks/lr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from torchmanager_core import torch
+from torchmanager_core import torch, Version
 from torchmanager_core.protocols import Frequency, SummaryWriteble
 from torchmanager_core.typing import Any, Dict, Generic, Optional, TypeVar
 
 from .callback import FrequencyCallback
 
-Scheduler = TypeVar("Scheduler", bound=torch.optim.lr_scheduler._LRScheduler)
+_LrScheduler = torch.optim.lr_scheduler._LRScheduler if Version(torch.__version__) < "2.0" else torch.optim.lr_scheduler.LRScheduler
+
+Scheduler = TypeVar("Scheduler", bound=_LrScheduler)
 Writer = TypeVar("Writer", bound=SummaryWriteble)
 
 
 class LrSchedueler(FrequencyCallback, Generic[Scheduler]):
     """
     The callback to step learning rate scheduler
```

### Comparing `torchmanager-1.1.5/torchmanager/callbacks/tensorboard.py` & `torchmanager-1.2rc5/torchmanager/callbacks/tensorboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+from torchmanager.callbacks import FrequencyCallback
 from torchmanager_core import tensorboard, torch
 from torchmanager_core.typing import Dict, Optional, Set, Tuple
 from torchmanager_core.protocols import Frequency
 
-from .callback import FrequencyCallback
 
 
 class TensorBoard(FrequencyCallback):
     """
     The callback to record summary to tensorboard for each epoch
 
     * extends: `.callback.FrequencyCallback`
@@ -29,14 +29,15 @@
         - Parameters:
             - log_dir: A `str` of logging directory
             - freq: A tensorboard record `.protocols.Frequency`
             - initial_step: An `int` of the initial step that starts with
         """
         super().__init__(freq, initial_step=initial_step)
         self.__writer = tensorboard.writer.SummaryWriter(log_dir)
+        assert self.freq == Frequency.EPOCH or self.freq == Frequency.BATCH, "Record to tensorboard at start of batch or epoch is not supported."
 
     def add_graph(self, model: torch.nn.Module, input_shape: Optional[Tuple[int, ...]] = None) -> None:
         """
         Add graph to TensorBoard
 
         - Parameters:
             - model: A `torch.nn.Module` to add
```

### Comparing `torchmanager-1.1.5/torchmanager/data/dataset.py` & `torchmanager-1.2rc5/torchmanager/data/dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from torch.utils.data import Dataset as _Dataset, DataLoader
 from torchmanager_core import abc, devices, math, os, torch, _raise
-from torchmanager_core.typing import Any, Callable, Iterator, Sequence, TypeVar
+from torchmanager_core.typing import Any, Callable, Iterator, Optional, Sequence, TypeVar
 
 T = TypeVar("T")
 
 
 class Dataset(_Dataset[T], abc.ABC):
     """
     A dataset that iterates with batch size
@@ -34,14 +34,15 @@
         - unbatched_len: A property method that returns the total length of unbatched dataset
         - __get_item__: The built in method to get items by index (as in `torch.utils.data.Dataset`)
     """
 
     __batch_size: int
     __device: torch.device
     drop_last: bool
+    num_workers: int
     shuffle: bool
 
     @property
     def batch_size(self) -> int:
         return self.__batch_size
 
     @batch_size.setter
@@ -64,52 +65,55 @@
     @property
     def batched_len(self) -> int:
         if self.drop_last:
             return int(self.unbatched_len / self.batch_size)
         else:
             return math.ceil(self.unbatched_len / self.batch_size)
 
-    def __init__(self, batch_size: int, device: torch.device = devices.CPU, drop_last: bool = False, shuffle: bool = False) -> None:
+    def __init__(self, batch_size: int, /, *, device: torch.device = devices.CPU, drop_last: bool = False, num_workers: Optional[int] = None, shuffle: bool = False) -> None:
         """
         Constructor
 
         - Parameters:
             - batch_size: An `int` of batch size for the current dataset
             - device: A `torch.device` for the data to be pinned during iteration
             - drop_last: A `bool` flag of if drop the last data that not enought for the batch size
+            - num_workers: An optional `int` of the number of cpus to load the data
             - shuffle: A `bool` flag of if shuffling the data
         """
         super().__init__()
         self.__device = device
         self.batch_size = batch_size
         self.drop_last = drop_last
         self.shuffle = shuffle
 
+        # initialize num workers
+        if num_workers is None:
+            cpu_count = os.cpu_count()
+            self.num_workers = 0 if cpu_count is None else cpu_count
+        else:
+            self.num_workers = self.num_workers
+
     def __contains__(self, value: Any) -> bool:
         for i in range(len(self)):
             if self[i] == value:
                 return True
         return False
 
     @abc.abstractmethod
     def __getitem__(self, index: Any) -> Any:
         """Returns an unbatched item"""
         return NotImplemented
 
     def __iter__(self) -> Iterator[T]:
-        # initialize devices
-        cpu_count = os.cpu_count()
-        if cpu_count is None:
-            cpu_count = 0
-
         # initialize loader
         if self.device != devices.CPU:
-            data_loader = DataLoader(self, batch_size=self.batch_size, drop_last=self.drop_last, shuffle=self.shuffle, num_workers=cpu_count, pin_memory=True, pin_memory_device=str(self.device))
+            data_loader = DataLoader(self, batch_size=self.batch_size, drop_last=self.drop_last, shuffle=self.shuffle, num_workers=self.num_workers, pin_memory=True, pin_memory_device=str(self.device))
         else:
-            data_loader = DataLoader(self, batch_size=self.batch_size, drop_last=self.drop_last, shuffle=self.shuffle, num_workers=cpu_count)
+            data_loader = DataLoader(self, batch_size=self.batch_size, drop_last=self.drop_last, shuffle=self.shuffle, num_workers=self.num_workers)
 
         # yield data
         for data in data_loader:
             yield self.unpack_data(data)
 
     def __len__(self) -> int:
         """Returns the unbatched length"""
@@ -154,25 +158,25 @@
         - batch_size: An `int` of batch size for the current dataset
         - device: A `torch.device` for the data to be pinned during iteration
         - drop_last: A `bool` flag of if drop the last data that not enought for the batch size
         - shuffle: A `bool` flag of if shuffling the data
     - Returns: A wrapped function that accepts a loading function which returns `torch.utils.data.Dataset` and returns a loading function which returns `DataLoader`
     """
     # wrap function
-    def wrapped_fn(*args: Any, batch_size: int = 1, device: torch.device = devices.CPU, drop_last: bool = False, shuffle: bool = False, **kwargs: Any) -> DataLoader:
+    def wrapped_fn(*args: Any, batch_size: int = 1, device: torch.device = devices.CPU, drop_last: bool = False, num_workers: Optional[int] = None, shuffle: bool = False, **kwargs: Any) -> DataLoader:
         # initialize devices
-        cpu_count = os.cpu_count()
-        if cpu_count is None:
-            cpu_count = 0
+        if num_workers is None:
+            cpu_count = os.cpu_count()
+            num_workers = 0 if cpu_count is None else cpu_count
         _, device, targeted_devices = devices.search(device)
         if device == devices.CPU:
             pin_memory = False
         else:
             devices.set_default(targeted_devices[0])
             pin_memory = True
 
         # load dataset
         loaded_dataset = fn(*args, **kwargs)
         assert not isinstance(loaded_dataset, Dataset), _raise(RuntimeError("The loaded dataset is a `torchmanager.data.Dataset` which has already been wrapped with batch loader during iteration."))
-        data_loader = DataLoader(loaded_dataset, batch_size=batch_size, shuffle=shuffle, drop_last=drop_last, pin_memory=pin_memory, num_workers=cpu_count, pin_memory_device=f"{targeted_devices[0].type}:{targeted_devices.index}")
+        data_loader = DataLoader(loaded_dataset, batch_size=batch_size, shuffle=shuffle, drop_last=drop_last, num_workers=num_workers, pin_memory=pin_memory, pin_memory_device=f"{targeted_devices[0].type}:{targeted_devices.index}")
         return data_loader
     return wrapped_fn
```

### Comparing `torchmanager-1.1.5/torchmanager/data/sliding.py` & `torchmanager-1.2rc5/torchmanager/data/sliding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from itertools import product
 from torchmanager_core import torch, _raise
 from torchmanager_core.typing import List, Tuple
 
-
-def sliding_window(image: torch.Tensor, window_size: Tuple[int, ...], stride: Tuple[int, ...]) -> torch.Tensor:
+def sliding_window(image: torch.Tensor, /, window_size: Tuple[int, ...], stride: Tuple[int, ...]) -> torch.Tensor:
     """
     Extract sliding windows from a multi-dimensional `torch.Tensor`.
 
     - Parameters:
         - image: The input image `torch.Tensor`. Can have any number of dimensions.
         - window_size: A `tuple` of the size of the sliding window in `int` to extract from the image, must have the same number of dimensions as the input image tensor.
         - stride: A `tuple` of the stride of the sliding window in `int`, must have the same number of dimensions as the input image tensor.
```

### Comparing `torchmanager-1.1.5/torchmanager/losses/cross_entropy.py` & `torchmanager-1.2rc5/torchmanager/losses/cross_entropy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from torchmanager_core import functional as F, torch, _raise
+from torchmanager_core import functional as F, torch, Version, _raise
 from torchmanager_core.typing import Any, Optional
 
 from .dice import Dice
 from .loss import Loss
 
 
 class CrossEntropy(Loss):
@@ -111,14 +111,19 @@
         loss_fn = torch.nn.KLDivLoss(*args, **kwargs)
         super().__init__(loss_fn, target=target, weight=weight)
         self._t = softmax_temperature
         if self._t is not None:
             assert self._t > 0, _raise(ValueError(f"Temperature must be a positive number, got {self._t}."))
         self.replace_nan = replace_nan
 
+    def convert(self, from_version: Version) -> None:
+        if from_version < Version("v1.1"):
+            self.replace_nan = False
+            self._t = None
+
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         # softmax input and target
         if self._t is not None:
             temperatured_input = input / self._t
             temperatured_target = target / self._t
             temperatured_input = temperatured_input.softmax(dim=1).log()
             temperatured_target = temperatured_target if self.log_target else target.softmax(dim=1)
```

### Comparing `torchmanager-1.1.5/torchmanager/losses/dice.py` & `torchmanager-1.2rc5/torchmanager/losses/dice.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     * extends: `.loss.Loss`
     """
     _dim: int
     _smooth: float
     _softmax_input: bool
 
-    def __init__(self, dim: int = 1, smooth: float = 1e-6, softmax_input: bool = True, **kwargs: Any) -> None:
+    def __init__(self, dim: int = 1, smooth: float = 1e-6, *, softmax_input: bool = True, **kwargs: Any) -> None:
         """
         Constructor
 
         - Parameters:
             - dim: An `int` of class dimension
             - smooth: An `float` of smooth value to avoid dividing zero
             - softmax_input: A `bool` flag of if softmax the input
```

### Comparing `torchmanager-1.1.5/torchmanager/losses/loss.py` & `torchmanager-1.2rc5/torchmanager/losses/loss.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from torchmanager_core import torch, _raise, deprecated
-from torchmanager_core.typing import Any, Callable, Dict, List, Optional
+from torchmanager_core import torch, _raise
+from torchmanager_core.typing import Any, Callable, List, Optional
 
-from ..metrics import Metric, Reduction
+from ..metrics import Metric
 
 
 class Loss(Metric):
     """
     The main loss function
 
     * extends: `..metrics.Metric`
@@ -114,52 +114,14 @@
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

### Comparing `torchmanager-1.1.5/torchmanager/losses/mse.py` & `torchmanager-1.2rc5/torchmanager/losses/mse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from torchmanager_core import torch
+from torchmanager_core.protocols import Reduction
 from torchmanager_core.typing import Any, Callable, Optional
 
-from .loss import Loss, Reduction
+from .loss import Loss
 
 
 class _ReductableLoss(Loss):
     """
     The MSE loss
 
     - Properties:
         - reduction: A `.loss.Reduction` of reduction method
         - replace_nan: A `boolean` flag of if replacing nan results to zeros
     """
     reduction: Reduction
     replace_nan: bool
 
-    def __init__(self, loss_fn: Optional[Callable[[Any, Any], torch.Tensor]] = None, reduction: Reduction = Reduction.MEAN, replace_nan: bool = False, target: Optional[str] = None, weight: float = 1) -> None:
+    def __init__(self, loss_fn: Optional[Callable[[Any, Any], torch.Tensor]] = None, *, reduction: Reduction = Reduction.MEAN, replace_nan: bool = False, target: Optional[str] = None, weight: float = 1) -> None:
         """
         Constructor
 
         - Parameters:
             - reduction: A `.loss.Reduction` of reduction method
             - replace_nan: A `boolean` flag of if replacing nan results to zeros
             - target: An optional `str` of target name in `input` and `target` during direct calling
@@ -43,19 +44,37 @@
             return loss.mean()
         elif self.reduction == Reduction.SUM:
             return loss.sum()
         else:
             return loss
 
 
+class MAE(_ReductableLoss):
+    """
+    The MSE loss
+    """
+    def __init__(self, *, reduction: Reduction = Reduction.MEAN, replace_nan: bool = False, target: Optional[str] = None, weight: float = 1) -> None:
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
-    def __init__(self, reduction: Reduction = Reduction.MEAN, replace_nan: bool = False, target: Optional[str] = None, weight: float = 1) -> None:
+    def __init__(self, *, reduction: Reduction = Reduction.MEAN, replace_nan: bool = False, target: Optional[str] = None, weight: float = 1) -> None:
         """
         Constructor
 
         - Parameters:
             - reduction: A `.loss.Reduction` of reduction method
             - replace_nan: A `boolean` flag of if replacing nan results to zeros
             - target: An optional `str` of target name in `input` and `target` during direct calling
```

### Comparing `torchmanager-1.1.5/torchmanager/metrics/iou.py` & `torchmanager-1.2rc5/torchmanager/metrics/iou.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from torchmanager_core import torch, _raise, deprecated
+from torchmanager_core import torch, _raise
 from torchmanager_core.typing import Optional
-from torchmanager_core.view import warnings
 
 from .conf_met import ConfusionMetrics
 from .metric import Metric
 
 
 class InstanceIoU(ConfusionMetrics):
     """
     The iIoU metric for segmentation
 
     * extends: `.conf_met.ConfusionMetrics`
     """
 
-    def __init__(self, num_classes: int, target: Optional[str] = None) -> None:
+    def __init__(self, num_classes: int, /, *, target: Optional[str] = None) -> None:
         super().__init__(num_classes, target=target)
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         # argmax for input
         iou = torch.diag(input) / (input.sum(1) + input.sum(0) - torch.diag(input))
         return iou.nanmean()
 
@@ -29,15 +28,15 @@
     * extends: `torch.nn.Module`
     * [Deprecation Warning]: The old `MIoU` metric in v1.0.3 calculates iIoU has been renamed to `InstanceIoU` in v1.1.0, and will be removed in v1.2.0.
     """
     _dim: int
     _smooth: float
     _threshold: float
 
-    def __init__(self, dim: int = 1, smooth: float = 1e-4, threshold: float = 0, target: Optional[str] = None) -> None:
+    def __init__(self, dim: int = 1, smooth: float = 1e-4, threshold: float = 0, *, target: Optional[str] = None) -> None:
         """
         Constructor
 
         - Parameters:
             - dim: An `int` of class dimension
             - smooth: A `float` of smooth value to avoid zero devision
             - threshold: A `float` of min mIoU threshold
@@ -53,14 +52,7 @@
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         input = input.argmax(self._dim) if input.shape[self._dim] > 1 else input > 0.5
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

### Comparing `torchmanager-1.1.5/torchmanager/metrics/metric.py` & `torchmanager-1.2rc5/torchmanager/metrics/metric.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-from torchmanager_core import torch, _raise
-from torchmanager_core.typing import Any, Callable, Enum, List, Optional
-
-
-class Reduction(Enum):
-    NONE = 0
-    MEAN = 1
-    SUM = 2
+from torchmanager_core import torch, Version, _raise
+from torchmanager_core.protocols import Reduction
+from torchmanager_core.typing import Any, Callable, List, Optional
 
 
 class Metric(torch.nn.Module):
     """
     The basic metric class
 
     * extends: `torch.nn.Module`
@@ -58,14 +53,17 @@
             assert self._target in input and self._target in target, _raise(TypeError(f"Target ‘{self._target}’ cannot be found not in input or target"))
             input, target = input[self._target], target[self._target]
 
         # call
         m: torch.Tensor = super().__call__(input, target)
         self._results.append(m.unsqueeze(0).cpu().detach())
         return m
+    
+    def convert(self, from_version: Version) -> None:
+        pass
 
     def forward(self, input: Any, target: Any) -> torch.Tensor:
         """
         Forward the current result method
 
         - Parameters:
             - input: The prediction, or `y_pred`, in `Any` kind
```

### Comparing `torchmanager-1.1.5/torchmanager/testing.py` & `torchmanager-1.2rc5/torchmanager/testing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,83 @@
 from torch.utils.data import DataLoader
-from torchmanager_core import devices, errors, torch, view, _raise
+from torchmanager_core import devices, errors, torch, view
 from torchmanager_core.protocols import Resulting
-from torchmanager_core.typing import Any, Collection, Dict, List, Module, Optional, Union
+from torchmanager_core.typing import Any, Collection, Dict, List, Module, Optional, Tuple, Union
 
 from .basic import BaseManager
 from .data import Dataset
-from .losses import Loss, ParallelLoss
 
 
 class Manager(BaseManager[Module]):
     """
     A testing manager, only used for testing
 
     * extends: `.basic.BaseManager`
 
     Testing the model using `test` function:
     >>> from torchmanager.data import Dataset
     >>> dataset = Dataset(...)
     >>> manager.test(dataset, ...)
 
     - Properties:
-        - compiled_losses: The loss function in `Loss` that must be exist
         - compiled_metrics: The `dict` of metrics in `Resulting` that does not contain losses
+        - summary: A `dict` of metrics summary with name in `str` and value in `float`
     """
     model: Union[Module, torch.nn.parallel.DataParallel]
 
     @property
     def compiled_metrics(self) -> Dict[str, Resulting]:
         return {name: m for name, m in self.metric_fns.items() if "loss" not in name}
 
+    @property
+    def summary(self) -> Dict[str, float]:
+        # initialize
+        summary: Dict[str, float] = {}
+
+        # summarize loss
+        if self.loss_fn is not None:
+            summary["loss"] = float(self.loss_fn.result.detach())
+
+        # summarize metrics
+        for name, fn in self.metric_fns.items():
+            if name.startswith("val_") and self.model.training:
+                continue
+            elif name.startswith("val_"):
+                name = name.replace("val_", "")
+            try:
+                summary[name] = float(fn.result.detach())
+            except Exception as metric_error:
+                runtime_error = errors.MetricError(name)
+                raise runtime_error from metric_error
+        return summary
+
+    def forward(self, input: Any, target: Optional[Any] = None, /) -> Tuple[Any, Optional[torch.Tensor]]:
+        """
+        Forward pass function
+
+        - Parameters:
+            - x_train: The training data
+        - Returns: `Any` kind of model output
+        """
+        # forward model
+        y = self.model(input)
+
+        # forward loss
+        if self.loss_fn is not None and target is not None:
+            try:
+                loss = self.loss_fn(y, target)
+            except Exception as loss_error:
+                runtime_error = errors.LossError()
+                raise loss_error from runtime_error
+        else:
+            loss = None
+        return y, loss
+
     @torch.no_grad()
-    def predict(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection[Any]], device: Optional[Union[torch.device, List[torch.device]]] = None, use_multi_gpus: bool = False, show_verbose: bool = False) -> List[Any]:
+    def predict(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection[Any]], /, *, device: Optional[Union[torch.device, List[torch.device]]] = None, use_multi_gpus: bool = False, show_verbose: bool = False) -> List[Any]:
         '''
         Predict the whole dataset
 
         - Parameters:
             - dataset: A `torch.utils.data.DataLoader` dataset to predict
             - device: An optional `torch.device` to test on if not using multi-GPUs or an optional default `torch.device` for testing otherwise
             - use_multi_gpus: A `bool` flag to use multi gpus during testing
@@ -54,28 +97,29 @@
             dataset_len = dataset.batched_len
         else:
             dataset_len = len(dataset)
         progress_bar = view.tqdm(total=dataset_len) if show_verbose else None
 
         # move model
         try:
-            if use_multi_gpus and not isinstance(self.model, torch.nn.parallel.DataParallel):
-                self.model, use_multi_gpus = devices.data_parallel(self.model, devices=target_devices)
+            # multi gpus support
+            if use_multi_gpus:
+                use_multi_gpus = self.data_parallel(target_devices)
 
             # initialize predictions
             self.model.eval()
             predictions: List[Any] = []
             self.to(device)
 
             # loop the dataset
             for data in dataset:
                 x, _ = self.unpack_data(data)
                 if use_multi_gpus is not True:
                     x = devices.move_to_device(x, device)
-                y = self.model(x)
+                y, _ = self.forward(x, None)
                 predictions.append(y)
                 if progress_bar is not None:
                     progress_bar.update()
 
             # reset model and loss
             return predictions
         except KeyboardInterrupt:
@@ -87,39 +131,35 @@
             raise runtime_error from error
         finally:
             # end epoch training
             if progress_bar is not None:
                 progress_bar.close()
 
             # empty cache
-            self.model = self.raw_model.to(cpu)
-            devices.empty_cache()
+            self.reset(cpu)
 
     @torch.no_grad()
-    def test(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection[Any]], device: Optional[Union[torch.device, List[torch.device]]] = None, empty_cache: bool = True, use_multi_gpus: bool = False, show_verbose: bool = False) -> Dict[str, float]:
+    def test(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection[Any]],  /, *,device: Optional[Union[torch.device, List[torch.device]]] = None, empty_cache: bool = True, use_multi_gpus: bool = False, show_verbose: bool = False) -> Dict[str, float]:
         """
         Test target model
 
         - Parameters:
             - dataset: A `torch.utils.data.DataLoader` or `.data.Dataset` dataset
             - device: An optional `torch.device` to test on if not using multi-GPUs or an optional default `torch.device` for testing otherwise
             - empyt_cache: A `bool` flag to empty cache after testing
             - use_multi_gpus: A `bool` flag to use multi gpus during testing
             - show_verbose: A `bool` flag to show the progress bar during testing
         - Returns: A `dict` of validation summary
         """
-        # initialize device
+        # find available device
         cpu, device, target_devices = devices.search(device)
         if device == cpu and len(target_devices) < 2:
             use_multi_gpus = False
         devices.set_default(target_devices[0])
 
-        # initialize summary
-        summary: Dict[str, float] = {}
-
         # initialize progress bar
         if len(dataset) == 0:
             return {}
         elif isinstance(dataset, Dataset):
             dataset_len = dataset.batched_len
         else:
             dataset_len = len(dataset)
@@ -128,27 +168,19 @@
         # reset loss function and metrics
         if self.loss_fn is not None:
             self.loss_fn.eval().reset()
         for _, m in self.metric_fns.items():
             m.eval().reset()
 
         try:
-            # multi-gpus support for model
-            if use_multi_gpus and not isinstance(self.model, torch.nn.parallel.DataParallel):
-                self.model, use_multi_gpus = devices.data_parallel(self.model, devices=target_devices)
-
-            # multi-gpus support for loss function
-            if use_multi_gpus and self.loss_fn is not None and not isinstance(self.loss_fn, torch.nn.parallel.DataParallel):
-                paralleled_loss_fn, use_multi_gpus = devices.data_parallel(self.loss_fn, devices=target_devices, parallel_type=ParallelLoss)
-                assert isinstance(paralleled_loss_fn, ParallelLoss) or isinstance(paralleled_loss_fn, Loss), _raise(TypeError("Paralleled function is not a valid `ParallelLoss` or `Loss` after parallel."))
-                self.loss_fn = paralleled_loss_fn
-
-            # set module status and move to device
-            self.model.eval()
+            # move to device
+            if use_multi_gpus:
+                use_multi_gpus = self.data_parallel(target_devices)
             self.to(device)
+            self.model.eval()
 
             # batch loop
             for data in dataset:
                 # move x_test, y_test to device
                 x_test, y_test = self.unpack_data(data)
                 if use_multi_gpus is not True:
                     x_test = devices.move_to_device(x_test, device)
@@ -158,76 +190,49 @@
                 step_summary = self.test_step(x_test, y_test)
 
                 # implement progress bar
                 if progress_bar is not None:
                     progress_bar.set_postfix(step_summary)
                     progress_bar.update()
 
-            # summarize
-            for name, fn in self.metric_fns.items():
-                if name.startswith("val_"):
-                    name = name.replace("val_", "")
-                try:
-                    summary[name] = float(fn.result.detach())
-                except Exception as metric_error:
-                    runtime_error = errors.MetricError(name)
-                    raise runtime_error from metric_error
-            if self.loss_fn is not None:
-                summary["loss"] = float(self.loss_fn.result.detach())
-
             # reset model and loss
-            return summary
+            return self.summary
         except KeyboardInterrupt:
             view.logger.info("Testing interrupted.")
             return {}
         except Exception as error:
             view.logger.error(error)
             runtime_error = errors.TestingError()
             raise runtime_error from error
         finally:
             # end epoch training
             if progress_bar is not None:
                 progress_bar.close()
 
             # empty cache
             if empty_cache:
-                self.model = self.raw_model.to(cpu)
-                self.loss_fn = self.raw_loss_fn.to(cpu) if self.raw_loss_fn is not None else self.raw_loss_fn
-                devices.empty_cache()
+                self.reset(cpu)
 
     def test_step(self, x_test: Any, y_test: Any) -> Dict[str, float]:
         """
         A single testing step
 
         - Parameters:
             - x_train: The testing data in `torch.Tensor`
             - y_train: The testing label in `torch.Tensor`
         - Returns: A `dict` of validation summary
         """
-        # initialize
-        summary: Dict[str, float] = {}
-
         # forward pass
-        y = self.model(x_test)
+        y, _ = self.forward(x_test, y_test)
 
         # forward metrics
         for name, fn in self.compiled_metrics.items():
             if name.startswith("val_"):
                 name = name.replace("val_", "")
             elif "loss" in name:
                 continue
             try:
                 fn(y, y_test)
-                summary[name] = float(fn.result.detach())
             except Exception as metric_error:
                 runtime_error = errors.MetricError(name)
                 raise runtime_error from metric_error
-
-        # forward loss
-        if self.loss_fn is not None:
-            try:
-                self.loss_fn(y, y_test)
-                summary["loss"] = float(self.loss_fn.result.detach())
-            except Exception as loss_error:
-                runtime_error = errors.LossError()
-                raise loss_error from runtime_error
-        return summary
+        return self.summary
```

### Comparing `torchmanager-1.1.5/torchmanager/train/checkpoint.py` & `torchmanager-1.2rc5/torchmanager_core/checkpoint/ckpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from torchmanager_core import os, torch, _raise
+import os, torch
 from torchmanager_core.protocols import StateDictLoadable
 from torchmanager_core.typing import Any, Dict, Generic, List, Optional, OrderedDict, TypeVar
 
 T = TypeVar("T", bound=StateDictLoadable)
 
 
 class Checkpoint(Generic[T]):
@@ -53,19 +53,20 @@
             - ckpt_path: A `str` of file path
             - model: Any object to be loaded
         """
         # load checkpint dictionary
         ckpt: Dict[str, Any] = torch.load(ckpt_path, map_location=map_location)
 
         # load model
-        if ckpt["save_weights_only"] is True:
-            assert model is not None, _raise(TypeError("Model must be given to load this checkpoint because `save_weights_only` was set to be `True`."))
+        if model is not None and ckpt["save_weights_only"] is True:
             state_dict: OrderedDict[str, Any] = ckpt["model"]
             model.load_state_dict(state_dict=state_dict)
             ckpt["model"] = model
+        elif model is None and ckpt["save_weights_only"] is True:
+            raise TypeError("Model must be given to load this checkpoint because `save_weights_only` was set to be `True`.")
         else:
             # remove data parallel wrap
             if isinstance(ckpt["model"], torch.nn.parallel.DataParallel):
                 ckpt["model"] = ckpt["model"].module
 
             # load model structure with checkpoint weights
             if model is not None:
```

### Comparing `torchmanager-1.1.5/torchmanager/training.py` & `torchmanager-1.2rc5/torchmanager/training.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from torch.utils.data import DataLoader
-from torchmanager_core import devices, errors, math, torch, view
+from torchmanager_core import devices, errors, math, torch, view, _raise
+from torchmanager_core.checkpoint import Checkpoint
 from torchmanager_core.protocols import Resulting
 from torchmanager_core.typing import Any, Collection, Dict, List, Module, Optional, Self, Union
 
 from .callbacks import Callback
 from .data import Dataset
-from .losses import Loss, ParallelLoss
+from .losses import Loss
 from .metrics import Metric
-from .train import Checkpoint, update_lr
 from .testing import Manager as _Manager
 
 
 class Manager(_Manager[Module]):
     """
     A training manager
 
@@ -51,15 +51,15 @@
         assert self.optimizer is not None, errors._raise(NotImplementedError("The manager is not compiled properly, `optimizer` is missing."))
         return self.optimizer
 
     def __init__(self, model: Module, optimizer: Optional[torch.optim.Optimizer] = None, loss_fn: Optional[Union[Loss, Dict[str, Loss]]] = None, metrics: Dict[str, Metric] = {}) -> None:
         super().__init__(model, optimizer, loss_fn, metrics)
         self.__current_epoch = 0
 
-    def _train(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection], iterations: Optional[int] = None, device: torch.device = devices.CPU, use_multi_gpus: bool = False, show_verbose: bool = False, verbose_type: view.VerboseType = view.VerboseType.ALL, callbacks_list: List[Callback] = []) -> Dict[str, float]:
+    def _train(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection], /, iterations: Optional[int] = None, *, device: torch.device = devices.CPU, use_multi_gpus: bool = False, show_verbose: bool = False, verbose_type: view.VerboseType = view.VerboseType.ALL, callbacks_list: List[Callback] = []) -> Dict[str, float]:
         """
         The single training step for an epoch
 
         - Parameters:
             - dataset: A `torch.utils.data.DataLoader` or `.data.Dataset` training dataset
             - iterations: An optional `int` of total training iterations, must be smaller than the size of dataset
             - device: A `torch.device` where the data is moved to, should be same as the model
@@ -124,84 +124,80 @@
                 # check for iterations
                 if batch + 1 >= iterations:
                     break
         finally:
             # end epoch training
             if progress_bar is not None:
                 progress_bar.close()
+        return self.summary
 
-        # summarize
-        summary = {name: float(fn.result.detach()) for name, fn in self.metric_fns.items() if not name.startswith("val_")}
-        summary["loss"] = float(self.compiled_losses.result.detach())
-        return summary
+    def backward(self, loss: torch.Tensor, /) -> None:
+        """
+        Backward function to calculate the gradients
+        
+        - Parameters:
+            - loss: A `torch.Tensor` of loss value
+        """
+        loss.backward()
 
-    def fit(self, training_dataset: Union[DataLoader[Any], Dataset[Any], Collection], epochs: Optional[int] = None, iterations: Optional[int] = None, initial_epoch: Optional[int] = None, lr_scheduler: Optional[torch.optim.lr_scheduler._LRScheduler] = None, val_dataset: Optional[Union[DataLoader[Any], Dataset[Any], Collection]] = None, device: Optional[Union[torch.device, List[torch.device]]] = None, use_multi_gpus: bool = False, callbacks_list: List[Callback] = [], **kwargs) -> Module:
+    def fit(self, training_dataset: Union[DataLoader[Any], Dataset[Any], Collection], /, epochs: Optional[int] = None, val_dataset: Optional[Union[DataLoader[Any], Dataset[Any], Collection]] = None, callbacks_list: List[Callback] = [], *, iterations: Optional[int] = None, initial_epoch: Optional[int] = None, device: Optional[Union[torch.device, List[torch.device]]] = None, use_multi_gpus: bool = False, **kwargs) -> Module:
         """
         Training algorithm
 
         - Parameters:
             - training_dataset: Any kind of training dataset in `torch.utils.data.DataLoader` or `.data.Dataset`
-            - epochs: An optional `int` number of training epochs
-            - iterations: An optional `int` number of training iterations
-            - lr_scheduelr: An optioanl `torch.optim.lr_scheduler._LRScheduler` to update the lr per epoch
+            - epochs: An optional `int` number of training epochs (`iterations` must be not given)
             - val_dataset: An optional validation `Any`
+            - callbacks_list: A `list` of callbacks in `Callback`
+            - iterations: An optional `int` number of training iterations (`epochs` must be not given)
             - device: An optional `torch.device` to test on if not using multi-GPUs or an optional default `torch.device` for testing otherwise
             - use_multi_gpus: A `bool` flag of if using multi gpus
-            - callbacks_list: A `list` of callbacks in `Callback`
             - **kwargs: Additional keyword arguments that will be passed to `train` method.
         - Returns: A trained `torch.nn.Module`
         """
         # arguments checking
         dataset_len = training_dataset.batched_len if isinstance(training_dataset, Dataset) else len(training_dataset)
         assert self.compiled is True, errors._raise(ValueError("Manager has not yet been compiled. Either loss_fn or optimizer, or both, are not given."))
         if epochs is not None:
             assert epochs > 0, errors._raise(ValueError(f"The epochs must be a positive integer, got {epochs}."))
             assert iterations is None, errors._raise(ValueError(f"The iterations must be given as `None` when epochs is given, got {iterations}."))
         else:
             assert iterations is not None, errors._raise(ValueError(f"The iterations must be given if epochs is not given."))
             assert iterations > 0, errors._raise(ValueError(f"The iterations must be a positive integer, got {iterations}."))
             assert epochs is None, errors._raise(ValueError(f"The epochs must be given as `None` when iterations is given, got {epochs}."))
             epochs = math.ceil(iterations / dataset_len)
+        if use_multi_gpus:
+            view.warnings.warn("The `use_multi_gpus` flag will be deprecated from v1.3 and will be removed from v1.4, multiple GPUs will be automatically used when `device` is given as a list or `None` is given when multiple GPUs are found.", PendingDeprecationWarning)
 
         # initialize initial epoch
         if initial_epoch is not None:
             assert initial_epoch >= 0, errors._raise(ValueError(f"The initial_epoch must be a non_negative integer, got {initial_epoch}."))
             assert initial_epoch < epochs, errors._raise(ValueError(f"The initial_epoch must be smaller than total epochs, got epochs={epochs} but initial_epoch={initial_epoch}."))
             self.current_epoch = initial_epoch
         elif self.current_epoch > 0:
             initial_epoch = self.current_epoch + 1  # skip the latest current epoch when resuming training
         else:
             initial_epoch = self.current_epoch
 
-        # initialize training
+        # find available device
         cpu, device, target_devices = devices.search(device)
-        if device == cpu and len(target_devices) < 2:
+        if device.type == devices.GPU.type and len(target_devices) > 1:
+            use_multi_gpus = True
+        elif use_multi_gpus:
             use_multi_gpus = False
         devices.set_default(target_devices[0])
-        if lr_scheduler is not None:
-            view.warnings.warn("Parameter `lr_scheduler` has been deprecated after v1.1.0 and will be removed from v1.2.0, use `.callbacks.LrScheduler` callback instead.", DeprecationWarning)
+
+        # initialize training
         for c in callbacks_list:
             c.on_train_start(initial_epoch)
 
         try:
-            # multi gpus support for model
-            if use_multi_gpus and not isinstance(self.model, torch.nn.parallel.DataParallel):
-                model, use_multi_gpus = devices.data_parallel(self.model, devices=target_devices)
-            else:
-                model = self.model
-            self.model = model
-
-            # multi gpus support for loss
-            if use_multi_gpus and not isinstance(self.compiled_losses, torch.nn.parallel.DataParallel):
-                assert isinstance(self.compiled_losses, Loss), errors._raise(TypeError("The compiled loss function is not a valid `Loss` object."))
-                paralleled_loss_fn, use_multi_gpus = devices.data_parallel(self.compiled_losses, devices=target_devices, parallel_type=ParallelLoss)
-                assert isinstance(paralleled_loss_fn, ParallelLoss) or isinstance(paralleled_loss_fn, Loss), errors._raise(TypeError("Paralleled function is not a valid `ParallelLoss` or `Loss` after parallel."))
-                self.loss_fn = paralleled_loss_fn
-
             # move to device
+            if use_multi_gpus:
+                use_multi_gpus = self.data_parallel(target_devices)
             self.to(device)
 
             # epoch loop
             for self.current_epoch in range(initial_epoch, epochs):
                 # initialize epoch
                 view.logger.info(f"Training epoch {self.current_epoch + 1}/{epochs}")
                 for c in callbacks_list:
@@ -225,80 +221,58 @@
                         c.on_epoch_end(self.current_epoch, summary=summary, val_summary=val_summary)
                     except errors.StopTraining:
                         # on train end
                         for c in callbacks_list:
                             c.on_train_end(self.raw_model)
                         return self.raw_model
 
-                # step lr scheduler
-                if lr_scheduler is not None:
-                    lr_summary = update_lr(lr_scheduler)
-                    summary.update(lr_summary)
-
                 # print summary info
                 val_message = f"Epoch {self.current_epoch + 1}/{epochs}: "
                 summary.update({f"val_{name}": value for name, value in val_summary.items()})
                 for i, (name, value) in enumerate(summary.items()):
                     if i > 0:
                         val_message += ", "
                     val_message += f"{name}={value:.4f}"
                 view.logger.info(val_message)
 
             # on train end
             for c in callbacks_list:
                 c.on_train_end(self.raw_model)
-            return self.raw_model
         except KeyboardInterrupt:
             view.logger.info("Training interrupted.")
-            return self.raw_model
+            pass
         except Exception as error:
             view.logger.error(error)
             runtime_error = errors.StopTraining(self.current_epoch, "Training failed.")
             raise runtime_error from error
         finally:
-            self.model = self.raw_model.to(cpu)
-            self.loss_fn = self.raw_loss_fn.to(cpu) if self.raw_loss_fn is not None else self.raw_loss_fn
-            devices.empty_cache()
+            self.reset(cpu)
+        return self.raw_model
 
     def train_step(self, x_train: Any, y_train: Any) -> Dict[str, float]:
         """
         A single training step
 
         - Parameters:
             - x_train: The training data
             - y_train: The training label
         - Returns: A summary of `dict` with keys as `str` and values as `float`
         """
         # forward pass
-        summary: Dict[str, float] = {}
-        y = self.model(x_train)
-        loss = self.compiled_losses(y, y_train)
+        y, loss = self.forward(x_train, y_train)
+        assert loss is not None, _raise(TypeError("Loss cannot be fetched."))
 
         # forward metrics
         for name, fn in self.compiled_metrics.items():
             if not name.startswith("val_") and "loss" not in name:
                 fn(y, y_train)
 
         # backward pass
         self.compiled_optimizer.zero_grad()
-        loss.backward()
+        self.backward(loss)
         self.compiled_optimizer.step()
-
-        # summary result
-        try:
-            summary["loss"] = float(self.compiled_losses.result.detach())
-        except Exception as e:
-            raise errors.LossError() from e
-        for name, fn in self.metric_fns.items():
-            if name.startswith("val_"):
-                continue
-            try:
-                summary[name] = float(fn.result.detach())
-            except Exception as metric_error:
-                runtime_error = errors.MetricError(name)
-                raise runtime_error from metric_error
-        return summary
+        return self.summary
 
     def to_checkpoint(self) -> Checkpoint[Self]:
         ckpt = super().to_checkpoint()
         ckpt.last_epoch = self.current_epoch
         return ckpt
```

### Comparing `torchmanager-1.1.5/torchmanager_core/devices/device.py` & `torchmanager-1.2rc5/torchmanager_core/devices/device.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import torch, warnings
+import torch
+import warnings
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Type, TypeVar, Union
 
 from .protocols import DeviceMovable
 
 CPU = torch.device('cpu')
 '''The main CPU'''
 
@@ -23,15 +24,16 @@
 except:
     DEFAULT = CPU
     GPU = NotImplemented
     GPUS = []
 
 Module = TypeVar('Module', bound=torch.nn.Module)
 
-def data_parallel(raw_model: Module, devices: List[torch.device] = GPUS, output_device: Optional[torch.device] = None, parallel_type: Type = torch.nn.parallel.DataParallel) -> Tuple[Union[Module, torch.nn.parallel.DataParallel], bool]:
+
+def data_parallel(raw_model: Module, /, devices: List[torch.device] = GPUS, *, output_device: Optional[torch.device] = None, parallel_type: Type = torch.nn.parallel.DataParallel) -> Tuple[Union[Module, torch.nn.parallel.DataParallel], bool]:
     """
     Make a `torch.nn.Module` data parallel
 
     - Parameters:
         - raw_model: A target `torch.nn.Module`
         - devices: A `list` of target `torch.device`
         - output_device: An optional `torch.device` of the target output device for the paralleled model
@@ -44,34 +46,20 @@
         device_ids = [d.index for d in devices]
         model = parallel_type(raw_model, device_ids=device_ids, output_device=output_device)
         return model, True
     else:
         warnings.warn(f"CUDA is not available, unable to use multi-GPUs.", ResourceWarning)
         return raw_model, False
 
+
 def empty_cache() -> None:
     """Empty CUDA cache"""
-    if GPU is not NotImplemented: torch.cuda.empty_cache()
+    if GPU is not NotImplemented:
+        torch.cuda.empty_cache()
 
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
 
 def search(specified: Optional[Union[torch.device, List[torch.device]]] = None) -> Tuple[torch.device, torch.device, List[torch.device]]:
     """
     Find available devices
 
     - Pameters:
         - specified: An optional `torch.device` of specified
@@ -88,33 +76,38 @@
         specified = [specified]
     elif len(specified) > 0:
         # set default device
         device = torch.device(specified[0].type)
 
         # check for each device
         for d in specified:
-            if d.type != specified[0].type: raise SystemError("All devices in the specified list must have the same device type.")
-            if d.index is None: raise SystemError("All devices in the specified list must have a device index.")
-    else: raise SystemError("Specified device list must not be empty")
+            if d.type != specified[0].type:
+                raise SystemError("All devices in the specified list must have the same device type.")
+            if d.index is None:
+                raise SystemError("All devices in the specified list must have a device index.")
+    else:
+        raise SystemError("Specified device list must not be empty")
     return CPU, device, specified
 
-def move_to_device(target: Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]], device: torch.device, recursive: bool = False) -> Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]]:
+
+def move_to_device(target: Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]], /, device: torch.device, *, recursive: bool = False) -> Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]]:
     """
     Recurrently move a target variable to device if elements perform to `DeviceMovable` protocol
-    
+
     - Parameters:
         - target: Either a target in `DeviceMovable`, a `dict` of targets in `DeviceMovable`, or a `list` of targets in `DeviceMovable`, targets in a `list` or `dict` that does not perform to `DeviceMovable` protocol will be returned without changing
         - device: A `torch.device` of target device
         - recursive: A `bool` flag of if move to device recursively
     - Returns: The same type of target but moved to target device
     """
     if isinstance(target, DeviceMovable):
         target = target.to(device)
     elif isinstance(target, dict):
         target = {k: move_to_device(t, device) if isinstance(t, DeviceMovable) or recursive else t for k, t in target.items()}
     elif isinstance(target, Iterable):
         target = [move_to_device(t, device) if isinstance(t, DeviceMovable) or recursive else t for t in target]
     return target
 
+
 def set_default(d: torch.device) -> None:
     if d.index is not None and d.type == "cuda":
-        torch.cuda.set_device(d)
+        torch.cuda.set_device(d)
```

### Comparing `torchmanager-1.1.5/torchmanager_core/errors/train.py` & `torchmanager-1.2rc5/torchmanager_core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.5/torchmanager_core/protocols.py` & `torchmanager-1.2rc5/torchmanager_core/protocols.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import abc, torch, sys
 from enum import Enum
-from typing import Any, Dict, List, Optional, OrderedDict, Protocol, runtime_checkable
+from typing import Any, Callable, Dict, List, Optional, OrderedDict, Protocol, runtime_checkable
 from typing_extensions import Self
 
 from .devices.protocols import DeviceMovable
+from .version import Version
 from .view.protocols import VerboseControllable
 
 
 class Frequency(Enum):
     """
     The frequency enum for learning rate
     """
 
     EPOCH = 0
+    EPOCH_START = -1
     BATCH = 1
+    BATCH_START = 2
 
 
 class MonitorType(Enum):
     """The enum of monitor types"""
 
     MIN = int(0)
     MAX = int(1)
@@ -49,15 +52,15 @@
     model: torch.nn.Module
 
 
 class StateDictLoadable(Protocol):
     """An object that can load state dict"""
 
     @abc.abstractmethod
-    def load_state_dict(self, state_dict: OrderedDict[str, Any], strict: bool = True) -> Any:
+    def load_state_dict(self, *, state_dict: OrderedDict[str, Any], strict: bool = True) -> Any:
         return NotImplemented
 
     @abc.abstractmethod
     def state_dict(self, *, prefix: str = "", keep_vars: bool = False) -> Dict[str, Any]:
         return NotImplemented
 
 
@@ -67,36 +70,59 @@
     def eval(self) -> Self:
         return NotImplemented
 
     @abc.abstractmethod
     def train(self, mode: bool = True) -> Self:
         return NotImplemented
 
-class Resulting(StateDictLoadable, Trainable, Protocol):
-    """An object that have result available with reset method"""
-    @property
-    @abc.abstractmethod
-    def _target(self) -> Optional[str]:
-        return NotImplemented
 
-    @_target.setter
-    @abc.abstractmethod
-    def _target(self, t: Optional[str]) -> None:
-        pass
+class Reduction(Enum):
+    NONE = 0
+    MEAN = 1
+    SUM = 2
+
+
+class Resulting(DeviceMovable, StateDictLoadable, Trainable, Protocol):
+    """An object that have result available with reset method"""
+    _metric_fn: Optional[Callable[[Any, Any], torch.Tensor]]
+    _target: Optional[str]
+    # @property
+    # @abc.abstractmethod
+    # def _metric_fn(self) -> Optional[Callable[[Any, Any], torch.Tensor]]:
+    #     return NotImplemented
+    
+    # @_metric_fn.setter
+    # @abc.abstractmethod
+    # def _metric_fn(self, fn: Optional[Callable[[Any, Any], torch.Tensor]]) -> None:
+    #     pass
+
+    # @property
+    # @abc.abstractmethod
+    # def _target(self) -> Optional[str]:
+    #     return NotImplemented
+
+    # @_target.setter
+    # @abc.abstractmethod
+    # def _target(self, t: Optional[str]) -> None:
+        # pass
 
     @property
     @abc.abstractmethod
     def result(self) -> torch.Tensor:
         return NotImplemented
 
     @abc.abstractmethod
     def __call__(self, input: Any, target: Any) -> torch.Tensor:
         return NotImplemented
 
     @abc.abstractmethod
+    def convert(self, from_version: Version) -> None:
+        pass
+
+    @abc.abstractmethod
     def reset(self) -> None:
         pass
 
 
 class SummaryWriteble(Protocol):
     """The SummaryWriter protocol"""
```

### Comparing `torchmanager-1.1.5/torchmanager_core/version.py` & `torchmanager-1.2rc5/torchmanager_core/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,51 +50,55 @@
     main_version: int
     minor_version: int
     pre_release: Optional[PreRelease]
     pre_release_version: int
     sub_version: int
 
     def __init__(self, v: Any, /) -> None:
-        # convert to string
-        version_str = str(v)
-
-        # format version
-        if version_str.startswith('v'):
-            version_str = version_str[1:]
-
-        # split pre-release version
-        if 'a' in version_str:
-            pre_release_parts = version_str.split('a')
-            self.pre_release = PreRelease.ALPHA
-        elif 'b' in version_str:
-            pre_release_parts = version_str.split('b')
-            self.pre_release = PreRelease.BETA
-        elif 'rc' in version_str:
-            pre_release_parts = version_str.split('rc')
-            self.pre_release = PreRelease.RELEASE_CANDIDATE
-        else:
-            pre_release_parts = [version_str, "0"]
-            self.pre_release = None
-        version_str = pre_release_parts[0]
-        self.pre_release_version = int(pre_release_parts[1]) if pre_release_parts[1] != '' else 1
-
-        # split version
-        version_parts = version_str.split('.')
-        self.main_version = int(version_parts[0])
-        self.minor_version = int(version_parts[1])
-        self.sub_version = int(version_parts[2]) if len(version_parts) > 2 else 0
+        try:
+            # convert to string
+            version_str = str(v)
+
+            # format version
+            if version_str.startswith('v'):
+                version_str = version_str[1:]
+
+            # split pre-release version
+            if 'a' in version_str:
+                pre_release_parts = version_str.split('a')
+                self.pre_release = PreRelease.ALPHA
+            elif 'b' in version_str:
+                pre_release_parts = version_str.split('b')
+                self.pre_release = PreRelease.BETA
+            elif 'rc' in version_str:
+                pre_release_parts = version_str.split('rc')
+                self.pre_release = PreRelease.RELEASE_CANDIDATE
+            else:
+                pre_release_parts = [version_str, "0"]
+                self.pre_release = None
+            version_str = pre_release_parts[0]
+            self.pre_release_version = int(pre_release_parts[1]) if pre_release_parts[1] != '' else 0
+
+            # split version
+            version_parts = version_str.split('.')
+            self.main_version = int(version_parts[0])
+            self.minor_version = int(version_parts[1])
+            self.sub_version = int(version_parts[2]) if len(version_parts) > 2 else 0
+        except Exception as e:
+            raise ValueError(f"The given version '{v}' is not in valid version format.") from e
 
     def __repr__(self) -> str:
         version_str = f"v{self.main_version}"
         if self.minor_version > 0 or self.sub_version > 0:
             version_str += f".{self.minor_version}"
         if self.sub_version > 0:
             version_str += f".{self.sub_version}"
         if self.pre_release is not None:
-            version_str += f"{self.pre_release.value}{self.pre_release_version}"
+            pre_release_version = self.pre_release_version if self.pre_release_version > 0 else ""
+            version_str += f"{self.pre_release.value}{pre_release_version}"
         return version_str
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Version):
             return self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release == other.pre_release and self.pre_release_version == other.pre_release_version
         else:
             other = Version(str(other))
@@ -139,17 +143,17 @@
     def __le__(self, other: Any) -> bool:
         return self == other or self < other
 
     def __ge__(self, other: Any) -> bool:
         return self == other or self > other
 
 
-API = Version("v1.1")
-CURRENT = Version("v1.1.5")
-DESCRIPTION: str = "PyTorch Training Manager v1.1.5"
+API = Version("v1.2")
+CURRENT = Version("v1.2rc5")
+DESCRIPTION: str = "PyTorch Training Manager {CURRENT}"
 
 
 class VersionError(SystemError):
     def __init__(self, method_name: str, maximum_supported_version: str) -> None:
         super().__init__(f"`{method_name}` has been deprecated and removed from version {maximum_supported_version}. Current version: {CURRENT}.")
```

