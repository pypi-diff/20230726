# Comparing `tmp/pytorch_ood-0.1.4-py3-none-any.whl.zip` & `tmp/pytorch_ood-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,53 +1,60 @@
-Zip file size: 110404 bytes, number of entries: 76
--rw-r--r--  2.0 unx      209 b- defN 23-Jul-19 08:13 pytorch_ood/__init__.py
+Zip file size: 121160 bytes, number of entries: 83
+-rw-r--r--  2.0 unx      209 b- defN 23-Jul-26 15:46 pytorch_ood/__init__.py
 -rw-r--r--  2.0 unx     2341 b- defN 23-Jul-18 10:04 pytorch_ood/api.py
 -rw-r--r--  2.0 unx     1404 b- defN 23-Jul-19 08:12 pytorch_ood/benchmark/__init__.py
 -rw-r--r--  2.0 unx      876 b- defN 23-Jul-18 10:04 pytorch_ood/benchmark/base.py
 -rw-r--r--  2.0 unx      144 b- defN 23-Jul-19 08:12 pytorch_ood/benchmark/img/__init__.py
 -rw-r--r--  2.0 unx     7122 b- defN 23-Jul-19 08:12 pytorch_ood/benchmark/img/cifar10.py
 -rw-r--r--  2.0 unx     7157 b- defN 23-Jul-19 08:12 pytorch_ood/benchmark/img/cifar100.py
 -rw-r--r--  2.0 unx     3922 b- defN 23-Jul-19 08:12 pytorch_ood/benchmark/img/imagenet.py
 -rw-r--r--  2.0 unx       11 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/__init__.py
 -rw-r--r--  2.0 unx      165 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/audio/__init__.py
 -rw-r--r--  2.0 unx     3059 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/audio/fsdd.py
--rw-r--r--  2.0 unx     3487 b- defN 23-Jul-19 08:12 pytorch_ood/dataset/img/__init__.py
+-rw-r--r--  2.0 unx     3491 b- defN 23-Jul-26 15:40 pytorch_ood/dataset/img/__init__.py
 -rw-r--r--  2.0 unx     2457 b- defN 23-Jul-19 08:12 pytorch_ood/dataset/img/base.py
 -rw-r--r--  2.0 unx     4329 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/img/chars74k.py
 -rw-r--r--  2.0 unx     3076 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/img/cifar.py
 -rw-r--r--  2.0 unx     1331 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/img/fooling.py
 -rw-r--r--  2.0 unx     5793 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/img/imagenet.py
 -rw-r--r--  2.0 unx     4270 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/img/mnistc.py
 -rw-r--r--  2.0 unx     5382 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/img/mvtech.py
 -rw-r--r--  2.0 unx     3936 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/img/noise.py
 -rw-r--r--  2.0 unx     4891 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/img/odin.py
 -rw-r--r--  2.0 unx     4836 b- defN 23-Jul-19 08:12 pytorch_ood/dataset/img/openood.py
 -rw-r--r--  2.0 unx     8477 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/img/pixmix.py
 -rw-r--r--  2.0 unx     4242 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/img/streethazards.py
 -rw-r--r--  2.0 unx     3001 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/img/textures.py
--rw-r--r--  2.0 unx     3766 b- defN 23-Jul-19 08:12 pytorch_ood/dataset/img/tinyimagenet.py
+-rw-r--r--  2.0 unx     3780 b- defN 23-Jul-20 09:45 pytorch_ood/dataset/img/tinyimagenet.py
 -rw-r--r--  2.0 unx     4692 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/img/tinyimages.py
 -rw-r--r--  2.0 unx      507 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/ossim/__init__.py
--rw-r--r--  2.0 unx     8194 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/ossim/ossim.py
+-rw-r--r--  2.0 unx     8194 b- defN 23-Jul-20 16:02 pytorch_ood/dataset/ossim/ossim.py
 -rw-r--r--  2.0 unx     1049 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/txt/__init__.py
--rw-r--r--  2.0 unx     2665 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/txt/multi30k.py
+-rw-r--r--  2.0 unx     2665 b- defN 23-Jul-26 15:40 pytorch_ood/dataset/txt/multi30k.py
 -rw-r--r--  2.0 unx     4002 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/txt/newsgroups.py
 -rw-r--r--  2.0 unx     5954 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/txt/reuters.py
 -rw-r--r--  2.0 unx     1983 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/txt/stop_words.py
 -rw-r--r--  2.0 unx     3331 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/txt/wiki.py
 -rw-r--r--  2.0 unx     2034 b- defN 23-Jul-18 10:04 pytorch_ood/dataset/txt/wmt16.py
--rw-r--r--  2.0 unx     2395 b- defN 23-Jul-18 10:04 pytorch_ood/detector/__init__.py
+-rw-r--r--  2.0 unx     3461 b- defN 23-Jul-26 15:40 pytorch_ood/detector/__init__.py
+-rw-r--r--  2.0 unx     4693 b- defN 23-Jul-26 15:40 pytorch_ood/detector/ash.py
+-rw-r--r--  2.0 unx     3050 b- defN 23-Jul-26 15:40 pytorch_ood/detector/dice.py
 -rw-r--r--  2.0 unx     2352 b- defN 23-Jul-18 10:04 pytorch_ood/detector/energy.py
 -rw-r--r--  2.0 unx     2046 b- defN 23-Jul-18 10:04 pytorch_ood/detector/entropy.py
 -rw-r--r--  2.0 unx     4402 b- defN 23-Jul-18 10:04 pytorch_ood/detector/klmatching.py
--rw-r--r--  2.0 unx     7749 b- defN 23-Jul-18 10:04 pytorch_ood/detector/mahalanobis.py
+-rw-r--r--  2.0 unx     3201 b- defN 23-Jul-26 15:40 pytorch_ood/detector/knn.py
+-rw-r--r--  2.0 unx     7841 b- defN 23-Jul-26 15:40 pytorch_ood/detector/mahalanobis.py
 -rw-r--r--  2.0 unx     1810 b- defN 23-Jul-18 10:04 pytorch_ood/detector/maxlogit.py
 -rw-r--r--  2.0 unx     3619 b- defN 23-Jul-18 10:04 pytorch_ood/detector/mcd.py
 -rw-r--r--  2.0 unx     5816 b- defN 23-Jul-18 10:04 pytorch_ood/detector/odin.py
