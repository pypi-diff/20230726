# Comparing `tmp/froog-0.1.6.tar.gz` & `tmp/froog-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froog-0.1.6.tar", last modified: Mon Jul 24 03:29:19 2023, max compression
+gzip compressed data, was "froog-0.1.7.tar", last modified: Wed Jul 26 06:37:17 2023, max compression
```

## Comparing `froog-0.1.6.tar` & `froog-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 03:29:19.273678 froog-0.1.6/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-07-16 20:10:22.000000 froog-0.1.6/LICENSE
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2437 2023-07-24 03:29:19.273590 froog-0.1.6/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2112 2023-07-24 01:58:06.000000 froog-0.1.6/README.md
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 03:29:19.272624 froog-0.1.6/frog/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       54 2023-07-24 00:15:18.000000 froog-0.1.6/frog/__init__.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2103 2023-07-19 07:06:24.000000 froog-0.1.6/frog/gradcheck.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)    10298 2023-07-24 00:13:42.000000 froog-0.1.6/frog/ops.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2016 2023-07-19 05:23:59.000000 froog-0.1.6/frog/optim.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     3802 2023-07-24 00:17:09.000000 froog-0.1.6/frog/tensor.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2685 2023-07-23 19:46:48.000000 froog-0.1.6/frog/utils.py
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-24 03:29:19.273452 froog-0.1.6/froog.egg-info/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2437 2023-07-24 03:29:19.000000 froog-0.1.6/froog.egg-info/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      260 2023-07-24 03:29:19.000000 froog-0.1.6/froog.egg-info/SOURCES.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-07-24 03:29:19.000000 froog-0.1.6/froog.egg-info/dependency_links.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       15 2023-07-24 03:29:19.000000 froog-0.1.6/froog.egg-info/requires.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        5 2023-07-24 03:29:19.000000 froog-0.1.6/froog.egg-info/top_level.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-07-24 03:29:19.273709 froog-0.1.6/setup.cfg
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      849 2023-07-24 03:29:13.000000 froog-0.1.6/setup.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-26 06:37:17.079475 froog-0.1.7/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-07-16 20:10:22.000000 froog-0.1.7/LICENSE
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2451 2023-07-26 06:37:17.079350 froog-0.1.7/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2125 2023-07-26 06:32:22.000000 froog-0.1.7/README.md
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-26 06:37:17.077371 froog-0.1.7/froog/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       57 2023-07-26 06:32:22.000000 froog-0.1.7/froog/__init__.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2107 2023-07-26 06:32:22.000000 froog-0.1.7/froog/gradcheck.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)    10300 2023-07-26 06:32:22.000000 froog-0.1.7/froog/ops.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2016 2023-07-19 05:23:59.000000 froog-0.1.7/froog/optim.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     3803 2023-07-26 06:32:22.000000 froog-0.1.7/froog/tensor.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2685 2023-07-23 19:46:48.000000 froog-0.1.7/froog/utils.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-26 06:37:17.077931 froog-0.1.7/froog.egg-info/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2451 2023-07-26 06:37:17.000000 froog-0.1.7/froog.egg-info/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      350 2023-07-26 06:37:17.000000 froog-0.1.7/froog.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-07-26 06:37:17.000000 froog-0.1.7/froog.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       15 2023-07-26 06:37:17.000000 froog-0.1.7/froog.egg-info/requires.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        6 2023-07-26 06:37:17.000000 froog-0.1.7/froog.egg-info/top_level.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-07-26 06:37:17.079508 froog-0.1.7/setup.cfg
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      852 2023-07-26 06:36:29.000000 froog-0.1.7/setup.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-26 06:37:17.079074 froog-0.1.7/tests/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     3184 2023-07-26 06:32:22.000000 froog-0.1.7/tests/test_conv_speed.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     4256 2023-07-26 06:32:22.000000 froog-0.1.7/tests/test_mnist.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2949 2023-07-26 06:32:22.000000 froog-0.1.7/tests/test_ops.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2604 2023-07-26 06:32:22.000000 froog-0.1.7/tests/test_tensor.py
```

### Comparing `froog-0.1.6/PKG-INFO` & `froog-0.1.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: froog
-Version: 0.1.6
-Summary: FROG: Fast Real-time Optimization of Gradients
+Version: 0.1.7
+Summary: FROOG: Fast Real-time Optimization Of Gradients
 Author: Kevin Buhler
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# frog <img src="https://github.com/kevbuh/frog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
+# froog <img src="https://github.com/kevbuh/froog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
 <div align="center" >
