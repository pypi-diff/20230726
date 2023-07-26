# Comparing `tmp/wavpool-0.1.1.tar.gz` & `tmp/wavpool-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wavpool-0.1.1.tar", max compression
+gzip compressed data, was "wavpool-0.1.2.tar", max compression
```

## Comparing `wavpool-0.1.1.tar` & `wavpool-0.1.2.tar`

### file list

```diff
@@ -1,51 +1,24 @@
--rw-r--r--   0        0        0     1067 2023-06-14 20:16:22.496915 wavpool-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     3803 2023-06-14 20:54:30.856171 wavpool-0.1.1/README.md
--rw-r--r--   0        0        0      740 2023-06-14 20:21:20.493657 wavpool-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-06-14 20:00:23.369261 wavpool-0.1.1/wavpool/.DS_Store
--rw-r--r--   0        0        0       37 2023-02-20 18:58:16.615880 wavpool-0.1.1/wavpool/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-02-20 18:58:16.615946 wavpool-0.1.1/wavpool/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2023-02-20 18:58:16.615778 wavpool-0.1.1/wavpool/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2023-02-20 19:11:14.275406 wavpool-0.1.1/wavpool/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-02-20 19:11:14.275582 wavpool-0.1.1/wavpool/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2023-03-02 20:20:15.450100 wavpool-0.1.1/wavpool/__init__.py
--rw-r--r--   0        0        0      216 2023-05-16 17:57:31.144622 wavpool-0.1.1/wavpool/data_generators/__init__.py
--rw-r--r--   0        0        0      409 2023-05-16 18:52:26.862156 wavpool-0.1.1/wavpool/data_generators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      906 2023-05-16 18:52:26.863176 wavpool-0.1.1/wavpool/data_generators/__pycache__/cifar_generator.cpython-310.pyc
--rw-r--r--   0        0        0     1699 2023-03-10 15:41:25.041784 wavpool-0.1.1/wavpool/data_generators/__pycache__/data_generator.cpython-310.pyc
--rw-r--r--   0        0        0      837 2023-05-16 18:52:27.027442 wavpool-0.1.1/wavpool/data_generators/__pycache__/fashion_mnist_generator.cpython-310.pyc
--rw-r--r--   0        0        0      795 2023-05-16 18:52:27.026890 wavpool-0.1.1/wavpool/data_generators/__pycache__/mnist_generator.cpython-310.pyc
--rw-r--r--   0        0        0      560 2023-05-16 17:57:31.144612 wavpool-0.1.1/wavpool/data_generators/cifar_generator.py
--rw-r--r--   0        0        0     2296 2023-03-10 15:17:25.706092 wavpool-0.1.1/wavpool/data_generators/data_generator.py
--rw-r--r--   0        0        0      438 2023-05-16 17:57:31.144634 wavpool-0.1.1/wavpool/data_generators/fashion_mnist_generator.py
--rw-r--r--   0        0        0      373 2023-05-16 17:57:31.144661 wavpool-0.1.1/wavpool/data_generators/mnist_generator.py
--rw-r--r--   0        0        0      182 2023-05-16 17:57:31.144651 wavpool-0.1.1/wavpool/models/__init__.py
--rw-r--r--   0        0        0      377 2023-05-16 18:52:26.842425 wavpool-0.1.1/wavpool/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2497 2023-03-24 14:17:48.365408 wavpool-0.1.1/wavpool/models/__pycache__/pooling_wav.cpython-310.pyc
--rw-r--r--   0        0        0     1435 2023-05-16 12:49:06.927343 wavpool-0.1.1/wavpool/models/__pycache__/vanillaCNN.cpython-310.pyc
--rw-r--r--   0        0        0     1990 2023-05-12 17:25:03.646772 wavpool-0.1.1/wavpool/models/__pycache__/vanillaMLP.cpython-310.pyc
--rw-r--r--   0        0        0     2413 2023-03-15 19:26:39.562765 wavpool-0.1.1/wavpool/models/__pycache__/voting_wavMLP.cpython-310.pyc
--rw-r--r--   0        0        0     2195 2023-03-16 13:39:06.604160 wavpool-0.1.1/wavpool/models/__pycache__/wavCNN.cpython-310.pyc
--rw-r--r--   0        0        0     1653 2023-05-16 18:52:26.843264 wavpool-0.1.1/wavpool/models/__pycache__/wavMLP.cpython-310.pyc
--rw-r--r--   0        0        0     2544 2023-05-16 18:52:26.857368 wavpool-0.1.1/wavpool/models/__pycache__/wavelet_layer.cpython-310.pyc
--rw-r--r--   0        0        0     3010 2023-05-16 18:52:26.861371 wavpool-0.1.1/wavpool/models/__pycache__/wavpool.cpython-310.pyc
--rw-r--r--   0        0        0     1478 2023-05-16 12:42:46.313669 wavpool-0.1.1/wavpool/models/vanillaCNN.py
--rw-r--r--   0        0        0     1768 2023-04-20 12:52:16.897105 wavpool-0.1.1/wavpool/models/vanillaMLP.py
--rw-r--r--   0        0        0     1630 2023-05-16 17:57:02.092990 wavpool-0.1.1/wavpool/models/wavMLP.py
--rw-r--r--   0        0        0     2122 2023-05-16 17:56:47.961851 wavpool-0.1.1/wavpool/models/wavelet_layer.py
--rw-r--r--   0        0        0     2867 2023-05-16 17:57:11.816319 wavpool-0.1.1/wavpool/models/wavpool.py
--rw-r--r--   0        0        0     5130 2023-05-12 17:25:05.871802 wavpool-0.1.1/wavpool/training/__pycache__/finetune_network.cpython-310.pyc
--rw-r--r--   0        0        0     4669 2023-05-17 17:19:32.067201 wavpool-0.1.1/wavpool/training/__pycache__/plot_results.cpython-310.pyc
--rw-r--r--   0        0        0     4308 2023-05-16 18:52:25.742806 wavpool-0.1.1/wavpool/training/__pycache__/train_model.cpython-310.pyc
--rw-r--r--   0        0        0     2115 2023-03-30 19:26:31.435099 wavpool-0.1.1/wavpool/training/__pycache__/training_metrics.cpython-310.pyc
--rw-r--r--   0        0        0     6850 2023-05-16 17:57:13.547418 wavpool-0.1.1/wavpool/training/finetune_network.py
--rw-r--r--   0        0        0     6092 2023-05-16 17:57:14.882187 wavpool-0.1.1/wavpool/training/plot_results.py
--rw-r--r--   0        0        0     5044 2023-05-16 17:57:31.144703 wavpool-0.1.1/wavpool/training/train_model.py
--rw-r--r--   0        0        0     1602 2023-03-30 19:15:46.046853 wavpool-0.1.1/wavpool/training/training_metrics.py
--rw-r--r--   0        0        0        0 2023-03-02 20:20:58.389105 wavpool-0.1.1/wavpool/utils/__init__.py
--rw-r--r--   0        0        0      148 2023-03-27 15:04:06.987733 wavpool-0.1.1/wavpool/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1751 2023-05-12 17:25:03.006087 wavpool-0.1.1/wavpool/utils/__pycache__/levels.cpython-310.pyc
--rw-r--r--   0        0        0      548 2023-03-27 15:04:06.987787 wavpool-0.1.1/wavpool/utils/__pycache__/voting.cpython-310.pyc
--rw-r--r--   0        0        0     1480 2023-05-04 14:32:31.422998 wavpool-0.1.1/wavpool/utils/levels.py
--rw-r--r--   0        0        0      367 2023-03-23 18:08:00.118508 wavpool-0.1.1/wavpool/utils/voting.py
--rw-r--r--   0        0        0     4946 1970-01-01 00:00:00.000000 wavpool-0.1.1/setup.py
--rw-r--r--   0        0        0     4758 1970-01-01 00:00:00.000000 wavpool-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-26 14:28:52.244207 wavpool-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     4141 2023-07-26 14:28:52.244207 wavpool-0.1.2/README.md
+-rw-r--r--   0        0        0      761 2023-07-26 14:47:05.019861 wavpool-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 14:28:52.244207 wavpool-0.1.2/wavpool/__init__.py
+-rw-r--r--   0        0        0      216 2023-07-26 14:28:52.244207 wavpool-0.1.2/wavpool/data_generators/__init__.py
+-rw-r--r--   0        0        0      560 2023-07-26 14:28:52.244207 wavpool-0.1.2/wavpool/data_generators/cifar_generator.py
+-rw-r--r--   0        0        0     2296 2023-07-26 14:28:52.244207 wavpool-0.1.2/wavpool/data_generators/data_generator.py
+-rw-r--r--   0        0        0      438 2023-07-26 14:28:52.244207 wavpool-0.1.2/wavpool/data_generators/fashion_mnist_generator.py
+-rw-r--r--   0        0        0      373 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/data_generators/mnist_generator.py
+-rw-r--r--   0        0        0      182 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/models/__init__.py
+-rw-r--r--   0        0        0     1478 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/models/vanillaCNN.py
+-rw-r--r--   0        0        0     1768 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/models/vanillaMLP.py
+-rw-r--r--   0        0        0     1630 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/models/wavMLP.py
+-rw-r--r--   0        0        0     2122 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/models/wavelet_layer.py
+-rw-r--r--   0        0        0     2867 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/models/wavpool.py
+-rw-r--r--   0        0        0     6850 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/training/finetune_network.py
+-rw-r--r--   0        0        0     6092 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/training/plot_results.py
+-rw-r--r--   0        0        0     5044 2023-07-26 14:56:31.209349 wavpool-0.1.2/wavpool/training/train_model.py
+-rw-r--r--   0        0        0     1602 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/training/training_metrics.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/utils/__init__.py
+-rw-r--r--   0        0        0     1480 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/utils/levels.py
+-rw-r--r--   0        0        0      367 2023-07-26 14:28:52.248207 wavpool-0.1.2/wavpool/utils/voting.py
+-rw-r--r--   0        0        0     5236 1970-01-01 00:00:00.000000 wavpool-0.1.2/setup.py
+-rw-r--r--   0        0        0     5095 1970-01-01 00:00:00.000000 wavpool-0.1.2/PKG-INFO
```

### Comparing `wavpool-0.1.1/LICENSE.txt` & `wavpool-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.1/README.md` & `wavpool-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://img.shields.io/pypi/v/wavpool)](https://pypi.org/project/wavpool/)
-[![arXiv](https://img.shields.io/badge/arXiv-1234.56789-b31b1b.svg)](https://arxiv.org/abs/1234.56789)
+[![arXiv](https://img.shields.io/badge/arXiv-2306.08734-b31b1b.svg)](https://arxiv.org/abs/2306.08734)
 
 # WavPool
 
 A network block with built in spacial and scale decomposition.
 
 
 >    Modern deep neural networks comprise many operational layers, such as dense or convolutional layers, which are often collected into blocks. In this work, we introduce a new, wavelet-transform-based network architecture that we call the multi-resolution perceptron: by adding a pooling layer, we create a new network block, the WavPool. The first step of the multi-resolution perceptron is transforming the data into its multi-resolution decomposition form by convolving the input data with filters of fixed coefficients but increasing size. Following image processing techniques, we are able to make scale and spatial information simultaneously accessible to the network without increasing the size of the data vector. WavPool outperforms a similar multilayer perceptron while using fewer parameters, and outperforms a comparable convolutional neural network by over 10% on accuracy on CIFAR-10.
 
 
 This codebase contains the experimental work supporting the paper. It is to be used additional material for replication.
 
 ## Installation
 
-Our project can be installed with pip [from pypi](https://pypi.org/project/wavpool/) using: 
+Our project can be installed with pip [from pypi](https://pypi.org/project/wavpool/) using:
 
 ```
 pip install wavpool
 ```
 
 This project is build with python `poetry`. And is our perfered method to install from source.
 
@@ -70,17 +70,29 @@
 Visualizations of experiments with plotting code for plots included in the paper, and code to produce weights.
 
 ### `run_experiments.py`
 
 Takes a configuration and trains an model.
 Current execution shows the optimization and subsquentical training and testing for a WavPool over CIFAR-10, Fashion MNIST and MNIST.
 
-### Acknowledgement 
+### Acknowledgement
 
 We acknowledge the Deep Skies Lab as a community of multi-domain experts and collaborators who've facilitated an environment of open discussion, idea-generation, and collaboration. This community was important for the development of this project.
 We thank Aleksandra Ciprijanovic, Andrew Hearin, and Shubhendu Trivedi for comments on the manuscript.
 This manuscript has been authored by Fermi Research Alliance, LLC under Contract No.~DE-AC02-07CH11359 with the U.S.~Department of Energy, Office of Science, Office of High Energy Physics.
 
 
 `FERMILAB-CONF-23-278-CSAID`
 
-### Citation 
+### Citation
+If you use our work or our code, we request you cite the arxiv paper! 
+
+```
+@misc{mcdermott2023wavpool,
+      title={WavPool: A New Block for Deep Neural Networks}, 
+      author={Samuel D. McDermott and M. Voetberg and Brian Nord},
+      year={2023},
+      eprint={2306.08734},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG}
+}
+```
```

### Comparing `wavpool-0.1.1/pyproject.toml` & `wavpool-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "WavPool"
-version = "0.1.1"
+version = "0.1.2"
 description = "A network block with built in spacial and scale decomposition."
 authors = ["M. Voetberg <maggiev@fnal.gov>"]
 readme = "README.md"
 license = "mit"
 homepage = "https://github.com/deepskies/DeepWavNN"
 repository = "https://github.com/deepskies/DeepWavNN"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-torch = "^1.13.1"
+torch = "^2.0.1"
 numpy = "^1.24.2"
 PyWavelets = "^1.4.1"
 pandas = "^1.5.3"
-torchvision = "^0.14.1"
 jupyter = "^1.0.0"
 kymatio = "^0.3.0"
 bayesian-optimization = "^1.4.2"
 torcheval = "^0.0.6"
+torchvision = "^0.15.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 pre-commit = "^3.0.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+include = ["WavPool"]
```

### Comparing `wavpool-0.1.1/wavpool/data_generators/cifar_generator.py` & `wavpool-0.1.2/wavpool/data_generators/cifar_generator.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.1/wavpool/data_generators/data_generator.py` & `wavpool-0.1.2/wavpool/data_generators/data_generator.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.1/wavpool/models/vanillaCNN.py` & `wavpool-0.1.2/wavpool/models/vanillaCNN.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.1/wavpool/models/vanillaMLP.py` & `wavpool-0.1.2/wavpool/models/vanillaMLP.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.1/wavpool/models/wavMLP.py` & `wavpool-0.1.2/wavpool/models/wavMLP.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.1/wavpool/models/wavelet_layer.py` & `wavpool-0.1.2/wavpool/models/wavelet_layer.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.1/wavpool/models/wavpool.py` & `wavpool-0.1.2/wavpool/models/wavpool.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.1/wavpool/training/finetune_network.py` & `wavpool-0.1.2/wavpool/training/finetune_network.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.1/wavpool/training/plot_results.py` & `wavpool-0.1.2/wavpool/training/plot_results.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.1/wavpool/training/train_model.py` & `wavpool-0.1.2/wavpool/training/train_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import pandas as pd
 import os
 import torch
 import tqdm
 
-from WavPool.training.training_metrics import TrainingMetrics
+from wavpool.training.training_metrics import TrainingMetrics
 
 
 class TrainingLoop:
     def __init__(
         self,
         model_class,
         model_params,
```

### Comparing `wavpool-0.1.1/wavpool/training/training_metrics.py` & `wavpool-0.1.2/wavpool/training/training_metrics.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.1/wavpool/utils/levels.py` & `wavpool-0.1.2/wavpool/utils/levels.py`

 * *Files identical despite different names*

### Comparing `wavpool-0.1.1/setup.py` & `wavpool-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 ['wavpool',
  'wavpool.data_generators',
  'wavpool.models',
  'wavpool.training',
  'wavpool.utils']
 
 package_data = \
-{'': ['*'], 'wavpool': ['.pytest_cache/*', '.pytest_cache/v/cache/*']}
+{'': ['*']}
 
 install_requires = \
 ['PyWavelets>=1.4.1,<2.0.0',
  'bayesian-optimization>=1.4.2,<2.0.0',
  'jupyter>=1.0.0,<2.0.0',
  'kymatio>=0.3.0,<0.4.0',
  'numpy>=1.24.2,<2.0.0',
  'pandas>=1.5.3,<2.0.0',
- 'torch>=1.13.1,<2.0.0',
+ 'torch>=2.0.1,<3.0.0',
  'torcheval>=0.0.6,<0.0.7',
- 'torchvision>=0.14.1,<0.15.0']
+ 'torchvision>=0.15.2,<0.16.0']
 
 setup_kwargs = {
     'name': 'wavpool',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A network block with built in spacial and scale decomposition.',
-    'long_description': "\n\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![PyPI version](https://img.shields.io/pypi/v/wavpool)](https://pypi.org/project/wavpool/)\n[![arXiv](https://img.shields.io/badge/arXiv-1234.56789-b31b1b.svg)](https://arxiv.org/abs/1234.56789)\n\n# WavPool\n\nA network block with built in spacial and scale decomposition.\n\n\n>    Modern deep neural networks comprise many operational layers, such as dense or convolutional layers, which are often collected into blocks. In this work, we introduce a new, wavelet-transform-based network architecture that we call the multi-resolution perceptron: by adding a pooling layer, we create a new network block, the WavPool. The first step of the multi-resolution perceptron is transforming the data into its multi-resolution decomposition form by convolving the input data with filters of fixed coefficients but increasing size. Following image processing techniques, we are able to make scale and spatial information simultaneously accessible to the network without increasing the size of the data vector. WavPool outperforms a similar multilayer perceptron while using fewer parameters, and outperforms a comparable convolutional neural network by over 10% on accuracy on CIFAR-10.\n\n\nThis codebase contains the experimental work supporting the paper. It is to be used additional material for replication.\n\n## Installation\n\nOur project can be installed with pip [from pypi](https://pypi.org/project/wavpool/) using: \n\n```\npip install wavpool\n```\n\nThis project is build with python `poetry`. And is our perfered method to install from source.\n\nCommands are as follows:\n\n```\npip install poetry\npoetry shell\npoetry init\npoetry install\n```\n\nTo install all the dependencies required for this project.\n\n\nWe also supply distribution files (found in \\dist), or you may use the provided pyproject.toml to install with your method of choice.\n\n## Contents\n\n### Data Generators\nThe pytorch data generator objects for the experiments done in this paper.\nWrapped to work with the training framework, but functionally unmodified.\nWe include CIFAR-10 (`cifar_generator.py`), Fashion MNIST (`fashion_mnist_generator.py`), and MNIST (`mnist_generator.py`).\n\n### Training\nTraining loops used in the experiments.\n\n`finetune_networks.py` generates a set of parameters optimial for a network/task combination.\n\n`train_model.py` Executes the training loop for a network/task/parameter combination.\n\n### Models\n\n`wavpool.py` Our implimentation of the novel WavPool block\n\n`vanillaCNN.py` Standard two layer CNN containing 2D Convolutions, batch norms, and a dense output\n\n`vanillaMLP.py` Standard two hidden layer MLP\n\n`wavelet_layer.py` The `MicroWav` MLR analysis layer\n\n`wavMLP.py` Single `MicroWav` layer network with an additional dense layer and output. Not included in the paper.\n\n\n### Notebooks\n\nVisualizations of experiments with plotting code for plots included in the paper, and code to produce weights.\n\n### `run_experiments.py`\n\nTakes a configuration and trains an model.\nCurrent execution shows the optimization and subsquentical training and testing for a WavPool over CIFAR-10, Fashion MNIST and MNIST.\n\n### Acknowledgement \n\nWe acknowledge the Deep Skies Lab as a community of multi-domain experts and collaborators who've facilitated an environment of open discussion, idea-generation, and collaboration. This community was important for the development of this project.\nWe thank Aleksandra Ciprijanovic, Andrew Hearin, and Shubhendu Trivedi for comments on the manuscript.\nThis manuscript has been authored by Fermi Research Alliance, LLC under Contract No.~DE-AC02-07CH11359 with the U.S.~Department of Energy, Office of Science, Office of High Energy Physics.\n\n\n`FERMILAB-CONF-23-278-CSAID`\n\n### Citation \n",
+    'long_description': "\n\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![PyPI version](https://img.shields.io/pypi/v/wavpool)](https://pypi.org/project/wavpool/)\n[![arXiv](https://img.shields.io/badge/arXiv-2306.08734-b31b1b.svg)](https://arxiv.org/abs/2306.08734)\n\n# WavPool\n\nA network block with built in spacial and scale decomposition.\n\n\n>    Modern deep neural networks comprise many operational layers, such as dense or convolutional layers, which are often collected into blocks. In this work, we introduce a new, wavelet-transform-based network architecture that we call the multi-resolution perceptron: by adding a pooling layer, we create a new network block, the WavPool. The first step of the multi-resolution perceptron is transforming the data into its multi-resolution decomposition form by convolving the input data with filters of fixed coefficients but increasing size. Following image processing techniques, we are able to make scale and spatial information simultaneously accessible to the network without increasing the size of the data vector. WavPool outperforms a similar multilayer perceptron while using fewer parameters, and outperforms a comparable convolutional neural network by over 10% on accuracy on CIFAR-10.\n\n\nThis codebase contains the experimental work supporting the paper. It is to be used additional material for replication.\n\n## Installation\n\nOur project can be installed with pip [from pypi](https://pypi.org/project/wavpool/) using:\n\n```\npip install wavpool\n```\n\nThis project is build with python `poetry`. And is our perfered method to install from source.\n\nCommands are as follows:\n\n```\npip install poetry\npoetry shell\npoetry init\npoetry install\n```\n\nTo install all the dependencies required for this project.\n\n\nWe also supply distribution files (found in \\dist), or you may use the provided pyproject.toml to install with your method of choice.\n\n## Contents\n\n### Data Generators\nThe pytorch data generator objects for the experiments done in this paper.\nWrapped to work with the training framework, but functionally unmodified.\nWe include CIFAR-10 (`cifar_generator.py`), Fashion MNIST (`fashion_mnist_generator.py`), and MNIST (`mnist_generator.py`).\n\n### Training\nTraining loops used in the experiments.\n\n`finetune_networks.py` generates a set of parameters optimial for a network/task combination.\n\n`train_model.py` Executes the training loop for a network/task/parameter combination.\n\n### Models\n\n`wavpool.py` Our implimentation of the novel WavPool block\n\n`vanillaCNN.py` Standard two layer CNN containing 2D Convolutions, batch norms, and a dense output\n\n`vanillaMLP.py` Standard two hidden layer MLP\n\n`wavelet_layer.py` The `MicroWav` MLR analysis layer\n\n`wavMLP.py` Single `MicroWav` layer network with an additional dense layer and output. Not included in the paper.\n\n\n### Notebooks\n\nVisualizations of experiments with plotting code for plots included in the paper, and code to produce weights.\n\n### `run_experiments.py`\n\nTakes a configuration and trains an model.\nCurrent execution shows the optimization and subsquentical training and testing for a WavPool over CIFAR-10, Fashion MNIST and MNIST.\n\n### Acknowledgement\n\nWe acknowledge the Deep Skies Lab as a community of multi-domain experts and collaborators who've facilitated an environment of open discussion, idea-generation, and collaboration. This community was important for the development of this project.\nWe thank Aleksandra Ciprijanovic, Andrew Hearin, and Shubhendu Trivedi for comments on the manuscript.\nThis manuscript has been authored by Fermi Research Alliance, LLC under Contract No.~DE-AC02-07CH11359 with the U.S.~Department of Energy, Office of Science, Office of High Energy Physics.\n\n\n`FERMILAB-CONF-23-278-CSAID`\n\n### Citation\nIf you use our work or our code, we request you cite the arxiv paper! \n\n```\n@misc{mcdermott2023wavpool,\n      title={WavPool: A New Block for Deep Neural Networks}, \n      author={Samuel D. McDermott and M. Voetberg and Brian Nord},\n      year={2023},\n      eprint={2306.08734},\n      archivePrefix={arXiv},\n      primaryClass={cs.LG}\n}\n```\n",
     'author': 'M. Voetberg',
     'author_email': 'maggiev@fnal.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/deepskies/DeepWavNN',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `wavpool-0.1.1/PKG-INFO` & `wavpool-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wavpool
-Version: 0.1.1
+Version: 0.1.2
 Summary: A network block with built in spacial and scale decomposition.
 Home-page: https://github.com/deepskies/DeepWavNN
 License: MIT
 Author: M. Voetberg
 Author-email: maggiev@fnal.gov
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,39 +13,39 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyWavelets (>=1.4.1,<2.0.0)
 Requires-Dist: bayesian-optimization (>=1.4.2,<2.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: kymatio (>=0.3.0,<0.4.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: torch (>=1.13.1,<2.0.0)
+Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: torcheval (>=0.0.6,<0.0.7)
-Requires-Dist: torchvision (>=0.14.1,<0.15.0)
+Requires-Dist: torchvision (>=0.15.2,<0.16.0)
 Project-URL: Repository, https://github.com/deepskies/DeepWavNN
 Description-Content-Type: text/markdown
 
 
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://img.shields.io/pypi/v/wavpool)](https://pypi.org/project/wavpool/)
-[![arXiv](https://img.shields.io/badge/arXiv-1234.56789-b31b1b.svg)](https://arxiv.org/abs/1234.56789)
+[![arXiv](https://img.shields.io/badge/arXiv-2306.08734-b31b1b.svg)](https://arxiv.org/abs/2306.08734)
 
 # WavPool
 
 A network block with built in spacial and scale decomposition.
 
 
 >    Modern deep neural networks comprise many operational layers, such as dense or convolutional layers, which are often collected into blocks. In this work, we introduce a new, wavelet-transform-based network architecture that we call the multi-resolution perceptron: by adding a pooling layer, we create a new network block, the WavPool. The first step of the multi-resolution perceptron is transforming the data into its multi-resolution decomposition form by convolving the input data with filters of fixed coefficients but increasing size. Following image processing techniques, we are able to make scale and spatial information simultaneously accessible to the network without increasing the size of the data vector. WavPool outperforms a similar multilayer perceptron while using fewer parameters, and outperforms a comparable convolutional neural network by over 10% on accuracy on CIFAR-10.
 
 
 This codebase contains the experimental work supporting the paper. It is to be used additional material for replication.
 
 ## Installation
 
-Our project can be installed with pip [from pypi](https://pypi.org/project/wavpool/) using: 
+Our project can be installed with pip [from pypi](https://pypi.org/project/wavpool/) using:
 
 ```
 pip install wavpool
 ```
 
 This project is build with python `poetry`. And is our perfered method to install from source.
 
@@ -95,18 +95,30 @@
 Visualizations of experiments with plotting code for plots included in the paper, and code to produce weights.
 
 ### `run_experiments.py`
 
 Takes a configuration and trains an model.
 Current execution shows the optimization and subsquentical training and testing for a WavPool over CIFAR-10, Fashion MNIST and MNIST.
 
-### Acknowledgement 
+### Acknowledgement
 
 We acknowledge the Deep Skies Lab as a community of multi-domain experts and collaborators who've facilitated an environment of open discussion, idea-generation, and collaboration. This community was important for the development of this project.
 We thank Aleksandra Ciprijanovic, Andrew Hearin, and Shubhendu Trivedi for comments on the manuscript.
 This manuscript has been authored by Fermi Research Alliance, LLC under Contract No.~DE-AC02-07CH11359 with the U.S.~Department of Energy, Office of Science, Office of High Energy Physics.
 
 
 `FERMILAB-CONF-23-278-CSAID`
 
-### Citation 
+### Citation
+If you use our work or our code, we request you cite the arxiv paper! 
+
+```
+@misc{mcdermott2023wavpool,
+      title={WavPool: A New Block for Deep Neural Networks}, 
+      author={Samuel D. McDermott and M. Voetberg and Brian Nord},
+      year={2023},
+      eprint={2306.08734},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG}
+}
+```
```