--rw-r--r--  2.0 unx     2316 b- defN 23-Jul-18 10:04 pytorch_ood/detector/softmax.py
+-rw-r--r--  2.0 unx     2633 b- defN 23-Jul-26 15:40 pytorch_ood/detector/react.py
+-rw-r--r--  2.0 unx     4362 b- defN 23-Jul-26 15:40 pytorch_ood/detector/rmd.py
+-rw-r--r--  2.0 unx     2812 b- defN 23-Jul-26 15:40 pytorch_ood/detector/she.py
+-rw-r--r--  2.0 unx     2621 b- defN 23-Jul-20 09:45 pytorch_ood/detector/softmax.py
+-rw-r--r--  2.0 unx     3428 b- defN 23-Jul-26 15:40 pytorch_ood/detector/tscaling.py
 -rw-r--r--  2.0 unx     5267 b- defN 23-Jul-18 10:04 pytorch_ood/detector/vim.py
 -rw-r--r--  2.0 unx      323 b- defN 23-Jul-18 10:04 pytorch_ood/detector/openmax/__init__.py
 -rw-r--r--  2.0 unx     7041 b- defN 23-Jul-18 10:04 pytorch_ood/detector/openmax/numpy.py
 -rw-r--r--  2.0 unx     3318 b- defN 23-Jul-18 10:04 pytorch_ood/detector/openmax/torch.py
 -rw-r--r--  2.0 unx     5408 b- defN 23-Jul-18 10:04 pytorch_ood/loss/__init__.py
 -rw-r--r--  2.0 unx     1589 b- defN 23-Jul-18 10:04 pytorch_ood/loss/background.py
 -rw-r--r--  2.0 unx     3877 b- defN 23-Jul-18 10:04 pytorch_ood/loss/cac.py
@@ -60,19 +67,19 @@
 -rw-r--r--  2.0 unx     4875 b- defN 23-Jul-18 10:04 pytorch_ood/loss/mchad.py
 -rw-r--r--  2.0 unx     2667 b- defN 23-Jul-18 10:04 pytorch_ood/loss/objectosphere.py
 -rw-r--r--  2.0 unx     2199 b- defN 23-Jul-18 10:04 pytorch_ood/loss/oe.py
 -rw-r--r--  2.0 unx     5289 b- defN 23-Jul-18 10:04 pytorch_ood/loss/svdd.py
 -rw-r--r--  2.0 unx      723 b- defN 23-Jul-18 10:04 pytorch_ood/model/__init__.py
 -rw-r--r--  2.0 unx     4684 b- defN 23-Jul-18 10:04 pytorch_ood/model/centers.py
 -rw-r--r--  2.0 unx     1611 b- defN 23-Jul-18 10:04 pytorch_ood/model/gru.py
--rw-r--r--  2.0 unx    12226 b- defN 23-Jul-18 10:04 pytorch_ood/model/wrn.py
+-rw-r--r--  2.0 unx    12629 b- defN 23-Jul-20 09:45 pytorch_ood/model/wrn.py
 -rw-r--r--  2.0 unx       70 b- defN 23-Jul-18 10:04 pytorch_ood/utils/__init__.py
 -rw-r--r--  2.0 unx    10960 b- defN 23-Jul-18 10:04 pytorch_ood/utils/gdown.py
 -rw-r--r--  2.0 unx     7093 b- defN 23-Jul-18 10:04 pytorch_ood/utils/metrics.py
--rw-r--r--  2.0 unx     2111 b- defN 23-Jul-18 10:04 pytorch_ood/utils/transforms.py
+-rw-r--r--  2.0 unx     1929 b- defN 23-Jul-26 15:40 pytorch_ood/utils/transforms.py
 -rw-r--r--  2.0 unx     8878 b- defN 23-Jul-18 10:04 pytorch_ood/utils/utils.py
--rw-r--r--  2.0 unx    11351 b- defN 23-Jul-19 08:24 pytorch_ood-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    23728 b- defN 23-Jul-19 08:24 pytorch_ood-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 08:24 pytorch_ood-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-19 08:24 pytorch_ood-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6666 b- defN 23-Jul-19 08:24 pytorch_ood-0.1.4.dist-info/RECORD
-76 files, 306146 bytes uncompressed, 99808 bytes compressed:  67.4%
+-rw-r--r--  2.0 unx    11351 b- defN 23-Jul-26 15:47 pytorch_ood-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    23760 b- defN 23-Jul-26 15:47 pytorch_ood-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 15:47 pytorch_ood-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-26 15:47 pytorch_ood-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     7262 b- defN 23-Jul-26 15:47 pytorch_ood-0.1.5.dist-info/RECORD
+83 files, 332655 bytes uncompressed, 109638 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -105,38 +105,59 @@
 
 Filename: pytorch_ood/dataset/txt/wmt16.py
 Comment: 
 
 Filename: pytorch_ood/detector/__init__.py
 Comment: 
 
+Filename: pytorch_ood/detector/ash.py
+Comment: 
+
+Filename: pytorch_ood/detector/dice.py
+Comment: 
+
 Filename: pytorch_ood/detector/energy.py
 Comment: 
 
 Filename: pytorch_ood/detector/entropy.py
 Comment: 
 
 Filename: pytorch_ood/detector/klmatching.py
 Comment: 
 
+Filename: pytorch_ood/detector/knn.py
+Comment: 
+
 Filename: pytorch_ood/detector/mahalanobis.py
 Comment: 
 
 Filename: pytorch_ood/detector/maxlogit.py
 Comment: 
 
 Filename: pytorch_ood/detector/mcd.py
 Comment: 
 
 Filename: pytorch_ood/detector/odin.py
 Comment: 
 