-  <img src="https://raw.githubusercontent.com/kevbuh/frog/main/assets/froog.jpeg" alt="froog the frog" height="300">
+  <img src="https://raw.githubusercontent.com/kevbuh/froog/main/assets/froog.jpeg" alt="froog the froog" height="300">
   <br/>
-  frog: fast real-time optimization of gradients 
+  froog: fast real-time optimization of gradients 
   <br/>
   a beautifully compact machine-learning library
   <br/>
-  <a href="https://github.com/kevbuh/frog">homepage</a> | <a href="https://github.com/kevbuh/frog/tree/main/docs">documentation</a> | <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> | <a href="https://pypi.org/project/froog/">pip</a>
+  <a href="https://github.com/kevbuh/froog">homepage</a> | <a href="https://github.com/kevbuh/froog/tree/main/docs">documentation</a> | <a href="https://github.com/kevbuh/froog/tree/main/examples">examples</a> | <a href="https://pypi.org/project/froog/">pip</a>
   <br/>
   <br/>
 </div>
 
 <!-- modern ml development is unintuitive, time consuming, and unaccessible. why not make it possible for anyone to build? -->
 # Installation
 ```bash
@@ -43,20 +43,20 @@
 - Scalar-Matrix Multiplication
 - Dot Product
 - Sum
 - ReLU
 - Log Softmax
 - 2D Convolutions
 - Avg & Max pooling
-- <a href="https://github.com/kevbuh/frog/blob/main/frog/ops.py">More</a> 
+- <a href="https://github.com/kevbuh/froog/blob/main/froog/ops.py">More</a> 
 
 # Bounties
 Want to help but don't know where to start? 
 
-Our top bounty is to get EfficientNet v2 model working inside of the <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> folder.
+Our top bounty is to get EfficientNet v2 model working inside of the <a href="https://github.com/kevbuh/froog/tree/main/examples">examples</a> folder.
 
 #### Easy
 - built in MLP model
 - binary cross entropy
 - flatten
 - batch_norm
 - pad
@@ -72,11 +72,11 @@
 - MPS support
 - CUDA support
 
 # Contributing
 here are some basic guidelines for contributing:
 * reduce complexity (currently at 585 lines of code)
 * increase speed
-* add features, must include <a href="https://github.com/kevbuh/frog/tree/main/tests">tests</a>
+* add features, must include <a href="https://github.com/kevbuh/froog/tree/main/tests">tests</a>
 * in that order
 
-more info on <a href="https://github.com/kevbuh/frog/blob/main/docs/contributing.md">contributing</a>
+more info on <a href="https://github.com/kevbuh/froog/blob/main/docs/contributing.md">contributing</a>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: froog Version: 0.1.6 Summary: FROG: Fast Real-time
-Optimization of Gradients Author: Kevin Buhler License: MIT Classifier:
+Metadata-Version: 2.1 Name: froog Version: 0.1.7 Summary: FROOG: Fast Real-time
+Optimization Of Gradients Author: Kevin Buhler License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
-File: LICENSE # frog [unit test badge]
-                               [froog the frog]
-                frog: fast real-time optimization of gradients
+File: LICENSE # froog [unit test badge]
+                              [froog the froog]
+               froog: fast real-time optimization of gradients
                 a beautifully compact machine-learning library
                   homepage | documentation | examples | pip
 
  # Installation ```bash pip install froog ``` ### Overview of Features -
 Tensors - Automatic Differentiation - Forward and backward passes - Input/
 gradient shape-tracking - MNIST example - 2D Convolutions (im2col) - Numerical
 gradient checking - The most common optimizers (SGD, Adam, RMSProp) ### Math
```

