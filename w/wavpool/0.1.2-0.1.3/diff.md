# Comparing `tmp/wavpool-0.1.2.tar.gz` & `tmp/wavpool-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wavpool-0.1.2.tar", max compression
+gzip compressed data, was "wavpool-0.1.3.tar", max compression
```

## Comparing `wavpool-0.1.2.tar` & `wavpool-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1067 2023-07-26 14:28:52.244207 wavpool-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     4141 2023-07-26 14:28:52.244207 wavpool-0.1.2/README.md
--rw-r--r--   0        0        0      761 2023-07-26 14:47:05.019861 wavpool-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-26 14:28:52.244207 wavpool-0.1.2/wavpool/__init__.py
--rw-r--r--   0        0        0      216 2023-07-26 14:28:52.244207 wavpool-0.1.2/wavpool/data_generators/__init__.py
--rw-r--r--   0        0        0      560 2023-07-26 14:28:52.244207 wavpool-0.1.2/wavpool/data_generators/cifar_generator.py
--rw-r--r--   0        0        0     2296 2023-07-26 14:28:52.244207 wavpool-0.1.2/wavpool/data_generators/data_generator.py
--rw-r--r--   0        0        0      438 2023-07-26 14:28:52.244207 wavpool-0.1.2/wavpool/data_generators/fashion_mnist_generator.py
--rw-r--r--   0        0        0      373 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/data_generators/mnist_generator.py
--rw-r--r--   0        0        0      182 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/models/__init__.py
--rw-r--r--   0        0        0     1478 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/models/vanillaCNN.py
--rw-r--r--   0        0        0     1768 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/models/vanillaMLP.py
--rw-r--r--   0        0        0     1630 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/models/wavMLP.py
--rw-r--r--   0        0        0     2122 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/models/wavelet_layer.py
--rw-r--r--   0        0        0     2867 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/models/wavpool.py
--rw-r--r--   0        0        0     6850 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/training/finetune_network.py
--rw-r--r--   0        0        0     6092 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/training/plot_results.py
--rw-r--r--   0        0        0     5044 2023-07-26 14:56:31.209349 wavpool-0.1.2/wavpool/training/train_model.py
--rw-r--r--   0        0        0     1602 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/training/training_metrics.py
--rw-r--r--   0        0        0        0 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/utils/__init__.py
--rw-r--r--   0        0        0     1480 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/utils/levels.py
--rw-r--r--   0        0        0      367 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/utils/voting.py
--rw-r--r--   0        0        0     5236 1970-01-01 00:00:00.000000 wavpool-0.1.2/setup.py
--rw-r--r--   0        0        0     5095 1970-01-01 00:00:00.000000 wavpool-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-26 14:28:52.244207 wavpool-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     4141 2023-07-26 14:28:52.244207 wavpool-0.1.3/README.md
+-rw-r--r--   0        0        0      720 2023-07-26 15:20:21.698736 wavpool-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 14:28:52.244207 wavpool-0.1.3/wavpool/__init__.py
+-rw-r--r--   0        0        0      216 2023-07-26 14:56:51.393388 wavpool-0.1.3/wavpool/data_generators/__init__.py
+-rw-r--r--   0        0        0      560 2023-07-26 14:56:51.393388 wavpool-0.1.3/wavpool/data_generators/cifar_generator.py
+-rw-r--r--   0        0        0     2296 2023-07-26 14:28:52.244207 wavpool-0.1.3/wavpool/data_generators/data_generator.py
+-rw-r--r--   0        0        0      438 2023-07-26 14:56:51.393388 wavpool-0.1.3/wavpool/data_generators/fashion_mnist_generator.py
+-rw-r--r--   0        0        0      373 2023-07-26 14:56:51.965389 wavpool-0.1.3/wavpool/data_generators/mnist_generator.py
+-rw-r--r--   0        0        0      182 2023-07-26 14:56:51.969389 wavpool-0.1.3/wavpool/models/__init__.py
+-rw-r--r--   0        0        0     1478 2023-07-26 14:28:52.248207 wavpool-0.1.3/wavpool/models/vanillaCNN.py
+-rw-r--r--   0        0        0     1768 2023-07-26 14:28:52.248207 wavpool-0.1.3/wavpool/models/vanillaMLP.py
+-rw-r--r--   0        0        0     1630 2023-07-26 14:56:51.969389 wavpool-0.1.3/wavpool/models/wavMLP.py
+-rw-r--r--   0        0        0     2122 2023-07-26 14:56:51.969389 wavpool-0.1.3/wavpool/models/wavelet_layer.py
+-rw-r--r--   0        0        0     2867 2023-07-26 14:56:51.969389 wavpool-0.1.3/wavpool/models/wavpool.py
+-rw-r--r--   0        0        0     6850 2023-07-26 14:56:51.969389 wavpool-0.1.3/wavpool/training/finetune_network.py
+-rw-r--r--   0        0        0     6092 2023-07-26 14:56:51.969389 wavpool-0.1.3/wavpool/training/plot_results.py
+-rw-r--r--   0        0        0     5044 2023-07-26 14:56:31.209349 wavpool-0.1.3/wavpool/training/train_model.py
+-rw-r--r--   0        0        0     1602 2023-07-26 14:28:52.248207 wavpool-0.1.3/wavpool/training/training_metrics.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:28:52.248207 wavpool-0.1.3/wavpool/utils/__init__.py
+-rw-r--r--   0        0        0     1480 2023-07-26 14:28:52.248207 wavpool-0.1.3/wavpool/utils/levels.py
+-rw-r--r--   0        0        0      367 2023-07-26 14:28:52.248207 wavpool-0.1.3/wavpool/utils/voting.py
+-rw-r--r--   0        0        0     5210 1970-01-01 00:00:00.000000 wavpool-0.1.3/setup.py
+-rw-r--r--   0        0        0     5055 1970-01-01 00:00:00.000000 wavpool-0.1.3/PKG-INFO
```

### Comparing `wavpool-0.1.2/LICENSE.txt` & `wavpool-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.2/README.md` & `wavpool-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.2/pyproject.toml` & `wavpool-0.1.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 [tool.poetry]
 name = "WavPool"