+Filename: pytorch_ood/detector/react.py
+Comment: 
+
+Filename: pytorch_ood/detector/rmd.py
+Comment: 
+
+Filename: pytorch_ood/detector/she.py
+Comment: 
+
 Filename: pytorch_ood/detector/softmax.py
 Comment: 
 
+Filename: pytorch_ood/detector/tscaling.py
+Comment: 
+
 Filename: pytorch_ood/detector/vim.py
 Comment: 
 
 Filename: pytorch_ood/detector/openmax/__init__.py
 Comment: 
 
 Filename: pytorch_ood/detector/openmax/numpy.py
@@ -207,23 +228,23 @@
 
 Filename: pytorch_ood/utils/transforms.py
 Comment: 
 
 Filename: pytorch_ood/utils/utils.py
 Comment: 
 
-Filename: pytorch_ood-0.1.4.dist-info/LICENSE
+Filename: pytorch_ood-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: pytorch_ood-0.1.4.dist-info/METADATA
+Filename: pytorch_ood-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: pytorch_ood-0.1.4.dist-info/WHEEL
+Filename: pytorch_ood-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: pytorch_ood-0.1.4.dist-info/top_level.txt
+Filename: pytorch_ood-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pytorch_ood-0.1.4.dist-info/RECORD
+Filename: pytorch_ood-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytorch_ood/__init__.py

```diff
@@ -1,8 +1,8 @@
 """
 PyTorch Out-of-Distribution Detection
 """
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 from . import api, dataset, detector, loss, model, utils
 
 __all__ = ["dataset", "detector", "loss", "model", "utils", "api", "__version__"]
```

## pytorch_ood/dataset/img/__init__.py

```diff
@@ -109,16 +109,17 @@
 
 
 Fractals
 `````````````
 ..  autoclass:: pytorch_ood.dataset.img.FractalDataset
     :members:
 
+
 Fooling Images
-`````````````
+````````````````
 ..  autoclass:: pytorch_ood.dataset.img.FoolingImages
     :members:
 
 
 Feature Visualizations
 ``````````````````````````
 ..  autoclass:: pytorch_ood.dataset.img.FeatureVisDataset
```

## pytorch_ood/dataset/img/tinyimagenet.py

```diff
@@ -69,17 +69,17 @@
                 self.paths += files
                 self.labels += [self.class_map[d]] * len(files)
 
         elif subset == "val":
             anno_file = join(self.basename, "val_annotations.txt")
             with open(anno_file, "r") as f:
                 for line in f.readlines():
-                    path, label, x, y, z, t = " ".join(line.split())
+                    path, label, x, y, z, t = " ".join(line.split()).split()
                     self.paths.append(join(self.basename, "images", path))
-                    self.labels = self.class_map[label]
+                    self.labels.append(self.class_map[label])
 
         elif subset == "test":
             d = join(self.basename, "images")
             self.paths = [join(d, img) for img in os.listdir(d)]
             self.labels = [-1] * len(self.paths)
 
     def download(self):
```

## pytorch_ood/dataset/txt/multi30k.py

```diff
@@ -20,15 +20,15 @@
     Usually used as OOD data, labels are -1 by default.
     """
 
     train_url = "https://github.com/hendrycks/outlier-exposure/raw/master/NLP_classification/multi30k/train.txt"
     test_url = "https://raw.githubusercontent.com/hendrycks/outlier-exposure/master/NLP_classification/multi30k/val.txt"
 
     test_md5 = "8d407ae05dbc61e3e61ffd3a3f9d39fb"
-    train_md5 = "4444a088dda968b44f7a6dec756698b3"
+    train_md5 = "094c68794632983239bf1bc1b37282a8"
     train_filename = "m30k-train.txt"
     test_filename = "m30k-test.txt"
 
     def __init__(self, root, transform=None, target_transform=None, train=True, download=True):
         super(Dataset, self).__init__()
         self.root = os.path.expanduser(root)
         self.transforms = transform
```

## pytorch_ood/detector/__init__.py

```diff
@@ -13,15 +13,15 @@
 
     detector = Detector(model)
     detector.fit(data_loader)
     scores = detector(x)
 
 
 Feature-based Interface
-^^^^^^^^^^^^^^^^^^^^^^^^
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Alternatively, you can also use the ``fit_features`` and ``predict_features`` methods.
 In that case, inputs will not be passed through the model. This can help to avoid passing
 data through the model multiple times when fitting several detectors. Detectors who do not
 support this will raise an exception.
 
 .. code:: python
@@ -33,59 +33,114 @@
 Some of the detectors support grid-like input, so that they can be used for anomaly segmentation
 without further adjustment.
 
 
 ..  autoclass:: pytorch_ood.api.Detector
     :members:
 
-Maximum Softmax (MSP)
+
+Probability-based
 -------------------------------
+
+Maximum Softmax (MSP)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 .. automodule:: pytorch_ood.detector.softmax
 
-Maximum Logit
+Monte Carlo Dropout (MCD)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+.. automodule:: pytorch_ood.detector.mcd
+
+Temperature Scaling
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+.. automodule:: pytorch_ood.detector.tscaling
+
+KL-Matching
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+.. automodule:: pytorch_ood.detector.klmatching
+
+Entropy
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+.. automodule:: pytorch_ood.detector.entropy
+
+
+Logit-based
 -------------------------------
+
+Maximum Logit
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 .. automodule:: pytorch_ood.detector.maxlogit
 
 OpenMax
--------------------------------
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 .. automodule:: pytorch_ood.detector.openmax
 
-ODIN Preprocessing
+Energy Based (EBO)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+.. automodule:: pytorch_ood.detector.energy
+
+
+Feature-based
 -------------------------------
+
+ODIN Preprocessing
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 .. automodule:: pytorch_ood.detector.odin
 
-Energy Based
--------------------------------
-.. automodule:: pytorch_ood.detector.energy
 
-Mahalanobis Method
--------------------------------
+Mahalanobis Distance (MD)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 .. automodule:: pytorch_ood.detector.mahalanobis
 
-Monte Carlo Dropout
--------------------------------
-.. automodule:: pytorch_ood.detector.mcd
 
-Virtual Logit Matching
--------------------------------
+Relative Mahalanobis Distance (RMD)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+.. automodule:: pytorch_ood.detector.rmd
+
+
+Virtual Logit Matching (ViM)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 .. automodule:: pytorch_ood.detector.vim
 
-KL-Matching
--------------------------------
-.. automodule:: pytorch_ood.detector.klmatching
 
-Entropy
--------------------------------
-.. automodule:: pytorch_ood.detector.entropy
+Nearest Neighbor (kNN)
+^^^^^^^^^^^^^^^^^^^^^^^^^
+.. automodule:: pytorch_ood.detector.knn
+
 
+Simplified Hopfield Energy (SHE)
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+.. automodule:: pytorch_ood.detector.she
+
+Activation Pruning
+---------------------
+
+Activation Shaping (ASH)
+^^^^^^^^^^^^^^^^^^^^^^^^^
+.. automodule:: pytorch_ood.detector.ash
+
+ReAct
+^^^^^^^^^^^^^^^^^^^^^^^^^
+.. automodule:: pytorch_ood.detector.react
+
+DICE
+^^^^^^^^^^^^^^^^^^^^^^^^^
+.. automodule:: pytorch_ood.detector.dice
 
 """
 from .energy import EnergyBased
 from .entropy import Entropy
 from .klmatching import KLMatching
 from .mahalanobis import Mahalanobis
 from .maxlogit import MaxLogit
 from .mcd import MCD
 from .odin import ODIN, odin_preprocessing
 from .openmax import OpenMax
 from .softmax import MaxSoftmax
+from .tscaling import TemperatureScaling
 from .vim import ViM
+from .knn import KNN
+from .ash import ASH
+from .react import ReAct
+from .rmd import RMD
+from .dice import DICE
+from .she import SHE
+
```

