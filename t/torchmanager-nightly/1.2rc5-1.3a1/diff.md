# Comparing `tmp/torchmanager_nightly-1.2rc5.tar.gz` & `tmp/torchmanager_nightly-1.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager_nightly-1.2rc5.tar", max compression
+gzip compressed data, was "torchmanager_nightly-1.3a1.tar", max compression
```

## Comparing `torchmanager_nightly-1.2rc5.tar` & `torchmanager_nightly-1.3a1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1318 2023-07-13 17:22:38.863844 torchmanager_nightly-1.2rc5/LICENSE
--rw-r--r--   0        0        0     2821 2023-07-26 14:06:41.049859 torchmanager_nightly-1.2rc5/README.md
--rw-r--r--   0        0        0      675 2023-07-26 14:06:24.190228 torchmanager_nightly-1.2rc5/pyproject.toml
--rw-r--r--   0        0        0      283 2023-07-25 15:49:54.097679 torchmanager_nightly-1.2rc5/torchmanager/__init__.py
--rw-r--r--   0        0        0    13736 2023-07-26 14:05:21.925006 torchmanager_nightly-1.2rc5/torchmanager/basic.py
--rw-r--r--   0        0        0      639 2023-07-24 19:15:32.190713 torchmanager_nightly-1.2rc5/torchmanager/callbacks/__init__.py
--rw-r--r--   0        0        0     4437 2023-07-25 15:49:54.098206 torchmanager_nightly-1.2rc5/torchmanager/callbacks/callback.py
--rw-r--r--   0        0        0     4707 2023-07-25 15:49:54.098394 torchmanager_nightly-1.2rc5/torchmanager/callbacks/ckpt.py
--rw-r--r--   0        0        0     3522 2023-07-19 18:01:53.901655 torchmanager_nightly-1.2rc5/torchmanager/callbacks/dynamic.py
--rw-r--r--   0        0        0     1984 2023-07-25 15:49:54.098560 torchmanager_nightly-1.2rc5/torchmanager/callbacks/early_stop.py
--rw-r--r--   0        0        0     4649 2023-07-25 15:49:54.098748 torchmanager_nightly-1.2rc5/torchmanager/callbacks/experiment.py
--rw-r--r--   0        0        0     2356 2023-07-26 14:05:21.925436 torchmanager_nightly-1.2rc5/torchmanager/callbacks/lr.py
--rw-r--r--   0        0        0     2613 2023-07-25 15:49:54.099079 torchmanager_nightly-1.2rc5/torchmanager/callbacks/tensorboard.py
--rw-r--r--   0        0        0      544 2023-07-26 14:05:21.925641 torchmanager_nightly-1.2rc5/torchmanager/compatibility.py
--rw-r--r--   0        0        0       26 2023-07-25 15:49:54.099263 torchmanager_nightly-1.2rc5/torchmanager/configs/__init__.py
--rw-r--r--   0        0        0     4799 2023-07-26 14:05:21.925877 torchmanager_nightly-1.2rc5/torchmanager/configs/basic.py
--rw-r--r--   0        0        0       85 2023-07-25 15:49:54.099434 torchmanager_nightly-1.2rc5/torchmanager/data/__init__.py
--rw-r--r--   0        0        0     7328 2023-07-25 15:49:54.099650 torchmanager_nightly-1.2rc5/torchmanager/data/dataset.py
--rw-r--r--   0        0        0     2238 2023-07-25 15:49:54.099868 torchmanager_nightly-1.2rc5/torchmanager/data/sliding.py
--rw-r--r--   0        0        0      180 2023-07-26 14:05:21.926295 torchmanager_nightly-1.2rc5/torchmanager/losses/__init__.py
--rw-r--r--   0        0        0     5557 2023-07-24 19:15:32.193172 torchmanager_nightly-1.2rc5/torchmanager/losses/cross_entropy.py
--rw-r--r--   0        0        0     1354 2023-07-26 14:05:21.926734 torchmanager_nightly-1.2rc5/torchmanager/losses/dice.py
--rw-r--r--   0        0        0     5856 2023-07-26 14:05:21.926954 torchmanager_nightly-1.2rc5/torchmanager/losses/loss.py
--rw-r--r--   0        0        0     3156 2023-07-24 19:15:32.194036 torchmanager_nightly-1.2rc5/torchmanager/losses/mse.py
--rw-r--r--   0        0        0      370 2023-07-26 14:05:21.927495 torchmanager_nightly-1.2rc5/torchmanager/metrics/__init__.py
--rw-r--r--   0        0        0     5577 2023-07-26 14:05:21.927911 torchmanager_nightly-1.2rc5/torchmanager/metrics/accuracy.py
--rw-r--r--   0        0        0     4801 2023-07-26 14:05:21.929634 torchmanager_nightly-1.2rc5/torchmanager/metrics/conf_met.py
--rw-r--r--   0        0        0     5139 2023-07-24 19:15:32.195469 torchmanager_nightly-1.2rc5/torchmanager/metrics/extractor.py
--rw-r--r--   0        0        0     2265 2023-07-26 14:05:21.929988 torchmanager_nightly-1.2rc5/torchmanager/metrics/iou.py
--rw-r--r--   0        0        0     4062 2023-07-25 15:49:54.100260 torchmanager_nightly-1.2rc5/torchmanager/metrics/metric.py
--rw-r--r--   0        0        0     2307 2023-07-25 15:49:54.100458 torchmanager_nightly-1.2rc5/torchmanager/metrics/similarity.py
--rw-r--r--   0        0        0     8779 2023-07-26 14:05:21.930314 torchmanager_nightly-1.2rc5/torchmanager/testing.py
--rw-r--r--   0        0        0      286 2023-07-26 14:05:21.930668 torchmanager_nightly-1.2rc5/torchmanager/train/__init__.py
--rw-r--r--   0        0        0       43 2023-07-24 19:15:32.196626 torchmanager_nightly-1.2rc5/torchmanager/train/checkpoint.py
--rw-r--r--   0        0        0      763 2023-07-24 19:15:32.196805 torchmanager_nightly-1.2rc5/torchmanager/train/learning_rate.py
--rw-r--r--   0        0        0    13195 2023-07-26 14:05:21.931269 torchmanager_nightly-1.2rc5/torchmanager/training.py
--rw-r--r--   0        0        0      641 2023-07-26 14:05:21.931662 torchmanager_nightly-1.2rc5/torchmanager_core/__init__.py
--rw-r--r--   0        0        0       52 2023-07-24 19:15:32.197389 torchmanager_nightly-1.2rc5/torchmanager_core/checkpoint/__init__.py
--rw-r--r--   0        0        0     5015 2023-07-25 15:49:54.101887 torchmanager_nightly-1.2rc5/torchmanager_core/checkpoint/ckpt.py
--rw-r--r--   0        0        0      109 2023-07-24 19:15:32.197702 torchmanager_nightly-1.2rc5/torchmanager_core/devices/__init__.py
--rw-r--r--   0        0        0     4935 2023-07-25 15:49:54.102127 torchmanager_nightly-1.2rc5/torchmanager_core/devices/device.py
--rw-r--r--   0        0        0      264 2023-07-19 18:01:53.907517 torchmanager_nightly-1.2rc5/torchmanager_core/devices/protocols.py
--rw-r--r--   0        0        0      153 2023-07-25 15:49:54.102340 torchmanager_nightly-1.2rc5/torchmanager_core/errors/__init__.py
--rw-r--r--   0        0        0      351 2023-07-25 15:49:54.102516 torchmanager_nightly-1.2rc5/torchmanager_core/errors/runtime.py
--rw-r--r--   0        0        0      669 2023-07-19 18:01:53.907838 torchmanager_nightly-1.2rc5/torchmanager_core/errors/train.py
--rw-r--r--   0        0        0     3394 2023-07-25 15:49:54.102727 torchmanager_nightly-1.2rc5/torchmanager_core/protocols.py
--rw-r--r--   0        0        0       44 2023-07-25 15:49:54.102911 torchmanager_nightly-1.2rc5/torchmanager_core/random/__init__.py
--rw-r--r--   0        0        0     1029 2023-07-24 19:15:32.198392 torchmanager_nightly-1.2rc5/torchmanager_core/random/seed.py
--rw-r--r--   0        0        0      204 2023-07-19 18:01:53.908282 torchmanager_nightly-1.2rc5/torchmanager_core/typing.py
--rw-r--r--   0        0        0     7694 2023-07-26 14:05:21.932226 torchmanager_nightly-1.2rc5/torchmanager_core/version.py
--rw-r--r--   0        0        0      476 2023-07-24 19:15:32.198912 torchmanager_nightly-1.2rc5/torchmanager_core/view/__init__.py
--rw-r--r--   0        0        0      313 2023-07-19 18:01:53.908597 torchmanager_nightly-1.2rc5/torchmanager_core/view/protocols.py
--rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 torchmanager_nightly-1.2rc5/PKG-INFO
+-rw-r--r--   0        0        0     1318 2023-07-13 17:22:38.863844 torchmanager_nightly-1.3a1/LICENSE
+-rw-r--r--   0        0        0     2821 2023-07-13 18:32:43.883322 torchmanager_nightly-1.3a1/README.md
+-rw-r--r--   0        0        0      681 2023-07-13 17:22:53.086356 torchmanager_nightly-1.3a1/pyproject.toml
+-rw-r--r--   0        0        0      283 2023-07-13 17:22:48.263633 torchmanager_nightly-1.3a1/torchmanager/__init__.py
+-rw-r--r--   0        0        0    13717 2023-07-13 18:32:43.883776 torchmanager_nightly-1.3a1/torchmanager/basic.py
+-rw-r--r--   0        0        0      639 2023-07-13 17:22:48.264124 torchmanager_nightly-1.3a1/torchmanager/callbacks/__init__.py
+-rw-r--r--   0        0        0     4431 2023-07-13 17:22:53.086823 torchmanager_nightly-1.3a1/torchmanager/callbacks/callback.py
+-rw-r--r--   0        0        0     4701 2023-07-13 17:22:53.087014 torchmanager_nightly-1.3a1/torchmanager/callbacks/ckpt.py
+-rw-r--r--   0        0        0     3522 2023-07-13 17:22:38.864820 torchmanager_nightly-1.3a1/torchmanager/callbacks/dynamic.py
+-rw-r--r--   0        0        0     1972 2023-07-13 17:22:53.087200 torchmanager_nightly-1.3a1/torchmanager/callbacks/early_stop.py
+-rw-r--r--   0        0        0     4637 2023-07-13 17:22:53.087403 torchmanager_nightly-1.3a1/torchmanager/callbacks/experiment.py
+-rw-r--r--   0        0        0     2350 2023-07-13 17:22:53.087591 torchmanager_nightly-1.3a1/torchmanager/callbacks/lr.py
+-rw-r--r--   0        0        0     2600 2023-07-13 17:22:53.087776 torchmanager_nightly-1.3a1/torchmanager/callbacks/tensorboard.py
+-rw-r--r--   0        0        0      544 2023-07-13 17:22:48.265294 torchmanager_nightly-1.3a1/torchmanager/compatibility.py
+-rw-r--r--   0        0        0       26 2023-07-13 17:22:48.265473 torchmanager_nightly-1.3a1/torchmanager/configs/__init__.py
+-rw-r--r--   0        0        0     4799 2023-07-13 17:22:48.265643 torchmanager_nightly-1.3a1/torchmanager/configs/basic.py
+-rw-r--r--   0        0        0       85 2023-07-13 17:22:38.865326 torchmanager_nightly-1.3a1/torchmanager/data/__init__.py
+-rw-r--r--   0        0        0     7328 2023-07-13 17:22:48.265864 torchmanager_nightly-1.3a1/torchmanager/data/dataset.py
+-rw-r--r--   0        0        0     2189 2023-07-13 17:22:53.087967 torchmanager_nightly-1.3a1/torchmanager/data/sliding.py
+-rw-r--r--   0        0        0      156 2023-07-13 17:22:48.266237 torchmanager_nightly-1.3a1/torchmanager/losses/__init__.py
+-rw-r--r--   0        0        0     5557 2023-07-13 17:22:48.266422 torchmanager_nightly-1.3a1/torchmanager/losses/cross_entropy.py
+-rw-r--r--   0        0        0     1047 2023-07-13 17:22:48.266593 torchmanager_nightly-1.3a1/torchmanager/losses/dice.py
+-rw-r--r--   0        0        0     5850 2023-07-13 17:22:53.088160 torchmanager_nightly-1.3a1/torchmanager/losses/loss.py
+-rw-r--r--   0        0        0     3156 2023-07-13 17:22:48.266987 torchmanager_nightly-1.3a1/torchmanager/losses/mse.py
+-rw-r--r--   0        0        0      351 2023-07-13 17:22:48.267154 torchmanager_nightly-1.3a1/torchmanager/metrics/__init__.py
+-rw-r--r--   0        0        0     4145 2023-07-13 17:22:48.267338 torchmanager_nightly-1.3a1/torchmanager/metrics/accuracy.py
+-rw-r--r--   0        0        0     3769 2023-07-13 17:22:48.267523 torchmanager_nightly-1.3a1/torchmanager/metrics/conf_met.py
+-rw-r--r--   0        0        0     5139 2023-07-13 17:22:48.267694 torchmanager_nightly-1.3a1/torchmanager/metrics/extractor.py
+-rw-r--r--   0        0        0     2271 2023-07-13 17:22:48.267858 torchmanager_nightly-1.3a1/torchmanager/metrics/iou.py
+-rw-r--r--   0        0        0     4163 2023-07-13 17:22:53.088362 torchmanager_nightly-1.3a1/torchmanager/metrics/metric.py
+-rw-r--r--   0        0        0     2307 2023-07-13 17:22:48.268141 torchmanager_nightly-1.3a1/torchmanager/metrics/similarity.py
+-rw-r--r--   0        0        0     9648 2023-07-13 17:22:53.088628 torchmanager_nightly-1.3a1/torchmanager/testing.py
+-rw-r--r--   0        0        0      286 2023-07-13 17:22:48.268523 torchmanager_nightly-1.3a1/torchmanager/train/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-13 17:22:48.268678 torchmanager_nightly-1.3a1/torchmanager/train/checkpoint.py
+-rw-r--r--   0        0        0      763 2023-07-13 17:22:48.268850 torchmanager_nightly-1.3a1/torchmanager/train/learning_rate.py
+-rw-r--r--   0        0        0    13490 2023-07-13 17:22:53.088908 torchmanager_nightly-1.3a1/torchmanager/training.py
+-rw-r--r--   0        0        0      641 2023-07-13 17:22:48.269312 torchmanager_nightly-1.3a1/torchmanager_core/__init__.py
+-rw-r--r--   0        0        0       52 2023-07-13 17:22:48.269453 torchmanager_nightly-1.3a1/torchmanager_core/checkpoint/__init__.py
+-rw-r--r--   0        0        0     5003 2023-07-13 17:22:53.089117 torchmanager_nightly-1.3a1/torchmanager_core/checkpoint/ckpt.py
+-rw-r--r--   0        0        0      109 2023-07-13 17:22:48.269784 torchmanager_nightly-1.3a1/torchmanager_core/devices/__init__.py
+-rw-r--r--   0        0        0     4916 2023-07-13 17:22:53.089325 torchmanager_nightly-1.3a1/torchmanager_core/devices/device.py
+-rw-r--r--   0        0        0      264 2023-07-13 17:22:38.867427 torchmanager_nightly-1.3a1/torchmanager_core/devices/protocols.py
+-rw-r--r--   0        0        0      153 2023-07-13 17:22:38.867527 torchmanager_nightly-1.3a1/torchmanager_core/errors/__init__.py
+-rw-r--r--   0        0        0      351 2023-07-13 17:22:48.270154 torchmanager_nightly-1.3a1/torchmanager_core/errors/runtime.py
+-rw-r--r--   0        0        0      669 2023-07-13 17:22:38.867665 torchmanager_nightly-1.3a1/torchmanager_core/errors/train.py
+-rw-r--r--   0        0        0     3382 2023-07-13 17:22:53.089507 torchmanager_nightly-1.3a1/torchmanager_core/protocols.py
+-rw-r--r--   0        0        0       44 2023-07-13 17:22:48.270462 torchmanager_nightly-1.3a1/torchmanager_core/random/__init__.py
+-rw-r--r--   0        0        0     1029 2023-07-13 17:22:48.270566 torchmanager_nightly-1.3a1/torchmanager_core/random/seed.py
+-rw-r--r--   0        0        0      204 2023-07-13 17:22:38.867803 torchmanager_nightly-1.3a1/torchmanager_core/typing.py
+-rw-r--r--   0        0        0     7599 2023-07-13 17:22:53.089691 torchmanager_nightly-1.3a1/torchmanager_core/version.py
+-rw-r--r--   0        0        0      476 2023-07-13 17:22:48.270939 torchmanager_nightly-1.3a1/torchmanager_core/view/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-13 17:22:38.868051 torchmanager_nightly-1.3a1/torchmanager_core/view/protocols.py
+-rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 torchmanager_nightly-1.3a1/PKG-INFO
```

### Comparing `torchmanager_nightly-1.2rc5/LICENSE` & `torchmanager_nightly-1.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc5/README.md` & `torchmanager_nightly-1.3a1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # torchmanager
 ### A highly-wrapped PyTorch training and testing manager
 
 ## Pre-request