-version = "0.1.2"
+version = "0.1.3"
 description = "A network block with built in spacial and scale decomposition."
 authors = ["M. Voetberg <maggiev@fnal.gov>"]
 readme = "README.md"
 license = "mit"
 homepage = "https://github.com/deepskies/DeepWavNN"
 repository = "https://github.com/deepskies/DeepWavNN"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 torch = "^2.0.1"
 numpy = "^1.24.2"
 PyWavelets = "^1.4.1"
 pandas = "^1.5.3"
-jupyter = "^1.0.0"
 kymatio = "^0.3.0"
 bayesian-optimization = "^1.4.2"
 torcheval = "^0.0.6"
 torchvision = "^0.15.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 pre-commit = "^3.0.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
-include = ["WavPool"]
```

### Comparing `wavpool-0.1.2/wavpool/data_generators/cifar_generator.py` & `wavpool-0.1.3/wavpool/data_generators/cifar_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from WavPool.data_generators.data_generator import DataGenerator
+from wavpool.data_generators.data_generator import DataGenerator
 from torchvision import transforms
 from torchvision.datasets import CIFAR10
 
 
 class CIFARGenerator(DataGenerator):
     def __init__(self):
         grayscale_transforms = transforms.Compose(
```

### Comparing `wavpool-0.1.2/wavpool/data_generators/data_generator.py` & `wavpool-0.1.3/wavpool/data_generators/data_generator.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.2/wavpool/models/vanillaCNN.py` & `wavpool-0.1.3/wavpool/models/vanillaCNN.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.2/wavpool/models/vanillaMLP.py` & `wavpool-0.1.3/wavpool/models/vanillaMLP.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.2/wavpool/models/wavMLP.py` & `wavpool-0.1.3/wavpool/models/wavMLP.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 import torch.nn as nn
 
-from WavPool.utils.levels import Levels
-from WavPool.models.wavelet_layer import MicroWav
+from wavpool.utils.levels import Levels
+from wavpool.models.wavelet_layer import MicroWav
 
 
 class WavMLP(nn.Module):
     def __init__(
         self,
         in_channels: int,
         hidden_size: int,
```

### Comparing `wavpool-0.1.2/wavpool/models/wavelet_layer.py` & `wavpool-0.1.3/wavpool/models/wavelet_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Union
 import numpy as np
 import torch
 import pywt
 from kymatio.torch import Scattering2D
-from WavPool.utils.levels import Levels
+from wavpool.utils.levels import Levels
 
 
 class WaveletLayer:
     def __init__(
         self, level: int, input_size: Union[int, None] = None, backend: str = "pywt"
     ) -> None:
```

### Comparing `wavpool-0.1.2/wavpool/models/wavpool.py` & `wavpool-0.1.3/wavpool/models/wavpool.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 > need to make a good diagram for this.
 """
 
 import torch
 import math
 import numpy as np
 
-from WavPool.utils.levels import Levels
-from WavPool.models.wavelet_layer import MicroWav
+from wavpool.utils.levels import Levels
+from wavpool.models.wavelet_layer import MicroWav
 
 
 class WavPool(torch.nn.Module):
     def __init__(
         self,
         in_channels: int,
         hidden_size: int,
```

### Comparing `wavpool-0.1.2/wavpool/training/finetune_network.py` & `wavpool-0.1.3/wavpool/training/finetune_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from typing import Union
 from bayes_opt import BayesianOptimization
 import os
 import numpy as np
 import math
 import pandas as pd
 
-from WavPool.training.train_model import TrainingLoop
-import WavPool
+from wavpool.training.train_model import TrainingLoop
+import wavpool
 
 
 class Optimize:
     def __init__(
         self,
         model,
         parameter_space,
```

### Comparing `wavpool-0.1.2/wavpool/training/plot_results.py` & `wavpool-0.1.3/wavpool/training/plot_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import matplotlib.pyplot as plt
 import pandas as pd
 import numpy as np
 
-from WavPool.training.training_metrics import TrainingMetrics
+from wavpool.training.training_metrics import TrainingMetrics
 
 
 def plot_test_results(predictions, labels, save_path=None):
     roc_curve = TrainingMetrics.auc_curve(predictions, labels)
     confusion = TrainingMetrics.confusion_matrix(predictions, labels)
 
     plt.plot(roc_curve[0], roc_curve[1])
```

### Comparing `wavpool-0.1.2/wavpool/training/train_model.py` & `wavpool-0.1.3/wavpool/training/train_model.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.2/wavpool/training/training_metrics.py` & `wavpool-0.1.3/wavpool/training/training_metrics.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.2/wavpool/utils/levels.py` & `wavpool-0.1.3/wavpool/utils/levels.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.2/setup.py` & `wavpool-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,24 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyWavelets>=1.4.1,<2.0.0',
  'bayesian-optimization>=1.4.2,<2.0.0',
- 'jupyter>=1.0.0,<2.0.0',
  'kymatio>=0.3.0,<0.4.0',
  'numpy>=1.24.2,<2.0.0',
  'pandas>=1.5.3,<2.0.0',
  'torch>=2.0.1,<3.0.0',
  'torcheval>=0.0.6,<0.0.7',
  'torchvision>=0.15.2,<0.16.0']
 
 setup_kwargs = {
     'name': 'wavpool',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'A network block with built in spacial and scale decomposition.',
     'long_description': "\n\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![PyPI version](https://img.shields.io/pypi/v/wavpool)](https://pypi.org/project/wavpool/)\n[![arXiv](https://img.shields.io/badge/arXiv-2306.08734-b31b1b.svg)](https://arxiv.org/abs/2306.08734)\n\n# WavPool\n\nA network block with built in spacial and scale decomposition.\n\n\n>    Modern deep neural networks comprise many operational layers, such as dense or convolutional layers, which are often collected into blocks. In this work, we introduce a new, wavelet-transform-based network architecture that we call the multi-resolution perceptron: by adding a pooling layer, we create a new network block, the WavPool. The first step of the multi-resolution perceptron is transforming the data into its multi-resolution decomposition form by convolving the input data with filters of fixed coefficients but increasing size. Following image processing techniques, we are able to make scale and spatial information simultaneously accessible to the network without increasing the size of the data vector. WavPool outperforms a similar multilayer perceptron while using fewer parameters, and outperforms a comparable convolutional neural network by over 10% on accuracy on CIFAR-10.\n\n\nThis codebase contains the experimental work supporting the paper. It is to be used additional material for replication.\n\n## Installation\n\nOur project can be installed with pip [from pypi](https://pypi.org/project/wavpool/) using:\n\n```\npip install wavpool\n```\n\nThis project is build with python `poetry`. And is our perfered method to install from source.\n\nCommands are as follows:\n\n```\npip install poetry\npoetry shell\npoetry init\npoetry install\n```\n\nTo install all the dependencies required for this project.\n\n\nWe also supply distribution files (found in \\dist), or you may use the provided pyproject.toml to install with your method of choice.\n\n## Contents\n\n### Data Generators\nThe pytorch data generator objects for the experiments done in this paper.\nWrapped to work with the training framework, but functionally unmodified.\nWe include CIFAR-10 (`cifar_generator.py`), Fashion MNIST (`fashion_mnist_generator.py`), and MNIST (`mnist_generator.py`).\n\n### Training\nTraining loops used in the experiments.\n\n`finetune_networks.py` generates a set of parameters optimial for a network/task combination.\n\n`train_model.py` Executes the training loop for a network/task/parameter combination.\n\n### Models\n\n`wavpool.py` Our implimentation of the novel WavPool block\n\n`vanillaCNN.py` Standard two layer CNN containing 2D Convolutions, batch norms, and a dense output\n\n`vanillaMLP.py` Standard two hidden layer MLP\n\n`wavelet_layer.py` The `MicroWav` MLR analysis layer\n\n`wavMLP.py` Single `MicroWav` layer network with an additional dense layer and output. Not included in the paper.\n\n\n### Notebooks\n\nVisualizations of experiments with plotting code for plots included in the paper, and code to produce weights.\n\n### `run_experiments.py`\n\nTakes a configuration and trains an model.\nCurrent execution shows the optimization and subsquentical training and testing for a WavPool over CIFAR-10, Fashion MNIST and MNIST.\n\n### Acknowledgement\n\nWe acknowledge the Deep Skies Lab as a community of multi-domain experts and collaborators who've facilitated an environment of open discussion, idea-generation, and collaboration. This community was important for the development of this project.\nWe thank Aleksandra Ciprijanovic, Andrew Hearin, and Shubhendu Trivedi for comments on the manuscript.\nThis manuscript has been authored by Fermi Research Alliance, LLC under Contract No.~DE-AC02-07CH11359 with the U.S.~Department of Energy, Office of Science, Office of High Energy Physics.\n\n\n`FERMILAB-CONF-23-278-CSAID`\n\n### Citation\nIf you use our work or our code, we request you cite the arxiv paper! \n\n```\n@misc{mcdermott2023wavpool,\n      title={WavPool: A New Block for Deep Neural Networks}, \n      author={Samuel D. McDermott and M. Voetberg and Brian Nord},\n      year={2023},\n      eprint={2306.08734},\n      archivePrefix={arXiv},\n      primaryClass={cs.LG}\n}\n```\n",
     'author': 'M. Voetberg',
     'author_email': 'maggiev@fnal.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/deepskies/DeepWavNN',
```

### Comparing `wavpool-0.1.2/PKG-INFO` & `wavpool-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: wavpool
-Version: 0.1.2
+Version: 0.1.3
 Summary: A network block with built in spacial and scale decomposition.
 Home-page: https://github.com/deepskies/DeepWavNN
 License: MIT
 Author: M. Voetberg
 Author-email: maggiev@fnal.gov
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyWavelets (>=1.4.1,<2.0.0)
 Requires-Dist: bayesian-optimization (>=1.4.2,<2.0.0)
-Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: kymatio (>=0.3.0,<0.4.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: torcheval (>=0.0.6,<0.0.7)
 Requires-Dist: torchvision (>=0.15.2,<0.16.0)
 Project-URL: Repository, https://github.com/deepskies/DeepWavNN
```