## pytorch_ood/detector/mahalanobis.py

```diff
@@ -28,26 +28,29 @@
 class Mahalanobis(Detector):
     """
     Implements the Mahalanobis Method from the paper *A Simple Unified Framework for Detecting
     Out-of-Distribution Samples and Adversarial Attacks*.
 
     This method calculates a class center :math:`\\mu_y` for each class,
     and a shared covariance matrix :math:`\\Sigma` from the data.
+    The outlier scores are then calculated as
+
+    .. math :: - \\max_k \\lbrace (f(x) - \\mu_k)^{\\top} \\Sigma^{-1} (f(x) - \\mu_k) \\rbrace
 
     Also uses ODIN preprocessing.
 
     :see Implementation: `GitHub <https://github.com/pokaxpoka/deep_Mahalanobis_detector>`__
     :see Paper: `ArXiv <https://arxiv.org/abs/1807.03888>`__
     """
 
     def __init__(
-        self,
-        model: Callable[[Tensor], Tensor],
-        eps: float = 0.002,
-        norm_std: Optional[List] = None,
+            self,
+            model: Callable[[Tensor], Tensor],
+            eps: float = 0.002,
+            norm_std: Optional[List] = None,
     ):
         """
         :param model: the Neural Network, should output features
         :param eps: magnitude for gradient based input preprocessing
         :param norm_std: Standard deviations for input normalization
         """
         super(Mahalanobis, self).__init__()
@@ -78,77 +81,76 @@
         Fit parameters of the multi variate gaussian.
 
         :param z: features
         :param y: class labels
         :param device: device to use
         :return:
         """
-
         if device is None:
             device = z.device
             log.warning(f"No device given. Will use '{device}'.")
 
         z, y = z.to(device), y.to(device)
 
         log.debug("Calculating mahalanobis parameters.")
         classes = y.unique()
 
         # we assume here that all class 0 >= labels <= classes.max() exist
         assert len(classes) == classes.max().item() + 1
         assert not contains_unknown(classes)
 
         n_classes = len(classes)
-        self.mu = torch.zeros(size=(n_classes, z.shape[-1])).to(device)
-        self.cov = torch.zeros(size=(z.shape[-1], z.shape[-1])).to(device)
+        self.mu = torch.zeros(size=(n_classes, z.shape[-1]), device=device)
+        self.cov = torch.zeros(size=(z.shape[-1], z.shape[-1]), device=device)
 
         for clazz in range(n_classes):
             idxs = y.eq(clazz)
             assert idxs.sum() != 0
-            zs = z[idxs].to(device)
+            zs = z[idxs]
             self.mu[clazz] = zs.mean(dim=0)
             self.cov += (zs - self.mu[clazz]).T.mm(zs - self.mu[clazz])
 
         self.cov += torch.eye(self.cov.shape[0], device=self.cov.device) * 1e-6
         self.precision = torch.linalg.inv(self.cov)
         return self
 
-    def predict_features(self, x: Tensor) -> Tensor:
+    def _calc_gaussian_scores(self, z: Tensor) -> Tensor:
         """
-        Calculates mahalanobis distance directly on features.
-        ODIN preprocessing will not be applied.
 
-        :param x: features, as given by the model.
         """
-        features = x.view(x.size(0), x.size(1), -1)
+        features = z.view(z.size(0), z.size(1), -1)
         features = torch.mean(features, 2)
-        noise_gaussian_scores = []
+        md_k = []
 
+        # calculate per class scores
         for clazz in range(self.n_classes):
-            centered_features = features.data - self.mu[clazz]
-            term_gau = (
-                -0.5
-                * torch.mm(
-                    torch.mm(centered_features, self.precision), centered_features.t()
-                ).diag()
-            )
+            centered_z = features.data - self.mu[clazz]
+            term_gau = -0.5 * torch.mm(torch.mm(centered_z, self.precision), centered_z.t()).diag()
+            md_k.append(term_gau.view(-1, 1))
+
+        return torch.cat(md_k, 1)
 
-            noise_gaussian_scores.append(term_gau.view(-1, 1))
+    def predict_features(self, z: Tensor) -> Tensor:
+        """
+        Calculates mahalanobis distance directly on features.
+        ODIN preprocessing will not be applied.
 
-        noise_gaussian_score = torch.cat(noise_gaussian_scores, 1)
+        :param z: features, as given by the model.
+        """
+        if self.mu is None:
+            raise RequiresFittingException
 