-* Python 3.8+
+* Python 3.9+
 * PyTorch
 * tqdm
 * scipy (Optional)
 * tensorboard (Optional)
 
 ## Installation
 * PyPi: `pip install torchmanager-nightly`
```

### Comparing `torchmanager_nightly-1.2rc5/pyproject.toml` & `torchmanager_nightly-1.3a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "torchmanager-nightly"
-version = "1.2rc5"
-description = "PyTorch Training Manager v1.2rc5"
+version = "1.3a1"
+description = "PyTorch Training Manager v1.3 (Alpha 1)"
 authors = ["Qisheng He <Qisheng.He@wayne.edu>"]
 repository = "https://github.com/kisonho/torchmanager.git"
 packages = [
     { include = "torchmanager" },
     { include = "torchmanager_core" },
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 torch = "*"
 tqdm = "*"
 
 [tool.poetry.optional-dependencies]
 scipy = { version = "*" }
 tensorboard = { version = "*" }
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/basic.py` & `torchmanager_nightly-1.3a1/torchmanager/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from torchmanager_core import devices, errors, torch, Version, deprecated, API_VERSION, VERSION as CURRENT_VERSION
 from torchmanager_core.checkpoint import Checkpoint
 from torchmanager_core.protocols import Resulting
-from torchmanager_core.typing import Any, Collection, Dict, Generic, List, Module, Optional, OrderedDict, Self, Tuple, Union
+from torchmanager_core.typing import Any, Collection, Generic, Module, Optional, OrderedDict, Self, Union
 
 from .losses import Loss, MultiLosses, ParallelLoss
 from .metrics import Metric
 
 
 class BaseManager(Generic[Module]):
     """
@@ -41,15 +41,15 @@
         - optimizer: A `torch.optim.Optimizer` to train the model
         - raw_loss_fn: An optional `Loss` of the non-paralleled loss function
         - raw_model: A non-paralleled target `torch.nn.Module` model
     """
     # properties
     loss_fn: Optional[Resulting]
     """The optional main loss function in `Resulting`"""
-    metric_fns: Dict[str, Resulting]
+    metric_fns: dict[str, Resulting]
     """A `dict` of the metric functions with names as keys in `str` and metric functions as values in `torch.metrics.Metric`"""
     model: Union[Module, torch.nn.DataParallel]
     optimizer: Optional[torch.optim.Optimizer]
     version: Version
 
     @property
     def compiled(self) -> bool:
@@ -70,15 +70,15 @@
             return self.loss_fn
 
     @property
     def raw_model(self) -> Module:
         """The `Module` controlled by this manager without `torch.nn.DataParallel` wrap"""
         return self.model.module if isinstance(self.model, torch.nn.DataParallel) else self.model  # type: ignore
 
-    def __init__(self, model: Module, optimizer: Optional[torch.optim.Optimizer] = None, loss_fn: Optional[Union[Loss, Dict[str, Loss]]] = None, metrics: Dict[str, Metric] = {}) -> None:
+    def __init__(self, model: Module, optimizer: Optional[torch.optim.Optimizer] = None, loss_fn: Optional[Union[Loss, dict[str, Loss]]] = None, metrics: dict[str, Metric] = {}) -> None:
         """
         Constructor
 
         - Parameters:
             - loss_fn: An optional `Loss` object to calculate the loss for single loss or a `dict` of losses in `Loss` with their names in `str` to calculate multiple losses
             - metrics: An optional `dict` of metrics with a name in `str` and a `Metric` object to calculate the metric
             - model: An optional target `torch.nn.Module` to be trained
@@ -87,52 +87,52 @@
         # initialize
         self.metric_fns = {}
         self.model = model
         self.version = CURRENT_VERSION
 
         # initialize loss
         if isinstance(loss_fn, dict):
-            loss_fn_mapping: Dict[str, Loss] = {f"{name}_loss": fn for name, fn in loss_fn.items()}
+            loss_fn_mapping: dict[str, Loss] = {f"{name}_loss": fn for name, fn in loss_fn.items()}
             self.metric_fns.update(loss_fn_mapping)
             loss_fn = MultiLosses([l for l in loss_fn_mapping.values()])
         self.loss_fn = loss_fn
 
         # initialize metrics
         for name, fn in metrics.items():
             self.metric_fns[name] = fn
 
         # initialize optimizer
         self.optimizer = optimizer
 
     @deprecated('v1.3', 'v1.4')
-    def _compile(self, optimizer: Optional[torch.optim.Optimizer] = None, loss_fn: Optional[Union[Loss, Dict[str, Loss]]] = None, metrics: Dict[str, Metric] = {}) -> None:
+    def _compile(self, optimizer: Optional[torch.optim.Optimizer] = None, loss_fn: Optional[Union[Loss, dict[str, Loss]]] = None, metrics: dict[str, Metric] = {}) -> None:
         """
         Compiles the manager
 
         - Parameters:
             - loss_fn: An optional `Loss` object to calculate the loss for single loss or a `dict` of losses in `Loss` with their names in `str` to calculate multiple losses
             - metrics: An optional `dict` of metrics with a name in `str` and a `Metric` object to calculate the metric
             - optimizer: An optional `torch.optim.Optimizer` to train the model
         """
         # initialize loss
         if isinstance(loss_fn, dict):
-            loss_fn_mapping: Dict[str, Loss] = {f"{name}_loss": fn for name, fn in loss_fn.items()}
+            loss_fn_mapping: dict[str, Loss] = {f"{name}_loss": fn for name, fn in loss_fn.items()}
             self.metric_fns.update(loss_fn_mapping)
             loss_fn = MultiLosses([l for l in loss_fn_mapping.values()])
         self.loss_fn = loss_fn
 
         # initialize metrics
         for name, fn in metrics.items():
             self.metric_fns[name] = fn
 
         # initialize optimizer
         self.optimizer = optimizer
 
     @deprecated('v1.3', 'v1.4')
-    def compile(self, optimizer: torch.optim.Optimizer, loss_fn: Union[Loss, Dict[str, Loss]], metrics: Dict[str, Metric] = {}) -> None:
+    def compile(self, optimizer: torch.optim.Optimizer, loss_fn: Union[Loss, dict[str, Loss]], metrics: dict[str, Metric] = {}) -> None:
         """
         Recompiles the manager with optimizer loss function and metrics
 
         - Parameters:
             - loss_fn: A `Loss` object to calculate the loss for single loss or a `dict` of losses in `Loss` with their names in `str` to calculate multiple losses
             - metrics: A `dict` of metrics with a name in `str` and a `Metric` object to calculate the metric
             - optimizer: A `torch.optim.Optimizer` to train the model
@@ -155,15 +155,15 @@
             # convert metrics version
             for m in self.metric_fns.values():
                 m.convert(from_version)
 
             # set version
             self.version = API_VERSION
 
-    def data_parallel(self, target_devices: List[torch.device]) -> bool:
+    def data_parallel(self, target_devices: list[torch.device]) -> bool:
         """
         Data parallel all available models
 
         - Parameters:
             - target_devices: The target multiple devices for data parallel
         - Returns: A `bool` flag of if use multi GPUs
         """
@@ -218,17 +218,17 @@
     def load_state_dict(self, state_dict: OrderedDict[str, Any], strict: bool = True) -> None:
         # load state dict elements
         assert "model" in state_dict, errors._raise(KeyError("The given dictionary does not have 'model' element."))
         assert "optimizer" in state_dict, errors._raise(KeyError("The given dictionary does not have 'optimizer' element."))
         assert "loss_fn" in state_dict, errors._raise(KeyError("The given dictionary does not have 'loss_fn' element."))
         assert "metrics" in state_dict, errors._raise(KeyError("The given dictionary does not have 'metrics' element."))
         model: OrderedDict[str, Any] = state_dict["model"]
-        optimizer: Optional[Dict[str, Any]] = state_dict["optimizer"]
+        optimizer: Optional[dict[str, Any]] = state_dict["optimizer"]
         loss_fn: Optional[OrderedDict[str, Any]] = state_dict["loss_fn"]
-        metrics: Dict[str, OrderedDict[str, Any]] = state_dict["metrics"]
+        metrics: dict[str, OrderedDict[str, Any]] = state_dict["metrics"]
 
         # load state dict to current model, optimizer, loss_fn, and metrics
         self.model.load_state_dict(model, strict=strict)  # type: ignore
         if optimizer is not None:
             assert self.optimizer is not None, errors._raise(ValueError("The manager has not been compiled with 'optimizer' given."))
             self.optimizer.load_state_dict(optimizer)
         if loss_fn is not None:
@@ -277,15 +277,15 @@
         Convert the current manager to a checkpoint
 
         - Returns: A `Checkpoint` with its model as the current manager
         """
         ckpt = Checkpoint(self)
         return ckpt
 
-    def unpack_data(self, data: Collection[Any]) -> Tuple[Any, Any]:
+    def unpack_data(self, data: Collection[Any]) -> tuple[Any, Any]:
         """
         Unpacks data to input and target
 
         - Parameters:
             - data: A `Collection` of `Any` kind of data objects
         - Returns: A `tuple` of `Any` kind of input and `Any` kind of target
         """
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/callbacks/__init__.py` & `torchmanager_nightly-1.3a1/torchmanager/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/callbacks/callback.py` & `torchmanager_nightly-1.3a1/torchmanager/callbacks/callback.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from torchmanager_core import abc, torch
 from torchmanager_core.protocols import Frequency
-from torchmanager_core.typing import Any, Dict, Optional
+from torchmanager_core.typing import Any, Optional
 
 
 class Callback:
     """An empty basic training callback"""
 
-    def on_batch_end(self, batch: int, summary: Dict[str, float] = {}) -> None:
+    def on_batch_end(self, batch: int, summary: dict[str, float] = {}) -> None:
         """
         The callback when batch ends
 
         - Parameters:
             - batch: An `int` of batch index
             - summary: A `dict` of summary with name in `str` and value in `float`
         """
@@ -21,15 +21,15 @@
         The callback when batch starts
 
         - Parameters:
             - batch: An `int` of batch index
         """
         pass
 
-    def on_epoch_end(self, epoch: int, summary: Dict[str, float] = {}, val_summary: Optional[Dict[str, float]] = None) -> None:
+    def on_epoch_end(self, epoch: int, summary: dict[str, float] = {}, val_summary: Optional[dict[str, float]] = None) -> None:
         """
         The callback when batch ends
 
         - Parameters:
             - epoch: An `int` of epoch index
             - summary: A `dict` of training summary with name in `str` and value in `float`
             - val_summary: An optional `dict` of validation summary with name in `str` and value in `float`
@@ -105,25 +105,25 @@
         Method to update with the result after step
 
         - Parameters:
             - result: `Any` kind of result value
         """
         pass
 
-    def on_batch_end(self, batch: int, summary: Dict[str, float] = {}) -> None:
+    def on_batch_end(self, batch: int, summary: dict[str, float] = {}) -> None:
         if self.freq == Frequency.BATCH:
             result = self.step(summary)
             self._update(result)
             self.current_step += 1
 
     def on_train_start(self, initial_epoch: int = 0) -> None:
         if self.freq == Frequency.EPOCH or self.freq == Frequency.EPOCH_START:
             self.current_step = initial_epoch
 
-    def on_epoch_end(self, epoch: int, summary: Dict[str, float] = {}, val_summary: Optional[Dict[str, float]] = None) -> None:
+    def on_epoch_end(self, epoch: int, summary: dict[str, float] = {}, val_summary: Optional[dict[str, float]] = None) -> None:
         if self.freq == Frequency.EPOCH:
             result = self.step(summary, val_summary)
             self._update(result)
             self.current_step += 1
 
     def on_epoch_start(self, epoch: int) -> None:
         if self.freq == Frequency.EPOCH_START:
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/callbacks/ckpt.py` & `torchmanager_nightly-1.3a1/torchmanager/callbacks/ckpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from torchmanager_core import os, torch, _raise
 from torchmanager_core.checkpoint import Checkpoint as Ckpt
 from torchmanager_core.protocols import ModelContainer, MonitorType, StateDictLoadable
-from torchmanager_core.typing import Any, Dict, Generic, Optional, TypeVar
+from torchmanager_core.typing import Any, Generic, Optional, TypeVar
 
 from .callback import Callback
 
 T = TypeVar('T', bound=StateDictLoadable)
 
 
 class _Checkpoint(Callback, Generic[T]):
@@ -41,15 +41,15 @@
             - ckpt_path: A `str` of the checkpoint path
             - **kwargs: Other arguments in `Checkpoint` constructor
         """
         super().__init__()
         self.__checkpoint = Ckpt(model, **kwargs)
         self.ckpt_path = os.path.normpath(ckpt_path)
 
-    def on_epoch_end(self, epoch: int, summary: Dict[str, float] = ..., val_summary: Optional[Dict[str, float]] = ...) -> None:
+    def on_epoch_end(self, epoch: int, summary: dict[str, float] = ..., val_summary: Optional[dict[str, float]] = ...) -> None:
         self.checkpoint.save(epoch, self.ckpt_path)
 
 
 class LastCheckpoint(_Checkpoint[T]):
     """
     Last checkpoint with frequency control support
 
@@ -69,15 +69,15 @@
         assert f > 0, _raise(ValueError(f"Frequency must be a positive number, got {f}. "))
         self.__freq = f
 
     def __init__(self, model: T, ckpt_path: str, freq: int = 1, **kwargs: Any) -> None:
         super().__init__(model, ckpt_path, **kwargs)
         self.freq = freq
 
-    def on_epoch_end(self, epoch: int, summary: Dict[str, float] = ..., val_summary: Optional[Dict[str, float]] = ...) -> None:
+    def on_epoch_end(self, epoch: int, summary: dict[str, float] = ..., val_summary: Optional[dict[str, float]] = ...) -> None:
         if epoch % self.freq == 0:
             super().on_epoch_end(epoch, summary, val_summary)
 
 
 class BestCheckpoint(_Checkpoint[T]):
     """
     The callback to save the latest checkpoint for each epoch
@@ -105,15 +105,15 @@
         """
         super().__init__(model, ckpt_path, **kwargs)
         self.best_score = monitor_type.init_score
         self.load_best = load_best
         self.monitor = monitor
         self.monitor_type = monitor_type
 
-    def on_epoch_end(self, epoch: int, summary: Dict[str, float] = ..., val_summary: Optional[Dict[str, float]] = ...) -> None:
+    def on_epoch_end(self, epoch: int, summary: dict[str, float] = ..., val_summary: Optional[dict[str, float]] = ...) -> None:
         # get score
         score = val_summary[self.monitor] if val_summary is not None else summary[self.monitor]
 
         # save when best
         if score >= self.best_score and self.monitor_type == MonitorType.MAX:
             self.best_score = score
             super().on_epoch_end(epoch, summary, val_summary)
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/callbacks/dynamic.py` & `torchmanager_nightly-1.3a1/torchmanager/callbacks/dynamic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/callbacks/early_stop.py` & `torchmanager_nightly-1.3a1/torchmanager/callbacks/early_stop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from torchmanager_core import errors, sys
-from torchmanager_core.typing import Dict, List, Optional
+from torchmanager_core.typing import Optional
 
 from .ckpt import Callback, MonitorType
 
 
 class EarlyStop(Callback):
     '''
     The early stop callback that raises `StopTraining` error during the training if monitored metric not improved for several steps
 
     - Properties:
         - monitor: A `str` of monitored metric
         - monitor_type: A `MonitorType` of either `MIN` of `MAX` mode for the best model
         - steps: An `int` of steps to monitor
     '''
-    __metrics: List[float]
+    __metrics: list[float]
     monitor: str
     monitor_type: MonitorType
     steps: int
 
     @property
-    def _metrics(self) -> List[float]:
+    def _metrics(self) -> list[float]:
         return self.__metrics
 
     def __init__(self, monitor: str, monitor_type: MonitorType = MonitorType.MAX, steps: int = 10) -> None:
         super().__init__()
         self.__metrics = [sys.float_info.min if monitor_type == MonitorType.MAX else sys.float_info.max]
         self.monitor = monitor
         self.monitor_type = monitor_type
         self.steps = steps
 
-    def on_epoch_end(self, epoch: int, summary: Dict[str, float] = ..., val_summary: Optional[Dict[str, float]] = None) -> None:
+    def on_epoch_end(self, epoch: int, summary: dict[str, float] = ..., val_summary: Optional[dict[str, float]] = None) -> None:
         # load monitoring value
         summary = val_summary if val_summary is not None else summary
         monitoring_value = summary[self.monitor]
 
         # compare with recorded metrics
         value = self._metrics[0]
         if self.monitor_type == MonitorType.MAX and monitoring_value <= value and len(self._metrics) > self.steps:
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/callbacks/experiment.py` & `torchmanager_nightly-1.3a1/torchmanager/callbacks/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from torchmanager.callbacks import Callback
 from torchmanager.callbacks import BestCheckpoint, LastCheckpoint
 from torchmanager_core import os, view
-from torchmanager_core.typing import Any, Dict, Generic, List, TypeVar, Union
+from torchmanager_core.typing import Any, Generic, TypeVar, Union
 from torchmanager_core.protocols import MonitorType, StateDictLoadable
 
 from .tensorboard import TensorBoard
 
 T = TypeVar('T', bound=StateDictLoadable)
 
 
@@ -17,19 +17,19 @@
     * requires: `tensorboard` package
 
     - Properties:
         - best_ckpts: A `list` of `.ckpt.BestCheckpoint` callbacks that records best checkpoints
         - last_ckpt: A `.ckpt.LastCheckpoint` callback that records the last checkpoint
         - tensorboard: A `.ckpt.TensorBoard` callback that records data to tensorboard
     """
-    best_ckpts: List[BestCheckpoint[T]]
+    best_ckpts: list[BestCheckpoint[T]]
     last_ckpt: LastCheckpoint[T]
     tensorboard: TensorBoard
 
-    def __init__(self, experiment: str, model: T, monitors: Union[Dict[str, MonitorType], List[str]] = {}, show_verbose: bool = True) -> None:
+    def __init__(self, experiment: str, model: T, monitors: Union[dict[str, MonitorType], list[str]] = {}, show_verbose: bool = True) -> None:
         """
         Constructor
 
         - Parameters:
             - experiment: A `str` of target folder for the experiment
             - model: A target model to be tracked during experiment in `T`
             - monitors: A `list` of metric name if all monitors are using `MonitorType.MAX` to track, or `dict` of metric name to be tracked for the best checkpoint in `str` and the `.ckpt.MonitorType` to track as values
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/callbacks/lr.py` & `torchmanager_nightly-1.3a1/torchmanager/callbacks/lr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from torchmanager_core import torch, Version
 from torchmanager_core.protocols import Frequency, SummaryWriteble
-from torchmanager_core.typing import Any, Dict, Generic, Optional, TypeVar
+from torchmanager_core.typing import Any, Generic, Optional, TypeVar
 
 from .callback import FrequencyCallback
 
 _LrScheduler = torch.optim.lr_scheduler._LRScheduler if Version(torch.__version__) < "2.0" else torch.optim.lr_scheduler.LRScheduler
 
 Scheduler = TypeVar("Scheduler", bound=_LrScheduler)
 Writer = TypeVar("Writer", bound=SummaryWriteble)
@@ -40,29 +40,29 @@
         self.__lr_scheduler = scheduler
         self.__name = name
         self.__writer = tf_board_writer
 
     def _update(self, result: Any) -> None:
         pass
 
-    def on_epoch_end(self, epoch: int, summary: Dict[str, float], val_summary: Optional[Dict[str, Any]] = None) -> None:
+    def on_epoch_end(self, epoch: int, summary: dict[str, float], val_summary: Optional[dict[str, Any]] = None) -> None:
         # get lr summary
         lr_summary = {}
         lr_list = self._scheduler.get_last_lr()
         if len(lr_list) > 1:
             for i, lr in enumerate(lr_list):
                 lr_summary[f'{self._name}_{i}'] = lr
         else:
             lr_summary[self._name] = lr_list[0]
 
         # write results to Tensorboard
         if self._writer is not None:
             # record summary
             for key in lr_summary.keys():
-                result: Dict[str, float] = {}
+                result: dict[str, float] = {}
                 result["train"] = lr_summary[key]
                 self._writer.add_scalars(key, result, epoch)
 
         # update lr scheduler
         summary.update(lr_summary)
         super().on_epoch_end(epoch, summary, val_summary)
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/callbacks/tensorboard.py` & `torchmanager_nightly-1.3a1/torchmanager/callbacks/tensorboard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from torchmanager.callbacks import FrequencyCallback
 from torchmanager_core import tensorboard, torch
-from torchmanager_core.typing import Dict, Optional, Set, Tuple
+from torchmanager_core.typing import Optional, Set
 from torchmanager_core.protocols import Frequency
 
 
 
 class TensorBoard(FrequencyCallback):
     """
     The callback to record summary to tensorboard for each epoch
@@ -31,37 +31,37 @@
             - freq: A tensorboard record `.protocols.Frequency`
             - initial_step: An `int` of the initial step that starts with
         """
         super().__init__(freq, initial_step=initial_step)
         self.__writer = tensorboard.writer.SummaryWriter(log_dir)
         assert self.freq == Frequency.EPOCH or self.freq == Frequency.BATCH, "Record to tensorboard at start of batch or epoch is not supported."
 
-    def add_graph(self, model: torch.nn.Module, input_shape: Optional[Tuple[int, ...]] = None) -> None:
+    def add_graph(self, model: torch.nn.Module, input_shape: Optional[tuple[int, ...]] = None) -> None:
         """
         Add graph to TensorBoard
 
         - Parameters:
             - model: A `torch.nn.Module` to add
             - input_shape: An optional `tuple` of in `int` for the inputs
         """
         inputs = torch.randn(input_shape) if input_shape is not None else None
         self.writer.add_graph(model, input_to_model=inputs)
 
-    def _update(self, result: Tuple[Set[str], Dict[str, float], Optional[Dict[str, float]]]) -> None:
+    def _update(self, result: tuple[Set[str], dict[str, float], Optional[dict[str, float]]]) -> None:
         keys, summary, val_summary = result
 
         # write results to Tensorboard
         for key in keys:
-            r: Dict[str, float] = {}
+            r: dict[str, float] = {}
             if key in summary:
                 r["train"] = summary[key]
             if val_summary is not None and key in val_summary:
                 r["val"] = val_summary[key]
             self.writer.add_scalars(key, r, self.current_step + 1)
 
-    def step(self, summary: Dict[str, float], val_summary: Optional[Dict[str, float]] = None) -> Tuple[Set[str], Dict[str, float], Optional[Dict[str, float]]]:
+    def step(self, summary: dict[str, float], val_summary: Optional[dict[str, float]] = None) -> tuple[Set[str], dict[str, float], Optional[dict[str, float]]]:
         # fetch keys
         keys = list(summary.keys())
         if val_summary is not None:
             keys += list(val_summary.keys())
         keys = set(keys)
         return keys, summary, val_summary
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/compatibility.py` & `torchmanager_nightly-1.3a1/torchmanager/compatibility.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/configs/basic.py` & `torchmanager_nightly-1.3a1/torchmanager/configs/basic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/data/dataset.py` & `torchmanager_nightly-1.3a1/torchmanager/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/data/sliding.py` & `torchmanager_nightly-1.3a1/torchmanager/data/sliding.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from itertools import product
 from torchmanager_core import torch, _raise
-from torchmanager_core.typing import List, Tuple
 
-def sliding_window(image: torch.Tensor, /, window_size: Tuple[int, ...], stride: Tuple[int, ...]) -> torch.Tensor:
+def sliding_window(image: torch.Tensor, /, window_size: tuple[int, ...], stride: tuple[int, ...]) -> torch.Tensor:
     """
     Extract sliding windows from a multi-dimensional `torch.Tensor`.
 
     - Parameters:
         - image: The input image `torch.Tensor`. Can have any number of dimensions.
         - window_size: A `tuple` of the size of the sliding window in `int` to extract from the image, must have the same number of dimensions as the input image tensor.
         - stride: A `tuple` of the stride of the sliding window in `int`, must have the same number of dimensions as the input image tensor.
@@ -21,17 +20,17 @@
     >>> windows = sliding_window(image, window_size, stride)
     >>> windows.shape[0]
     36
     ```
     """
     # initialize
     assert len(window_size) == len(stride), _raise(ValueError(f"Window size dimension ({len(window_size)}) and stride dimension ({stride}) must be the same."))
-    stride_dims: List[int] = []
-    windows: List[torch.Tensor] = []
-    window_dims: List[int] = []
+    stride_dims: list[int] = []
+    windows: list[torch.Tensor] = []
+    window_dims: list[int] = []
 
     # Calculate number of windows in each dimension
     for dim_size, window_dim, stride_dim in zip(image.shape[1:], window_size, stride):
         num_windows = (dim_size - window_dim) // stride_dim + 1
         window_dims.append(num_windows)
         stride_dims.append(stride_dim)
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/losses/cross_entropy.py` & `torchmanager_nightly-1.3a1/torchmanager/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/losses/dice.py` & `torchmanager_nightly-1.3a1/torchmanager/losses/dice.py`

 * *Files 26% similar despite different names*

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
 
-    def __init__(self, dim: int = 1, smooth: float = 1e-6, *, softmax_input: bool = True, **kwargs: Any) -> None:
+    def __init__(self, smooth: int = 1, *, softmax_input: bool = True, **kwargs: Any) -> None:
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

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/losses/loss.py` & `torchmanager_nightly-1.3a1/torchmanager/losses/loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from torchmanager_core import torch, _raise
-from torchmanager_core.typing import Any, Callable, List, Optional
+from torchmanager_core.typing import Any, Callable, Optional
 
 from ..metrics import Metric
 
 
 class Loss(Metric):
     """
     The main loss function
@@ -81,15 +81,15 @@
 
     __losses: torch.nn.ModuleList
 
     @property
     def losses(self) -> torch.nn.ModuleList:
         return self.__losses
 
-    def __init__(self, losses: List[Loss], target: Optional[str] = None, weight: float = 1) -> None:
+    def __init__(self, losses: list[Loss], target: Optional[str] = None, weight: float = 1) -> None:
         """
         Constructor
 
         - Parameters:
             - losses: A `list` of `Loss` function
             - target: An optional `str` of target name in `input` and `target` during direct calling
             - weight: A `float` of the loss weight
@@ -128,15 +128,15 @@
     - Properties:
         - result: A `torch.Tensor` of current result
         - results: A `torch.Tensor` of concatenated results
     """
     _metric_fn: torch.nn.DataParallel
     module: Loss
 
-    def __init__(self, module: Loss, device_ids: Optional[List[int]] = None, output_device: Optional[torch.device] = None, dim: int = 0) -> None:
+    def __init__(self, module: Loss, device_ids: Optional[list[int]] = None, output_device: Optional[torch.device] = None, dim: int = 0) -> None:
         super().__init__(torch.nn.DataParallel(module, device_ids, output_device, dim=dim))
         self.module = module
 
     def forward(self, input: Any, target: Any) -> torch.Tensor:
         loss: torch.Tensor = super().forward(input, target)
         return loss.mean()
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/losses/mse.py` & `torchmanager_nightly-1.3a1/torchmanager/losses/mse.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/metrics/accuracy.py` & `torchmanager_nightly-1.3a1/torchmanager/metrics/accuracy.py`

 * *Files 18% similar despite different names*

```diff
@@ -68,32 +68,26 @@
     """
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         target = target.argmax(dim=self._dim)
         return super().forward(input, target)
 
 
-class Dice(BinaryConfusionMetric):
-    """The dice score metrics"""
-    def forward_metric(self, tp: torch.Tensor, tn: torch.Tensor, fp: torch.Tensor, fn: torch.Tensor) -> torch.Tensor:
-        dice = 2 * tp / (2 * tp + fp + fn + self._eps)
-        return dice.mean()
-
-
 class F1(BinaryConfusionMetric):
     """The F1 metrics"""
 
-    def forward_metric(self, tp: torch.Tensor, tn: torch.Tensor, fp: torch.Tensor, fn: torch.Tensor) -> torch.Tensor:
+    def forward(self, tp: torch.Tensor, tn: torch.Tensor, fp: torch.Tensor, fn: torch.Tensor) -> torch.Tensor:
         # calculate precision and recall
         precision = tp / (tp + fp + self._eps)
         recall = tp / (tp + fn + self._eps)
 
         # calculate F1
         f1 = 2 * precision * recall / (precision + recall + self._eps)
-        return f1.mean()
+        f1 = torch.mean(f1)
+        return f1
 
 
 class MAE(Metric):
     """
     The Mean Absolute Error metric
 
     * extends: `.metrics.Metric`
@@ -124,52 +118,19 @@
             return error.mean()
         elif self.reduction == Reduction.SUM:
             return error.sum()
         else:
             return error
 
 
-class PartialDice(Dice):
-    """
-    The partial dice score for a specific class index
-
-    - Properties:
-        - class_idx: An `int` of the target class index
-    """
-    class_idx: int
-
-    def __init__(self, c: int, /, dim: int = 1, *, eps: float = 1e-7, target:Optional[str] = None):
-        """
-        Constructor
-
-        - Parameters:
-            - c: The target class index in `int`
-            - dim: The class channel dimmension index in `int`
-            - eps: A `float` of the small number to avoid zero divide
-            - target: A `str` of target name in `input` and `target` during direct calling
-        """
-        super().__init__(dim, eps=eps, target=target)
-        self.class_idx = c
-
-    def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
-        input = input.argmax(self._dim)
-        input_mask = input == self.class_idx
-        target_mask = target == self.class_idx
-        intersection = input_mask * target_mask
-        dice = (2 * intersection.sum() + self._eps) / (input_mask.sum() + target_mask.sum() + self._eps)
-        return dice.mean()
-
-
 class Precision(BinaryConfusionMetric):
     """The Precision metrics"""
 
     def forward_metric(self, tp: torch.Tensor, tn: torch.Tensor, fp: torch.Tensor, fn: torch.Tensor) -> torch.Tensor:
-        precision = tp / (tp + fp + self._eps)
-        return precision.mean()
+        return tp / (tp + fp + self._eps)
 
 
 class Recall(BinaryConfusionMetric):
     """The Recall metrics"""
 
     def forward_metric(self, tp: torch.Tensor, tn: torch.Tensor, fp: torch.Tensor, fn: torch.Tensor) -> torch.Tensor:
-        recall = tp / (tp + fn + self._eps)
-        return recall.mean()
+        return tp / (tp + fn + self._eps)
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/metrics/conf_met.py` & `torchmanager_nightly-1.3a1/torchmanager/metrics/conf_met.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,44 @@
-from torch.nn import functional as F
 from torchmanager_core import abc, torch, deprecated, _raise
-from torchmanager_core.typing import Any, Optional, Tuple
+from torchmanager_core.typing import Any, Optional
 
 from .metric import Metric
 
 
 class BinaryConfusionMetric(Metric, abc.ABC):
     """
     The binary confusion metrics that calculates TP, FP, and FN and forward further to calculate the final metric
 
     * extends: `.metric.Metric`
     * Abstract class
 
     - Methods to implement:
-        - forward_metric: The main method that accepts TP, TN, FP, and FN as `torch.Tensor` and returns the final metric as `torch.Tensor`
+        - forward_metric: The main method that accepts TP, FP, and FN as `torch.Tensor` and returns the final metric as `torch.Tensor`
     """
     _dim: int
     _eps: float
 
-    def __init__(self, dim: int = 1, *, eps: float=1e-7, target: Optional[str] = None):
-        """
-        Constructor
-
-        - Parameters:
-            - dim: The class channel dimmension index in `int`
-            - eps: A `float` of the small number to avoid zero divide
-            - target: A `str` of target name in `input` and `target` during direct calling
-        """
+    def __init__(self, dim: int = -1, *, eps: float=1e-7, target: Optional[str] = None):
         super().__init__(target=target)
         self._dim = dim
         self._eps = eps
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         # argmax input
-        num_classes = input.shape[self._dim]
-        input = F.one_hot(input.argmax(dim=self._dim), num_classes)
-        target = F.one_hot(target, num_classes)
+        input = input.argmax(dim=self._dim)
 
         # calculate TP, FP, and FN
-        tp, tn, fp, fn = self.forward_conf_met(input, target)
-        return self.forward_metric(tp, tn, fp, fn)
-
-    def forward_conf_met(self, input: torch.Tensor, target: torch.Tensor) -> Tuple[torch.Tensor, ...]:
         tp = torch.sum(target * input, dim=0)
         tn = ((1 - target) * (1 - input)).sum(dim=0)
         fp = torch.sum((1 - target) * input, dim=0)
         fn = torch.sum(target * (1 - input), dim=0)
-        return tp, tn, fp, fn
+        return self.forward_metric(tp, tn, fp, fn)
 
     @abc.abstractmethod
     def forward_metric(self, tp: torch.Tensor, tn: torch.Tensor, fp: torch.Tensor, fn: torch.Tensor) -> torch.Tensor:
-        """
-        The main method to calculate the final metric from confusion metrics
-
-        - Parameters:
-            - tp: The true positive `torch.Tensor`
-            - tn: The true negative `torch.Tensor`
-            - fp: The false positive `torch.Tensor`
-            - fn: The false negative `torch.Tensor`
-        - Returns: The final metric `torch.Tensor`
-        """
         return NotImplemented
 
 
 class ConfusionMetrics(Metric, abc.ABC):
     """
     The metric that forward confusion metrics calculated by given `input` and `target` as final `input` in `forward` method
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/metrics/extractor.py` & `torchmanager_nightly-1.3a1/torchmanager/metrics/extractor.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/metrics/iou.py` & `torchmanager_nightly-1.3a1/torchmanager/metrics/iou.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,13 +46,13 @@
         assert dim > 0, _raise(ValueError(f"The dimension must be a positive number, got {dim}."))
         assert threshold >= 0 and threshold <= 1, _raise(ValueError(f"The threshold must be in range [0,1], got {threshold}."))
         self._dim = dim
         self._smooth = smooth
         self._threshold = threshold
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
-        input = input.argmax(self._dim) if input.shape[self._dim] > 1 else input > 0.5
+        input = input.argmax(self._dim) if input.shape[self._dim] > 1 else (input > 0).int()
         intersection = (input & target).float().sum()
         union = (input | target).float().sum()
         iou = (intersection + self._smooth) / (union + self._smooth)
         thresholded = torch.clamp(10 / (1 - self._threshold) * (iou - self._threshold), 0, 10).ceil() / 10
         return thresholded
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/metrics/metric.py` & `torchmanager_nightly-1.3a1/torchmanager/metrics/metric.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from torchmanager_core import torch, Version, _raise
 from torchmanager_core.protocols import Reduction
-from torchmanager_core.typing import Any, Callable, List, Optional
+from torchmanager_core.typing import Any, Callable, Optional
 
 
 class Metric(torch.nn.Module):
     """
     The basic metric class
 
     * extends: `torch.nn.Module`
@@ -12,23 +12,17 @@
     * Metric tensor is released from memory as soon as the result returned
 
     - Properties:
         - result: The `torch.Tensor` of average metric results
         - results: An optional `torch.Tensor` of all metric results
     """
     _metric_fn: Optional[Callable[[Any, Any], torch.Tensor]]
-    _results: List[torch.Tensor]
+    _results: list[torch.Tensor]
     _target: Optional[str]
-
-    @property
-    def result(self) -> torch.Tensor:
-        if len(self._results) > 0:
-            return torch.concat(self._results).mean()
-        else:
-            return torch.tensor(torch.nan)
+    result: torch.Tensor
 
     @property
     def results(self) -> Optional[torch.Tensor]:
         if len(self._results) > 0:
             return torch.concat(self._results)
         else:
             return None
@@ -39,31 +33,35 @@
 
         - Parameters:
             - metric_fn: An optional `Callable` metrics function that accepts `Any` kind of prediction input and target and returns a metric `torch.Tensor`. A `call` method must be overriden if this parameter is set as `None`.
             - target: A `str` of target name in `input` and `target` during direct calling
         """
         super().__init__()
         self._metric_fn = metric_fn
+        self.result = torch.tensor(0, dtype=torch.float)
         self._results = []
         self._target = target
 
     def __call__(self, input: Any, target: Any) -> torch.Tensor:
         # unpack input and target
         if self._target is not None:
             assert isinstance(input, dict) and isinstance(target, dict), _raise(TypeError(f"Given input or target must be dictionaries, got {type(input)} and {type(target)}."))
             assert self._target in input and self._target in target, _raise(TypeError(f"Target ‘{self._target}’ cannot be found not in input or target"))
             input, target = input[self._target], target[self._target]
 
         # call
         m: torch.Tensor = super().__call__(input, target)
+        self.result *= len(self._results)
         self._results.append(m.unsqueeze(0).cpu().detach())
+        self.result = (self.result + self._results[-1]) / len(self.result)
         return m
     
     def convert(self, from_version: Version) -> None:
-        pass
+        if from_version < "v1.3":
+            self.result = torch.tensor(0, dtype=torch.float)
 
     def forward(self, input: Any, target: Any) -> torch.Tensor:
         """
         Forward the current result method
 
         - Parameters:
             - input: The prediction, or `y_pred`, in `Any` kind
@@ -74,14 +72,15 @@
         if self._metric_fn is not None:
             return self._metric_fn(input, target)
         else:
             raise NotImplementedError("metric_fn is not given.")
 
     def reset(self) -> None:
         """Reset the current results list"""
+        self.result *= 0
         self._results.clear()
 
 
 def metric(fn: Callable[[Any, Any], torch.Tensor]) -> Metric:
     """
     The metric wrapping function that wrap a function into a metric
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/metrics/similarity.py` & `torchmanager_nightly-1.3a1/torchmanager/metrics/similarity.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/testing.py` & `torchmanager_nightly-1.3a1/torchmanager/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from torch.utils.data import DataLoader
 from torchmanager_core import devices, errors, torch, view
 from torchmanager_core.protocols import Resulting
-from torchmanager_core.typing import Any, Collection, Dict, List, Module, Optional, Tuple, Union
+from torchmanager_core.typing import Any, Callable, Collection, Module, Optional, Union
 
 from .basic import BaseManager
 from .data import Dataset
 
 
 class Manager(BaseManager[Module]):
     """
@@ -21,21 +21,21 @@
     - Properties:
         - compiled_metrics: The `dict` of metrics in `Resulting` that does not contain losses
         - summary: A `dict` of metrics summary with name in `str` and value in `float`
     """
     model: Union[Module, torch.nn.parallel.DataParallel]
 
     @property
-    def compiled_metrics(self) -> Dict[str, Resulting]:
+    def compiled_metrics(self) -> dict[str, Resulting]:
         return {name: m for name, m in self.metric_fns.items() if "loss" not in name}
 
     @property
-    def summary(self) -> Dict[str, float]:
+    def summary(self) -> dict[str, float]:
         # initialize
-        summary: Dict[str, float] = {}
+        summary: dict[str, float] = {}
 
         # summarize loss
         if self.loss_fn is not None:
             summary["loss"] = float(self.loss_fn.result.detach())
 
         # summarize metrics
         for name, fn in self.metric_fns.items():
@@ -46,15 +46,15 @@
             try:
                 summary[name] = float(fn.result.detach())
             except Exception as metric_error:
                 runtime_error = errors.MetricError(name)
                 raise runtime_error from metric_error
         return summary
 
-    def forward(self, input: Any, target: Optional[Any] = None, /) -> Tuple[Any, Optional[torch.Tensor]]:
+    def forward(self, input: Any, target: Optional[Any] = None, /) -> tuple[Any, Optional[torch.Tensor]]:
         """
         Forward pass function
 
         - Parameters:
             - x_train: The training data
         - Returns: `Any` kind of model output
         """
@@ -68,16 +68,40 @@
             except Exception as loss_error:
                 runtime_error = errors.LossError()
                 raise loss_error from runtime_error
         else:
             loss = None
         return y, loss
 
+    def forward_fn(self, fn: Callable[[Any, Optional[Any]], tuple[Any, Optional[torch.Tensor]]], /) -> None:
+        """
+        The wrapper function to override `forward` method
+
+        * Example:
+
+        ```
+        >>> manager = Manager(...) # define a manager
+
+        >>> @manager.forward_fn
+        >>> def forward(input: Any, target: Optional[Any]) -> tuple[Any, Optional[torch.Tensor]]: # the forward function to override
+        >>>     y = manager.model(input)
+        >>>     loss = manager.compiled_loss(y, target)
+        >>>     return y, loss
+
+        >>> ...
+        >>> manager.fit(...)
+        ```
+
+        - Parameters:
+            - fn: A forward function that accepts `Any` type of `x` and optional `Any` type of `y` and returns a `tuple` of `Any` kind of model output and an optional `torch.Tensor` loss
+        """
+        setattr(self, "forward", fn)
+
     @torch.no_grad()
-    def predict(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection[Any]], /, *, device: Optional[Union[torch.device, List[torch.device]]] = None, use_multi_gpus: bool = False, show_verbose: bool = False) -> List[Any]:
+    def predict(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection[Any]], /, *, device: Optional[Union[torch.device, list[torch.device]]] = None, use_multi_gpus: bool = False, show_verbose: bool = False) -> list[Any]:
         '''
         Predict the whole dataset
 
         - Parameters:
             - dataset: A `torch.utils.data.DataLoader` dataset to predict
             - device: An optional `torch.device` to test on if not using multi-GPUs or an optional default `torch.device` for testing otherwise
             - use_multi_gpus: A `bool` flag to use multi gpus during testing
@@ -103,15 +127,15 @@
         try:
             # multi gpus support
             if use_multi_gpus:
                 use_multi_gpus = self.data_parallel(target_devices)
 
             # initialize predictions
             self.model.eval()
-            predictions: List[Any] = []
+            predictions: list[Any] = []
             self.to(device)
 
             # loop the dataset
             for data in dataset:
                 x, _ = self.unpack_data(data)
                 if use_multi_gpus is not True:
                     x = devices.move_to_device(x, device)
@@ -134,15 +158,15 @@
             if progress_bar is not None:
                 progress_bar.close()
 
             # empty cache
             self.reset(cpu)
 
     @torch.no_grad()
-    def test(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection[Any]],  /, *,device: Optional[Union[torch.device, List[torch.device]]] = None, empty_cache: bool = True, use_multi_gpus: bool = False, show_verbose: bool = False) -> Dict[str, float]:
+    def test(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection[Any]],  /, *,device: Optional[Union[torch.device, list[torch.device]]] = None, empty_cache: bool = True, use_multi_gpus: bool = False, show_verbose: bool = False) -> dict[str, float]:
         """
         Test target model
 
         - Parameters:
             - dataset: A `torch.utils.data.DataLoader` or `.data.Dataset` dataset
             - device: An optional `torch.device` to test on if not using multi-GPUs or an optional default `torch.device` for testing otherwise
             - empyt_cache: A `bool` flag to empty cache after testing
@@ -208,15 +232,15 @@
             if progress_bar is not None:
                 progress_bar.close()
 
             # empty cache
             if empty_cache:
                 self.reset(cpu)
 
-    def test_step(self, x_test: Any, y_test: Any) -> Dict[str, float]:
+    def test_step(self, x_test: Any, y_test: Any) -> dict[str, float]:
         """
         A single testing step
 
         - Parameters:
             - x_train: The testing data in `torch.Tensor`
             - y_train: The testing label in `torch.Tensor`
         - Returns: A `dict` of validation summary
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/train/learning_rate.py` & `torchmanager_nightly-1.3a1/torchmanager/train/learning_rate.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc5/torchmanager/training.py` & `torchmanager_nightly-1.3a1/torchmanager/training.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from torch.utils.data import DataLoader
 from torchmanager_core import devices, errors, math, torch, view, _raise
 from torchmanager_core.checkpoint import Checkpoint
 from torchmanager_core.protocols import Resulting
-from torchmanager_core.typing import Any, Collection, Dict, List, Module, Optional, Self, Union
+from torchmanager_core.typing import Any, Callable, Collection, Module, Optional, Self, Union
 
 from .callbacks import Callback
 from .data import Dataset
 from .losses import Loss
 from .metrics import Metric
 from .testing import Manager as _Manager
 
@@ -47,19 +47,19 @@
         return self.loss_fn
 
     @property
     def compiled_optimizer(self) -> torch.optim.Optimizer:
         assert self.optimizer is not None, errors._raise(NotImplementedError("The manager is not compiled properly, `optimizer` is missing."))
         return self.optimizer
 
-    def __init__(self, model: Module, optimizer: Optional[torch.optim.Optimizer] = None, loss_fn: Optional[Union[Loss, Dict[str, Loss]]] = None, metrics: Dict[str, Metric] = {}) -> None:
+    def __init__(self, model: Module, optimizer: Optional[torch.optim.Optimizer] = None, loss_fn: Optional[Union[Loss, dict[str, Loss]]] = None, metrics: dict[str, Metric] = {}) -> None:
         super().__init__(model, optimizer, loss_fn, metrics)
         self.__current_epoch = 0
 
-    def _train(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection], /, iterations: Optional[int] = None, *, device: torch.device = devices.CPU, use_multi_gpus: bool = False, show_verbose: bool = False, verbose_type: view.VerboseType = view.VerboseType.ALL, callbacks_list: List[Callback] = []) -> Dict[str, float]:
+    def _train(self, dataset: Union[DataLoader[Any], Dataset[Any], Collection], /, iterations: Optional[int] = None, *, device: torch.device = devices.CPU, use_multi_gpus: bool = False, show_verbose: bool = False, verbose_type: view.VerboseType = view.VerboseType.ALL, callbacks_list: list[Callback] = []) -> dict[str, float]:
         """
         The single training step for an epoch
 
         - Parameters:
             - dataset: A `torch.utils.data.DataLoader` or `.data.Dataset` training dataset
             - iterations: An optional `int` of total training iterations, must be smaller than the size of dataset
             - device: A `torch.device` where the data is moved to, should be same as the model
@@ -135,15 +135,39 @@
         Backward function to calculate the gradients
         
         - Parameters:
             - loss: A `torch.Tensor` of loss value
         """
         loss.backward()
 
-    def fit(self, training_dataset: Union[DataLoader[Any], Dataset[Any], Collection], /, epochs: Optional[int] = None, val_dataset: Optional[Union[DataLoader[Any], Dataset[Any], Collection]] = None, callbacks_list: List[Callback] = [], *, iterations: Optional[int] = None, initial_epoch: Optional[int] = None, device: Optional[Union[torch.device, List[torch.device]]] = None, use_multi_gpus: bool = False, **kwargs) -> Module:
+    def backward_fn(self, fn: Callable[[torch.Tensor], None], /) -> None:
+        """
+        The wrapper function to override `backward` method
+
+        * Example:
+
+        ```
+        >>> manager = Manager(...) # define a manager
+
+        >>> @manager.backward_fn
+        >>> def backward(loss: torch.Tensor) -> None: # the backward function to override
+        >>>     manager.optimizer.zero_grad()
+        >>>     loss.backward()
+        >>>     manager.optimizer.step()
+
+        >>> ...
+        >>> manager.fit(...)
+        ```
+
+        - Parameters:
+            - fn: A backward function that accepts a loss `torch.Tensor`
+        """
+        setattr(self, "backward", fn)
+
+    def fit(self, training_dataset: Union[DataLoader[Any], Dataset[Any], Collection], /, epochs: Optional[int] = None, val_dataset: Optional[Union[DataLoader[Any], Dataset[Any], Collection]] = None, callbacks_list: list[Callback] = [], *, iterations: Optional[int] = None, initial_epoch: Optional[int] = None, device: Optional[Union[torch.device, list[torch.device]]] = None, use_multi_gpus: bool = False, **kwargs) -> Module:
         """
         Training algorithm
 
         - Parameters:
             - training_dataset: Any kind of training dataset in `torch.utils.data.DataLoader` or `.data.Dataset`
             - epochs: An optional `int` number of training epochs (`iterations` must be not given)
             - val_dataset: An optional validation `Any`
@@ -161,32 +185,28 @@
             assert epochs > 0, errors._raise(ValueError(f"The epochs must be a positive integer, got {epochs}."))
             assert iterations is None, errors._raise(ValueError(f"The iterations must be given as `None` when epochs is given, got {iterations}."))
         else:
             assert iterations is not None, errors._raise(ValueError(f"The iterations must be given if epochs is not given."))
             assert iterations > 0, errors._raise(ValueError(f"The iterations must be a positive integer, got {iterations}."))
             assert epochs is None, errors._raise(ValueError(f"The epochs must be given as `None` when iterations is given, got {epochs}."))
             epochs = math.ceil(iterations / dataset_len)
-        if use_multi_gpus:
-            view.warnings.warn("The `use_multi_gpus` flag will be deprecated from v1.3 and will be removed from v1.4, multiple GPUs will be automatically used when `device` is given as a list or `None` is given when multiple GPUs are found.", PendingDeprecationWarning)
 
         # initialize initial epoch
         if initial_epoch is not None:
             assert initial_epoch >= 0, errors._raise(ValueError(f"The initial_epoch must be a non_negative integer, got {initial_epoch}."))
             assert initial_epoch < epochs, errors._raise(ValueError(f"The initial_epoch must be smaller than total epochs, got epochs={epochs} but initial_epoch={initial_epoch}."))
             self.current_epoch = initial_epoch
         elif self.current_epoch > 0:
             initial_epoch = self.current_epoch + 1  # skip the latest current epoch when resuming training
         else:
             initial_epoch = self.current_epoch
 
         # find available device
         cpu, device, target_devices = devices.search(device)
-        if device.type == devices.GPU.type and len(target_devices) > 1:
-            use_multi_gpus = True
-        elif use_multi_gpus:
+        if device == cpu and len(target_devices) < 2:
             use_multi_gpus = False
         devices.set_default(target_devices[0])
 
         # initialize training
         for c in callbacks_list:
             c.on_train_start(initial_epoch)
 
@@ -223,15 +243,15 @@
                         # on train end
                         for c in callbacks_list:
                             c.on_train_end(self.raw_model)
                         return self.raw_model
 
                 # print summary info
                 val_message = f"Epoch {self.current_epoch + 1}/{epochs}: "
-                summary.update({f"val_{name}": value for name, value in val_summary.items()})
+                summary |= {f"val_{name}": value for name, value in val_summary.items()}
                 for i, (name, value) in enumerate(summary.items()):
                     if i > 0:
                         val_message += ", "
                     val_message += f"{name}={value:.4f}"
                 view.logger.info(val_message)
 
             # on train end
@@ -244,15 +264,15 @@
             view.logger.error(error)
             runtime_error = errors.StopTraining(self.current_epoch, "Training failed.")
             raise runtime_error from error
         finally:
             self.reset(cpu)
         return self.raw_model
 
-    def train_step(self, x_train: Any, y_train: Any) -> Dict[str, float]:
+    def train_step(self, x_train: Any, y_train: Any) -> dict[str, float]:
         """
         A single training step
 
         - Parameters:
             - x_train: The training data
             - y_train: The training label
         - Returns: A summary of `dict` with keys as `str` and values as `float`
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager_core/__init__.py` & `torchmanager_nightly-1.3a1/torchmanager_core/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc5/torchmanager_core/checkpoint/ckpt.py` & `torchmanager_nightly-1.3a1/torchmanager_core/checkpoint/ckpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os, torch
 from torchmanager_core.protocols import StateDictLoadable
-from torchmanager_core.typing import Any, Dict, Generic, List, Optional, OrderedDict, TypeVar
+from torchmanager_core.typing import Any, Generic, Optional, OrderedDict, TypeVar
 
 T = TypeVar("T", bound=StateDictLoadable)
 
 
 class Checkpoint(Generic[T]):
     """
     The callback to save the latest checkpoint for each epoch
@@ -16,20 +16,20 @@
         - model: Any type of model to be saved
         - optimizer: A `torch.nn.Optimizer` to be saved
         - save_weights_only: A `bool` flag of if only save state_dict of model
     """
 
     last_epoch: int
     loss_fn: Optional[StateDictLoadable]
-    metrics: Dict[str, StateDictLoadable]
+    metrics: dict[str, StateDictLoadable]
     model: T
     optimizer: Optional[torch.optim.Optimizer]
     save_weights_only: bool
 
-    def __init__(self, model: T, last_epoch: int = 0, optimizer: Optional[torch.optim.Optimizer] = None, loss_fn: Optional[StateDictLoadable] = None, metrics: Optional[Dict[str, StateDictLoadable]] = None, save_weights_only: bool = False) -> None:
+    def __init__(self, model: T, last_epoch: int = 0, optimizer: Optional[torch.optim.Optimizer] = None, loss_fn: Optional[StateDictLoadable] = None, metrics: Optional[dict[str, StateDictLoadable]] = None, save_weights_only: bool = False) -> None:
         """
         Constructor
 
         - Parameters:
             - model: Any type of model to be saved
             - epoch: An `int` of epoch index
             - optimizer: An optional `torch.optim.Optimizer` to be recorded
@@ -50,15 +50,15 @@
         Load checkpoint from a saved checkpoint file
 
         - Parameters:
             - ckpt_path: A `str` of file path
             - model: Any object to be loaded
         """
         # load checkpint dictionary
-        ckpt: Dict[str, Any] = torch.load(ckpt_path, map_location=map_location)
+        ckpt: dict[str, Any] = torch.load(ckpt_path, map_location=map_location)
 
         # load model
         if model is not None and ckpt["save_weights_only"] is True:
             state_dict: OrderedDict[str, Any] = ckpt["model"]
             model.load_state_dict(state_dict=state_dict)
             ckpt["model"] = model
         elif model is None and ckpt["save_weights_only"] is True:
@@ -92,15 +92,15 @@
             ckpt["model"] = ckpt["model"].module
         ckpt_path = os.path.normpath(ckpt_path)
         ckpt_dir = os.path.dirname(ckpt_path)
         os.makedirs(ckpt_dir, exist_ok=True)
         torch.save(ckpt, ckpt_path)
 
 
-def list_checkpoints(experiment_dir: str) -> List[str]:
+def list_checkpoints(experiment_dir: str) -> list[str]:
     """
     List all checkpoints in the given experiment folder
 
     - Parameters:
         - experiment_dir: A `str` of experiment directory
     - Returns: A `list` of checkpoints name in the experiment
     """
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager_core/devices/device.py` & `torchmanager_nightly-1.3a1/torchmanager_core/devices/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 import warnings
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Type, TypeVar, Union
+from typing import Any, Iterable, Optional, Type, TypeVar, Union
 
 from .protocols import DeviceMovable
 
 CPU = torch.device('cpu')
 '''The main CPU'''
 
 try:
@@ -25,15 +25,15 @@
     DEFAULT = CPU
     GPU = NotImplemented
     GPUS = []
 
 Module = TypeVar('Module', bound=torch.nn.Module)
 
 
-def data_parallel(raw_model: Module, /, devices: List[torch.device] = GPUS, *, output_device: Optional[torch.device] = None, parallel_type: Type = torch.nn.parallel.DataParallel) -> Tuple[Union[Module, torch.nn.parallel.DataParallel], bool]:
+def data_parallel(raw_model: Module, /, devices: list[torch.device] = GPUS, *, output_device: Optional[torch.device] = None, parallel_type: Type = torch.nn.parallel.DataParallel) -> tuple[Union[Module, torch.nn.parallel.DataParallel], bool]:
     """
     Make a `torch.nn.Module` data parallel
 
     - Parameters:
         - raw_model: A target `torch.nn.Module`
         - devices: A `list` of target `torch.device`
         - output_device: An optional `torch.device` of the target output device for the paralleled model
@@ -53,15 +53,15 @@
 
 def empty_cache() -> None:
     """Empty CUDA cache"""
     if GPU is not NotImplemented:
         torch.cuda.empty_cache()
 
 
-def search(specified: Optional[Union[torch.device, List[torch.device]]] = None) -> Tuple[torch.device, torch.device, List[torch.device]]:
+def search(specified: Optional[Union[torch.device, list[torch.device]]] = None) -> tuple[torch.device, torch.device, list[torch.device]]:
     """
     Find available devices
 
     - Pameters:
         - specified: An optional `torch.device` of specified
     - Returns: A `tuple` of CPU in `torch.device`, available device in `torch.device` and `list` of specified devices in `torch.device`
     """
@@ -85,15 +85,15 @@
             if d.index is None:
                 raise SystemError("All devices in the specified list must have a device index.")
     else:
         raise SystemError("Specified device list must not be empty")
     return CPU, device, specified
 
 
-def move_to_device(target: Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]], /, device: torch.device, *, recursive: bool = False) -> Union[DeviceMovable,  Dict[str, Union[DeviceMovable,  Any]], List[Union[DeviceMovable,  Any]]]:
+def move_to_device(target: Union[DeviceMovable,  dict[str, Union[DeviceMovable,  Any]], list[Union[DeviceMovable,  Any]]], /, device: torch.device, *, recursive: bool = False) -> Union[DeviceMovable,  dict[str, Union[DeviceMovable,  Any]], list[Union[DeviceMovable,  Any]]]:
     """
     Recurrently move a target variable to device if elements perform to `DeviceMovable` protocol
 
     - Parameters:
         - target: Either a target in `DeviceMovable`, a `dict` of targets in `DeviceMovable`, or a `list` of targets in `DeviceMovable`, targets in a `list` or `dict` that does not perform to `DeviceMovable` protocol will be returned without changing
         - device: A `torch.device` of target device
         - recursive: A `bool` flag of if move to device recursively
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager_core/errors/train.py` & `torchmanager_nightly-1.3a1/torchmanager_core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc5/torchmanager_core/protocols.py` & `torchmanager_nightly-1.3a1/torchmanager_core/protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import abc, torch, sys
 from enum import Enum
-from typing import Any, Callable, Dict, List, Optional, OrderedDict, Protocol, runtime_checkable
+from typing import Any, Callable, Optional, OrderedDict, Protocol, runtime_checkable
 from typing_extensions import Self
 
 from .devices.protocols import DeviceMovable
 from .version import Version
 from .view.protocols import VerboseControllable
 
 
@@ -33,15 +33,15 @@
             return sys.float_info.max
         else:
             raise TypeError(f"Monitor type {self} is not supported.")
 
 
 class LrSteping(Protocol):
     @abc.abstractmethod
-    def get_last_lr(self) -> List[float]:
+    def get_last_lr(self) -> list[float]:
         return NotImplemented
 
     @abc.abstractmethod
     def step(self, epoch: Optional[int] = None) -> None:
         pass
 
 
@@ -56,15 +56,15 @@
     """An object that can load state dict"""
 
     @abc.abstractmethod
     def load_state_dict(self, *, state_dict: OrderedDict[str, Any], strict: bool = True) -> Any:
         return NotImplemented
 
     @abc.abstractmethod
-    def state_dict(self, *, prefix: str = "", keep_vars: bool = False) -> Dict[str, Any]:
+    def state_dict(self, *, prefix: str = "", keep_vars: bool = False) -> dict[str, Any]:
         return NotImplemented
 
 
 class Trainable(Protocol):
     """An object that can switch training mode"""
     @abc.abstractmethod
     def eval(self) -> Self:
```

### Comparing `torchmanager_nightly-1.2rc5/torchmanager_core/random/seed.py` & `torchmanager_nightly-1.3a1/torchmanager_core/random/seed.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2rc5/torchmanager_core/version.py` & `torchmanager_nightly-1.3a1/torchmanager_core/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             elif 'rc' in version_str:
                 pre_release_parts = version_str.split('rc')
                 self.pre_release = PreRelease.RELEASE_CANDIDATE
             else:
                 pre_release_parts = [version_str, "0"]
                 self.pre_release = None
             version_str = pre_release_parts[0]
-            self.pre_release_version = int(pre_release_parts[1]) if pre_release_parts[1] != '' else 0
+            self.pre_release_version = int(pre_release_parts[1]) if pre_release_parts[1] != '' else 1
 
             # split version
             version_parts = version_str.split('.')
             self.main_version = int(version_parts[0])
             self.minor_version = int(version_parts[1])
             self.sub_version = int(version_parts[2]) if len(version_parts) > 2 else 0
         except Exception as e:
@@ -89,16 +89,15 @@
     def __repr__(self) -> str:
         version_str = f"v{self.main_version}"
         if self.minor_version > 0 or self.sub_version > 0:
             version_str += f".{self.minor_version}"
         if self.sub_version > 0:
             version_str += f".{self.sub_version}"
         if self.pre_release is not None:
-            pre_release_version = self.pre_release_version if self.pre_release_version > 0 else ""
-            version_str += f"{self.pre_release.value}{pre_release_version}"
+            version_str += f"{self.pre_release.value}{self.pre_release_version}"
         return version_str
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Version):
             return self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release == other.pre_release and self.pre_release_version == other.pre_release_version
         else:
             other = Version(str(other))
