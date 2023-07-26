# Comparing `tmp/torchmanager-1.2b3.tar.gz` & `tmp/torchmanager-1.2b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager-1.2b3.tar", last modified: Wed Jul 26 18:23:30 2023, max compression
+gzip compressed data, was "torchmanager-1.2b4.tar", max compression
```

## Comparing `torchmanager-1.2b3.tar` & `torchmanager-1.2b4.tar`

### file list

```diff
@@ -1,70 +1,48 @@
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:23:30.623205 torchmanager-1.2b3/
--rw-r--r--   0 kisonho    (501) staff       (20)     1318 2023-07-13 17:22:38.000000 torchmanager-1.2b3/LICENSE
--rw-r--r--   0 kisonho    (501) staff       (20)     2109 2023-07-26 18:23:30.623097 torchmanager-1.2b3/PKG-INFO
--rw-r--r--   0 kisonho    (501) staff       (20)     1806 2023-07-26 18:22:19.000000 torchmanager-1.2b3/README.md
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:23:30.617555 torchmanager-1.2b3/core/
--rw-r--r--   0 kisonho    (501) staff       (20)      466 2023-07-26 18:22:25.000000 torchmanager-1.2b3/core/__init__.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:23:30.617919 torchmanager-1.2b3/core/devices/
--rw-r--r--   0 kisonho    (501) staff       (20)      109 2023-07-26 18:22:19.000000 torchmanager-1.2b3/core/devices/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4879 2023-07-26 18:22:25.000000 torchmanager-1.2b3/core/devices/device.py
--rw-r--r--   0 kisonho    (501) staff       (20)      264 2023-07-26 18:22:19.000000 torchmanager-1.2b3/core/devices/protocols.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:23:30.618280 torchmanager-1.2b3/core/errors/
--rw-r--r--   0 kisonho    (501) staff       (20)      153 2023-07-26 18:22:19.000000 torchmanager-1.2b3/core/errors/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)      350 2023-07-26 18:22:19.000000 torchmanager-1.2b3/core/errors/runtime.py
--rw-r--r--   0 kisonho    (501) staff       (20)      669 2023-07-26 18:22:19.000000 torchmanager-1.2b3/core/errors/train.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2731 2023-07-26 18:22:25.000000 torchmanager-1.2b3/core/protocols.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:23:30.618505 torchmanager-1.2b3/core/random/
--rw-r--r--   0 kisonho    (501) staff       (20)       44 2023-07-26 18:22:19.000000 torchmanager-1.2b3/core/random/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)      879 2023-07-26 18:22:25.000000 torchmanager-1.2b3/core/random/seed.py
--rw-r--r--   0 kisonho    (501) staff       (20)      204 2023-07-26 18:22:19.000000 torchmanager-1.2b3/core/typing.py
--rw-r--r--   0 kisonho    (501) staff       (20)     5137 2023-07-26 18:22:25.000000 torchmanager-1.2b3/core/version.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:23:30.618747 torchmanager-1.2b3/core/view/
--rw-r--r--   0 kisonho    (501) staff       (20)      439 2023-07-26 18:22:19.000000 torchmanager-1.2b3/core/view/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)      313 2023-07-26 18:22:19.000000 torchmanager-1.2b3/core/view/protocols.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:23:30.619327 torchmanager-1.2b3/lib/
--rw-r--r--   0 kisonho    (501) staff       (20)      290 2023-07-26 18:22:19.000000 torchmanager-1.2b3/lib/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)    10862 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/basic.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:23:30.620225 torchmanager-1.2b3/lib/callbacks/
--rw-r--r--   0 kisonho    (501) staff       (20)      658 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/callbacks/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4255 2023-07-26 18:22:19.000000 torchmanager-1.2b3/lib/callbacks/callback.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4542 2023-07-26 18:22:19.000000 torchmanager-1.2b3/lib/callbacks/ckpt.py
--rw-r--r--   0 kisonho    (501) staff       (20)     3523 2023-07-26 18:22:19.000000 torchmanager-1.2b3/lib/callbacks/dynamic.py
--rw-r--r--   0 kisonho    (501) staff       (20)     1608 2023-07-26 18:22:19.000000 torchmanager-1.2b3/lib/callbacks/early_stop.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4611 2023-07-26 18:22:19.000000 torchmanager-1.2b3/lib/callbacks/experiment.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2224 2023-07-26 18:22:19.000000 torchmanager-1.2b3/lib/callbacks/lr.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2440 2023-07-26 18:22:19.000000 torchmanager-1.2b3/lib/callbacks/tensorboard.py
--rw-r--r--   0 kisonho    (501) staff       (20)      963 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/compatibility.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:23:30.620464 torchmanager-1.2b3/lib/configs/
--rw-r--r--   0 kisonho    (501) staff       (20)       26 2023-07-26 18:22:19.000000 torchmanager-1.2b3/lib/configs/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2938 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/configs/basic.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:23:30.620804 torchmanager-1.2b3/lib/data/
--rw-r--r--   0 kisonho    (501) staff       (20)       85 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/data/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     6872 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/data/dataset.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2238 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/data/sliding.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:23:30.621377 torchmanager-1.2b3/lib/losses/
--rw-r--r--   0 kisonho    (501) staff       (20)      156 2023-07-26 18:22:19.000000 torchmanager-1.2b3/lib/losses/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     5386 2023-07-26 18:22:19.000000 torchmanager-1.2b3/lib/losses/cross_entropy.py
--rw-r--r--   0 kisonho    (501) staff       (20)     1047 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/losses/dice.py
--rw-r--r--   0 kisonho    (501) staff       (20)     5763 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/losses/loss.py
--rw-r--r--   0 kisonho    (501) staff       (20)     3117 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/losses/mse.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:23:30.622036 torchmanager-1.2b3/lib/metrics/
--rw-r--r--   0 kisonho    (501) staff       (20)      332 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/metrics/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4033 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/metrics/accuracy.py
--rw-r--r--   0 kisonho    (501) staff       (20)     3678 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/metrics/conf_met.py
--rw-r--r--   0 kisonho    (501) staff       (20)     5145 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/metrics/extractor.py
--rw-r--r--   0 kisonho    (501) staff       (20)     2070 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/metrics/iou.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4003 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/metrics/metric.py
--rw-r--r--   0 kisonho    (501) staff       (20)     9661 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/testing.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:23:30.622345 torchmanager-1.2b3/lib/train/
--rw-r--r--   0 kisonho    (501) staff       (20)       96 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/train/__init__.py
--rw-r--r--   0 kisonho    (501) staff       (20)     4964 2023-07-26 18:22:19.000000 torchmanager-1.2b3/lib/train/checkpoint.py
--rw-r--r--   0 kisonho    (501) staff       (20)      694 2023-07-26 18:22:19.000000 torchmanager-1.2b3/lib/train/learning_rate.py
--rw-r--r--   0 kisonho    (501) staff       (20)    14613 2023-07-26 18:22:25.000000 torchmanager-1.2b3/lib/training.py
--rw-r--r--   0 kisonho    (501) staff       (20)       38 2023-07-26 18:23:30.623241 torchmanager-1.2b3/setup.cfg
--rw-r--r--   0 kisonho    (501) staff       (20)     1550 2023-07-26 18:23:14.000000 torchmanager-1.2b3/setup.py
-drwxr-xr-x   0 kisonho    (501) staff       (20)        0 2023-07-26 18:23:30.622932 torchmanager-1.2b3/torchmanager.egg-info/
--rw-r--r--   0 kisonho    (501) staff       (20)     2109 2023-07-26 18:23:30.000000 torchmanager-1.2b3/torchmanager.egg-info/PKG-INFO
--rw-r--r--   0 kisonho    (501) staff       (20)     1211 2023-07-26 18:23:30.000000 torchmanager-1.2b3/torchmanager.egg-info/SOURCES.txt
--rw-r--r--   0 kisonho    (501) staff       (20)        1 2023-07-26 18:23:30.000000 torchmanager-1.2b3/torchmanager.egg-info/dependency_links.txt
--rw-r--r--   0 kisonho    (501) staff       (20)       11 2023-07-26 18:23:30.000000 torchmanager-1.2b3/torchmanager.egg-info/requires.txt
--rw-r--r--   0 kisonho    (501) staff       (20)       31 2023-07-26 18:23:30.000000 torchmanager-1.2b3/torchmanager.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1318 2023-07-13 17:22:38.863844 torchmanager-1.2b4/LICENSE
+-rw-r--r--   0        0        0      622 2023-07-26 18:25:45.912514 torchmanager-1.2b4/pyproject.toml
+-rw-r--r--   0        0        0      290 2023-07-26 18:24:39.703807 torchmanager-1.2b4/torchmanager/__init__.py
+-rw-r--r--   0        0        0    10862 2023-07-26 18:24:39.704060 torchmanager-1.2b4/torchmanager/basic.py
+-rw-r--r--   0        0        0      407 2023-07-26 18:24:39.704232 torchmanager-1.2b4/torchmanager/callbacks/__init__.py
+-rw-r--r--   0        0        0     4444 2023-07-26 18:24:39.704376 torchmanager-1.2b4/torchmanager/callbacks/callback.py
+-rw-r--r--   0        0        0     4542 2023-07-26 18:24:39.704533 torchmanager-1.2b4/torchmanager/callbacks/ckpt.py
+-rw-r--r--   0        0        0     3523 2023-07-26 18:24:39.704676 torchmanager-1.2b4/torchmanager/callbacks/dynamic.py
+-rw-r--r--   0        0        0     1608 2023-07-26 18:24:39.704817 torchmanager-1.2b4/torchmanager/callbacks/early_stop.py
+-rw-r--r--   0        0        0     2224 2023-07-26 18:24:39.704986 torchmanager-1.2b4/torchmanager/callbacks/lr.py
+-rw-r--r--   0        0        0      963 2023-07-26 18:24:39.705104 torchmanager-1.2b4/torchmanager/compatibility.py
+-rw-r--r--   0        0        0       26 2023-07-26 18:24:39.705242 torchmanager-1.2b4/torchmanager/configs/__init__.py
+-rw-r--r--   0        0        0     2938 2023-07-26 18:24:39.705396 torchmanager-1.2b4/torchmanager/configs/basic.py
+-rw-r--r--   0        0        0       85 2023-07-26 18:24:39.705531 torchmanager-1.2b4/torchmanager/data/__init__.py
+-rw-r--r--   0        0        0     6872 2023-07-26 18:24:39.705855 torchmanager-1.2b4/torchmanager/data/dataset.py
+-rw-r--r--   0        0        0     2238 2023-07-26 18:24:39.706045 torchmanager-1.2b4/torchmanager/data/sliding.py
+-rw-r--r--   0        0        0      156 2023-07-26 18:24:39.706191 torchmanager-1.2b4/torchmanager/losses/__init__.py
+-rw-r--r--   0        0        0     5386 2023-07-26 18:24:39.706333 torchmanager-1.2b4/torchmanager/losses/cross_entropy.py
+-rw-r--r--   0        0        0     1047 2023-07-26 18:24:39.706444 torchmanager-1.2b4/torchmanager/losses/dice.py
+-rw-r--r--   0        0        0     5757 2023-07-26 18:24:39.706586 torchmanager-1.2b4/torchmanager/losses/loss.py
+-rw-r--r--   0        0        0     3117 2023-07-26 18:24:39.706750 torchmanager-1.2b4/torchmanager/losses/mse.py
+-rw-r--r--   0        0        0      333 2023-07-26 18:24:39.706879 torchmanager-1.2b4/torchmanager/metrics/__init__.py
+-rw-r--r--   0        0        0     4033 2023-07-26 18:24:39.706997 torchmanager-1.2b4/torchmanager/metrics/accuracy.py
+-rw-r--r--   0        0        0     3678 2023-07-26 18:24:39.707119 torchmanager-1.2b4/torchmanager/metrics/conf_met.py
+-rw-r--r--   0        0        0     2738 2023-07-26 18:24:39.707255 torchmanager-1.2b4/torchmanager/metrics/extractor.py
+-rw-r--r--   0        0        0     2070 2023-07-26 18:24:39.707414 torchmanager-1.2b4/torchmanager/metrics/iou.py
+-rw-r--r--   0        0        0     4003 2023-07-26 18:24:39.707636 torchmanager-1.2b4/torchmanager/metrics/metric.py
+-rw-r--r--   0        0        0     9661 2023-07-26 18:24:39.707800 torchmanager-1.2b4/torchmanager/testing.py
+-rw-r--r--   0        0        0       96 2023-07-26 18:24:39.707946 torchmanager-1.2b4/torchmanager/train/__init__.py
+-rw-r--r--   0        0        0     4964 2023-07-26 18:24:39.708080 torchmanager-1.2b4/torchmanager/train/checkpoint.py
+-rw-r--r--   0        0        0      694 2023-07-26 18:24:39.708211 torchmanager-1.2b4/torchmanager/train/learning_rate.py
+-rw-r--r--   0        0        0    14606 2023-07-26 18:24:39.708411 torchmanager-1.2b4/torchmanager/training.py
+-rw-r--r--   0        0        0      459 2023-07-26 18:24:39.708541 torchmanager-1.2b4/torchmanager_core/__init__.py
+-rw-r--r--   0        0        0      109 2023-07-26 18:24:39.708665 torchmanager-1.2b4/torchmanager_core/devices/__init__.py
+-rw-r--r--   0        0        0     4879 2023-07-26 18:24:39.708814 torchmanager-1.2b4/torchmanager_core/devices/device.py
+-rw-r--r--   0        0        0      264 2023-07-26 18:24:39.708914 torchmanager-1.2b4/torchmanager_core/devices/protocols.py
+-rw-r--r--   0        0        0      212 2023-07-26 18:24:39.709040 torchmanager-1.2b4/torchmanager_core/errors/__init__.py
+-rw-r--r--   0        0        0      435 2023-07-26 18:24:39.709142 torchmanager-1.2b4/torchmanager_core/errors/dependencies.py
+-rw-r--r--   0        0        0      350 2023-07-26 18:24:39.709236 torchmanager-1.2b4/torchmanager_core/errors/runtime.py
+-rw-r--r--   0        0        0      669 2023-07-26 18:24:39.709333 torchmanager-1.2b4/torchmanager_core/errors/train.py
+-rw-r--r--   0        0        0     2772 2023-07-26 18:24:39.709460 torchmanager-1.2b4/torchmanager_core/protocols.py
+-rw-r--r--   0        0        0       44 2023-07-26 18:24:39.709561 torchmanager-1.2b4/torchmanager_core/random/__init__.py
+-rw-r--r--   0        0        0     1029 2023-07-26 18:24:39.709656 torchmanager-1.2b4/torchmanager_core/random/seed.py
+-rw-r--r--   0        0        0      204 2023-07-26 18:24:39.709751 torchmanager-1.2b4/torchmanager_core/typing.py
+-rw-r--r--   0        0        0     5137 2023-07-26 18:24:39.709903 torchmanager-1.2b4/torchmanager_core/version.py
+-rw-r--r--   0        0        0      439 2023-07-26 18:24:39.710016 torchmanager-1.2b4/torchmanager_core/view/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-26 18:24:39.710122 torchmanager-1.2b4/torchmanager_core/view/protocols.py
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 torchmanager-1.2b4/PKG-INFO
```

### Comparing `torchmanager-1.2b3/LICENSE` & `torchmanager-1.2b4/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/core/devices/device.py` & `torchmanager-1.2b4/torchmanager_core/devices/device.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/core/errors/train.py` & `torchmanager-1.2b4/torchmanager_core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/core/protocols.py` & `torchmanager-1.2b4/torchmanager_core/protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
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
```

### Comparing `torchmanager-1.2b3/core/random/seed.py` & `torchmanager-1.2b4/torchmanager_core/random/seed.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-import numpy as np, random, torch
+import random, torch
+
+try:
+    import numpy as np  # type: ignore
+except ImportError:
+    np = NotImplemented
 
 from .. import devices
 
 def freeze_seed(seed: int, /) -> None:
     """
     Freeze random with given seed
 
     - Parameters:
         - seed: An `int` for the random seed
     """
     random.seed(seed)