-        noise_gaussian_score = torch.max(noise_gaussian_score, dim=1).values
-        return -noise_gaussian_score
+        md_k = self._calc_gaussian_scores(z)
+        score = - torch.max(md_k, dim=1).values
+        return score
 
     def predict(self, x: Tensor) -> Tensor:
         """
         :param x: input tensor
         """
-        if self.mu is None:
-            raise RequiresFittingException
-
         if self.model is None:
             raise ModelNotSetException
 
         if self.eps > 0:
             x = self._odin_preprocess(x, x.device)
 
         features = self.model(x)
@@ -171,37 +173,37 @@
                 features = self.model(x)
                 features = features.view(features.shape[0], -1)  # flatten
                 score = None
 
                 for clazz in range(self.n_classes):
                     centered_features = features.data - self.mu[clazz]
                     term_gau = (
-                        -0.5
-                        * torch.mm(
-                            torch.mm(centered_features, self.precision),
-                            centered_features.t(),
-                        ).diag()
+                            -0.5
+                            * torch.mm(
+                        torch.mm(centered_features, self.precision),
+                        centered_features.t(),
+                    ).diag()
                     )
 
                     if clazz == 0:
                         score = term_gau.view(-1, 1)
                     else:
                         score = torch.cat((score, term_gau.view(-1, 1)), dim=1)
 
                 # calculate gradient of inputs with respect to score of predicted class,
                 # according to mahalanobis distance
                 sample_pred = score.max(dim=1).indices
                 batch_sample_mean = self.mu.index_select(0, sample_pred)
                 centered_features = features - Variable(batch_sample_mean)
                 pure_gau = (
-                    -0.5
-                    * torch.mm(
-                        torch.mm(centered_features, Variable(self.precision)),
-                        centered_features.t(),
-                    ).diag()
+                        -0.5
+                        * torch.mm(
+                    torch.mm(centered_features, Variable(self.precision)),
+                    centered_features.t(),
+                ).diag()
                 )
                 loss = torch.mean(-pure_gau)
                 loss.backward()
 
                 gradient = torch.sign(x.grad.data)
 
         if self.norm_std:
```

## pytorch_ood/detector/softmax.py

```diff
@@ -7,28 +7,35 @@
 
 ..  autoclass:: pytorch_ood.detector.MaxSoftmax
     :members:
 
 """
 from typing import Optional, TypeVar
 
-from torch import Tensor
+import torch.nn
+from torch import Tensor, tensor
+from torch.nn.functional import nll_loss
 from torch.nn import Module
+from torch.optim import LBFGS
+from torch.utils.data import DataLoader
+import logging
 
-from ..api import Detector, ModelNotSetException
+from ..api import Detector, ModelNotSetException, RequiresFittingException
+from pytorch_ood.utils import extract_features, is_known
 
+log = logging.getLogger(__name__)
 Self = TypeVar("Self")
 
 
 class MaxSoftmax(Detector):
     """
     Implements the Maximum Softmax Probability (MSP) Thresholding baseline for OOD detection.
 
     Optionally, implements temperature scaling, which divides the logits by a constant temperature :math:`T`
-    before calculating the softmax.
+    before calculating the softmax. The score is calculated as:
 
     .. math:: - \\max_y \\sigma_y(f(x) / T)
 
     where :math:`\\sigma` is the softmax function and :math:`\\sigma_y`  indicates the :math:`y^{th}` value of the
     resulting probability vector.
 
     :see Paper:
@@ -40,25 +47,25 @@
 
     def __init__(self, model: Module, t: Optional[float] = 1.0):
         """
         :param model: neural network to use
         :param t: temperature value :math:`T`. Default is 1.
         """
         super(MaxSoftmax, self).__init__()
-        self.t = t
+        self.t = tensor(t)
         self.model = model
 
     def predict(self, x: Tensor) -> Tensor:
         """
         :param x: input, will be passed through model
         """
         if self.model is None:
             raise ModelNotSetException
 
-        return self.score(self.model(x), t=self.t)
+        return self.predict_features(self.model(x))
 
     def fit(self: Self, *args, **kwargs) -> Self:
         """
         Not required
         """
         return self
 
@@ -77,7 +84,8 @@
     @staticmethod
     def score(logits: Tensor, t: Optional[float] = 1.0) -> Tensor:
         """
         :param logits: logits for samples
         :param t: temperature value
         """
         return -logits.div(t).softmax(dim=1).max(dim=1).values
+
```

## pytorch_ood/model/wrn.py

```diff
@@ -242,14 +242,27 @@
         out = self.block2(out)
         out = self.block3(out)
         out = self.relu(self.bn1(out))
         out = F.avg_pool2d(out, 8)
         out = out.view(-1, self.nChannels)
         return self.fc(out)
 
+    def features_before_pool(self, x: Tensor) -> Tensor:
+        out = self.conv1(x)
+        out = self.block1(out)
+        out = self.block2(out)
+        out = self.block3(out)
+        out = self.relu(self.bn1(out))
+        return out
+
+    def forward_from_before_pool(self, x: Tensor) -> Tensor:
+        out = F.avg_pool2d(x, 8)
+        out = out.view(-1, self.nChannels)
+        return self.fc(out)
+
     def features(self, x: Tensor) -> Tensor:
         """
         Extracts (flattened) features before the last fully connected layer.
         """
         out = self.conv1(x)
         out = self.block1(out)
         out = self.block2(out)
```

## pytorch_ood/utils/transforms.py

```diff
@@ -5,14 +5,17 @@
 
 ..  autoclass:: pytorch_ood.utils.ToRGB
     :members:
 
 ..  autoclass:: pytorch_ood.utils.TargetMapping
     :members:
 """
+from typing import Set
+
+import torch
 
 
 class ToUnknown(object):
     """
     Callable that returns a negative number, used in pipelines to mark specific datasets as OOD or unknown.
     """
 
@@ -44,30 +47,30 @@
     If we split up a dataset so that the classes 2,3,4,9 are considered *known* or *IN*, these class
     labels have to be remapped to 0,1,2,3 to be able to train
     using cross entropy with 1-of-K-vectors. All other classes have to be mapped to values :math:`<1`.
 
     Target mappings have to be known at evaluation time.
     """
 