### Comparing `froog-0.1.6/README.md` & `froog-0.1.7/froog.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,28 @@
-# frog <img src="https://github.com/kevbuh/frog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
+Metadata-Version: 2.1
+Name: froog
+Version: 0.1.7
+Summary: FROOG: Fast Real-time Optimization Of Gradients
+Author: Kevin Buhler
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# froog <img src="https://github.com/kevbuh/froog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
 <div align="center" >
-  <img src="https://raw.githubusercontent.com/kevbuh/frog/main/assets/froog.jpeg" alt="froog the frog" height="300">
+  <img src="https://raw.githubusercontent.com/kevbuh/froog/main/assets/froog.jpeg" alt="froog the froog" height="300">
   <br/>
-  frog: fast real-time optimization of gradients 
+  froog: fast real-time optimization of gradients 
   <br/>
   a beautifully compact machine-learning library
   <br/>
-  <a href="https://github.com/kevbuh/frog">homepage</a> | <a href="https://github.com/kevbuh/frog/tree/main/docs">documentation</a> | <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> | <a href="https://pypi.org/project/froog/">pip</a>
+  <a href="https://github.com/kevbuh/froog">homepage</a> | <a href="https://github.com/kevbuh/froog/tree/main/docs">documentation</a> | <a href="https://github.com/kevbuh/froog/tree/main/examples">examples</a> | <a href="https://pypi.org/project/froog/">pip</a>
   <br/>
   <br/>
 </div>
 
 <!-- modern ml development is unintuitive, time consuming, and unaccessible. why not make it possible for anyone to build? -->
 # Installation
 ```bash
@@ -31,20 +43,20 @@
 - Scalar-Matrix Multiplication
 - Dot Product
 - Sum
 - ReLU
 - Log Softmax
 - 2D Convolutions
 - Avg & Max pooling
-- <a href="https://github.com/kevbuh/frog/blob/main/frog/ops.py">More</a> 
+- <a href="https://github.com/kevbuh/froog/blob/main/froog/ops.py">More</a> 
 
 # Bounties
 Want to help but don't know where to start? 
 
-Our top bounty is to get EfficientNet v2 model working inside of the <a href="https://github.com/kevbuh/frog/tree/main/examples">examples</a> folder.
+Our top bounty is to get EfficientNet v2 model working inside of the <a href="https://github.com/kevbuh/froog/tree/main/examples">examples</a> folder.
 
 #### Easy
 - built in MLP model
 - binary cross entropy
 - flatten
 - batch_norm
 - pad
@@ -60,11 +72,11 @@
 - MPS support
 - CUDA support
 
 # Contributing
 here are some basic guidelines for contributing:
 * reduce complexity (currently at 585 lines of code)
 * increase speed
-* add features, must include <a href="https://github.com/kevbuh/frog/tree/main/tests">tests</a>
+* add features, must include <a href="https://github.com/kevbuh/froog/tree/main/tests">tests</a>
 * in that order
 
-more info on <a href="https://github.com/kevbuh/frog/blob/main/docs/contributing.md">contributing</a>
+more info on <a href="https://github.com/kevbuh/froog/blob/main/docs/contributing.md">contributing</a>
```

#### html2text {}

```diff
@@ -1,10 +1,14 @@
-# frog [unit test badge]
-                               [froog the frog]
-                frog: fast real-time optimization of gradients
+Metadata-Version: 2.1 Name: froog Version: 0.1.7 Summary: FROOG: Fast Real-time
+Optimization Of Gradients Author: Kevin Buhler License: MIT Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
+File: LICENSE # froog [unit test badge]
+                              [froog the froog]
+               froog: fast real-time optimization of gradients
                 a beautifully compact machine-learning library
                   homepage | documentation | examples | pip
 
  # Installation ```bash pip install froog ``` ### Overview of Features -
 Tensors - Automatic Differentiation - Forward and backward passes - Input/
 gradient shape-tracking - MNIST example - 2D Convolutions (im2col) - Numerical
 gradient checking - The most common optimizers (SGD, Adam, RMSProp) ### Math
```