-    np.random.seed(seed)
+    if np is not NotImplemented:
+        np.random.seed(seed)
     torch.manual_seed(seed)
 
     if devices.GPU is not NotImplemented:
         torch.cuda.manual_seed_all(seed)
 
 def unfreeze_seed() -> int:
     """
@@ -24,13 +30,14 @@
     """
     # random PyTorch seed
     seed_64 = torch.random.seed()
     
     # set 32 bit seed for random and np package
     seed_32 = int(seed_64 / (2 ** 32)) if seed_64 > 2 ** 32 - 1 else seed_64 # convert to 32 bit seed
     random.seed(seed_32)
-    np.random.seed(seed_32)
+    if np is not NotImplemented:
+        np.random.seed(seed_32)
 
     # set cuda seed
     if devices.GPU is not NotImplemented:
         torch.cuda.manual_seed_all(seed_64)
     return seed_64
```

### Comparing `torchmanager-1.2b3/core/version.py` & `torchmanager-1.2b4/torchmanager_core/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,16 +88,16 @@
         return self == other or self < other
 
     def __ge__(self, other: Any) -> bool:
         return self == other or self > other
 
 
 API = Version("v1.2")
-CURRENT = Version("v1.2b3")
-DESCRIPTION: str = "PyTorch Training Manager v1.2 (Beta 3)"
+CURRENT = Version("v1.2b4")
+DESCRIPTION: str = "PyTorch Training Manager v1.2 (Beta 4)"
 
 
 class VersionError(SystemError):
     def __init__(self, method_name: str, maximum_supported_version: str) -> None:
         super().__init__(f"`{method_name}` has been deprecated and removed from version {maximum_supported_version}. Current version: {CURRENT}.")