-    def __init__(self, train_in_classes, train_out_classes, test_out_classes):
-        self.train_in_classes = train_in_classes
-        self.train_out_classes = train_out_classes
-        self.test_out_classes = test_out_classes
+    def __init__(self, known: Set, unknown: Set):
         self._map = dict()
-        self._map.update({clazz: index for index, clazz in enumerate(train_in_classes)})
-        # mapping test_out classes to < -1000
-        self._map.update({clazz: (-clazz - 1000) for index, clazz in enumerate(test_out_classes)})
+        self._map.update({clazz: index for index, clazz in enumerate(set(known))})
         # mapping train_out classes to < 0
-        self._map.update({clazz: (-clazz) for index, clazz in enumerate(train_out_classes)})
+        self._map.update({clazz: (-clazz) for index, clazz in enumerate(set(unknown))})
 
     def __call__(self, target):
-        # log.info(f"Target: {target} known: {target in self._map}")
+        if isinstance(target, torch.Tensor):
+            return self._map.get(target.item(), -1)
+
         return self._map.get(target, -1)
 
     def __getitem__(self, item):
+        if isinstance(item, torch.Tensor):
+            return self._map[item.item()]
+
         return self._map[item]
 
     def items(self):
         return self._map.items()
 
     def __repr__(self):
         return str(self._map)
```

## Comparing `pytorch_ood-0.1.4.dist-info/LICENSE` & `pytorch_ood-0.1.5.dist-info/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2022 Konstantin Kirchheim
+   Copyright 2023 Konstantin Kirchheim
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

## Comparing `pytorch_ood-0.1.4.dist-info/METADATA` & `pytorch_ood-0.1.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ood
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Library for Out-of-Distribution Detection with PyTorch
 Home-page: https://github.com/kkirchheim/pytorch-ood
 Author: Konstantin Kirchheim
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/kkirchheim/pytorch-ood/issues
 Project-URL: repository, https://github.com/kkirchheim/pytorch-ood
 Keywords: OOD,PyTorch,Out-of-Distribution Detection
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: torch (>=1.7.0)
 Requires-Dist: torchvision (>=0.12.0)
 Requires-Dist: torchmetrics (>=1.0.0)
 Requires-Dist: scipy (>=1.7.0)
+Requires-Dist: numpy (>=1.23.0)
 
 PyTorch Out-of-Distribution Detection
 ****************************************
 
 .. image:: https://img.shields.io/badge/docs-online-blue
    :target: https://pytorch-ood.readthedocs.io/en/latest/
    :alt: Documentation
```

## Comparing `pytorch_ood-0.1.4.dist-info/RECORD` & `pytorch_ood-0.1.5.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,59 @@
-pytorch_ood/__init__.py,sha256=8C0gUZGqnsI_3e4qRaRP3gfXMvEDm_8iHaeWxBruaeQ,209
+pytorch_ood/__init__.py,sha256=nllKeaM47eScMYKNnbJ1yiPw32YpV-rbN8naflvdbP8,209
 pytorch_ood/api.py,sha256=eOp1WgYknpzDq8v1hY8V7oWXsI6SQHyCAC1C1dSL6MI,2341
 pytorch_ood/benchmark/__init__.py,sha256=sRY6Sh4aPdcIuuGbvApXq_uAnVBA5xkslpPod3Za-Vo,1404
 pytorch_ood/benchmark/base.py,sha256=2uX-drzDBoz1sG4S2W3Bgsa2riZV_-OsQbP8lf2dD4w,876
 pytorch_ood/benchmark/img/__init__.py,sha256=Iq_4O1y3fl3cGZyzq5-6bVEf_abHmKwHeuEL-75FhqM,144
 pytorch_ood/benchmark/img/cifar10.py,sha256=rKkIBukethyNUZU3GI7lDOGF8H8hpvcZ9S9SXffu-TI,7122
 pytorch_ood/benchmark/img/cifar100.py,sha256=Pt-C-KNiHTx5LZWiO1O6gY9OTmocbF-ORnLqzfQ18YM,7157
 pytorch_ood/benchmark/img/imagenet.py,sha256=esPDHIg_hNJcssqWDE1FynPlDFQ4px2H-OU24RpBDME,3922
 pytorch_ood/dataset/__init__.py,sha256=4mwJ-YED4MXBlZXeqi04Qg5zxqDMxaszHOupjVy9LAQ,11
 pytorch_ood/dataset/audio/__init__.py,sha256=zYLehvyFdN4DjcGRPpoLVMgSp9HNiAiXAfjxT8CH10k,165
 pytorch_ood/dataset/audio/fsdd.py,sha256=cYKcHtbV7BhGKav_d5qFvNiLRwhvwzWTC93txgu2ezg,3059