### Comparing `froog-0.1.6/frog/gradcheck.py` & `froog-0.1.7/froog/gradcheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
-from frog.tensor import Tensor
-from frog.utils import mask_like
+from froog.tensor import Tensor
+from froog.utils import mask_like
 
 def jacobian(model, input):
   output = model(input)
 
   ji = input.data.reshape(-1).shape[-1]  # jacobian of input
   jo = output.data.reshape(-1).shape[-1] # jacobian of output
   J = np.zeros((jo, ji), dtype=np.float32)
@@ -19,15 +19,15 @@
 
 def numerical_jacobian(model, input, eps = 1e-6):
 #     """
 #     https://timvieira.github.io/blog/post/2017/04/21/how-to-test-gradient-implementations/
 #     Computes :
 #         First-order partial derivatives using Finite-Difference Approximation with Central Difference Method (CDM)
 #     Params:
-#         model : A frog model
+#         model : A froog model
 #         input : An input
 #         eps   : Perturbation step
 #     Returns:
 #         NJ    : an approx. of the Jacobian
 #     """
   output = model(input)
 
@@ -47,15 +47,15 @@
       NJ[o][i] = grad_approx
   return NJ
 
 def gradcheck(model, input, eps = 1e-06, atol = 1e-5, rtol = 0.001):
   """
   Checks whether computed gradient is close to numerical approximation of the Jacobian
   Params:
-    model       : frog model   
+    model       : froog model   
     eps         : eps used to see if gradient is within tolerances
     atol        : absolute tolerance
     rtol        : relative tolerance 
   Returns:
     test_passed : bool of whether the test passed
   """
   NJ = numerical_jacobian(model, input, eps)
```

### Comparing `froog-0.1.6/frog/ops.py` & `froog-0.1.7/froog/ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
-from frog.tensor import Function, register
-from frog.utils import im2col, col2im
+from froog.tensor import Function, register
+from froog.utils import im2col, col2im
 
 # *********** Elementary Functions ***********
 # Add, Mul, ReLU, Dot, Sum, Conv2D, Reshape 
 # grad_output is the gradient of the loss with respect to the output of the operation.
 
 # ******* core ops *******
```

### Comparing `froog-0.1.6/frog/optim.py` & `froog-0.1.7/froog/optim.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.6/frog/tensor.py` & `froog-0.1.7/froog/tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,8 +119,8 @@
   e.g. x.dot(w).relu(), where w is a tensor.
 
   partialmethod is used to create a new method that has some of the arguments to another method already filled in
   the apply method of that instance is added
   """
   setattr(Tensor, name, partialmethod(fxn.apply, fxn))
 
-import frog.ops # this registers all the operations
+import froog.ops # this registers all the operations
```

### Comparing `froog-0.1.6/frog/utils.py` & `froog-0.1.7/froog/utils.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.6/setup.py` & `froog-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
 #!/usr/bin/env python3
-# this file specifies how the frog package is installed, including any necessary dependencies required to run
+# this file specifies how the froog package is installed, including any necessary dependencies required to run
 
 import os
 from setuptools import setup
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 setup(name='froog',
-      version='0.1.6',
-      description='FROG: Fast Real-time Optimization of Gradients',
+      version='0.1.7',
+      description='FROOG: Fast Real-time Optimization Of Gradients',
       author='Kevin Buhler',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
-      packages = ['frog'],
+      packages = ['froog'],
       classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
       ],
       install_requires=['numpy', 'requests'],
       python_requires='>=3.6',
       include_package_data=True)
```