```

### Comparing `torchmanager-1.2b3/lib/basic.py` & `torchmanager-1.2b4/torchmanager/basic.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/callbacks/callback.py` & `torchmanager-1.2b4/torchmanager/callbacks/callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,25 +111,31 @@
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

### Comparing `torchmanager-1.2b3/lib/callbacks/ckpt.py` & `torchmanager-1.2b4/torchmanager/callbacks/ckpt.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/callbacks/dynamic.py` & `torchmanager-1.2b4/torchmanager/callbacks/dynamic.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/callbacks/early_stop.py` & `torchmanager-1.2b4/torchmanager/callbacks/early_stop.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/callbacks/lr.py` & `torchmanager-1.2b4/torchmanager/callbacks/lr.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/compatibility.py` & `torchmanager-1.2b4/torchmanager/compatibility.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/configs/basic.py` & `torchmanager-1.2b4/torchmanager/configs/basic.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/data/dataset.py` & `torchmanager-1.2b4/torchmanager/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/data/sliding.py` & `torchmanager-1.2b4/torchmanager/data/sliding.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/losses/cross_entropy.py` & `torchmanager-1.2b4/torchmanager/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/losses/dice.py` & `torchmanager-1.2b4/torchmanager/losses/dice.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/losses/loss.py` & `torchmanager-1.2b4/torchmanager/losses/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from torchmanager_core import torch, _raise
-from torchmanager_core.typing import Any, Callable, Dict, List, Optional
+from torchmanager_core.typing import Any, Callable, List, Optional
 
 from ..metrics import Metric, Reduction
 
 
 class Loss(Metric):
     """
     The main loss function
```

### Comparing `torchmanager-1.2b3/lib/losses/mse.py` & `torchmanager-1.2b4/torchmanager/losses/mse.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/metrics/accuracy.py` & `torchmanager-1.2b4/torchmanager/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/metrics/conf_met.py` & `torchmanager-1.2b4/torchmanager/metrics/conf_met.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/metrics/iou.py` & `torchmanager-1.2b4/torchmanager/metrics/iou.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/metrics/metric.py` & `torchmanager-1.2b4/torchmanager/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/testing.py` & `torchmanager-1.2b4/torchmanager/testing.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/train/checkpoint.py` & `torchmanager-1.2b4/torchmanager/train/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/train/learning_rate.py` & `torchmanager-1.2b4/torchmanager/train/learning_rate.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.2b3/lib/training.py` & `torchmanager-1.2b4/torchmanager/training.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from torch.utils.data import DataLoader
 from torchmanager_core import devices, errors, math, torch, view
 from torchmanager_core.protocols import Resulting
-from torchmanager_core.typing import Any, Collection, Dict, List, Module, Optional, Self, Tuple, Union
+from torchmanager_core.typing import Any, Collection, Dict, List, Module, Optional, Self, Union
 
 from .callbacks import Callback
 from .data import Dataset
 from .losses import Loss, ParallelLoss
 from .metrics import Metric
 from .train import Checkpoint
 from .testing import Manager as _Manager
```