-pytorch_ood/dataset/img/__init__.py,sha256=RN_xTWNyZCERYt7y8_xMrt1EIfBN5Cvf-PiOAGX3iBg,3487
+pytorch_ood/dataset/img/__init__.py,sha256=qfcHkUbHSNU2ZOOq4N3larL_YOA1coWAOB_ylMCpwK0,3491
 pytorch_ood/dataset/img/base.py,sha256=4MGJXE2eQ35sSobrn5rVictgdRcYaNlAB1hV5zcBl6E,2457
 pytorch_ood/dataset/img/chars74k.py,sha256=YA4Hx92fS29jxrpG0zEc09RaRSpmGRdMQMBJ4lyAm2E,4329
 pytorch_ood/dataset/img/cifar.py,sha256=seM3RpADphYfIt9ON5Wpslv5_QNTs5fhi3JfEkVH-vE,3076
 pytorch_ood/dataset/img/fooling.py,sha256=IBi0nWCIYRZJSgFrJejhpgmTB5CWswlc466wXTo41EA,1331
 pytorch_ood/dataset/img/imagenet.py,sha256=MpA-6DD6R1JlIWmS1Ytuik-kfImCnPc-H_Urzj13eqU,5793
 pytorch_ood/dataset/img/mnistc.py,sha256=Wp06GFhRi9_iM6SSe_rUG3GuolMUtuZ_qlR7ctpY4l0,4270
 pytorch_ood/dataset/img/mvtech.py,sha256=Ki5BjbohoWQ-W3tGNAh_1yxidutiujQfBI8tvgEL5R4,5382
 pytorch_ood/dataset/img/noise.py,sha256=Nt0AF6iFAns0amJ1y3TZHu_WY1qyyb3splVa9Lt-49c,3936
 pytorch_ood/dataset/img/odin.py,sha256=ryBc43DqdRzQ5HMc1X6JNMy_-InR74mbO_-9AAxKOf4,4891
 pytorch_ood/dataset/img/openood.py,sha256=fxq9rhSAhHN1S-4hxa_uAZoFsEoGKpLLBi-iYL2iIlI,4836
 pytorch_ood/dataset/img/pixmix.py,sha256=um3PfP9Gb03TwjoEyOCxatI_ci824FHY35ygX-E7kBU,8477
 pytorch_ood/dataset/img/streethazards.py,sha256=R4-EMG9voEOshJEBmFtf17KijNcuveuufOVwQVMhqGE,4242
 pytorch_ood/dataset/img/textures.py,sha256=VLEv5Md6pNqivOhAp4vUwxuEWfAwfvkPMvnd7zSmDrM,3001
-pytorch_ood/dataset/img/tinyimagenet.py,sha256=EkXQ3Lb6gFS480mf40HXKJl00SUNXoi732Kv09bcH6g,3766
+pytorch_ood/dataset/img/tinyimagenet.py,sha256=OdBRd4mKP819YqmzSl2Ay7zWi2rW2sbxgCc2rWD8f74,3780
 pytorch_ood/dataset/img/tinyimages.py,sha256=sOw_TIPUxqFaqR5rxAISizkKPNf4BgBcn_kp_bVsiTI,4692
 pytorch_ood/dataset/ossim/__init__.py,sha256=v3qdGAIvb1X6NUHDOK4-jAk1R8nq6Oisjds3ZG2IEp4,507
 pytorch_ood/dataset/ossim/ossim.py,sha256=W6MlSCxrTs_EGlYhB8sSpboh1EDztJJ9YhLVyXv1zSQ,8194
 pytorch_ood/dataset/txt/__init__.py,sha256=wpmf8nqnJkDI-CAgAI-pH07PoV0UKu_miSreNaEX9dw,1049
-pytorch_ood/dataset/txt/multi30k.py,sha256=35ssfLwz8zrj50UwxA0s9rw5VKXMQADuwRXt3Bmcspg,2665
+pytorch_ood/dataset/txt/multi30k.py,sha256=cIigkuGikYOpKwjgp79nzHvb3WVvtg8Of9TwMlQbp1g,2665
 pytorch_ood/dataset/txt/newsgroups.py,sha256=4tTVikOfXEEUw0CX0vm2pzPKhund5VYNaUYlyGWCNIQ,4002
 pytorch_ood/dataset/txt/reuters.py,sha256=ZWyQ_8VfmPu-9CdDf1PByMqy6HMoxjXGqscmICcHQTk,5954
 pytorch_ood/dataset/txt/stop_words.py,sha256=qSZlcCeyoKKpHfvJJjU6PHcXeG1pia324VdT6jE1HgI,1983
 pytorch_ood/dataset/txt/wiki.py,sha256=Mqvke4I6gh7nvTTw66lcJcamn7TXJ-CnDKSPHYPBHOU,3331
 pytorch_ood/dataset/txt/wmt16.py,sha256=5DVHikenTFOtwn0LaqEEh6xEYeZ9rhQYdrXEzWyDt14,2034
-pytorch_ood/detector/__init__.py,sha256=Z8XLIhK5XVRENoaFLZa8iPT6TqGIuTLcGENYoJ9Jk38,2395
+pytorch_ood/detector/__init__.py,sha256=du5bKt4ZoJS90DS3CznYJAN0wyKGo_OZabHRMZQDGTs,3461
+pytorch_ood/detector/ash.py,sha256=efxXeq1u-Yz2pUahs5JFyXAzZtOyCM8M2JjkG7pb7Co,4693
+pytorch_ood/detector/dice.py,sha256=xArOhczC-dn2fRIpJdP_LEXeeFHaO9SA1i0xzgvEv0M,3050
 pytorch_ood/detector/energy.py,sha256=HtLHQAZ1Oh_xcuyRf3CwJxc0Bov2WeQe6k8inhFjukM,2352
 pytorch_ood/detector/entropy.py,sha256=n2V7rUcORUf9xTnN7wDtMb3waUy9c47QSlcsi3-6_gI,2046
 pytorch_ood/detector/klmatching.py,sha256=NKv0Boyo8GlpTWPv8O4ESA5cWOL1_OeZILEZYVwJ6sY,4402
-pytorch_ood/detector/mahalanobis.py,sha256=sKlRdiVF4qiq_DWcgAKgsLpIaaezQsIE3IgV0Gtw8rE,7749
+pytorch_ood/detector/knn.py,sha256=j2NiRHmLhZ8JeB5vStdpIQyKg8KYwEuF_3ampkYSM1I,3201
+pytorch_ood/detector/mahalanobis.py,sha256=3gmzLU84D0BEWZaEGVnWoOdtsU20vrmJAGUOSYcBfIY,7841
 pytorch_ood/detector/maxlogit.py,sha256=vkOO3fLWVLLQjKAupGe4H8CFi_A2rWwGLEFhz26M45Q,1810
 pytorch_ood/detector/mcd.py,sha256=GSRw_p86ss5PN1NZSiykGhh-xRYpQfJ6vaU4-4btSRs,3619
 pytorch_ood/detector/odin.py,sha256=rFjyD_sVgRzqTnQq43tXg38pUzyAUrQtWODfC8JgplE,5816
