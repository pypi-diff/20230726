# Comparing `tmp/ai2_kit-0.5.3.tar.gz` & `tmp/ai2_kit-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2_kit-0.5.3.tar", max compression
+gzip compressed data, was "ai2_kit-0.5.4.tar", max compression
```

## Comparing `ai2_kit-0.5.3.tar` & `ai2_kit-0.5.4.tar`

### file list

```diff
@@ -1,79 +1,40 @@
--rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.5.3/LICENSE
--rw-r--r--   0        0        0     2012 2023-07-21 03:28:16.683182 ai2_kit-0.5.3/README.md
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.3/ai2_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.5.3/ai2_kit/algorithm/__init__.py
--rw-r--r--   0        0        0      144 2023-06-15 02:12:13.145370 ai2_kit-0.5.3/ai2_kit/algorithm/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9573 2023-06-15 02:12:13.155370 ai2_kit-0.5.3/ai2_kit/algorithm/__pycache__/proton_transfer.cpython-39.pyc
--rw-r--r--   0        0        0    14221 2023-07-06 07:55:32.150324 ai2_kit-0.5.3/ai2_kit/algorithm/proton_transfer.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.3/ai2_kit/core/__init__.py
--rw-r--r--   0        0        0      139 2023-02-14 03:43:41.260120 ai2_kit-0.5.3/ai2_kit/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2243 2023-07-20 03:31:49.016223 ai2_kit-0.5.3/ai2_kit/core/__pycache__/artifact.cpython-39.pyc
--rw-r--r--   0        0        0     5928 2023-07-20 03:31:48.996223 ai2_kit-0.5.3/ai2_kit/core/__pycache__/checkpoint.cpython-39.pyc
--rw-r--r--   0        0        0      512 2023-06-15 07:55:24.192005 ai2_kit-0.5.3/ai2_kit/core/__pycache__/cmd.cpython-39.pyc
--rw-r--r--   0        0        0     7307 2023-07-24 07:57:09.456574 ai2_kit-0.5.3/ai2_kit/core/__pycache__/connector.cpython-39.pyc
--rw-r--r--   0        0        0     9586 2023-07-24 09:28:27.095300 ai2_kit-0.5.3/ai2_kit/core/__pycache__/executor.cpython-39.pyc
--rw-r--r--   0        0        0      894 2023-06-29 05:30:14.695752 ai2_kit-0.5.3/ai2_kit/core/__pycache__/future.cpython-39.pyc
--rw-r--r--   0        0        0     2847 2023-07-20 03:31:48.996223 ai2_kit-0.5.3/ai2_kit/core/__pycache__/job.cpython-39.pyc
--rw-r--r--   0        0        0      436 2023-06-29 05:30:14.695752 ai2_kit-0.5.3/ai2_kit/core/__pycache__/log.cpython-39.pyc
--rw-r--r--   0        0        0    10069 2023-07-21 03:41:53.042985 ai2_kit-0.5.3/ai2_kit/core/__pycache__/queue_system.cpython-39.pyc
--rw-r--r--   0        0        0     3063 2023-07-20 03:31:49.026223 ai2_kit-0.5.3/ai2_kit/core/__pycache__/resource_manager.cpython-39.pyc
--rw-r--r--   0        0        0     2611 2023-07-21 03:41:53.282985 ai2_kit-0.5.3/ai2_kit/core/__pycache__/script.cpython-39.pyc
--rw-r--r--   0        0        0     8116 2023-07-24 09:28:27.215300 ai2_kit-0.5.3/ai2_kit/core/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0     1854 2023-07-06 07:55:32.150324 ai2_kit-0.5.3/ai2_kit/core/artifact.py
--rw-r--r--   0        0        0     5894 2023-07-25 01:13:41.843210 ai2_kit-0.5.3/ai2_kit/core/checkpoint.py
--rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.5.3/ai2_kit/core/cmd.py
--rw-r--r--   0        0        0     5766 2023-07-21 04:37:23.322249 ai2_kit-0.5.3/ai2_kit/core/connector.py
--rw-r--r--   0        0        0     8006 2023-07-24 09:25:32.885347 ai2_kit-0.5.3/ai2_kit/core/executor.py
--rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.5.3/ai2_kit/core/future.py
--rw-r--r--   0        0        0     1991 2023-07-06 07:55:32.150324 ai2_kit-0.5.3/ai2_kit/core/job.py
--rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.5.3/ai2_kit/core/log.py
--rw-r--r--   0        0        0     9587 2023-07-21 01:27:23.144801 ai2_kit-0.5.3/ai2_kit/core/queue_system.py
--rw-r--r--   0        0        0     2572 2023-07-06 07:55:32.150324 ai2_kit-0.5.3/ai2_kit/core/resource_manager.py
--rw-r--r--   0        0        0     2363 2023-07-21 01:27:23.144801 ai2_kit-0.5.3/ai2_kit/core/script.py
--rw-r--r--   0        0        0     5900 2023-07-24 09:25:32.885347 ai2_kit-0.5.3/ai2_kit/core/util.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.3/ai2_kit/dflow/__init__.py
--rw-r--r--   0        0        0      110 2023-06-15 07:55:24.202005 ai2_kit-0.5.3/ai2_kit/dflow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.3/ai2_kit/domain/__init__.py
--rw-r--r--   0        0        0      141 2023-02-14 03:43:41.670121 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4703 2023-07-25 00:52:37.103514 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/asap.cpython-39.pyc
--rw-r--r--   0        0        0     2517 2023-06-29 05:30:14.805753 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/cll.cpython-39.pyc
--rw-r--r--   0        0        0     3221 2023-02-23 07:10:20.489990 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/common.cpython-39.pyc
--rw-r--r--   0        0        0     1532 2023-07-24 09:28:27.285300 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/constant.cpython-39.pyc
--rw-r--r--   0        0        0     5609 2023-07-21 03:41:53.572985 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/cp2k.cpython-39.pyc
--rw-r--r--   0        0        0     5117 2023-07-24 09:28:27.245300 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/data.cpython-39.pyc
--rw-r--r--   0        0        0     6200 2023-06-27 02:27:16.171507 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/data_helper.cpython-39.pyc
--rw-r--r--   0        0        0     6358 2023-07-21 03:41:53.282985 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/deepmd.cpython-39.pyc
--rw-r--r--   0        0        0     2519 2023-07-20 03:31:49.026223 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/iface.cpython-39.pyc
--rw-r--r--   0        0        0    12264 2023-07-21 03:41:53.392985 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/lammps.cpython-39.pyc
--rw-r--r--   0        0        0     9323 2023-07-24 09:28:27.295300 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/lasp.cpython-39.pyc
--rw-r--r--   0        0        0    10687 2023-07-24 09:28:27.305300 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/selector.cpython-39.pyc
--rw-r--r--   0        0        0      538 2023-07-21 03:41:53.862985 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/updater.cpython-39.pyc
--rw-r--r--   0        0        0     3360 2023-07-24 08:47:10.485875 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/util.cpython-39.pyc
--rw-r--r--   0        0        0     6463 2023-07-21 03:41:53.572985 ai2_kit-0.5.3/ai2_kit/domain/__pycache__/vasp.cpython-39.pyc
--rw-r--r--   0        0        0     5449 2023-07-25 00:53:24.333505 ai2_kit-0.5.3/ai2_kit/domain/asap.py
--rw-r--r--   0        0        0     1805 2023-07-24 09:25:32.885347 ai2_kit-0.5.3/ai2_kit/domain/constant.py
--rw-r--r--   0        0        0     6585 2023-07-21 01:27:23.144801 ai2_kit-0.5.3/ai2_kit/domain/cp2k.py
--rw-r--r--   0        0        0     5454 2023-07-24 09:25:32.885347 ai2_kit-0.5.3/ai2_kit/domain/data.py
--rw-r--r--   0        0        0     7895 2023-07-25 02:20:46.132275 ai2_kit-0.5.3/ai2_kit/domain/deepmd.py
--rw-r--r--   0        0        0     1121 2023-07-06 07:55:32.160324 ai2_kit-0.5.3/ai2_kit/domain/iface.py
--rw-r--r--   0        0        0    17292 2023-07-25 01:07:27.943305 ai2_kit-0.5.3/ai2_kit/domain/lammps.py
--rw-r--r--   0        0        0     9046 2023-07-24 09:25:32.885347 ai2_kit-0.5.3/ai2_kit/domain/lasp.py
--rw-r--r--   0        0        0    13569 2023-07-25 03:06:53.751626 ai2_kit-0.5.3/ai2_kit/domain/selector.py
--rw-r--r--   0        0        0      186 2023-07-21 01:27:23.144801 ai2_kit-0.5.3/ai2_kit/domain/updater.py
--rw-r--r--   0        0        0     6882 2023-07-24 08:46:11.435884 ai2_kit-0.5.3/ai2_kit/domain/util.py
--rw-r--r--   0        0        0     7678 2023-07-25 03:06:53.751626 ai2_kit-0.5.3/ai2_kit/domain/vasp.py
--rw-r--r--   0        0        0     1900 2023-07-06 07:55:32.150324 ai2_kit-0.5.3/ai2_kit/main.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.3/ai2_kit/tool/__init__.py
--rw-r--r--   0        0        0      139 2023-06-28 08:15:51.392260 ai2_kit-0.5.3/ai2_kit/tool/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1616 2023-06-28 08:15:51.392260 ai2_kit-0.5.3/ai2_kit/tool/__pycache__/ase.cpython-39.pyc
--rw-r--r--   0        0        0     1039 2023-07-07 01:23:16.068582 ai2_kit-0.5.3/ai2_kit/tool/ase.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.3/ai2_kit/workflow/__init__.py
--rw-r--r--   0        0        0      143 2023-02-14 03:43:41.260120 ai2_kit-0.5.3/ai2_kit/workflow/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7937 2023-07-24 09:28:27.095300 ai2_kit-0.5.3/ai2_kit/workflow/__pycache__/cll_mlp.cpython-39.pyc
--rw-r--r--   0        0        0     5996 2023-06-15 08:55:37.729603 ai2_kit-0.5.3/ai2_kit/workflow/__pycache__/ec_fep.cpython-39.pyc
--rw-r--r--   0        0        0     5966 2023-02-14 03:43:41.260120 ai2_kit-0.5.3/ai2_kit/workflow/__pycache__/fep.cpython-39.pyc
--rw-r--r--   0        0        0     6336 2023-07-20 03:31:49.786223 ai2_kit-0.5.3/ai2_kit/workflow/__pycache__/fep_mlp.cpython-39.pyc
--rw-r--r--   0        0        0    10064 2023-07-24 09:25:32.885347 ai2_kit-0.5.3/ai2_kit/workflow/cll_mlp.py
--rw-r--r--   0        0        0     9135 2023-07-24 09:25:32.885347 ai2_kit-0.5.3/ai2_kit/workflow/fep_mlp.py
--rw-r--r--   0        0        0      953 2023-07-25 03:07:12.751625 ai2_kit-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 ai2_kit-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.5.4/LICENSE
+-rw-r--r--   0        0        0     2012 2023-07-21 03:28:16.683182 ai2_kit-0.5.4/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.4/ai2_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.5.4/ai2_kit/algorithm/__init__.py
+-rw-r--r--   0        0        0    14221 2023-07-06 07:55:32.150324 ai2_kit-0.5.4/ai2_kit/algorithm/proton_transfer.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.4/ai2_kit/core/__init__.py
+-rw-r--r--   0        0        0     1854 2023-07-06 07:55:32.150324 ai2_kit-0.5.4/ai2_kit/core/artifact.py
+-rw-r--r--   0        0        0     5894 2023-07-25 01:13:41.843210 ai2_kit-0.5.4/ai2_kit/core/checkpoint.py
+-rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.5.4/ai2_kit/core/cmd.py
+-rw-r--r--   0        0        0     5766 2023-07-21 04:37:23.322249 ai2_kit-0.5.4/ai2_kit/core/connector.py
+-rw-r--r--   0        0        0     8127 2023-07-25 07:20:18.077054 ai2_kit-0.5.4/ai2_kit/core/executor.py
+-rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.5.4/ai2_kit/core/future.py
+-rw-r--r--   0        0        0     1991 2023-07-06 07:55:32.150324 ai2_kit-0.5.4/ai2_kit/core/job.py
+-rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.5.4/ai2_kit/core/log.py
+-rw-r--r--   0        0        0     9587 2023-07-21 01:27:23.144801 ai2_kit-0.5.4/ai2_kit/core/queue_system.py
+-rw-r--r--   0        0        0     2572 2023-07-06 07:55:32.150324 ai2_kit-0.5.4/ai2_kit/core/resource_manager.py
+-rw-r--r--   0        0        0     2363 2023-07-25 08:15:29.956291 ai2_kit-0.5.4/ai2_kit/core/script.py
+-rw-r--r--   0        0        0     5894 2023-07-26 03:27:15.718128 ai2_kit-0.5.4/ai2_kit/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.4/ai2_kit/dflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.4/ai2_kit/domain/__init__.py
+-rw-r--r--   0        0        0     5449 2023-07-25 00:53:24.333505 ai2_kit-0.5.4/ai2_kit/domain/asap.py
+-rw-r--r--   0        0        0     1805 2023-07-24 09:25:32.885347 ai2_kit-0.5.4/ai2_kit/domain/constant.py
+-rw-r--r--   0        0        0     6585 2023-07-21 01:27:23.144801 ai2_kit-0.5.4/ai2_kit/domain/cp2k.py
+-rw-r--r--   0        0        0     5454 2023-07-24 09:25:32.885347 ai2_kit-0.5.4/ai2_kit/domain/data.py
+-rw-r--r--   0        0        0     7895 2023-07-25 02:20:46.132275 ai2_kit-0.5.4/ai2_kit/domain/deepmd.py
+-rw-r--r--   0        0        0     1121 2023-07-06 07:55:32.160324 ai2_kit-0.5.4/ai2_kit/domain/iface.py
+-rw-r--r--   0        0        0    17292 2023-07-25 01:07:27.943305 ai2_kit-0.5.4/ai2_kit/domain/lammps.py
+-rw-r--r--   0        0        0     9046 2023-07-24 09:25:32.885347 ai2_kit-0.5.4/ai2_kit/domain/lasp.py
+-rw-r--r--   0        0        0    13433 2023-07-26 03:43:28.387903 ai2_kit-0.5.4/ai2_kit/domain/selector.py
+-rw-r--r--   0        0        0      186 2023-07-21 01:27:23.144801 ai2_kit-0.5.4/ai2_kit/domain/updater.py
+-rw-r--r--   0        0        0     6882 2023-07-24 08:46:11.435884 ai2_kit-0.5.4/ai2_kit/domain/util.py
+-rw-r--r--   0        0        0     7678 2023-07-25 03:06:53.751626 ai2_kit-0.5.4/ai2_kit/domain/vasp.py
+-rw-r--r--   0        0        0     1900 2023-07-06 07:55:32.150324 ai2_kit-0.5.4/ai2_kit/main.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.5.4/ai2_kit/tool/__init__.py
+-rw-r--r--   0        0        0     1039 2023-07-07 01:23:16.068582 ai2_kit-0.5.4/ai2_kit/tool/ase.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.5.4/ai2_kit/workflow/__init__.py
+-rw-r--r--   0        0        0    10064 2023-07-24 09:25:32.885347 ai2_kit-0.5.4/ai2_kit/workflow/cll_mlp.py
+-rw-r--r--   0        0        0     9135 2023-07-24 09:25:32.885347 ai2_kit-0.5.4/ai2_kit/workflow/fep_mlp.py
+-rw-r--r--   0        0        0      953 2023-07-26 03:46:11.947863 ai2_kit-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 ai2_kit-0.5.4/PKG-INFO
```

### Comparing `ai2_kit-0.5.3/LICENSE` & `ai2_kit-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/README.md` & `ai2_kit-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/algorithm/proton_transfer.py` & `ai2_kit-0.5.4/ai2_kit/algorithm/proton_transfer.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/core/artifact.py` & `ai2_kit-0.5.4/ai2_kit/core/artifact.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/core/checkpoint.py` & `ai2_kit-0.5.4/ai2_kit/core/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/core/connector.py` & `ai2_kit-0.5.4/ai2_kit/core/connector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/core/executor.py` & `ai2_kit-0.5.4/ai2_kit/core/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .util import s_uuid
 from .log import get_logger
 
 logger = get_logger(__name__)
 
 
 from pydantic import BaseModel