@@ -143,16 +142,16 @@
     def __le__(self, other: Any) -> bool:
         return self == other or self < other
 
     def __ge__(self, other: Any) -> bool:
         return self == other or self > other
 
 
-API = Version("v1.2")
-CURRENT = Version("v1.2rc5")
+API = Version("v1.3")
+CURRENT = Version("v1.3a1")
 DESCRIPTION: str = "PyTorch Training Manager {CURRENT}"
 
 
 class VersionError(SystemError):
     def __init__(self, method_name: str, maximum_supported_version: str) -> None:
         super().__init__(f"`{method_name}` has been deprecated and removed from version {maximum_supported_version}. Current version: {CURRENT}.")
```

### Comparing `torchmanager_nightly-1.2rc5/PKG-INFO` & `torchmanager_nightly-1.3a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: torchmanager-nightly
-Version: 1.2rc5
-Summary: PyTorch Training Manager v1.2rc5
+Version: 1.3a1
+Summary: PyTorch Training Manager v1.3 (Alpha 1)
 Home-page: https://github.com/kisonho/torchmanager.git
 Author: Qisheng He
 Author-email: Qisheng.He@wayne.edu
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: scipy
 Provides-Extra: tensorboard
 Requires-Dist: torch
@@ -19,15 +18,15 @@
 Project-URL: Repository, https://github.com/kisonho/torchmanager.git
 Description-Content-Type: text/markdown
 
 # torchmanager
 ### A highly-wrapped PyTorch training and testing manager
 
 ## Pre-request
-* Python 3.8+
+* Python 3.9+
 * PyTorch
 * tqdm
 * scipy (Optional)
 * tensorboard (Optional)
 
 ## Installation
 * PyPi: `pip install torchmanager-nightly`
```