-pytorch_ood/detector/softmax.py,sha256=9LbSwPVPb_GCU3ABIRuG4m2wY2-MqyLK-rgo4qR1bFg,2316
+pytorch_ood/detector/react.py,sha256=hwMfdS0WQ88qB5m2D0J0wcsYtcuxpR9RcRzi_B7-XKs,2633
+pytorch_ood/detector/rmd.py,sha256=aE5q7ILgMQ4hubykvtVddIPVIs1MVGRUj6sIObAEnrg,4362
+pytorch_ood/detector/she.py,sha256=Y6AyYhOpcfAgAyt4K3ig1jGwt9A5eBSRkEjTAchlL_Q,2812
+pytorch_ood/detector/softmax.py,sha256=MX49Tn0JG9J0LWyqokCNH1_nmS9y-DoeexlGKA5aXUA,2621
+pytorch_ood/detector/tscaling.py,sha256=bt00wPkO9NFf8Uo9tWVLq1eeXcoxgqFVQJyhrYuGI0E,3428
 pytorch_ood/detector/vim.py,sha256=v5Og7bL3oGEXSPfv9WQv1iF0wRofNfKrVttO4EDSE6I,5267
 pytorch_ood/detector/openmax/__init__.py,sha256=aLSjSeuO9EgxWo5SBbLyOqMLcIMIbgpju9WUL8wtgyE,323
 pytorch_ood/detector/openmax/numpy.py,sha256=zh5SHjrHhfeWX9Tol5aaDbaKtxT70j8JjSC7EtHi1s0,7041
 pytorch_ood/detector/openmax/torch.py,sha256=Ztzt7Y8IRgRocVZ-TzBbBBmGFIFlH5RZyITiMtAC-EQ,3318
 pytorch_ood/loss/__init__.py,sha256=p3b1JB96f4YjaDkk1PvaaMFs7tDxUyPW6_lZqR5gFGI,5408
 pytorch_ood/loss/background.py,sha256=d9TNUzeWqsZ7c-EjAGFrWPdOagnQIcJ4hTmTtJD50sc,1589
 pytorch_ood/loss/cac.py,sha256=p1qGxb3i447r6fY1vk3Hh7MWrPUC1KHD4aeh2wUAqmU,3877
@@ -59,18 +66,18 @@
 pytorch_ood/loss/mchad.py,sha256=u-a4tOnDqHeKgwtUb8XPtJqdCsGPtOIUcOnm1p9LgaE,4875
 pytorch_ood/loss/objectosphere.py,sha256=eubnoMhEkmdIhuFAB485CBX-eT0NObxt7FTCkp8HAJE,2667
 pytorch_ood/loss/oe.py,sha256=k9VRWIGyodwk5crz6snu8KGb2VSzGRmP8lCYBxm10WE,2199
 pytorch_ood/loss/svdd.py,sha256=raL0nldFjwk77UM-IDM3B0mGHv50neBZULEPXd5zcaM,5289
 pytorch_ood/model/__init__.py,sha256=U2iKbCxQMfzkk1q9eeo2Wg2Bm81-UUpN9nA2o5dDwZ0,723
 pytorch_ood/model/centers.py,sha256=4pJ5_fWQ_BOO-QRkwAqc5lGZbUsO6F-ZHOlAmQQWYbs,4684
 pytorch_ood/model/gru.py,sha256=bWgH_9kHofqaqK19K0fm3VA-AimQ6EWuoq3pS6FUo48,1611
-pytorch_ood/model/wrn.py,sha256=hAOGgBiOGPdWubvlYZLEfL0-VC6eTXY145GvyT71CgQ,12226
+pytorch_ood/model/wrn.py,sha256=TgXij1K1XsX5PEBhBTePn4vDMHY1_smjfhxBV6dumXg,12629
 pytorch_ood/utils/__init__.py,sha256=7HadmLfYRDYnSzWduQZdcIIOzfH-8-_BO8lbq1g-wNk,70
 pytorch_ood/utils/gdown.py,sha256=EC-bvd3Qp82zO0wrpLpwh2QVzDQSCKM5SwwO759B5_0,10960
 pytorch_ood/utils/metrics.py,sha256=0a9-c9fUPMK3MjLGo6amWSn18wVGJZv3VotNv9oaILg,7093
-pytorch_ood/utils/transforms.py,sha256=uf2MAtsq0BezMv2Vv4e3_EgJNWPeTM7yeEC7eGtVPO0,2111
+pytorch_ood/utils/transforms.py,sha256=VawQSFMclq7jTjbCjRiCGJvV_AXvuc9K4k09R3imcP4,1929
 pytorch_ood/utils/utils.py,sha256=mod65a7ibuaNcwc7fSe0VdWJFNlqDyCU7whrGMMtY_k,8878
-pytorch_ood-0.1.4.dist-info/LICENSE,sha256=sCskNJvx8BCnWvaR8F3J3W0pm3bJhObe3XZKfuLTvnA,11351
-pytorch_ood-0.1.4.dist-info/METADATA,sha256=qqC8tyXxLl3jSdsD8PaOK0J6wno991qfLUnVGHnts-o,23728
-pytorch_ood-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pytorch_ood-0.1.4.dist-info/top_level.txt,sha256=DQdb7oLs5bEbGwRkFDMkBe3xeGccj8U-P4eHsi8VOS0,12
-pytorch_ood-0.1.4.dist-info/RECORD,,
+pytorch_ood-0.1.5.dist-info/LICENSE,sha256=oE9hL_1c39hhaBzmIHPW_5r_4InRrWOI02jxskyrYyQ,11351
+pytorch_ood-0.1.5.dist-info/METADATA,sha256=GWIJFtEwsR9dYo86uHm7DVzAd9-LAKUeRDHiuTo8Peo,23760
+pytorch_ood-0.1.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pytorch_ood-0.1.5.dist-info/top_level.txt,sha256=DQdb7oLs5bEbGwRkFDMkBe3xeGccj8U-P4eHsi8VOS0,12
+pytorch_ood-0.1.5.dist-info/RECORD,,
```