-from typing import Optional, Dict, List, TypeVar, Callable, Mapping
+from typing import Optional, Dict, List, TypeVar, Callable, Mapping, Union
 from abc import ABC, abstractmethod
 from invoke import Result
 import os
 import shlex
 import base64
 import bz2
 import cloudpickle
@@ -89,15 +89,18 @@
             self.mkdir(path)
             logger.info('create path: %s', path)
         return paths
 
 class HpcExecutor(Executor):
 
     @classmethod
-    def from_config(cls, config: BaseExecutorConfig, name: str):
+    def from_config(cls, config: Union[dict, BaseExecutorConfig], name: str = ''):
+        if isinstance(config, dict):
+            config = BaseExecutorConfig.parse_obj(config)
+
         if config.ssh:
             connector = SshConnector.from_config(config.ssh)
         else:
             connector = LocalConnector()
         queue_system = None
         if config.queue_system.slurm:
             queue_system = Slurm()
```

### Comparing `ai2_kit-0.5.3/ai2_kit/core/job.py` & `ai2_kit-0.5.4/ai2_kit/core/job.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/core/queue_system.py` & `ai2_kit-0.5.4/ai2_kit/core/queue_system.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/core/resource_manager.py` & `ai2_kit-0.5.4/ai2_kit/core/resource_manager.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/core/script.py` & `ai2_kit-0.5.4/ai2_kit/core/script.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/core/util.py` & `ai2_kit-0.5.4/ai2_kit/core/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         >>> flat_evenly([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
         [1, 4, 7, 2, 5, 8, 3, 6, 9]
         Ref: https://stackoverflow.com/questions/76751171/how-to-flat-a-list-of-lists-and-ensure-the-output-result-distributed-evenly-in-p
         """
         return [e for tup in zip_longest(*list_of_lists) for e in tup if e is not None]
 
 
-    def dump_json(obj: dict, path: str):
+    def dump_json(obj, path: str):
         with open(path, 'w', encoding='utf-8') as f:
             json.dump(obj, f, indent=2)
 
     def flush_stdio():
         import sys
         sys.stdout.flush()
         sys.stderr.flush()
```

### Comparing `ai2_kit-0.5.3/ai2_kit/domain/asap.py` & `ai2_kit-0.5.4/ai2_kit/domain/asap.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/domain/constant.py` & `ai2_kit-0.5.4/ai2_kit/domain/constant.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/domain/cp2k.py` & `ai2_kit-0.5.4/ai2_kit/domain/cp2k.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/domain/data.py` & `ai2_kit-0.5.4/ai2_kit/domain/data.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/domain/deepmd.py` & `ai2_kit-0.5.4/ai2_kit/domain/deepmd.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/domain/iface.py` & `ai2_kit-0.5.4/ai2_kit/domain/iface.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/domain/lammps.py` & `ai2_kit-0.5.4/ai2_kit/domain/lammps.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/domain/lasp.py` & `ai2_kit-0.5.4/ai2_kit/domain/lasp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/domain/selector.py` & `ai2_kit-0.5.4/ai2_kit/domain/selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from asaplib.data.xyz import ASAPXYZ
 from ai2_kit.core.artifact import Artifact, ArtifactDict
 from ai2_kit.core.log import get_logger
 from ai2_kit.core.util import flat_evenly, dump_json, flush_stdio
 
-from typing import List, Optional
+from typing import List, Optional, Tuple
 from io import StringIO
 from pydantic import BaseModel
 from dataclasses import dataclass
 import pandas as pd
 from tabulate import tabulate
 from itertools import groupby
 from operator import itemgetter
@@ -72,47 +72,47 @@
     executor = ctx.resource_manager.default_executor
     work_dir = os.path.join(executor.work_dir, ctx.path_prefix)
     executor.mkdir(work_dir)
 
     f_trust_lo = input.config.f_trust_lo
     f_trust_hi = input.config.f_trust_hi
 
-    candidates = executor.run_python_fn(bulk_select_structures_by_model_devi)(
+    results = executor.run_python_fn(bulk_select_structures_by_model_devi)(
         model_devi_outputs=[a.to_dict() for a in input.model_devi_data],
         model_devi_filename=input.model_devi_out_filename,
         f_trust_lo=f_trust_lo, f_trust_hi=f_trust_hi,
         type_map=input.type_map, work_dir=work_dir,
     )
 
+    candidates = [candidate for candidate, _ in results if candidate is not None]  # filter out None
+    stats = [stats for _, stats in results]
+
     # write model_deviation stats report
-    def _get_row(candidate: ArtifactDict):
-        attrs = candidate['attrs']
-        url = attrs['model_devi_file']
+    def _get_row(stat: dict):
+        url = stat['src']
         url = f'...{url[-30:]}' if len(url) > 30 else url  # wrap url if it is too long
-        result = attrs['model_devi_result']
-        total, good, decent, poor = result['total'], result['good'], result['decent'], result['poor']
+        total, good, decent, poor = stat['total'], stat['good'], stat['decent'], stat['poor']
         return [
             url, total, good, decent, poor,
             f'{good / total * 100:.2f}%', f'{decent / total * 100:.2f}%', f'{poor / total * 100:.2f}%',
         ]
-
     headers = ['file', 'total', 'good', 'decent', 'poor', 'good%', 'decent%', 'poor%']
-    table = [ _get_row(candidate) for candidate in candidates]
+    table = [ _get_row(stat) for stat in stats]
     total = sum(row[1] for row in table)
     total_good = sum(row[2] for row in table)
 
     stats_report = tabulate(table, headers=headers, tablefmt='tsv')
-    logger.info('stats report: \n%s', stats_report)
+    logger.info('stats report: \n%s\n', stats_report)
     executor.dump_text(stats_report, os.path.join(work_dir, 'stats.tsv'))
 
     # further select candidates by ASAP
     if input.config.asap_options and not input.config.asap_options.disable:
         asap_options = input.config.asap_options
         candidates = executor.run_python_fn(bulk_select_distinct_structures)(
-            candidates=[c for c in candidates if c['attrs']['size'] > 0],  # filter empty structures
+            candidates=candidates,
             descriptor_opt=asap_options.descriptor,
             dim_reducer_opt=asap_options.dim_reducer,
             cluster_opt=asap_options.cluster,
             type_map=input.type_map,
             work_dir=work_dir,
             max_structures_per_system=asap_options.max_structures_per_system,
         )
@@ -128,15 +128,15 @@
     def bulk_select_structures_by_model_devi(model_devi_outputs: List[ArtifactDict],
                                              model_devi_filename: str,
                                              f_trust_lo: float,
                                              f_trust_hi: float,
                                              type_map: List[str],
                                              work_dir: str,
                                              workers: int = 4,
-                                             ) -> List[ArtifactDict]:
+                                             ) -> List[Tuple[Optional[ArtifactDict], dict]]:
         import joblib
         return joblib.Parallel(n_jobs=workers)(
             joblib.delayed(select_structures_by_model_devi)(
                 model_devi_output=output,
                 model_devi_filename=model_devi_filename,
                 f_trust_lo=f_trust_lo, f_trust_hi=f_trust_hi,
                 type_map=type_map,
@@ -148,15 +148,15 @@
 
     def select_structures_by_model_devi(model_devi_output: ArtifactDict,
                                         model_devi_filename: str,
                                         f_trust_lo: float,
                                         f_trust_hi: float,
                                         type_map: List[str],
                                         work_dir: str,
-                                        ) -> ArtifactDict:
+                                        ) -> Tuple[Optional[ArtifactDict], dict]:
         """
         analysis the model_devi output of explore stage and select candidates
         """
         os.makedirs(work_dir, exist_ok=True)
         model_devi_out_url = model_devi_output['url']
         force_col = 'max_devi_f'
         print(f'criteria: {f_trust_lo} <= {force_col} < {f_trust_hi}')
@@ -180,91 +180,90 @@
         # 1      100    0.006987    0.000550    0.003952    0.128178    0.006042    0.022608
 
         # evaluate new found structures by their model_devi score in 3 levels: good, decent, poor
         good_df   = df[df[force_col] < f_trust_lo]
         decent_df = df[(df[force_col] >= f_trust_lo) & (df[force_col] < f_trust_hi)]
         poor_df   = df[df[force_col] >= f_trust_hi]
 
-        model_devi_result = {
+        stats = {
+            'src': model_devi_out_file,
             'total': len(df),
             'good': len(good_df),
             'decent': len(decent_df),
             'poor': len(poor_df),
         }
 
         # write decent structures into ase atoms and write to file
-        model_devi_decent_file = os.path.join(work_dir, 'model_devi_decent.xyz')
-        atoms_list = []
+        decent_structures_artifact = None
         if len(decent_df) > 0:
+            model_devi_decent_file = os.path.join(work_dir, 'model_devi_decent.xyz')
             if data_format == DataFormat.LAMMPS_OUTPUT_DIR:
+                atoms_list = []
                 for frame_id in decent_df.step:
                     dump_file = os.path.join(model_devi_out_url, LAMMPS_TRAJ_DIR, f'{frame_id}{LAMMPS_TRAJ_SUFFIX}')
                     atoms_list.extend(ase.io.read(dump_file, ':', format='lammps-dump-text', specorder=type_map))
             elif data_format == DataFormat.LASP_LAMMPS_OUT_DIR:
                 structures_file = os.path.join(model_devi_out_url, 'structures.xyz')
-                atoms_list.extend(itemgetter(*decent_df.step)(ase.io.read(structures_file, ':', format='extxyz')))  # type: ignore
+                atoms_list = list(itemgetter(*decent_df.step)(ase.io.read(structures_file, ':', format='extxyz')))  # type: ignore
             else:
                 raise ValueError('unknown model_devi_data types')
             ase.io.write(model_devi_decent_file, atoms_list, format='extxyz')
-
-        output = {
-            'url': model_devi_decent_file,
-            'format': DataFormat.EXTXYZ,
-            'attrs': {
-                **model_devi_output['attrs'],
-                'model_devi_file': model_devi_out_file,
-                'model_devi_result': model_devi_result,
-                'size': len(atoms_list)
+            decent_structures_artifact = {
+                'url': model_devi_decent_file,
+                'format': DataFormat.EXTXYZ,
+                'attrs': {
+                    **model_devi_output['attrs'],
+                    'size': len(atoms_list)
+                }
             }
-        }
-        dump_json(output, os.path.join(work_dir, 'output.debug.json'))
-        return output  # type: ignore
+        dump_json([decent_structures_artifact, stats], os.path.join(work_dir, 'output.debug.json'))
+        return decent_structures_artifact, stats  # type: ignore
 
     def bulk_select_distinct_structures(candidates: List[ArtifactDict],
                                         descriptor_opt: dict,
                                         dim_reducer_opt: dict,
                                         cluster_opt: dict,
                                         type_map: List[str],
                                         work_dir: str,
                                         max_structures_per_system: int = -1,
                                         workers: int = 4,
                                         ) -> List[ArtifactDict]:
 
         inputs = []
-        for i, (ancestor, candidate_group) in enumerate(groupby(candidates, key=lambda c: c['attrs']['ancestor'])):
+        for i, (ancestor_key, candidate_group) in enumerate(groupby(candidates, key=lambda c: c['attrs']['ancestor'])):
             candidate_group = list(candidate_group)
             inputs.append((candidate_group, candidate_group[0]['attrs']))
 
         import joblib
         return joblib.Parallel(n_jobs=workers)(
             joblib.delayed(select_distinct_structures)(
                 candidates=group,
-                ancestor_attrs=attrs,
+                attrs=attrs,
                 descriptor_opt=descriptor_opt,
                 dim_reducer_opt=dim_reducer_opt,
                 cluster_opt=cluster_opt,
                 type_map=type_map,
                 work_dir=os.path.join(work_dir, 'asap', f'{i:06}'),
                 max_structures_per_system=max_structures_per_system,
             ) for i, (group, attrs) in enumerate(inputs)
         )  # type: ignore
 
 
     def select_distinct_structures(candidates: List[ArtifactDict],
-                                   ancestor_attrs: dict,
+                                   attrs: dict,
                                    descriptor_opt: dict,
                                    dim_reducer_opt: dict,
                                    cluster_opt: dict,
                                    type_map: List[str],
                                    work_dir: str,
                                    max_structures_per_system: int = -1,
                                    ):
         os.makedirs(work_dir, exist_ok=True)
 
-        dump_json(ancestor_attrs, os.path.join(work_dir, 'attrs.debug.json'))
+        dump_json(attrs, os.path.join(work_dir, 'attrs.debug.json'))
         # load structures and save it to a tmp file for ASAP to load
         atoms_list = [atoms for _, atoms in artifacts_to_ase_atoms(candidates, type_map=type_map)]
 
         if len(atoms_list) < max_structures_per_system:
             ...  # TODO: no need for extra screening
 
         tmp_structures_file = os.path.join(work_dir, '.tmp-structures.xyz')
@@ -276,40 +275,34 @@
         # group structures
         path_prefix = os.path.join(work_dir, 'asap')
         descriptors, _ = get_descriptor(asapxyz, descriptor_opt, path_prefix=path_prefix)
         reduced_descriptors = reduce_dimension(descriptors, dim_reducer_opt)
         trainer = get_trainer(reduced_descriptors, cluster_opt)
         cluster_labels = get_cluster(asapxyz, reduced_descriptors, trainer, path_prefix=path_prefix)
 
-        # remove noise group from result
-        if -1 in cluster_labels:
-            del cluster_labels[-1]
-
         # if max_structures_per_system is not set
         # selected at least 1 structure from each group
         if max_structures_per_system <= 0:
             max_structures_per_system = len(cluster_labels)
 
-        # break up the clusters into a list and
+        # unpack clusters into a list and
         # ensure frames of the same group won't be next to each other
         # so that we can pick up distinct structures by simply choose the first N frames
-        selected_frames = flat_evenly(cluster_labels.values())[:max_structures_per_system]
+        order_frames = flat_evenly(cluster_labels.values())
+        selected_frames = order_frames[:max_structures_per_system]
         selected_atoms_list = [atoms_list[i] for i in selected_frames]
 
         # write selected structures to file
         distinct_structures_file = os.path.join(work_dir,  'distinct_structures.xyz')
         ase.io.write(distinct_structures_file, selected_atoms_list, format='extxyz')
 
         output = {
             'url': distinct_structures_file,
             'format': DataFormat.EXTXYZ,
-            'attrs': {
-                **ancestor_attrs,
-                'distinct_structures_file': distinct_structures_file,
-            }
+            'attrs': attrs,
         }
         dump_json(output, os.path.join(work_dir, 'output.debug.json'))
         flush_stdio()  # flush joblib stdio buffer
         return output
 
     return (
         bulk_select_structures_by_model_devi,
```

### Comparing `ai2_kit-0.5.3/ai2_kit/domain/util.py` & `ai2_kit-0.5.4/ai2_kit/domain/util.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/domain/vasp.py` & `ai2_kit-0.5.4/ai2_kit/domain/vasp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/main.py` & `ai2_kit-0.5.4/ai2_kit/main.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/tool/ase.py` & `ai2_kit-0.5.4/ai2_kit/tool/ase.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/workflow/cll_mlp.py` & `ai2_kit-0.5.4/ai2_kit/workflow/cll_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/ai2_kit/workflow/fep_mlp.py` & `ai2_kit-0.5.4/ai2_kit/workflow/fep_mlp.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.5.3/pyproject.toml` & `ai2_kit-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai2-kit"
-version = "0.5.3"
+version = "0.5.4"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ai2_kit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `ai2_kit-0.5.3/PKG-INFO` & `ai2_kit-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai2-kit
-Version: 0.5.3
+Version: 0.5.4
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

