# Comparing `tmp/NeuralFoil-0.1.7.tar.gz` & `tmp/NeuralFoil-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NeuralFoil-0.1.7.tar", last modified: Fri Jul 21 20:12:10 2023, max compression
+gzip compressed data, was "NeuralFoil-0.1.8.tar", last modified: Wed Jul 26 17:49:43 2023, max compression
```

## Comparing `NeuralFoil-0.1.7.tar` & `NeuralFoil-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:12:10.008917 NeuralFoil-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-21 20:11:59.000000 NeuralFoil-0.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 20:11:59.000000 NeuralFoil-0.1.7/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:12:10.000917 NeuralFoil-0.1.7/NeuralFoil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23661 2023-07-21 20:12:09.000000 NeuralFoil-0.1.7/NeuralFoil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-21 20:12:09.000000 NeuralFoil-0.1.7/NeuralFoil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:12:09.000000 NeuralFoil-0.1.7/NeuralFoil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-21 20:12:09.000000 NeuralFoil-0.1.7/NeuralFoil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 20:12:09.000000 NeuralFoil-0.1.7/NeuralFoil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23661 2023-07-21 20:12:10.008917 NeuralFoil-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22630 2023-07-21 20:11:59.000000 NeuralFoil-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:12:10.000917 NeuralFoil-0.1.7/neuralfoil/
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-21 20:11:59.000000 NeuralFoil-0.1.7/neuralfoil/CL_linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-21 20:11:59.000000 NeuralFoil-0.1.7/neuralfoil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-07-21 20:11:59.000000 NeuralFoil-0.1.7/neuralfoil/neuralfoil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:12:10.004917 NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/
--rw-r--r--   0 runner    (1001) docker     (123)   139485 2023-07-21 20:11:59.000000 NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-large.npz
--rw-r--r--   0 runner    (1001) docker     (123)    39576 2023-07-21 20:11:59.000000 NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-medium.npz
--rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-07-21 20:11:59.000000 NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-small.npz
--rw-r--r--   0 runner    (1001) docker     (123)   532014 2023-07-21 20:11:59.000000 NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-xlarge.npz
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-21 20:11:59.000000 NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-xsmall.npz
--rw-r--r--   0 runner    (1001) docker     (123)   779729 2023-07-21 20:11:59.000000 NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-21 20:11:59.000000 NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz
--rw-r--r--   0 runner    (1001) docker     (123)  3052473 2023-07-21 20:11:59.000000 NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 20:12:10.008917 NeuralFoil-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-21 20:11:59.000000 NeuralFoil-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:49:43.285121 NeuralFoil-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-26 17:49:33.000000 NeuralFoil-0.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-26 17:49:33.000000 NeuralFoil-0.1.8/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:49:43.277121 NeuralFoil-0.1.8/NeuralFoil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24170 2023-07-26 17:49:43.000000 NeuralFoil-0.1.8/NeuralFoil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-26 17:49:43.000000 NeuralFoil-0.1.8/NeuralFoil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:49:43.000000 NeuralFoil-0.1.8/NeuralFoil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-26 17:49:43.000000 NeuralFoil-0.1.8/NeuralFoil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 17:49:43.000000 NeuralFoil-0.1.8/NeuralFoil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    24170 2023-07-26 17:49:43.285121 NeuralFoil-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23139 2023-07-26 17:49:33.000000 NeuralFoil-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:49:43.277121 NeuralFoil-0.1.8/neuralfoil/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-26 17:49:33.000000 NeuralFoil-0.1.8/neuralfoil/CL_linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-26 17:49:33.000000 NeuralFoil-0.1.8/neuralfoil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-07-26 17:49:33.000000 NeuralFoil-0.1.8/neuralfoil/neuralfoil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:49:43.281121 NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/
+-rw-r--r--   0 runner    (1001) docker     (123)   139485 2023-07-26 17:49:33.000000 NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-large.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    39576 2023-07-26 17:49:33.000000 NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-medium.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-07-26 17:49:33.000000 NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-small.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   532014 2023-07-26 17:49:33.000000 NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-xlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-26 17:49:33.000000 NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-xsmall.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   779729 2023-07-26 17:49:33.000000 NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-26 17:49:33.000000 NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz
+-rw-r--r--   0 runner    (1001) docker     (123)  3052473 2023-07-26 17:49:33.000000 NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 17:49:43.285121 NeuralFoil-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-26 17:49:33.000000 NeuralFoil-0.1.8/setup.py
```

### Comparing `NeuralFoil-0.1.7/LICENSE.txt` & `NeuralFoil-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.7/NeuralFoil.egg-info/PKG-INFO` & `NeuralFoil-0.1.8/NeuralFoil.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralFoil
-Version: 0.1.7
+Version: 0.1.8
 Summary: NeuralFoil is an airfoil aerodynamics analysis tool using physics-informed machine learning, in pure Python/NumPy.
 Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe
 Author-email: pds@mit.edu
 Project-URL: Source, https://github.com/peterdsharpe/NeuralFoil
 Project-URL: Bug Reports, https://github.com/peterdsharpe/NeuralFoil/issues
 Keywords: python machine learning analysis optimization aerospace airplane cfd aircraft hydrodynamics aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed neural network
@@ -22,29 +22,28 @@
 
 <p align="center">
     <img src="./media/neuralfoil_logo.svg" width="800" />
 </p>
 
 by [Peter Sharpe](https://peterdsharpe.github.io) (<pds [at] mit [dot] edu>)
 
-
-[!![PyPI](https://img.shields.io/pypi/v/neuralfoil)
-](https://pypi.org/project/NeuralFoil/)
+[![PyPI](https://img.shields.io/pypi/v/neuralfoil)](https://pypi.org/project/NeuralFoil/)
 [![Build Status](https://github.com/peterdsharpe/NeuralFoil/workflows/Tests/badge.svg)](https://github.com/peterdsharpe/NeuralFoil/actions/workflows/run-pytest.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-g.svg)](https://opensource.org/licenses/MIT)
 
 -----
 
 NeuralFoil is a tool for rapid aerodynamics analysis of airfoils, similar to [XFoil](https://web.mit.edu/drela/Public/web/xfoil/). Under the hood, NeuralFoil consists of physics-informed neural networks trained on [tens of millions of XFoil runs](#geometry-parameterization-and-training-data).
 
-NeuralFoil is available here as a pure Python+NumPy standalone, but it is also [available within AeroSandbox](#extended-features-transonics-post-stall-control-surface-deflections), which extends it with many more advanced features. Using the AeroSandbox extension, NeuralFoil can give you **viscous, compressible airfoil aerodynamics for (nearly) any airfoil, with control surface deflections, across $360^\circ$ angle of attack, at any Reynolds number, all nearly instantly** (~5 milliseconds). And, it's guaranteed to return an answer (no non-convergence issues), it's vectorized, and it's $C^1$-continuous (all very useful for gradient-based optimization). 
+NeuralFoil is available here as a pure Python+NumPy standalone, but it is also [available within AeroSandbox](#extended-features-transonics-post-stall-control-surface-deflections), which extends it with many more advanced features. Using the AeroSandbox extension, NeuralFoil can give you **viscous, compressible airfoil aerodynamics for (nearly) any airfoil, with control surface deflections, across $360^\circ$ angle of attack, at any Reynolds number, all nearly instantly** (~5 milliseconds). And, it's guaranteed to return an answer (no non-convergence issues), it's vectorized, and it's $C^1$-continuous (all very useful for gradient-based optimization).
 
 NeuralFoil is [~10x faster than XFoil for a single analysis, and ~1000x faster for multipoint analysis](#table), all with [minimal loss in accuracy compared to XFoil](#performance). Due to the wide variety of training data and the embedding of several physics-based invariants, [this accuracy is seen even on out-of-sample airfoils](#performance) (i.e., airfoils it wasn't trained on). It also has [many nice features](#xfoil-benefit-question) (e.g., smoothness, vectorization, all in Python+NumPy) that make it much easier to use.
 
- NeuralFoil aims to be lightweight, with [minimal dependencies](#dependencies-question) and a [tight, efficient, and easily-understood code-base](./neuralfoil) (less than 500 lines of user-facing code).
+NeuralFoil aims to be lightweight, with [minimal dependencies](#dependencies-question) and a [tight, efficient, and easily-understood code-base](./neuralfoil) (less than 500 lines of user-facing code).
+
 ```
 pip install neuralfoil
 ```
 
 ## Overview
 
 NeuralFoil comes with 8 different neural network models, with increasing levels of complexity:
@@ -62,15 +61,15 @@
 		<td>"xxxlarge"</td>
 	 </tr>
 	</table>
 </div>
 
 This spectrum offers a tradeoff between accuracy and computational cost.
 
-In addition to its neural network models, NeuralFoil also has a bonus "Linear $C_L$ model" that predicts lift coefficient $C_L$ as a purely-linear function of angle of attack $\alpha$. This model is well-suited for linear lifting-line or blade-element-method analyses, where the $C_L(\alpha)$ linearity can be used to solve the resulting system of equations "in one shot" as a linear solve, rather than a less-numerically-robust iterative nonlinear solve.
+In addition to its neural network models, NeuralFoil also has a bonus "Linear $C_L$ model" that predicts lift coefficient $C_L$ as a purely-affine function of angle of attack $\alpha$. This model is well-suited for linear lifting-line or blade-element-method analyses, where the $C_L(\alpha)$ linearity can be used to solve the resulting system of equations "in one shot" as a linear solve, rather than a less-numerically-robust iterative nonlinear solve.
 
 Using NeuralFoil is dead-simple, and also offers several possible "entry points" for inputs. Here's an example showing this:
 
 ```python
 import neuralfoil as nf  # `pip install neuralfoil`
 import numpy as np
 
@@ -93,24 +92,24 @@
 )
 
 # `aero` is a dictionary with keys: ["CL", "CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"]
 ```
 
 ## Performance
 
-Qualitatively, NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$ values. In the figure below, we compare the performance of NeuralFoil to XFoil on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was developed "from scratch" for a [real-world aircraft development program](https://www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-research-aircraft-301633713.html) and is completely separate from [the airfoils used during NeuralFoil's training](#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance: 
+Qualitatively, NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$ values. In the figure below, we compare the performance of NeuralFoil to XFoil on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was developed "from scratch" for a [real-world aircraft development program](https://www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-research-aircraft-301633713.html) and is completely separate from [the airfoils used during NeuralFoil's training](#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance:
 
 <a name="clcd-polar"></a>
 <p align="center">
 	<img src="./benchmarking/neuralfoil_point_validation.svg" width="1000" />
 </p>
 
-NeuralFoil is typically accurate to within a few percent of XFoil's predictions. Note that this figure is on a truly out-of-sample airfoil, so airfoils that are closer to the training set will have even more accurate results. 
+NeuralFoil is typically accurate to within a few percent of XFoil's predictions. Note that this figure is on a truly out-of-sample airfoil, so airfoils that are closer to the training set will have even more accurate results.
 
-NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is not reliably converging, which would otherwise make optimization difficult. 
+NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is not reliably converging, which would otherwise make optimization difficult.
 
 In the table below, we quantify the performance of the NeuralFoil ("NF") models with respect to XFoil more precisely. At a basic level, we care about two things:
 
 - **Accuracy**: how close are the predictions to XFoil's?
 - **Computational Cost**: how long does it take to run?
 
 This table details both of these considerations. The first few columns show the error with respect to XFoil on the test dataset. [The test dataset is completely isolated from the training dataset, and NeuralFoil was not allowed to learn from the test dataset](#geometry-parameterization-and-training-data). Thus, the performance on the test dataset gives a good idea of NeuralFoil's performance "in the wild". The second set of columns gives the runtime speed of the models, both for a single analysis and for a large batch analysis.
@@ -119,25 +118,25 @@
 
 <table><thead><tr><th>Aerodynamics Model</th><th colspan="6">Mean Absolute Error (MAE) of Given Metric, on the Test Dataset, with respect to XFoil</th><th colspan="2">Computational Cost to Run</th></tr></thead><tbody><tr><td></td><td>Lift Coeff.<br>$C_L$</td><td>Fractional Drag Coeff.<br>$\ln(C_D)$   †</td><td>Moment Coeff.<br>$C_M$</td><td>Max Overspeed<br>$u_\max / u_\infty$&nbsp;&nbsp;&nbsp;‡</td><td>Top Transition Loc.<br>$x_{tr, top}/c$</td><td>Bottom Trans. Loc.<br>$x_{tr, bot}/c$</td><td>Runtime<br>(1 run)</td><td>Total Runtime<br>(100,000 runs)</td></tr><tr><td>NF Linear $C_L$ Model</td><td>0.116</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>1 ms</td><td>0.020 sec</td></tr><tr><td>NF "xxsmall"</td><td>0.065</td><td>0.121</td><td>0.010</td><td>0.215</td><td>0.073</td><td>0.100</td><td>3 ms</td><td>0.190 sec</td></tr><tr><td>NF "xsmall"</td><td>0.042</td><td>0.075</td><td>0.007</td><td>0.134</td><td>0.039</td><td>0.055</td><td>4 ms</td><td>0.284 sec</td></tr><tr><td>NF "small"</td><td>0.039</td><td>0.069</td><td>0.006</td><td>0.122</td><td>0.036</td><td>0.050</td><td>4 ms</td><td>0.402 sec</td></tr><tr><td>NF "medium"</td><td>0.027</td><td>0.051</td><td>0.004</td><td>0.088</td><td>0.022</td><td>0.033</td><td>5 ms</td><td>0.784 sec</td></tr><tr><td>NF "large"</td><td>0.024</td><td>0.045</td><td>0.004</td><td>0.079</td><td>0.020</td><td>0.029</td><td>6 ms</td><td>1.754 sec</td></tr><tr><td>NF "xlarge"</td><td>0.023</td><td>0.043</td><td>0.004</td><td>0.076</td><td>0.019</td><td>0.028</td><td>10 ms</td><td>3.330 sec</td></tr><tr><td>NF "xxlarge"</td><td>0.021</td><td>0.040</td><td>0.003</td><td>0.071</td><td>0.018</td><td>0.025</td><td>13 ms</td><td>4.297 sec</td></tr><tr><td>NF "xxxlarge"</td><td>0.020</td><td>0.039</td><td>0.003</td><td>0.070</td><td>0.016</td><td>0.024</td><td>38 ms</td><td>8.980 sec</td></tr><tr><td>XFoil</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>73 ms</td><td>42 min</td></tr></tbody></table>
 
 > † The deviation of $\ln(C_D)$ can be thought of as "the typical relative error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm) of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil is *less* accurate than XFoil - although XFoil is quite accurate, it is clearly not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure above](#clcd-polar)). So, NeuralFoil's true accuracy compared to experiment may differ (in either direction) from the numbers in this table.
 > 
 > ‡ This "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm{crit}$. [More details below.](#extended-features-transonics-post-stall-control-surface-deflections)
 
-Based on these performance numbers, you can select the right tradeoff between accuracy and computational cost for your application. In general, I recommend starting with the "large" model and adjusting from there.
+Based on these performance numbers, you can select the right tradeoff between accuracy and computational cost for your application. In general, I recommend starting with the ["large"](#overview) model and adjusting from there.
 
 In addition to accuracy vs. speed, another consideration when choosing the right model is what you're trying to use NeuralFoil for. Larger models will be more complicated ("less parsimonious," as the math kids would say), which means that they may have more "wiggles" in their outputs—this might be undesirable for gradient-based optimization. On the other hand, larger models will be able to capture a wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-optimization), so larger models could have a benefit in that sense. If you try a specific application and have better/worse results with a specific model, let me know by opening a GitHub issue!
 
 ## Extended Features (transonics, post-stall, control surface deflections)
 
 For more sophisticated airfoil aerodynamics calculations, consider using NeuralFoil via [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) (specifically, through [`asb.Airfoil.get_aero_from_neuralfoil()`](https://github.com/peterdsharpe/AeroSandbox/blob/8ad83aa4e4e40c503884c722143b7730c08089fa/aerosandbox/geometry/airfoil/airfoil.py#L607)). This provides several advanced features:
 
-* Compressible aerodynamics, including transonic and supersonic aerodynamics. AeroSandbox will generally get the critical Mach number accurate to within $\pm 0.01$ or so. Subsonic corrections done using a Laitone correction (a higher-order variant of Prandtl-Glauert and Karman-Tsien). Wave drag accuracy is, of course, less reliable beyond the drag-divergence Mach number, although it still [agrees reasonably closely when compared to RANS CFD](https://github.com/peterdsharpe/AeroSandbox/blob/master/studies/WingTransonics/compare_methods.py).
-* Post-stall (i.e., truly 360 degree range of $\alpha$) aerodynamics. This is useful for applications like wind turbine blades or propeller roots, where the airfoil may be operating at high angles of attack.
-* Control surface deflections. Currently only trailing-edge control surface deflections are supported in AeroSandbox's NeuralFoil interface.
+* **Compressible aerodynamics**, including transonic and supersonic aerodynamics. AeroSandbox will generally get the critical Mach number accurate to within $\pm 0.01$ or so. Subsonic corrections done using a Laitone correction (a higher-order variant of Prandtl-Glauert and Karman-Tsien). Wave drag accuracy is, of course, less reliable beyond the drag-divergence Mach number, although it still [agrees reasonably closely when compared to RANS CFD](https://github.com/peterdsharpe/AeroSandbox/blob/master/studies/WingTransonics/compare_methods.py).
+* **Post-stall aerodynamics** (i.e., truly 360 degree range of $\alpha$). This is useful for applications like wind turbine blades or propeller roots, where the airfoil may be operating at high angles of attack.
+* **Control surface deflections**. Currently only trailing-edge control surface deflections are supported in AeroSandbox's NeuralFoil interface.
 
 ## Installation
 
 [Install from PyPI](https://pypi.org/project/NeuralFoil/) with `pip install neuralfoil`.
 
 <a name="dependencies-question"></a>
 To run models, NeuralFoil currently requires minimal dependencies:
@@ -148,18 +147,37 @@
 
 Currently, NeuralFoil only uses AeroSandbox for airfoil geometry parameterization (i.e., converting from a set of points to a CST parameterization, which is solved as an optimization problem)—the actual math is implemented in pure NumPy. Recent progress on this CST parameterization-fitting problem has allowed it to be recast as a least-squares problem, which is potentially amenable to a pure-NumPy implementation. That being said, AeroSandbox provides a bunch of nice peripheral utilities (e.g., geometry manipulation, visualization, etc.), so it's a nice dependency to have anyway. However, if you'd like to work on a pure-NumPy implementation, open an issue and let me know!
 
 ## Geometry Parameterization and Training Data
 
 #### Geometry Parameterization
 
-To be written, but it's basically an 8-parameter-per-side CST (Kulfan) parameterization, with Kulfan's added leading-edge-modification (LEM) and trailing-edge thickness parameter. This gives a total of (8 * 2 + 1 + 1) = 18 parameters to describe a given airfoil shape. I'll write more here, but in the meantime read:
+<a name="parameterization-question"></a>
+
+As a user, you can give an airfoil in many different formats—for example, as a set of $(x,y)$ coordinates, as a .dat file, or as an AeroSandbox `Airfoil` object. However, under the hood, NeuralFoil parameterizes the airfoil geometry using the CST (Kulfan) parameterization. (You can also directly pass in Kulfan parameters if preferred.)
+
+The airfoil shape fed into NeuralFoil's neural networks is in the form of an 8-parameter-per-side CST (Kulfan) parameterization, with Kulfan's added leading-edge-modification (LEM) and trailing-edge thickness parameter. This gives a total of (8 * 2 + 1 + 1) = 18 parameters to describe a given airfoil shape.
+
+<p align="center">
+	<img src="./media/kulfan_parameterization_illustration.svg" width="1000" />
+</p>
+
+For more details on this parameterization, or why it is a good choice, read:
+
 - [D. A. Masters, "Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943)
 - The seminal paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan, "Universal Parametric Geometry Representation Method"](http://mx1.brendakulfan.com/docs/CST6.pdf)
 
+To convert between airfoil coordinates and the CST parameterization, use the following functions:
+
+```python
+from aerosandbox.geometry.airfoil.airfoil_families import get_kulfan_parameters, get_kulfan_coordinates
+```
+
+with documentation [here](https://aerosandbox.readthedocs.io/en/master/autoapi/aerosandbox/geometry/airfoil/airfoil_families/index.html) or in the source ([here](https://github.com/peterdsharpe/AeroSandbox/blob/8ad83aa4e4e40c503884c722143b7730c08089fa/aerosandbox/geometry/airfoil/airfoil_families.py#L128), [here](https://github.com/peterdsharpe/AeroSandbox/blob/8ad83aa4e4e40c503884c722143b7730c08089fa/aerosandbox/geometry/airfoil/airfoil_families.py#L265)).
+
 #### Training Data
 
 To be written, but in the meantime [see here](https://github.com/peterdsharpe/NeuralFoil/tree/master/training_data). Training data is not (yet) uploaded to GitHub, but will be soon - need to figure out Git LFS, as it's many gigabytes. Contact me if you need it sooner.
 
 ## FAQs
 
 Will NeuralFoil be integrated directly into [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox)?
@@ -191,22 +209,14 @@
 >
 > One advantage of a RANS CFD approach over the NeuralFoil XFoil approach is, of course, transonic modeling. NeuralFoil attempts to get around this a little bit by estimating $C_{p, min}$, which in turn allows you to estimate the critical Mach number. (For an implementation of that, [see here](#extended-features-transonics-post-stall-control-surface-deflections)) But fundamentally, NeuralFoil is likely less accurate in the transonic range because of this. The tradeoff is that the much larger training data set allows NeuralFoil to be more accurate in the subsonic range, where [XFoil is actually usually more accurate than RANS CFD](https://www.sciencedirect.com/science/article/abs/pii/S1270963816300839).
 
 Why not use a neural network trained on wind tunnel data?
 
 > This is a super-cool idea, and I'd love to see someone try it! My guess is that you'd need some kind of morphing wing section (and a way of precisely measuring the shape) in order to get enough data samples to "span" the airfoil design space. Then, you'd just let the wing section sit in the wind tunnel for a few days morphing itself around to collect data, then train a model on that. This would be really awesome, someone should do it!
 
-
-<a name="parameterization-question"></a>
-Why parameterize the airfoil geometry using the CST (Kulfan) parameterization? What exactly does the CST parameterization mean, and how can I convert this parameterization to/from actual airfoil coordinates? Why discretize with 8 CST modes per side? Can NeuralFoil accurately analyze airfoils with thick trailing edges?
-
-> To be written, but in the meantime read:
-> - [D. A. Masters, "Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943)
-> - The seminal paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan, "Universal Parametric Geometry Representation Method"](http://mx1.brendakulfan.com/docs/CST6.pdf)
-
 What's the underlying neural network architecture used in NeuralFoil?
 
 > To be written, but it is essentially a feed-forward neural network with a varying number of total layers and layer width depending on model size. Layer counts and widths were [determined through extensive trial and error](./training/supercloud_job_id_notes.log), in conjunction with observed test- and train-loss values. All layers are dense (fully connected, with weights and biases). All activation functions between layers are $\tanh$, to preserve $C^\infty$-continuity. The number of layers and layer width are as follows:
 >
 > * xxsmall: 2 layers,  32 wide.
 > * xsmall:  3 layers,  32 wide.
 > * small:   3 layers,  48 wide.
@@ -214,15 +224,15 @@
 > * large:   4 layers, 128 wide.
 > * xlarge:  4 layers, 256 wide.
 > * xxlarge: 5 layers, 256 wide.
 > * xxxlarge:5 layers, 512 wide.
 
 ## Acknowledgements
 
-NeuralFoil was trained on MIT Supercloud, a high-performance computing cluster operated by the MIT Lincoln Laboratory Supercomputing Center (LLSC). 
+NeuralFoil was trained on MIT Supercloud, a high-performance computing cluster operated by the MIT Lincoln Laboratory Supercomputing Center (LLSC).
 
 ## License
 
 NeuralFoil is licensed under the MIT license. Please see the [LICENSE](LICENSE.txt) file for details.
 
 ## Citing NeuralFoil
 
@@ -232,8 +242,9 @@
 @misc{neuralfoil,
   author = {Peter Sharpe},
   title = {{NeuralFoil}: An airfoil aerodynamics analysis tool using physics-informed machine learning},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/peterdsharpe/NeuralFoil}},
+}
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.7 Summary: NeuralFoil is an
+Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.8 Summary: NeuralFoil is an
 airfoil aerodynamics analysis tool using physics-informed machine learning, in
 pure Python/NumPy. Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe Author-email: pds@mit.edu Project-URL: Source, https://
 github.com/peterdsharpe/NeuralFoil Project-URL: Bug Reports, https://
 github.com/peterdsharpe/NeuralFoil/issues Keywords: python machine learning
 analysis optimization aerospace airplane cfd aircraft hydrodynamics
 aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed
@@ -10,16 +10,16 @@
 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Physics Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.7
 Description-Content-Type: text/markdown Provides-Extra: training Provides-
 Extra: test Provides-Extra: docs License-File: LICENSE.txt
                          [./media/neuralfoil_logo.svg]
 by [Peter Sharpe](https://peterdsharpe.github.io) (
-at] mit [dot] edu>) [!![PyPI](https://img.shields.io/pypi/v/neuralfoil) ]
-(https://pypi.org/project/NeuralFoil/) [![Build Status](https://github.com/
+at] mit [dot] edu>) [![PyPI](https://img.shields.io/pypi/v/neuralfoil)](https:/
+/pypi.org/project/NeuralFoil/) [![Build Status](https://github.com/
 peterdsharpe/NeuralFoil/workflows/Tests/badge.svg)](https://github.com/
 peterdsharpe/NeuralFoil/actions/workflows/run-pytest.yml) [![License: MIT]
 (https://img.shields.io/badge/License-MIT-g.svg)](https://opensource.org/
 licenses/MIT) ----- NeuralFoil is a tool for rapid aerodynamics analysis of
 airfoils, similar to [XFoil](https://web.mit.edu/drela/Public/web/xfoil/).
 Under the hood, NeuralFoil consists of physics-informed neural networks trained
 on [tens of millions of XFoil runs](#geometry-parameterization-and-training-
@@ -43,15 +43,15 @@
 efficient, and easily-understood code-base](./neuralfoil) (less than 500 lines
 of user-facing code). ``` pip install neuralfoil ``` ## Overview NeuralFoil
 comes with 8 different neural network models, with increasing levels of
 complexity:
    "xxsmall" "xsmall" "small" "medium" "large" "xlarge" "xxlarge" "xxxlarge"
 This spectrum offers a tradeoff between accuracy and computational cost. In
 addition to its neural network models, NeuralFoil also has a bonus "Linear
-$C_L$ model" that predicts lift coefficient $C_L$ as a purely-linear function
+$C_L$ model" that predicts lift coefficient $C_L$ as a purely-affine function
 of angle of attack $\alpha$. This model is well-suited for linear lifting-line
 or blade-element-method analyses, where the $C_L(\alpha)$ linearity can be used
 to solve the resulting system of equations "in one shot" as a linear solve,
 rather than a less-numerically-robust iterative nonlinear solve. Using
 NeuralFoil is dead-simple, and also offers several possible "entry points" for
 inputs. Here's an example showing this: ```python import neuralfoil as nf #
 `pip install neuralfoil` import numpy as np aero = nf.get_aero_from_dat_file( #
@@ -130,142 +130,159 @@
 above](#clcd-polar)). So, NeuralFoil's true accuracy compared to experiment may
 differ (in either direction) from the numbers in this table. > > â¡ This
 "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to
 calculate the critical Mach number $M_\mathrm{crit}$. [More details below.]
 (#extended-features-transonics-post-stall-control-surface-deflections) Based on
 these performance numbers, you can select the right tradeoff between accuracy
 and computational cost for your application. In general, I recommend starting
-with the "large" model and adjusting from there. In addition to accuracy vs.
-speed, another consideration when choosing the right model is what you're
-trying to use NeuralFoil for. Larger models will be more complicated ("less
-parsimonious," as the math kids would say), which means that they may have more
-"wiggles" in their outputsâthis might be undesirable for gradient-based
-optimization. On the other hand, larger models will be able to capture a wider
-range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be
-seen mid-optimization), so larger models could have a benefit in that sense. If
-you try a specific application and have better/worse results with a specific
+with the ["large"](#overview) model and adjusting from there. In addition to
+accuracy vs. speed, another consideration when choosing the right model is what
+you're trying to use NeuralFoil for. Larger models will be more complicated
+("less parsimonious," as the math kids would say), which means that they may
+have more "wiggles" in their outputsâthis might be undesirable for gradient-
+based optimization. On the other hand, larger models will be able to capture a
+wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might
+be seen mid-optimization), so larger models could have a benefit in that sense.
+If you try a specific application and have better/worse results with a specific
 model, let me know by opening a GitHub issue! ## Extended Features (transonics,
 post-stall, control surface deflections) For more sophisticated airfoil
 aerodynamics calculations, consider using NeuralFoil via [AeroSandbox](https://
 github.com/peterdsharpe/AeroSandbox) (specifically, through
 [`asb.Airfoil.get_aero_from_neuralfoil()`](https://github.com/peterdsharpe/
 AeroSandbox/blob/8ad83aa4e4e40c503884c722143b7730c08089fa/aerosandbox/geometry/
 airfoil/airfoil.py#L607)). This provides several advanced features: *
-Compressible aerodynamics, including transonic and supersonic aerodynamics.
+**Compressible aerodynamics**, including transonic and supersonic aerodynamics.
 AeroSandbox will generally get the critical Mach number accurate to within $\pm
 0.01$ or so. Subsonic corrections done using a Laitone correction (a higher-
 order variant of Prandtl-Glauert and Karman-Tsien). Wave drag accuracy is, of
 course, less reliable beyond the drag-divergence Mach number, although it still
 [agrees reasonably closely when compared to RANS CFD](https://github.com/
 peterdsharpe/AeroSandbox/blob/master/studies/WingTransonics/
-compare_methods.py). * Post-stall (i.e., truly 360 degree range of $\alpha$)
-aerodynamics. This is useful for applications like wind turbine blades or
+compare_methods.py). * **Post-stall aerodynamics** (i.e., truly 360 degree
+range of $\alpha$). This is useful for applications like wind turbine blades or
 propeller roots, where the airfoil may be operating at high angles of attack. *
-Control surface deflections. Currently only trailing-edge control surface
+**Control surface deflections**. Currently only trailing-edge control surface
 deflections are supported in AeroSandbox's NeuralFoil interface. ##
 Installation [Install from PyPI](https://pypi.org/project/NeuralFoil/) with
 `pip install neuralfoil`.  To run models, NeuralFoil currently requires minimal
 dependencies: * Python 3.7+ * [NumPy](https://numpy.org/) * [AeroSandbox]
 (https://github.com/peterdsharpe/AeroSandbox) 4.0.10+ Currently, NeuralFoil
 only uses AeroSandbox for airfoil geometry parameterization (i.e., converting
 from a set of points to a CST parameterization, which is solved as an
 optimization problem)âthe actual math is implemented in pure NumPy. Recent
 progress on this CST parameterization-fitting problem has allowed it to be
 recast as a least-squares problem, which is potentially amenable to a pure-
 NumPy implementation. That being said, AeroSandbox provides a bunch of nice
 peripheral utilities (e.g., geometry manipulation, visualization, etc.), so
 it's a nice dependency to have anyway. However, if you'd like to work on a
 pure-NumPy implementation, open an issue and let me know! ## Geometry
-Parameterization and Training Data #### Geometry Parameterization To be
-written, but it's basically an 8-parameter-per-side CST (Kulfan)
+Parameterization and Training Data #### Geometry Parameterization  As a user,
+you can give an airfoil in many different formatsâfor example, as a set of $
+(x,y)$ coordinates, as a .dat file, or as an AeroSandbox `Airfoil` object.
+However, under the hood, NeuralFoil parameterizes the airfoil geometry using
+the CST (Kulfan) parameterization. (You can also directly pass in Kulfan
+parameters if preferred.) The airfoil shape fed into NeuralFoil's neural
+networks is in the form of an 8-parameter-per-side CST (Kulfan)
 parameterization, with Kulfan's added leading-edge-modification (LEM) and
 trailing-edge thickness parameter. This gives a total of (8 * 2 + 1 + 1) = 18
-parameters to describe a given airfoil shape. I'll write more here, but in the
-meantime read: - [D. A. Masters, "Geometric Comparison of Aerofoil Shape
-Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/
-10.2514/1.J054943) - The seminal paper on the CST (Kulfan) parameterization
-technique: [Brenda Kulfan, "Universal Parametric Geometry Representation
-Method"](http://mx1.brendakulfan.com/docs/CST6.pdf) #### Training Data To be
-written, but in the meantime [see here](https://github.com/peterdsharpe/
-NeuralFoil/tree/master/training_data). Training data is not (yet) uploaded to
-GitHub, but will be soon - need to figure out Git LFS, as it's many gigabytes.
-Contact me if you need it sooner. ## FAQs Will NeuralFoil be integrated
-directly into [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox)? >
-Yes, absolutely. However, the goal is to keep this NeuralFoil repository also
-available as a stand-alone module, if desired. This simplifies dependencies for
-people using NeuralFoil in other applications (e.g., flight simulation, real-
-time control on embedded systems, etc.), and makes it easier if someone wanted
-to port NeuralFoil to another language (e.g., C++, for use on an Arduino).  Why
-not just use XFoil directly? > XFoil is a truly excellent piece of aerospace
-software engineering and is the gold standard of airfoil analysis, for good
-reason. When its assumptions hold (airfoils in subsonic flow without massive
-separation), its accuracy exceeds that of RANS CFD, yet it has ~1000x lower
-computational cost. XFoil shines in particular for human-in-the-loop airfoil
-design. However, XFoil is not the right tool for all applications, for a few
-reasons: > > - XFoil exhibits hysteresis: you can get slightly different
-solutions (for the same airfoil, $\alpha$, and $Re$) depending on whether you
-sweep $\alpha$ up or down, as Newton iteration is resumed from the last
-converged solution and uniqueness is not guaranteed. This hysteresis can be a
-big problem for design optimization. > - XFoil is not differentiable, in the
-sense that it doesn't tell you how performance changes w.r.t. airfoil shape
-(via, for example, an adjoint). That's okayâNeuralFoil doesn't either, at
-least out-of-the-box. However, the "path to obtain an efficient gradient" is
-very straightforward for NeuralFoil's pure NumPy code, where many excellent
-options exist (e.g., JAX). In contrast, gradient options for Fortran code (the
-language XFoil is in) either don't exist or are significantly less advanced
-(e.g., Tapenade). The most promising option for XFoil is probably [CMPLXFOIL]
-(https://github.com/mdolab/CMPLXFOIL), which computes complex-step
-(effectively, forward-mode) gradients. However, even if you can get a gradient,
-it still may present issues, because... > - XFoil's solutions lack $C^1$-
-continuity. NeuralFoil, by contrast, is guaranteed to be $C^\infty$-continuous
-by construction. This is critical for gradient-based optimization. > - Even if
-one tries to compute gradients of XFoil's outputs by finite-differencing or
-complex-stepping, these gradients are often inaccurate. > - A bit into the
-weeds, but: this comes down to how XFoil handles transition (onset of
-turbulence). XFoil does a cut-cell approach on the transitioning interval, and
-while this specific cut-cell implementation restores $C^0$-continuity (i.e.,
-transition won't truly "jump" from one node to another discretely), gradients
-of the laminar and turbulent BL closure functions still change at the cell
-interface due to the differing BL parameters ($H$ and $Re_\theta$) from node to
-node. This loses $C^1$ continuity, causing a "ragged" polar at the microscopic
-level. In theory $C^1$-continuity could be restored by also blending the BL
-shape variables through the transitioning cell interval, but that unleashes
-some ugly integrals and is not done in XFoil. > - For more on this, see [Adler,
-Gray, and Martins, "To CFD or not to CFD?..."](http://websites.umich.edu/
-~mdolaboratory/pdf/Adler2022c.pdf), Figure 7. > - While XFoil is ~1000x faster
-than RANS CFD, NeuralFoil [can be another ~1000x faster to evaluate than XFoil]
-(#performance). NeuralFoil is also much easier to interface with on a memory
-level than XFoil, which means you won't find yourself I/O bound from file
-reading/writing like you will with XFoil. > - XFoil is not vectorized, which
-exacerbates the speed advantage of a (vectorized) neural network when analyzing
-large batches of airfoil cases simultaneously. > - XFoil is not guaranteed to
-produce a solution. Instead, XFoil often crashes when "ambitious" calculations
-are attempted, rather than producing a less-accurate answer. In some
-applications, that's okay or even desirable; in others, that's a deal-breaker.
-Example applications where this is a problem include: > - Real-time control,
-where one wants to estimate forces (e.g., for a MPC trajectory), but you can't
-have the controller crash if XFoil fails to converge or hangs the CPU. > -
-Flight simulation: similar to real-time control where "a less-accurate answer"
-is much better than "no answer." > - Design optimization, where the optimizer
-needs "an answer" in order to recover from a bad design point and send the
-search back to a reasonable design. > - XFoil can be a serious pain to compile
-from source, which is often required if running on Mac or Linux (i.e., all
-supercomputers, some lab computers). NeuralFoil is pure Python and NumPy, so
-it's easy to install and run anywhere. Why not use a neural network trained on
-RANS CFD instead? > This is a cool idea too, and it has been done (See
-[Bouhlel, He, and Martins, "Scalable gradient-enhanced artificial..."](https://
-link.springer.com/article/10.1007/s00158-020-02488-5))! The fundamental
-challenge here, of course, is the cost of training data. RANS CFD is much more
-expensive than XFoil, so it's much harder to get sufficient training data to
-build a neural network that will generalize well out-of-sample. For example, in
-the linked work by Bouhlel et al., the authors trained a neural network on
-42,000 RANS CFD runs (and they were sweeping over Mach as well, so the data
-becomes even sparser). In contrast, NeuralFoil was trained on tens of millions
-of XFoil runs. Ultimately, this exposes NeuralFoil to a much larger "span" of
-the airfoil design space, which is critical for accurate predictions on out-of-
+parameters to describe a given airfoil shape.
+              [./media/kulfan_parameterization_illustration.svg]
+For more details on this parameterization, or why it is a good choice, read: -
+[D. A. Masters, "Geometric Comparison of Aerofoil Shape Parameterization
+Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943)
+- The seminal paper on the CST (Kulfan) parameterization technique: [Brenda
+Kulfan, "Universal Parametric Geometry Representation Method"](http://
+mx1.brendakulfan.com/docs/CST6.pdf) To convert between airfoil coordinates and
+the CST parameterization, use the following functions: ```python from
+aerosandbox.geometry.airfoil.airfoil_families import get_kulfan_parameters,
+get_kulfan_coordinates ``` with documentation [here](https://
+aerosandbox.readthedocs.io/en/master/autoapi/aerosandbox/geometry/airfoil/
+airfoil_families/index.html) or in the source ([here](https://github.com/
+peterdsharpe/AeroSandbox/blob/8ad83aa4e4e40c503884c722143b7730c08089fa/
+aerosandbox/geometry/airfoil/airfoil_families.py#L128), [here](https://
+github.com/peterdsharpe/AeroSandbox/blob/
+8ad83aa4e4e40c503884c722143b7730c08089fa/aerosandbox/geometry/airfoil/
+airfoil_families.py#L265)). #### Training Data To be written, but in the
+meantime [see here](https://github.com/peterdsharpe/NeuralFoil/tree/master/
+training_data). Training data is not (yet) uploaded to GitHub, but will be soon
+- need to figure out Git LFS, as it's many gigabytes. Contact me if you need it
+sooner. ## FAQs Will NeuralFoil be integrated directly into [AeroSandbox]
+(https://github.com/peterdsharpe/AeroSandbox)? > Yes, absolutely. However, the
+goal is to keep this NeuralFoil repository also available as a stand-alone
+module, if desired. This simplifies dependencies for people using NeuralFoil in
+other applications (e.g., flight simulation, real-time control on embedded
+systems, etc.), and makes it easier if someone wanted to port NeuralFoil to
+another language (e.g., C++, for use on an Arduino).  Why not just use XFoil
+directly? > XFoil is a truly excellent piece of aerospace software engineering
+and is the gold standard of airfoil analysis, for good reason. When its
+assumptions hold (airfoils in subsonic flow without massive separation), its
+accuracy exceeds that of RANS CFD, yet it has ~1000x lower computational cost.
+XFoil shines in particular for human-in-the-loop airfoil design. However, XFoil
+is not the right tool for all applications, for a few reasons: > > - XFoil
+exhibits hysteresis: you can get slightly different solutions (for the same
+airfoil, $\alpha$, and $Re$) depending on whether you sweep $\alpha$ up or
+down, as Newton iteration is resumed from the last converged solution and
+uniqueness is not guaranteed. This hysteresis can be a big problem for design
+optimization. > - XFoil is not differentiable, in the sense that it doesn't
+tell you how performance changes w.r.t. airfoil shape (via, for example, an
+adjoint). That's okayâNeuralFoil doesn't either, at least out-of-the-box.
+However, the "path to obtain an efficient gradient" is very straightforward for
+NeuralFoil's pure NumPy code, where many excellent options exist (e.g., JAX).
+In contrast, gradient options for Fortran code (the language XFoil is in)
+either don't exist or are significantly less advanced (e.g., Tapenade). The
+most promising option for XFoil is probably [CMPLXFOIL](https://github.com/
+mdolab/CMPLXFOIL), which computes complex-step (effectively, forward-mode)
+gradients. However, even if you can get a gradient, it still may present
+issues, because... > - XFoil's solutions lack $C^1$-continuity. NeuralFoil, by
+contrast, is guaranteed to be $C^\infty$-continuous by construction. This is
+critical for gradient-based optimization. > - Even if one tries to compute
+gradients of XFoil's outputs by finite-differencing or complex-stepping, these
+gradients are often inaccurate. > - A bit into the weeds, but: this comes down
+to how XFoil handles transition (onset of turbulence). XFoil does a cut-cell
+approach on the transitioning interval, and while this specific cut-cell
+implementation restores $C^0$-continuity (i.e., transition won't truly "jump"
+from one node to another discretely), gradients of the laminar and turbulent BL
+closure functions still change at the cell interface due to the differing BL
+parameters ($H$ and $Re_\theta$) from node to node. This loses $C^1$
+continuity, causing a "ragged" polar at the microscopic level. In theory $C^1$-
+continuity could be restored by also blending the BL shape variables through
+the transitioning cell interval, but that unleashes some ugly integrals and is
+not done in XFoil. > - For more on this, see [Adler, Gray, and Martins, "To CFD
+or not to CFD?..."](http://websites.umich.edu/~mdolaboratory/pdf/
+Adler2022c.pdf), Figure 7. > - While XFoil is ~1000x faster than RANS CFD,
+NeuralFoil [can be another ~1000x faster to evaluate than XFoil](#performance).
+NeuralFoil is also much easier to interface with on a memory level than XFoil,
+which means you won't find yourself I/O bound from file reading/writing like
+you will with XFoil. > - XFoil is not vectorized, which exacerbates the speed
+advantage of a (vectorized) neural network when analyzing large batches of
+airfoil cases simultaneously. > - XFoil is not guaranteed to produce a
+solution. Instead, XFoil often crashes when "ambitious" calculations are
+attempted, rather than producing a less-accurate answer. In some applications,
+that's okay or even desirable; in others, that's a deal-breaker. Example
+applications where this is a problem include: > - Real-time control, where one
+wants to estimate forces (e.g., for a MPC trajectory), but you can't have the
+controller crash if XFoil fails to converge or hangs the CPU. > - Flight
+simulation: similar to real-time control where "a less-accurate answer" is much
+better than "no answer." > - Design optimization, where the optimizer needs "an
+answer" in order to recover from a bad design point and send the search back to
+a reasonable design. > - XFoil can be a serious pain to compile from source,
+which is often required if running on Mac or Linux (i.e., all supercomputers,
+some lab computers). NeuralFoil is pure Python and NumPy, so it's easy to
+install and run anywhere. Why not use a neural network trained on RANS CFD
+instead? > This is a cool idea too, and it has been done (See [Bouhlel, He, and
+Martins, "Scalable gradient-enhanced artificial..."](https://link.springer.com/
+article/10.1007/s00158-020-02488-5))! The fundamental challenge here, of
+course, is the cost of training data. RANS CFD is much more expensive than
+XFoil, so it's much harder to get sufficient training data to build a neural
+network that will generalize well out-of-sample. For example, in the linked
+work by Bouhlel et al., the authors trained a neural network on 42,000 RANS CFD
+runs (and they were sweeping over Mach as well, so the data becomes even
+sparser). In contrast, NeuralFoil was trained on tens of millions of XFoil
+runs. Ultimately, this exposes NeuralFoil to a much larger "span" of the
+airfoil design space, which is critical for accurate predictions on out-of-
 sample airfoils. > > One advantage of a RANS CFD approach over the NeuralFoil
 XFoil approach is, of course, transonic modeling. NeuralFoil attempts to get
 around this a little bit by estimating $C_{p, min}$, which in turn allows you
 to estimate the critical Mach number. (For an implementation of that, [see
 here](#extended-features-transonics-post-stall-control-surface-deflections))
 But fundamentally, NeuralFoil is likely less accurate in the transonic range
 because of this. The tradeoff is that the much larger training data set allows
@@ -273,38 +290,28 @@
 usually more accurate than RANS CFD](https://www.sciencedirect.com/science/
 article/abs/pii/S1270963816300839). Why not use a neural network trained on
 wind tunnel data? > This is a super-cool idea, and I'd love to see someone try
 it! My guess is that you'd need some kind of morphing wing section (and a way
 of precisely measuring the shape) in order to get enough data samples to "span"
 the airfoil design space. Then, you'd just let the wing section sit in the wind
 tunnel for a few days morphing itself around to collect data, then train a
-model on that. This would be really awesome, someone should do it!  Why
-parameterize the airfoil geometry using the CST (Kulfan) parameterization? What
-exactly does the CST parameterization mean, and how can I convert this
-parameterization to/from actual airfoil coordinates? Why discretize with 8 CST
-modes per side? Can NeuralFoil accurately analyze airfoils with thick trailing
-edges? > To be written, but in the meantime read: > - [D. A. Masters,
-"Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA
-Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943) > - The seminal
-paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan,
-"Universal Parametric Geometry Representation Method"](http://
-mx1.brendakulfan.com/docs/CST6.pdf) What's the underlying neural network
-architecture used in NeuralFoil? > To be written, but it is essentially a feed-
-forward neural network with a varying number of total layers and layer width
-depending on model size. Layer counts and widths were [determined through
-extensive trial and error](./training/supercloud_job_id_notes.log), in
-conjunction with observed test- and train-loss values. All layers are dense
-(fully connected, with weights and biases). All activation functions between
-layers are $\tanh$, to preserve $C^\infty$-continuity. The number of layers and
-layer width are as follows: > > * xxsmall: 2 layers, 32 wide. > * xsmall: 3
-layers, 32 wide. > * small: 3 layers, 48 wide. > * medium: 4 layers, 64 wide. >
-* large: 4 layers, 128 wide. > * xlarge: 4 layers, 256 wide. > * xxlarge: 5
-layers, 256 wide. > * xxxlarge:5 layers, 512 wide. ## Acknowledgements
-NeuralFoil was trained on MIT Supercloud, a high-performance computing cluster
-operated by the MIT Lincoln Laboratory Supercomputing Center (LLSC). ## License
-NeuralFoil is licensed under the MIT license. Please see the [LICENSE]
-(LICENSE.txt) file for details. ## Citing NeuralFoil If you use NeuralFoil in
-your research, please cite it as follows: ``` @misc{neuralfoil, author = {Peter
-Sharpe}, title = {{NeuralFoil}: An airfoil aerodynamics analysis tool using
-physics-informed machine learning}, year = {2023}, publisher = {GitHub},
-journal = {GitHub repository}, howpublished = {\url{https://github.com/
-peterdsharpe/NeuralFoil}}, ```
+model on that. This would be really awesome, someone should do it! What's the
+underlying neural network architecture used in NeuralFoil? > To be written, but
+it is essentially a feed-forward neural network with a varying number of total
+layers and layer width depending on model size. Layer counts and widths were
+[determined through extensive trial and error](./training/
+supercloud_job_id_notes.log), in conjunction with observed test- and train-loss
+values. All layers are dense (fully connected, with weights and biases). All
+activation functions between layers are $\tanh$, to preserve $C^\infty$-
+continuity. The number of layers and layer width are as follows: > > * xxsmall:
+2 layers, 32 wide. > * xsmall: 3 layers, 32 wide. > * small: 3 layers, 48 wide.
+> * medium: 4 layers, 64 wide. > * large: 4 layers, 128 wide. > * xlarge: 4
+layers, 256 wide. > * xxlarge: 5 layers, 256 wide. > * xxxlarge:5 layers, 512
+wide. ## Acknowledgements NeuralFoil was trained on MIT Supercloud, a high-
+performance computing cluster operated by the MIT Lincoln Laboratory
+Supercomputing Center (LLSC). ## License NeuralFoil is licensed under the MIT
+license. Please see the [LICENSE](LICENSE.txt) file for details. ## Citing
+NeuralFoil If you use NeuralFoil in your research, please cite it as follows:
+``` @misc{neuralfoil, author = {Peter Sharpe}, title = {{NeuralFoil}: An
+airfoil aerodynamics analysis tool using physics-informed machine learning},
+year = {2023}, publisher = {GitHub}, journal = {GitHub repository},
+howpublished = {\url{https://github.com/peterdsharpe/NeuralFoil}}, } ```
```

### Comparing `NeuralFoil-0.1.7/NeuralFoil.egg-info/SOURCES.txt` & `NeuralFoil-0.1.8/NeuralFoil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.7/PKG-INFO` & `NeuralFoil-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuralFoil
-Version: 0.1.7
+Version: 0.1.8
 Summary: NeuralFoil is an airfoil aerodynamics analysis tool using physics-informed machine learning, in pure Python/NumPy.
 Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe
 Author-email: pds@mit.edu
 Project-URL: Source, https://github.com/peterdsharpe/NeuralFoil
 Project-URL: Bug Reports, https://github.com/peterdsharpe/NeuralFoil/issues
 Keywords: python machine learning analysis optimization aerospace airplane cfd aircraft hydrodynamics aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed neural network
@@ -22,29 +22,28 @@
 
 <p align="center">
     <img src="./media/neuralfoil_logo.svg" width="800" />
 </p>
 
 by [Peter Sharpe](https://peterdsharpe.github.io) (<pds [at] mit [dot] edu>)
 
-
-[!![PyPI](https://img.shields.io/pypi/v/neuralfoil)
-](https://pypi.org/project/NeuralFoil/)
+[![PyPI](https://img.shields.io/pypi/v/neuralfoil)](https://pypi.org/project/NeuralFoil/)
 [![Build Status](https://github.com/peterdsharpe/NeuralFoil/workflows/Tests/badge.svg)](https://github.com/peterdsharpe/NeuralFoil/actions/workflows/run-pytest.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-g.svg)](https://opensource.org/licenses/MIT)
 
 -----
 
 NeuralFoil is a tool for rapid aerodynamics analysis of airfoils, similar to [XFoil](https://web.mit.edu/drela/Public/web/xfoil/). Under the hood, NeuralFoil consists of physics-informed neural networks trained on [tens of millions of XFoil runs](#geometry-parameterization-and-training-data).
 
-NeuralFoil is available here as a pure Python+NumPy standalone, but it is also [available within AeroSandbox](#extended-features-transonics-post-stall-control-surface-deflections), which extends it with many more advanced features. Using the AeroSandbox extension, NeuralFoil can give you **viscous, compressible airfoil aerodynamics for (nearly) any airfoil, with control surface deflections, across $360^\circ$ angle of attack, at any Reynolds number, all nearly instantly** (~5 milliseconds). And, it's guaranteed to return an answer (no non-convergence issues), it's vectorized, and it's $C^1$-continuous (all very useful for gradient-based optimization). 
+NeuralFoil is available here as a pure Python+NumPy standalone, but it is also [available within AeroSandbox](#extended-features-transonics-post-stall-control-surface-deflections), which extends it with many more advanced features. Using the AeroSandbox extension, NeuralFoil can give you **viscous, compressible airfoil aerodynamics for (nearly) any airfoil, with control surface deflections, across $360^\circ$ angle of attack, at any Reynolds number, all nearly instantly** (~5 milliseconds). And, it's guaranteed to return an answer (no non-convergence issues), it's vectorized, and it's $C^1$-continuous (all very useful for gradient-based optimization).
 
 NeuralFoil is [~10x faster than XFoil for a single analysis, and ~1000x faster for multipoint analysis](#table), all with [minimal loss in accuracy compared to XFoil](#performance). Due to the wide variety of training data and the embedding of several physics-based invariants, [this accuracy is seen even on out-of-sample airfoils](#performance) (i.e., airfoils it wasn't trained on). It also has [many nice features](#xfoil-benefit-question) (e.g., smoothness, vectorization, all in Python+NumPy) that make it much easier to use.
 
- NeuralFoil aims to be lightweight, with [minimal dependencies](#dependencies-question) and a [tight, efficient, and easily-understood code-base](./neuralfoil) (less than 500 lines of user-facing code).
+NeuralFoil aims to be lightweight, with [minimal dependencies](#dependencies-question) and a [tight, efficient, and easily-understood code-base](./neuralfoil) (less than 500 lines of user-facing code).
+
 ```
 pip install neuralfoil
 ```
 
 ## Overview
 
 NeuralFoil comes with 8 different neural network models, with increasing levels of complexity:
@@ -62,15 +61,15 @@
 		<td>"xxxlarge"</td>
 	 </tr>
 	</table>
 </div>
 
 This spectrum offers a tradeoff between accuracy and computational cost.
 
-In addition to its neural network models, NeuralFoil also has a bonus "Linear $C_L$ model" that predicts lift coefficient $C_L$ as a purely-linear function of angle of attack $\alpha$. This model is well-suited for linear lifting-line or blade-element-method analyses, where the $C_L(\alpha)$ linearity can be used to solve the resulting system of equations "in one shot" as a linear solve, rather than a less-numerically-robust iterative nonlinear solve.
+In addition to its neural network models, NeuralFoil also has a bonus "Linear $C_L$ model" that predicts lift coefficient $C_L$ as a purely-affine function of angle of attack $\alpha$. This model is well-suited for linear lifting-line or blade-element-method analyses, where the $C_L(\alpha)$ linearity can be used to solve the resulting system of equations "in one shot" as a linear solve, rather than a less-numerically-robust iterative nonlinear solve.
 
 Using NeuralFoil is dead-simple, and also offers several possible "entry points" for inputs. Here's an example showing this:
 
 ```python
 import neuralfoil as nf  # `pip install neuralfoil`
 import numpy as np
 
@@ -93,24 +92,24 @@
 )
 
 # `aero` is a dictionary with keys: ["CL", "CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"]
 ```
 
 ## Performance
 
-Qualitatively, NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$ values. In the figure below, we compare the performance of NeuralFoil to XFoil on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was developed "from scratch" for a [real-world aircraft development program](https://www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-research-aircraft-301633713.html) and is completely separate from [the airfoils used during NeuralFoil's training](#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance: 
+Qualitatively, NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$ values. In the figure below, we compare the performance of NeuralFoil to XFoil on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was developed "from scratch" for a [real-world aircraft development program](https://www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-research-aircraft-301633713.html) and is completely separate from [the airfoils used during NeuralFoil's training](#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance:
 
 <a name="clcd-polar"></a>
 <p align="center">
 	<img src="./benchmarking/neuralfoil_point_validation.svg" width="1000" />
 </p>
 
-NeuralFoil is typically accurate to within a few percent of XFoil's predictions. Note that this figure is on a truly out-of-sample airfoil, so airfoils that are closer to the training set will have even more accurate results. 
+NeuralFoil is typically accurate to within a few percent of XFoil's predictions. Note that this figure is on a truly out-of-sample airfoil, so airfoils that are closer to the training set will have even more accurate results.
 
-NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is not reliably converging, which would otherwise make optimization difficult. 
+NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is not reliably converging, which would otherwise make optimization difficult.
 
 In the table below, we quantify the performance of the NeuralFoil ("NF") models with respect to XFoil more precisely. At a basic level, we care about two things:
 
 - **Accuracy**: how close are the predictions to XFoil's?
 - **Computational Cost**: how long does it take to run?
 
 This table details both of these considerations. The first few columns show the error with respect to XFoil on the test dataset. [The test dataset is completely isolated from the training dataset, and NeuralFoil was not allowed to learn from the test dataset](#geometry-parameterization-and-training-data). Thus, the performance on the test dataset gives a good idea of NeuralFoil's performance "in the wild". The second set of columns gives the runtime speed of the models, both for a single analysis and for a large batch analysis.
@@ -119,25 +118,25 @@
 
 <table><thead><tr><th>Aerodynamics Model</th><th colspan="6">Mean Absolute Error (MAE) of Given Metric, on the Test Dataset, with respect to XFoil</th><th colspan="2">Computational Cost to Run</th></tr></thead><tbody><tr><td></td><td>Lift Coeff.<br>$C_L$</td><td>Fractional Drag Coeff.<br>$\ln(C_D)$   †</td><td>Moment Coeff.<br>$C_M$</td><td>Max Overspeed<br>$u_\max / u_\infty$&nbsp;&nbsp;&nbsp;‡</td><td>Top Transition Loc.<br>$x_{tr, top}/c$</td><td>Bottom Trans. Loc.<br>$x_{tr, bot}/c$</td><td>Runtime<br>(1 run)</td><td>Total Runtime<br>(100,000 runs)</td></tr><tr><td>NF Linear $C_L$ Model</td><td>0.116</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>1 ms</td><td>0.020 sec</td></tr><tr><td>NF "xxsmall"</td><td>0.065</td><td>0.121</td><td>0.010</td><td>0.215</td><td>0.073</td><td>0.100</td><td>3 ms</td><td>0.190 sec</td></tr><tr><td>NF "xsmall"</td><td>0.042</td><td>0.075</td><td>0.007</td><td>0.134</td><td>0.039</td><td>0.055</td><td>4 ms</td><td>0.284 sec</td></tr><tr><td>NF "small"</td><td>0.039</td><td>0.069</td><td>0.006</td><td>0.122</td><td>0.036</td><td>0.050</td><td>4 ms</td><td>0.402 sec</td></tr><tr><td>NF "medium"</td><td>0.027</td><td>0.051</td><td>0.004</td><td>0.088</td><td>0.022</td><td>0.033</td><td>5 ms</td><td>0.784 sec</td></tr><tr><td>NF "large"</td><td>0.024</td><td>0.045</td><td>0.004</td><td>0.079</td><td>0.020</td><td>0.029</td><td>6 ms</td><td>1.754 sec</td></tr><tr><td>NF "xlarge"</td><td>0.023</td><td>0.043</td><td>0.004</td><td>0.076</td><td>0.019</td><td>0.028</td><td>10 ms</td><td>3.330 sec</td></tr><tr><td>NF "xxlarge"</td><td>0.021</td><td>0.040</td><td>0.003</td><td>0.071</td><td>0.018</td><td>0.025</td><td>13 ms</td><td>4.297 sec</td></tr><tr><td>NF "xxxlarge"</td><td>0.020</td><td>0.039</td><td>0.003</td><td>0.070</td><td>0.016</td><td>0.024</td><td>38 ms</td><td>8.980 sec</td></tr><tr><td>XFoil</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>73 ms</td><td>42 min</td></tr></tbody></table>
 
 > † The deviation of $\ln(C_D)$ can be thought of as "the typical relative error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm) of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil is *less* accurate than XFoil - although XFoil is quite accurate, it is clearly not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure above](#clcd-polar)). So, NeuralFoil's true accuracy compared to experiment may differ (in either direction) from the numbers in this table.
 > 
 > ‡ This "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm{crit}$. [More details below.](#extended-features-transonics-post-stall-control-surface-deflections)
 
-Based on these performance numbers, you can select the right tradeoff between accuracy and computational cost for your application. In general, I recommend starting with the "large" model and adjusting from there.
+Based on these performance numbers, you can select the right tradeoff between accuracy and computational cost for your application. In general, I recommend starting with the ["large"](#overview) model and adjusting from there.
 
 In addition to accuracy vs. speed, another consideration when choosing the right model is what you're trying to use NeuralFoil for. Larger models will be more complicated ("less parsimonious," as the math kids would say), which means that they may have more "wiggles" in their outputs—this might be undesirable for gradient-based optimization. On the other hand, larger models will be able to capture a wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-optimization), so larger models could have a benefit in that sense. If you try a specific application and have better/worse results with a specific model, let me know by opening a GitHub issue!
 
 ## Extended Features (transonics, post-stall, control surface deflections)
 
 For more sophisticated airfoil aerodynamics calculations, consider using NeuralFoil via [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) (specifically, through [`asb.Airfoil.get_aero_from_neuralfoil()`](https://github.com/peterdsharpe/AeroSandbox/blob/8ad83aa4e4e40c503884c722143b7730c08089fa/aerosandbox/geometry/airfoil/airfoil.py#L607)). This provides several advanced features:
 
-* Compressible aerodynamics, including transonic and supersonic aerodynamics. AeroSandbox will generally get the critical Mach number accurate to within $\pm 0.01$ or so. Subsonic corrections done using a Laitone correction (a higher-order variant of Prandtl-Glauert and Karman-Tsien). Wave drag accuracy is, of course, less reliable beyond the drag-divergence Mach number, although it still [agrees reasonably closely when compared to RANS CFD](https://github.com/peterdsharpe/AeroSandbox/blob/master/studies/WingTransonics/compare_methods.py).
-* Post-stall (i.e., truly 360 degree range of $\alpha$) aerodynamics. This is useful for applications like wind turbine blades or propeller roots, where the airfoil may be operating at high angles of attack.
-* Control surface deflections. Currently only trailing-edge control surface deflections are supported in AeroSandbox's NeuralFoil interface.
+* **Compressible aerodynamics**, including transonic and supersonic aerodynamics. AeroSandbox will generally get the critical Mach number accurate to within $\pm 0.01$ or so. Subsonic corrections done using a Laitone correction (a higher-order variant of Prandtl-Glauert and Karman-Tsien). Wave drag accuracy is, of course, less reliable beyond the drag-divergence Mach number, although it still [agrees reasonably closely when compared to RANS CFD](https://github.com/peterdsharpe/AeroSandbox/blob/master/studies/WingTransonics/compare_methods.py).
+* **Post-stall aerodynamics** (i.e., truly 360 degree range of $\alpha$). This is useful for applications like wind turbine blades or propeller roots, where the airfoil may be operating at high angles of attack.
+* **Control surface deflections**. Currently only trailing-edge control surface deflections are supported in AeroSandbox's NeuralFoil interface.
 
 ## Installation
 
 [Install from PyPI](https://pypi.org/project/NeuralFoil/) with `pip install neuralfoil`.
 
 <a name="dependencies-question"></a>
 To run models, NeuralFoil currently requires minimal dependencies:
@@ -148,18 +147,37 @@
 
 Currently, NeuralFoil only uses AeroSandbox for airfoil geometry parameterization (i.e., converting from a set of points to a CST parameterization, which is solved as an optimization problem)—the actual math is implemented in pure NumPy. Recent progress on this CST parameterization-fitting problem has allowed it to be recast as a least-squares problem, which is potentially amenable to a pure-NumPy implementation. That being said, AeroSandbox provides a bunch of nice peripheral utilities (e.g., geometry manipulation, visualization, etc.), so it's a nice dependency to have anyway. However, if you'd like to work on a pure-NumPy implementation, open an issue and let me know!
 
 ## Geometry Parameterization and Training Data
 
 #### Geometry Parameterization
 
-To be written, but it's basically an 8-parameter-per-side CST (Kulfan) parameterization, with Kulfan's added leading-edge-modification (LEM) and trailing-edge thickness parameter. This gives a total of (8 * 2 + 1 + 1) = 18 parameters to describe a given airfoil shape. I'll write more here, but in the meantime read:
+<a name="parameterization-question"></a>
+
+As a user, you can give an airfoil in many different formats—for example, as a set of $(x,y)$ coordinates, as a .dat file, or as an AeroSandbox `Airfoil` object. However, under the hood, NeuralFoil parameterizes the airfoil geometry using the CST (Kulfan) parameterization. (You can also directly pass in Kulfan parameters if preferred.)
+
+The airfoil shape fed into NeuralFoil's neural networks is in the form of an 8-parameter-per-side CST (Kulfan) parameterization, with Kulfan's added leading-edge-modification (LEM) and trailing-edge thickness parameter. This gives a total of (8 * 2 + 1 + 1) = 18 parameters to describe a given airfoil shape.
+
+<p align="center">
+	<img src="./media/kulfan_parameterization_illustration.svg" width="1000" />
+</p>
+
+For more details on this parameterization, or why it is a good choice, read:
+
 - [D. A. Masters, "Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943)
 - The seminal paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan, "Universal Parametric Geometry Representation Method"](http://mx1.brendakulfan.com/docs/CST6.pdf)
 
+To convert between airfoil coordinates and the CST parameterization, use the following functions:
+
+```python
+from aerosandbox.geometry.airfoil.airfoil_families import get_kulfan_parameters, get_kulfan_coordinates
+```
+
+with documentation [here](https://aerosandbox.readthedocs.io/en/master/autoapi/aerosandbox/geometry/airfoil/airfoil_families/index.html) or in the source ([here](https://github.com/peterdsharpe/AeroSandbox/blob/8ad83aa4e4e40c503884c722143b7730c08089fa/aerosandbox/geometry/airfoil/airfoil_families.py#L128), [here](https://github.com/peterdsharpe/AeroSandbox/blob/8ad83aa4e4e40c503884c722143b7730c08089fa/aerosandbox/geometry/airfoil/airfoil_families.py#L265)).
+
 #### Training Data
 
 To be written, but in the meantime [see here](https://github.com/peterdsharpe/NeuralFoil/tree/master/training_data). Training data is not (yet) uploaded to GitHub, but will be soon - need to figure out Git LFS, as it's many gigabytes. Contact me if you need it sooner.
 
 ## FAQs
 
 Will NeuralFoil be integrated directly into [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox)?
@@ -191,22 +209,14 @@
 >
 > One advantage of a RANS CFD approach over the NeuralFoil XFoil approach is, of course, transonic modeling. NeuralFoil attempts to get around this a little bit by estimating $C_{p, min}$, which in turn allows you to estimate the critical Mach number. (For an implementation of that, [see here](#extended-features-transonics-post-stall-control-surface-deflections)) But fundamentally, NeuralFoil is likely less accurate in the transonic range because of this. The tradeoff is that the much larger training data set allows NeuralFoil to be more accurate in the subsonic range, where [XFoil is actually usually more accurate than RANS CFD](https://www.sciencedirect.com/science/article/abs/pii/S1270963816300839).
 
 Why not use a neural network trained on wind tunnel data?
 
 > This is a super-cool idea, and I'd love to see someone try it! My guess is that you'd need some kind of morphing wing section (and a way of precisely measuring the shape) in order to get enough data samples to "span" the airfoil design space. Then, you'd just let the wing section sit in the wind tunnel for a few days morphing itself around to collect data, then train a model on that. This would be really awesome, someone should do it!
 
-
-<a name="parameterization-question"></a>
-Why parameterize the airfoil geometry using the CST (Kulfan) parameterization? What exactly does the CST parameterization mean, and how can I convert this parameterization to/from actual airfoil coordinates? Why discretize with 8 CST modes per side? Can NeuralFoil accurately analyze airfoils with thick trailing edges?
-
-> To be written, but in the meantime read:
-> - [D. A. Masters, "Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943)
-> - The seminal paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan, "Universal Parametric Geometry Representation Method"](http://mx1.brendakulfan.com/docs/CST6.pdf)
-
 What's the underlying neural network architecture used in NeuralFoil?
 
 > To be written, but it is essentially a feed-forward neural network with a varying number of total layers and layer width depending on model size. Layer counts and widths were [determined through extensive trial and error](./training/supercloud_job_id_notes.log), in conjunction with observed test- and train-loss values. All layers are dense (fully connected, with weights and biases). All activation functions between layers are $\tanh$, to preserve $C^\infty$-continuity. The number of layers and layer width are as follows:
 >
 > * xxsmall: 2 layers,  32 wide.
 > * xsmall:  3 layers,  32 wide.
 > * small:   3 layers,  48 wide.
@@ -214,15 +224,15 @@
 > * large:   4 layers, 128 wide.
 > * xlarge:  4 layers, 256 wide.
 > * xxlarge: 5 layers, 256 wide.
 > * xxxlarge:5 layers, 512 wide.
 
 ## Acknowledgements
 
-NeuralFoil was trained on MIT Supercloud, a high-performance computing cluster operated by the MIT Lincoln Laboratory Supercomputing Center (LLSC). 
+NeuralFoil was trained on MIT Supercloud, a high-performance computing cluster operated by the MIT Lincoln Laboratory Supercomputing Center (LLSC).
 
 ## License
 
 NeuralFoil is licensed under the MIT license. Please see the [LICENSE](LICENSE.txt) file for details.
 
 ## Citing NeuralFoil
 
@@ -232,8 +242,9 @@
 @misc{neuralfoil,
   author = {Peter Sharpe},
   title = {{NeuralFoil}: An airfoil aerodynamics analysis tool using physics-informed machine learning},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/peterdsharpe/NeuralFoil}},
+}
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.7 Summary: NeuralFoil is an
+Metadata-Version: 2.1 Name: NeuralFoil Version: 0.1.8 Summary: NeuralFoil is an
 airfoil aerodynamics analysis tool using physics-informed machine learning, in
 pure Python/NumPy. Home-page: https://github.com/peterdsharpe/NeuralFoil
 Author: Peter Sharpe Author-email: pds@mit.edu Project-URL: Source, https://
 github.com/peterdsharpe/NeuralFoil Project-URL: Bug Reports, https://
 github.com/peterdsharpe/NeuralFoil/issues Keywords: python machine learning
 analysis optimization aerospace airplane cfd aircraft hydrodynamics
 aerodynamics sailing propeller airfoil xfoil design mdo mdao physics informed
@@ -10,16 +10,16 @@
 Classifier: Intended Audience :: Science/Research Classifier: Topic ::
 Scientific/Engineering :: Physics Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.7
 Description-Content-Type: text/markdown Provides-Extra: training Provides-
 Extra: test Provides-Extra: docs License-File: LICENSE.txt
                          [./media/neuralfoil_logo.svg]
 by [Peter Sharpe](https://peterdsharpe.github.io) (
-at] mit [dot] edu>) [!![PyPI](https://img.shields.io/pypi/v/neuralfoil) ]
-(https://pypi.org/project/NeuralFoil/) [![Build Status](https://github.com/
+at] mit [dot] edu>) [![PyPI](https://img.shields.io/pypi/v/neuralfoil)](https:/
+/pypi.org/project/NeuralFoil/) [![Build Status](https://github.com/
 peterdsharpe/NeuralFoil/workflows/Tests/badge.svg)](https://github.com/
 peterdsharpe/NeuralFoil/actions/workflows/run-pytest.yml) [![License: MIT]
 (https://img.shields.io/badge/License-MIT-g.svg)](https://opensource.org/
 licenses/MIT) ----- NeuralFoil is a tool for rapid aerodynamics analysis of
 airfoils, similar to [XFoil](https://web.mit.edu/drela/Public/web/xfoil/).
 Under the hood, NeuralFoil consists of physics-informed neural networks trained
 on [tens of millions of XFoil runs](#geometry-parameterization-and-training-
@@ -43,15 +43,15 @@
 efficient, and easily-understood code-base](./neuralfoil) (less than 500 lines
 of user-facing code). ``` pip install neuralfoil ``` ## Overview NeuralFoil
 comes with 8 different neural network models, with increasing levels of
 complexity:
    "xxsmall" "xsmall" "small" "medium" "large" "xlarge" "xxlarge" "xxxlarge"
 This spectrum offers a tradeoff between accuracy and computational cost. In
 addition to its neural network models, NeuralFoil also has a bonus "Linear
-$C_L$ model" that predicts lift coefficient $C_L$ as a purely-linear function
+$C_L$ model" that predicts lift coefficient $C_L$ as a purely-affine function
 of angle of attack $\alpha$. This model is well-suited for linear lifting-line
 or blade-element-method analyses, where the $C_L(\alpha)$ linearity can be used
 to solve the resulting system of equations "in one shot" as a linear solve,
 rather than a less-numerically-robust iterative nonlinear solve. Using
 NeuralFoil is dead-simple, and also offers several possible "entry points" for
 inputs. Here's an example showing this: ```python import neuralfoil as nf #
 `pip install neuralfoil` import numpy as np aero = nf.get_aero_from_dat_file( #
@@ -130,142 +130,159 @@
 above](#clcd-polar)). So, NeuralFoil's true accuracy compared to experiment may
 differ (in either direction) from the numbers in this table. > > â¡ This
 "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to
 calculate the critical Mach number $M_\mathrm{crit}$. [More details below.]
 (#extended-features-transonics-post-stall-control-surface-deflections) Based on
 these performance numbers, you can select the right tradeoff between accuracy
 and computational cost for your application. In general, I recommend starting
-with the "large" model and adjusting from there. In addition to accuracy vs.
-speed, another consideration when choosing the right model is what you're
-trying to use NeuralFoil for. Larger models will be more complicated ("less
-parsimonious," as the math kids would say), which means that they may have more
-"wiggles" in their outputsâthis might be undesirable for gradient-based
-optimization. On the other hand, larger models will be able to capture a wider
-range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be
-seen mid-optimization), so larger models could have a benefit in that sense. If
-you try a specific application and have better/worse results with a specific
+with the ["large"](#overview) model and adjusting from there. In addition to
+accuracy vs. speed, another consideration when choosing the right model is what
+you're trying to use NeuralFoil for. Larger models will be more complicated
+("less parsimonious," as the math kids would say), which means that they may
+have more "wiggles" in their outputsâthis might be undesirable for gradient-
+based optimization. On the other hand, larger models will be able to capture a
+wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might
+be seen mid-optimization), so larger models could have a benefit in that sense.
+If you try a specific application and have better/worse results with a specific
 model, let me know by opening a GitHub issue! ## Extended Features (transonics,
 post-stall, control surface deflections) For more sophisticated airfoil
 aerodynamics calculations, consider using NeuralFoil via [AeroSandbox](https://
 github.com/peterdsharpe/AeroSandbox) (specifically, through
 [`asb.Airfoil.get_aero_from_neuralfoil()`](https://github.com/peterdsharpe/
 AeroSandbox/blob/8ad83aa4e4e40c503884c722143b7730c08089fa/aerosandbox/geometry/
 airfoil/airfoil.py#L607)). This provides several advanced features: *
-Compressible aerodynamics, including transonic and supersonic aerodynamics.
+**Compressible aerodynamics**, including transonic and supersonic aerodynamics.
 AeroSandbox will generally get the critical Mach number accurate to within $\pm
 0.01$ or so. Subsonic corrections done using a Laitone correction (a higher-
 order variant of Prandtl-Glauert and Karman-Tsien). Wave drag accuracy is, of
 course, less reliable beyond the drag-divergence Mach number, although it still
 [agrees reasonably closely when compared to RANS CFD](https://github.com/
 peterdsharpe/AeroSandbox/blob/master/studies/WingTransonics/
-compare_methods.py). * Post-stall (i.e., truly 360 degree range of $\alpha$)
-aerodynamics. This is useful for applications like wind turbine blades or
+compare_methods.py). * **Post-stall aerodynamics** (i.e., truly 360 degree
+range of $\alpha$). This is useful for applications like wind turbine blades or
 propeller roots, where the airfoil may be operating at high angles of attack. *
-Control surface deflections. Currently only trailing-edge control surface
+**Control surface deflections**. Currently only trailing-edge control surface
 deflections are supported in AeroSandbox's NeuralFoil interface. ##
 Installation [Install from PyPI](https://pypi.org/project/NeuralFoil/) with
 `pip install neuralfoil`.  To run models, NeuralFoil currently requires minimal
 dependencies: * Python 3.7+ * [NumPy](https://numpy.org/) * [AeroSandbox]
 (https://github.com/peterdsharpe/AeroSandbox) 4.0.10+ Currently, NeuralFoil
 only uses AeroSandbox for airfoil geometry parameterization (i.e., converting
 from a set of points to a CST parameterization, which is solved as an
 optimization problem)âthe actual math is implemented in pure NumPy. Recent
 progress on this CST parameterization-fitting problem has allowed it to be
 recast as a least-squares problem, which is potentially amenable to a pure-
 NumPy implementation. That being said, AeroSandbox provides a bunch of nice
 peripheral utilities (e.g., geometry manipulation, visualization, etc.), so
 it's a nice dependency to have anyway. However, if you'd like to work on a
 pure-NumPy implementation, open an issue and let me know! ## Geometry
-Parameterization and Training Data #### Geometry Parameterization To be
-written, but it's basically an 8-parameter-per-side CST (Kulfan)
+Parameterization and Training Data #### Geometry Parameterization  As a user,
+you can give an airfoil in many different formatsâfor example, as a set of $
+(x,y)$ coordinates, as a .dat file, or as an AeroSandbox `Airfoil` object.
+However, under the hood, NeuralFoil parameterizes the airfoil geometry using
+the CST (Kulfan) parameterization. (You can also directly pass in Kulfan
+parameters if preferred.) The airfoil shape fed into NeuralFoil's neural
+networks is in the form of an 8-parameter-per-side CST (Kulfan)
 parameterization, with Kulfan's added leading-edge-modification (LEM) and
 trailing-edge thickness parameter. This gives a total of (8 * 2 + 1 + 1) = 18
-parameters to describe a given airfoil shape. I'll write more here, but in the
-meantime read: - [D. A. Masters, "Geometric Comparison of Aerofoil Shape
-Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/
-10.2514/1.J054943) - The seminal paper on the CST (Kulfan) parameterization
-technique: [Brenda Kulfan, "Universal Parametric Geometry Representation
-Method"](http://mx1.brendakulfan.com/docs/CST6.pdf) #### Training Data To be
-written, but in the meantime [see here](https://github.com/peterdsharpe/
-NeuralFoil/tree/master/training_data). Training data is not (yet) uploaded to
-GitHub, but will be soon - need to figure out Git LFS, as it's many gigabytes.
-Contact me if you need it sooner. ## FAQs Will NeuralFoil be integrated
-directly into [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox)? >
-Yes, absolutely. However, the goal is to keep this NeuralFoil repository also
-available as a stand-alone module, if desired. This simplifies dependencies for
-people using NeuralFoil in other applications (e.g., flight simulation, real-
-time control on embedded systems, etc.), and makes it easier if someone wanted
-to port NeuralFoil to another language (e.g., C++, for use on an Arduino).  Why
-not just use XFoil directly? > XFoil is a truly excellent piece of aerospace
-software engineering and is the gold standard of airfoil analysis, for good
-reason. When its assumptions hold (airfoils in subsonic flow without massive
-separation), its accuracy exceeds that of RANS CFD, yet it has ~1000x lower
-computational cost. XFoil shines in particular for human-in-the-loop airfoil
-design. However, XFoil is not the right tool for all applications, for a few
-reasons: > > - XFoil exhibits hysteresis: you can get slightly different
-solutions (for the same airfoil, $\alpha$, and $Re$) depending on whether you
-sweep $\alpha$ up or down, as Newton iteration is resumed from the last
-converged solution and uniqueness is not guaranteed. This hysteresis can be a
-big problem for design optimization. > - XFoil is not differentiable, in the
-sense that it doesn't tell you how performance changes w.r.t. airfoil shape
-(via, for example, an adjoint). That's okayâNeuralFoil doesn't either, at
-least out-of-the-box. However, the "path to obtain an efficient gradient" is
-very straightforward for NeuralFoil's pure NumPy code, where many excellent
-options exist (e.g., JAX). In contrast, gradient options for Fortran code (the
-language XFoil is in) either don't exist or are significantly less advanced
-(e.g., Tapenade). The most promising option for XFoil is probably [CMPLXFOIL]
-(https://github.com/mdolab/CMPLXFOIL), which computes complex-step
-(effectively, forward-mode) gradients. However, even if you can get a gradient,
-it still may present issues, because... > - XFoil's solutions lack $C^1$-
-continuity. NeuralFoil, by contrast, is guaranteed to be $C^\infty$-continuous
-by construction. This is critical for gradient-based optimization. > - Even if
-one tries to compute gradients of XFoil's outputs by finite-differencing or
-complex-stepping, these gradients are often inaccurate. > - A bit into the
-weeds, but: this comes down to how XFoil handles transition (onset of
-turbulence). XFoil does a cut-cell approach on the transitioning interval, and
-while this specific cut-cell implementation restores $C^0$-continuity (i.e.,
-transition won't truly "jump" from one node to another discretely), gradients
-of the laminar and turbulent BL closure functions still change at the cell
-interface due to the differing BL parameters ($H$ and $Re_\theta$) from node to
-node. This loses $C^1$ continuity, causing a "ragged" polar at the microscopic
-level. In theory $C^1$-continuity could be restored by also blending the BL
-shape variables through the transitioning cell interval, but that unleashes
-some ugly integrals and is not done in XFoil. > - For more on this, see [Adler,
-Gray, and Martins, "To CFD or not to CFD?..."](http://websites.umich.edu/
-~mdolaboratory/pdf/Adler2022c.pdf), Figure 7. > - While XFoil is ~1000x faster
-than RANS CFD, NeuralFoil [can be another ~1000x faster to evaluate than XFoil]
-(#performance). NeuralFoil is also much easier to interface with on a memory
-level than XFoil, which means you won't find yourself I/O bound from file
-reading/writing like you will with XFoil. > - XFoil is not vectorized, which
-exacerbates the speed advantage of a (vectorized) neural network when analyzing
-large batches of airfoil cases simultaneously. > - XFoil is not guaranteed to
-produce a solution. Instead, XFoil often crashes when "ambitious" calculations
-are attempted, rather than producing a less-accurate answer. In some
-applications, that's okay or even desirable; in others, that's a deal-breaker.
-Example applications where this is a problem include: > - Real-time control,
-where one wants to estimate forces (e.g., for a MPC trajectory), but you can't
-have the controller crash if XFoil fails to converge or hangs the CPU. > -
-Flight simulation: similar to real-time control where "a less-accurate answer"
-is much better than "no answer." > - Design optimization, where the optimizer
-needs "an answer" in order to recover from a bad design point and send the
-search back to a reasonable design. > - XFoil can be a serious pain to compile
-from source, which is often required if running on Mac or Linux (i.e., all
-supercomputers, some lab computers). NeuralFoil is pure Python and NumPy, so
-it's easy to install and run anywhere. Why not use a neural network trained on
-RANS CFD instead? > This is a cool idea too, and it has been done (See
-[Bouhlel, He, and Martins, "Scalable gradient-enhanced artificial..."](https://
-link.springer.com/article/10.1007/s00158-020-02488-5))! The fundamental
-challenge here, of course, is the cost of training data. RANS CFD is much more
-expensive than XFoil, so it's much harder to get sufficient training data to
-build a neural network that will generalize well out-of-sample. For example, in
-the linked work by Bouhlel et al., the authors trained a neural network on
-42,000 RANS CFD runs (and they were sweeping over Mach as well, so the data
-becomes even sparser). In contrast, NeuralFoil was trained on tens of millions
-of XFoil runs. Ultimately, this exposes NeuralFoil to a much larger "span" of
-the airfoil design space, which is critical for accurate predictions on out-of-
+parameters to describe a given airfoil shape.
+              [./media/kulfan_parameterization_illustration.svg]
+For more details on this parameterization, or why it is a good choice, read: -
+[D. A. Masters, "Geometric Comparison of Aerofoil Shape Parameterization
+Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943)
+- The seminal paper on the CST (Kulfan) parameterization technique: [Brenda
+Kulfan, "Universal Parametric Geometry Representation Method"](http://
+mx1.brendakulfan.com/docs/CST6.pdf) To convert between airfoil coordinates and
+the CST parameterization, use the following functions: ```python from
+aerosandbox.geometry.airfoil.airfoil_families import get_kulfan_parameters,
+get_kulfan_coordinates ``` with documentation [here](https://
+aerosandbox.readthedocs.io/en/master/autoapi/aerosandbox/geometry/airfoil/
+airfoil_families/index.html) or in the source ([here](https://github.com/
+peterdsharpe/AeroSandbox/blob/8ad83aa4e4e40c503884c722143b7730c08089fa/
+aerosandbox/geometry/airfoil/airfoil_families.py#L128), [here](https://
+github.com/peterdsharpe/AeroSandbox/blob/
+8ad83aa4e4e40c503884c722143b7730c08089fa/aerosandbox/geometry/airfoil/
+airfoil_families.py#L265)). #### Training Data To be written, but in the
+meantime [see here](https://github.com/peterdsharpe/NeuralFoil/tree/master/
+training_data). Training data is not (yet) uploaded to GitHub, but will be soon
+- need to figure out Git LFS, as it's many gigabytes. Contact me if you need it
+sooner. ## FAQs Will NeuralFoil be integrated directly into [AeroSandbox]
+(https://github.com/peterdsharpe/AeroSandbox)? > Yes, absolutely. However, the
+goal is to keep this NeuralFoil repository also available as a stand-alone
+module, if desired. This simplifies dependencies for people using NeuralFoil in
+other applications (e.g., flight simulation, real-time control on embedded
+systems, etc.), and makes it easier if someone wanted to port NeuralFoil to
+another language (e.g., C++, for use on an Arduino).  Why not just use XFoil
+directly? > XFoil is a truly excellent piece of aerospace software engineering
+and is the gold standard of airfoil analysis, for good reason. When its
+assumptions hold (airfoils in subsonic flow without massive separation), its
+accuracy exceeds that of RANS CFD, yet it has ~1000x lower computational cost.
+XFoil shines in particular for human-in-the-loop airfoil design. However, XFoil
+is not the right tool for all applications, for a few reasons: > > - XFoil
+exhibits hysteresis: you can get slightly different solutions (for the same
+airfoil, $\alpha$, and $Re$) depending on whether you sweep $\alpha$ up or
+down, as Newton iteration is resumed from the last converged solution and
+uniqueness is not guaranteed. This hysteresis can be a big problem for design
+optimization. > - XFoil is not differentiable, in the sense that it doesn't
+tell you how performance changes w.r.t. airfoil shape (via, for example, an
+adjoint). That's okayâNeuralFoil doesn't either, at least out-of-the-box.
+However, the "path to obtain an efficient gradient" is very straightforward for
+NeuralFoil's pure NumPy code, where many excellent options exist (e.g., JAX).
+In contrast, gradient options for Fortran code (the language XFoil is in)
+either don't exist or are significantly less advanced (e.g., Tapenade). The
+most promising option for XFoil is probably [CMPLXFOIL](https://github.com/
+mdolab/CMPLXFOIL), which computes complex-step (effectively, forward-mode)
+gradients. However, even if you can get a gradient, it still may present
+issues, because... > - XFoil's solutions lack $C^1$-continuity. NeuralFoil, by
+contrast, is guaranteed to be $C^\infty$-continuous by construction. This is
+critical for gradient-based optimization. > - Even if one tries to compute
+gradients of XFoil's outputs by finite-differencing or complex-stepping, these
+gradients are often inaccurate. > - A bit into the weeds, but: this comes down
+to how XFoil handles transition (onset of turbulence). XFoil does a cut-cell
+approach on the transitioning interval, and while this specific cut-cell
+implementation restores $C^0$-continuity (i.e., transition won't truly "jump"
+from one node to another discretely), gradients of the laminar and turbulent BL
+closure functions still change at the cell interface due to the differing BL
+parameters ($H$ and $Re_\theta$) from node to node. This loses $C^1$
+continuity, causing a "ragged" polar at the microscopic level. In theory $C^1$-
+continuity could be restored by also blending the BL shape variables through
+the transitioning cell interval, but that unleashes some ugly integrals and is
+not done in XFoil. > - For more on this, see [Adler, Gray, and Martins, "To CFD
+or not to CFD?..."](http://websites.umich.edu/~mdolaboratory/pdf/
+Adler2022c.pdf), Figure 7. > - While XFoil is ~1000x faster than RANS CFD,
+NeuralFoil [can be another ~1000x faster to evaluate than XFoil](#performance).
+NeuralFoil is also much easier to interface with on a memory level than XFoil,
+which means you won't find yourself I/O bound from file reading/writing like
+you will with XFoil. > - XFoil is not vectorized, which exacerbates the speed
+advantage of a (vectorized) neural network when analyzing large batches of
+airfoil cases simultaneously. > - XFoil is not guaranteed to produce a
+solution. Instead, XFoil often crashes when "ambitious" calculations are
+attempted, rather than producing a less-accurate answer. In some applications,
+that's okay or even desirable; in others, that's a deal-breaker. Example
+applications where this is a problem include: > - Real-time control, where one
+wants to estimate forces (e.g., for a MPC trajectory), but you can't have the
+controller crash if XFoil fails to converge or hangs the CPU. > - Flight
+simulation: similar to real-time control where "a less-accurate answer" is much
+better than "no answer." > - Design optimization, where the optimizer needs "an
+answer" in order to recover from a bad design point and send the search back to
+a reasonable design. > - XFoil can be a serious pain to compile from source,
+which is often required if running on Mac or Linux (i.e., all supercomputers,
+some lab computers). NeuralFoil is pure Python and NumPy, so it's easy to
+install and run anywhere. Why not use a neural network trained on RANS CFD
+instead? > This is a cool idea too, and it has been done (See [Bouhlel, He, and
+Martins, "Scalable gradient-enhanced artificial..."](https://link.springer.com/
+article/10.1007/s00158-020-02488-5))! The fundamental challenge here, of
+course, is the cost of training data. RANS CFD is much more expensive than
+XFoil, so it's much harder to get sufficient training data to build a neural
+network that will generalize well out-of-sample. For example, in the linked
+work by Bouhlel et al., the authors trained a neural network on 42,000 RANS CFD
+runs (and they were sweeping over Mach as well, so the data becomes even
+sparser). In contrast, NeuralFoil was trained on tens of millions of XFoil
+runs. Ultimately, this exposes NeuralFoil to a much larger "span" of the
+airfoil design space, which is critical for accurate predictions on out-of-
 sample airfoils. > > One advantage of a RANS CFD approach over the NeuralFoil
 XFoil approach is, of course, transonic modeling. NeuralFoil attempts to get
 around this a little bit by estimating $C_{p, min}$, which in turn allows you
 to estimate the critical Mach number. (For an implementation of that, [see
 here](#extended-features-transonics-post-stall-control-surface-deflections))
 But fundamentally, NeuralFoil is likely less accurate in the transonic range
 because of this. The tradeoff is that the much larger training data set allows
@@ -273,38 +290,28 @@
 usually more accurate than RANS CFD](https://www.sciencedirect.com/science/
 article/abs/pii/S1270963816300839). Why not use a neural network trained on
 wind tunnel data? > This is a super-cool idea, and I'd love to see someone try
 it! My guess is that you'd need some kind of morphing wing section (and a way
 of precisely measuring the shape) in order to get enough data samples to "span"
 the airfoil design space. Then, you'd just let the wing section sit in the wind
 tunnel for a few days morphing itself around to collect data, then train a
-model on that. This would be really awesome, someone should do it!  Why
-parameterize the airfoil geometry using the CST (Kulfan) parameterization? What
-exactly does the CST parameterization mean, and how can I convert this
-parameterization to/from actual airfoil coordinates? Why discretize with 8 CST
-modes per side? Can NeuralFoil accurately analyze airfoils with thick trailing
-edges? > To be written, but in the meantime read: > - [D. A. Masters,
-"Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA
-Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943) > - The seminal
-paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan,
-"Universal Parametric Geometry Representation Method"](http://
-mx1.brendakulfan.com/docs/CST6.pdf) What's the underlying neural network
-architecture used in NeuralFoil? > To be written, but it is essentially a feed-
-forward neural network with a varying number of total layers and layer width
-depending on model size. Layer counts and widths were [determined through
-extensive trial and error](./training/supercloud_job_id_notes.log), in
-conjunction with observed test- and train-loss values. All layers are dense
-(fully connected, with weights and biases). All activation functions between
-layers are $\tanh$, to preserve $C^\infty$-continuity. The number of layers and
-layer width are as follows: > > * xxsmall: 2 layers, 32 wide. > * xsmall: 3
-layers, 32 wide. > * small: 3 layers, 48 wide. > * medium: 4 layers, 64 wide. >
-* large: 4 layers, 128 wide. > * xlarge: 4 layers, 256 wide. > * xxlarge: 5
-layers, 256 wide. > * xxxlarge:5 layers, 512 wide. ## Acknowledgements
-NeuralFoil was trained on MIT Supercloud, a high-performance computing cluster
-operated by the MIT Lincoln Laboratory Supercomputing Center (LLSC). ## License
-NeuralFoil is licensed under the MIT license. Please see the [LICENSE]
-(LICENSE.txt) file for details. ## Citing NeuralFoil If you use NeuralFoil in
-your research, please cite it as follows: ``` @misc{neuralfoil, author = {Peter
-Sharpe}, title = {{NeuralFoil}: An airfoil aerodynamics analysis tool using
-physics-informed machine learning}, year = {2023}, publisher = {GitHub},
-journal = {GitHub repository}, howpublished = {\url{https://github.com/
-peterdsharpe/NeuralFoil}}, ```
+model on that. This would be really awesome, someone should do it! What's the
+underlying neural network architecture used in NeuralFoil? > To be written, but
+it is essentially a feed-forward neural network with a varying number of total
+layers and layer width depending on model size. Layer counts and widths were
+[determined through extensive trial and error](./training/
+supercloud_job_id_notes.log), in conjunction with observed test- and train-loss
+values. All layers are dense (fully connected, with weights and biases). All
+activation functions between layers are $\tanh$, to preserve $C^\infty$-
+continuity. The number of layers and layer width are as follows: > > * xxsmall:
+2 layers, 32 wide. > * xsmall: 3 layers, 32 wide. > * small: 3 layers, 48 wide.
+> * medium: 4 layers, 64 wide. > * large: 4 layers, 128 wide. > * xlarge: 4
+layers, 256 wide. > * xxlarge: 5 layers, 256 wide. > * xxxlarge:5 layers, 512
+wide. ## Acknowledgements NeuralFoil was trained on MIT Supercloud, a high-
+performance computing cluster operated by the MIT Lincoln Laboratory
+Supercomputing Center (LLSC). ## License NeuralFoil is licensed under the MIT
+license. Please see the [LICENSE](LICENSE.txt) file for details. ## Citing
+NeuralFoil If you use NeuralFoil in your research, please cite it as follows:
+``` @misc{neuralfoil, author = {Peter Sharpe}, title = {{NeuralFoil}: An
+airfoil aerodynamics analysis tool using physics-informed machine learning},
+year = {2023}, publisher = {GitHub}, journal = {GitHub repository},
+howpublished = {\url{https://github.com/peterdsharpe/NeuralFoil}}, } ```
```

### Comparing `NeuralFoil-0.1.7/README.md` & `NeuralFoil-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 <p align="center">
     <img src="./media/neuralfoil_logo.svg" width="800" />
 </p>
 
 by [Peter Sharpe](https://peterdsharpe.github.io) (<pds [at] mit [dot] edu>)
 
-
-[!![PyPI](https://img.shields.io/pypi/v/neuralfoil)
-](https://pypi.org/project/NeuralFoil/)
+[![PyPI](https://img.shields.io/pypi/v/neuralfoil)](https://pypi.org/project/NeuralFoil/)
 [![Build Status](https://github.com/peterdsharpe/NeuralFoil/workflows/Tests/badge.svg)](https://github.com/peterdsharpe/NeuralFoil/actions/workflows/run-pytest.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-g.svg)](https://opensource.org/licenses/MIT)
 
 -----
 
 NeuralFoil is a tool for rapid aerodynamics analysis of airfoils, similar to [XFoil](https://web.mit.edu/drela/Public/web/xfoil/). Under the hood, NeuralFoil consists of physics-informed neural networks trained on [tens of millions of XFoil runs](#geometry-parameterization-and-training-data).
 
-NeuralFoil is available here as a pure Python+NumPy standalone, but it is also [available within AeroSandbox](#extended-features-transonics-post-stall-control-surface-deflections), which extends it with many more advanced features. Using the AeroSandbox extension, NeuralFoil can give you **viscous, compressible airfoil aerodynamics for (nearly) any airfoil, with control surface deflections, across $360^\circ$ angle of attack, at any Reynolds number, all nearly instantly** (~5 milliseconds). And, it's guaranteed to return an answer (no non-convergence issues), it's vectorized, and it's $C^1$-continuous (all very useful for gradient-based optimization). 
+NeuralFoil is available here as a pure Python+NumPy standalone, but it is also [available within AeroSandbox](#extended-features-transonics-post-stall-control-surface-deflections), which extends it with many more advanced features. Using the AeroSandbox extension, NeuralFoil can give you **viscous, compressible airfoil aerodynamics for (nearly) any airfoil, with control surface deflections, across $360^\circ$ angle of attack, at any Reynolds number, all nearly instantly** (~5 milliseconds). And, it's guaranteed to return an answer (no non-convergence issues), it's vectorized, and it's $C^1$-continuous (all very useful for gradient-based optimization).
 
 NeuralFoil is [~10x faster than XFoil for a single analysis, and ~1000x faster for multipoint analysis](#table), all with [minimal loss in accuracy compared to XFoil](#performance). Due to the wide variety of training data and the embedding of several physics-based invariants, [this accuracy is seen even on out-of-sample airfoils](#performance) (i.e., airfoils it wasn't trained on). It also has [many nice features](#xfoil-benefit-question) (e.g., smoothness, vectorization, all in Python+NumPy) that make it much easier to use.
 
- NeuralFoil aims to be lightweight, with [minimal dependencies](#dependencies-question) and a [tight, efficient, and easily-understood code-base](./neuralfoil) (less than 500 lines of user-facing code).
+NeuralFoil aims to be lightweight, with [minimal dependencies](#dependencies-question) and a [tight, efficient, and easily-understood code-base](./neuralfoil) (less than 500 lines of user-facing code).
+
 ```
 pip install neuralfoil
 ```
 
 ## Overview
 
 NeuralFoil comes with 8 different neural network models, with increasing levels of complexity:
@@ -40,15 +39,15 @@
 		<td>"xxxlarge"</td>
 	 </tr>
 	</table>
 </div>
 
 This spectrum offers a tradeoff between accuracy and computational cost.
 
-In addition to its neural network models, NeuralFoil also has a bonus "Linear $C_L$ model" that predicts lift coefficient $C_L$ as a purely-linear function of angle of attack $\alpha$. This model is well-suited for linear lifting-line or blade-element-method analyses, where the $C_L(\alpha)$ linearity can be used to solve the resulting system of equations "in one shot" as a linear solve, rather than a less-numerically-robust iterative nonlinear solve.
+In addition to its neural network models, NeuralFoil also has a bonus "Linear $C_L$ model" that predicts lift coefficient $C_L$ as a purely-affine function of angle of attack $\alpha$. This model is well-suited for linear lifting-line or blade-element-method analyses, where the $C_L(\alpha)$ linearity can be used to solve the resulting system of equations "in one shot" as a linear solve, rather than a less-numerically-robust iterative nonlinear solve.
 
 Using NeuralFoil is dead-simple, and also offers several possible "entry points" for inputs. Here's an example showing this:
 
 ```python
 import neuralfoil as nf  # `pip install neuralfoil`
 import numpy as np
 
@@ -71,24 +70,24 @@
 )
 
 # `aero` is a dictionary with keys: ["CL", "CD", "CM", "Cpmin", "Top_Xtr", "Bot_Xtr"]
 ```
 
 ## Performance
 
-Qualitatively, NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$ values. In the figure below, we compare the performance of NeuralFoil to XFoil on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was developed "from scratch" for a [real-world aircraft development program](https://www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-research-aircraft-301633713.html) and is completely separate from [the airfoils used during NeuralFoil's training](#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance: 
+Qualitatively, NeuralFoil tracks XFoil very closely across a wide range of $\alpha$ and $Re$ values. In the figure below, we compare the performance of NeuralFoil to XFoil on $C_L, C_D$ polar prediction. Notably, the airfoil analyzed here was developed "from scratch" for a [real-world aircraft development program](https://www.prnewswire.com/news-releases/electra-flies-solar-electric-hybrid-research-aircraft-301633713.html) and is completely separate from [the airfoils used during NeuralFoil's training](#geometry-parameterization-and-training-data), so NeuralFoil isn't cheating by "memorizing" this airfoil's performance:
 
 <a name="clcd-polar"></a>
 <p align="center">
 	<img src="./benchmarking/neuralfoil_point_validation.svg" width="1000" />
 </p>
 
-NeuralFoil is typically accurate to within a few percent of XFoil's predictions. Note that this figure is on a truly out-of-sample airfoil, so airfoils that are closer to the training set will have even more accurate results. 
+NeuralFoil is typically accurate to within a few percent of XFoil's predictions. Note that this figure is on a truly out-of-sample airfoil, so airfoils that are closer to the training set will have even more accurate results.
 
-NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is not reliably converging, which would otherwise make optimization difficult. 
+NeuralFoil also [has the benefit of smoothing out XFoil's "jagged" predictions](#xfoil-benefit-question) (for example, near $C_L=1.4$ at $Re=\mathrm{90k}$) in cases where XFoil is not reliably converging, which would otherwise make optimization difficult.
 
 In the table below, we quantify the performance of the NeuralFoil ("NF") models with respect to XFoil more precisely. At a basic level, we care about two things:
 
 - **Accuracy**: how close are the predictions to XFoil's?
 - **Computational Cost**: how long does it take to run?
 
 This table details both of these considerations. The first few columns show the error with respect to XFoil on the test dataset. [The test dataset is completely isolated from the training dataset, and NeuralFoil was not allowed to learn from the test dataset](#geometry-parameterization-and-training-data). Thus, the performance on the test dataset gives a good idea of NeuralFoil's performance "in the wild". The second set of columns gives the runtime speed of the models, both for a single analysis and for a large batch analysis.
@@ -97,25 +96,25 @@
 
 <table><thead><tr><th>Aerodynamics Model</th><th colspan="6">Mean Absolute Error (MAE) of Given Metric, on the Test Dataset, with respect to XFoil</th><th colspan="2">Computational Cost to Run</th></tr></thead><tbody><tr><td></td><td>Lift Coeff.<br>$C_L$</td><td>Fractional Drag Coeff.<br>$\ln(C_D)$   †</td><td>Moment Coeff.<br>$C_M$</td><td>Max Overspeed<br>$u_\max / u_\infty$&nbsp;&nbsp;&nbsp;‡</td><td>Top Transition Loc.<br>$x_{tr, top}/c$</td><td>Bottom Trans. Loc.<br>$x_{tr, bot}/c$</td><td>Runtime<br>(1 run)</td><td>Total Runtime<br>(100,000 runs)</td></tr><tr><td>NF Linear $C_L$ Model</td><td>0.116</td><td>-</td><td>-</td><td>-</td><td>-</td><td>-</td><td>1 ms</td><td>0.020 sec</td></tr><tr><td>NF "xxsmall"</td><td>0.065</td><td>0.121</td><td>0.010</td><td>0.215</td><td>0.073</td><td>0.100</td><td>3 ms</td><td>0.190 sec</td></tr><tr><td>NF "xsmall"</td><td>0.042</td><td>0.075</td><td>0.007</td><td>0.134</td><td>0.039</td><td>0.055</td><td>4 ms</td><td>0.284 sec</td></tr><tr><td>NF "small"</td><td>0.039</td><td>0.069</td><td>0.006</td><td>0.122</td><td>0.036</td><td>0.050</td><td>4 ms</td><td>0.402 sec</td></tr><tr><td>NF "medium"</td><td>0.027</td><td>0.051</td><td>0.004</td><td>0.088</td><td>0.022</td><td>0.033</td><td>5 ms</td><td>0.784 sec</td></tr><tr><td>NF "large"</td><td>0.024</td><td>0.045</td><td>0.004</td><td>0.079</td><td>0.020</td><td>0.029</td><td>6 ms</td><td>1.754 sec</td></tr><tr><td>NF "xlarge"</td><td>0.023</td><td>0.043</td><td>0.004</td><td>0.076</td><td>0.019</td><td>0.028</td><td>10 ms</td><td>3.330 sec</td></tr><tr><td>NF "xxlarge"</td><td>0.021</td><td>0.040</td><td>0.003</td><td>0.071</td><td>0.018</td><td>0.025</td><td>13 ms</td><td>4.297 sec</td></tr><tr><td>NF "xxxlarge"</td><td>0.020</td><td>0.039</td><td>0.003</td><td>0.070</td><td>0.016</td><td>0.024</td><td>38 ms</td><td>8.980 sec</td></tr><tr><td>XFoil</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>0</td><td>73 ms</td><td>42 min</td></tr></tbody></table>
 
 > † The deviation of $\ln(C_D)$ can be thought of as "the typical relative error in $C_D$". For example, if the mean absolute error ("MAE", or $L^1$ norm) of $\ln(C_D)$ is 0.039, you can think of it as "typically, drag is accurate to within 3.9% of XFoil." Note that this doesn't necessarily mean that NeuralFoil is *less* accurate than XFoil - although XFoil is quite accurate, it is clearly not a perfect "ground truth" in all cases (see $Re=\mathrm{90k}$ in the [figure above](#clcd-polar)). So, NeuralFoil's true accuracy compared to experiment may differ (in either direction) from the numbers in this table.
 > 
 > ‡ This "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to calculate the critical Mach number $M_\mathrm{crit}$. [More details below.](#extended-features-transonics-post-stall-control-surface-deflections)
 
-Based on these performance numbers, you can select the right tradeoff between accuracy and computational cost for your application. In general, I recommend starting with the "large" model and adjusting from there.
+Based on these performance numbers, you can select the right tradeoff between accuracy and computational cost for your application. In general, I recommend starting with the ["large"](#overview) model and adjusting from there.
 
 In addition to accuracy vs. speed, another consideration when choosing the right model is what you're trying to use NeuralFoil for. Larger models will be more complicated ("less parsimonious," as the math kids would say), which means that they may have more "wiggles" in their outputs—this might be undesirable for gradient-based optimization. On the other hand, larger models will be able to capture a wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be seen mid-optimization), so larger models could have a benefit in that sense. If you try a specific application and have better/worse results with a specific model, let me know by opening a GitHub issue!
 
 ## Extended Features (transonics, post-stall, control surface deflections)
 
 For more sophisticated airfoil aerodynamics calculations, consider using NeuralFoil via [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox) (specifically, through [`asb.Airfoil.get_aero_from_neuralfoil()`](https://github.com/peterdsharpe/AeroSandbox/blob/8ad83aa4e4e40c503884c722143b7730c08089fa/aerosandbox/geometry/airfoil/airfoil.py#L607)). This provides several advanced features:
 
-* Compressible aerodynamics, including transonic and supersonic aerodynamics. AeroSandbox will generally get the critical Mach number accurate to within $\pm 0.01$ or so. Subsonic corrections done using a Laitone correction (a higher-order variant of Prandtl-Glauert and Karman-Tsien). Wave drag accuracy is, of course, less reliable beyond the drag-divergence Mach number, although it still [agrees reasonably closely when compared to RANS CFD](https://github.com/peterdsharpe/AeroSandbox/blob/master/studies/WingTransonics/compare_methods.py).
-* Post-stall (i.e., truly 360 degree range of $\alpha$) aerodynamics. This is useful for applications like wind turbine blades or propeller roots, where the airfoil may be operating at high angles of attack.
-* Control surface deflections. Currently only trailing-edge control surface deflections are supported in AeroSandbox's NeuralFoil interface.
+* **Compressible aerodynamics**, including transonic and supersonic aerodynamics. AeroSandbox will generally get the critical Mach number accurate to within $\pm 0.01$ or so. Subsonic corrections done using a Laitone correction (a higher-order variant of Prandtl-Glauert and Karman-Tsien). Wave drag accuracy is, of course, less reliable beyond the drag-divergence Mach number, although it still [agrees reasonably closely when compared to RANS CFD](https://github.com/peterdsharpe/AeroSandbox/blob/master/studies/WingTransonics/compare_methods.py).
+* **Post-stall aerodynamics** (i.e., truly 360 degree range of $\alpha$). This is useful for applications like wind turbine blades or propeller roots, where the airfoil may be operating at high angles of attack.
+* **Control surface deflections**. Currently only trailing-edge control surface deflections are supported in AeroSandbox's NeuralFoil interface.
 
 ## Installation
 
 [Install from PyPI](https://pypi.org/project/NeuralFoil/) with `pip install neuralfoil`.
 
 <a name="dependencies-question"></a>
 To run models, NeuralFoil currently requires minimal dependencies:
@@ -126,18 +125,37 @@
 
 Currently, NeuralFoil only uses AeroSandbox for airfoil geometry parameterization (i.e., converting from a set of points to a CST parameterization, which is solved as an optimization problem)—the actual math is implemented in pure NumPy. Recent progress on this CST parameterization-fitting problem has allowed it to be recast as a least-squares problem, which is potentially amenable to a pure-NumPy implementation. That being said, AeroSandbox provides a bunch of nice peripheral utilities (e.g., geometry manipulation, visualization, etc.), so it's a nice dependency to have anyway. However, if you'd like to work on a pure-NumPy implementation, open an issue and let me know!
 
 ## Geometry Parameterization and Training Data
 
 #### Geometry Parameterization
 
-To be written, but it's basically an 8-parameter-per-side CST (Kulfan) parameterization, with Kulfan's added leading-edge-modification (LEM) and trailing-edge thickness parameter. This gives a total of (8 * 2 + 1 + 1) = 18 parameters to describe a given airfoil shape. I'll write more here, but in the meantime read:
+<a name="parameterization-question"></a>
+
+As a user, you can give an airfoil in many different formats—for example, as a set of $(x,y)$ coordinates, as a .dat file, or as an AeroSandbox `Airfoil` object. However, under the hood, NeuralFoil parameterizes the airfoil geometry using the CST (Kulfan) parameterization. (You can also directly pass in Kulfan parameters if preferred.)
+
+The airfoil shape fed into NeuralFoil's neural networks is in the form of an 8-parameter-per-side CST (Kulfan) parameterization, with Kulfan's added leading-edge-modification (LEM) and trailing-edge thickness parameter. This gives a total of (8 * 2 + 1 + 1) = 18 parameters to describe a given airfoil shape.
+
+<p align="center">
+	<img src="./media/kulfan_parameterization_illustration.svg" width="1000" />
+</p>
+
+For more details on this parameterization, or why it is a good choice, read:
+
 - [D. A. Masters, "Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943)
 - The seminal paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan, "Universal Parametric Geometry Representation Method"](http://mx1.brendakulfan.com/docs/CST6.pdf)
 
+To convert between airfoil coordinates and the CST parameterization, use the following functions:
+
+```python
+from aerosandbox.geometry.airfoil.airfoil_families import get_kulfan_parameters, get_kulfan_coordinates
+```
+
+with documentation [here](https://aerosandbox.readthedocs.io/en/master/autoapi/aerosandbox/geometry/airfoil/airfoil_families/index.html) or in the source ([here](https://github.com/peterdsharpe/AeroSandbox/blob/8ad83aa4e4e40c503884c722143b7730c08089fa/aerosandbox/geometry/airfoil/airfoil_families.py#L128), [here](https://github.com/peterdsharpe/AeroSandbox/blob/8ad83aa4e4e40c503884c722143b7730c08089fa/aerosandbox/geometry/airfoil/airfoil_families.py#L265)).
+
 #### Training Data
 
 To be written, but in the meantime [see here](https://github.com/peterdsharpe/NeuralFoil/tree/master/training_data). Training data is not (yet) uploaded to GitHub, but will be soon - need to figure out Git LFS, as it's many gigabytes. Contact me if you need it sooner.
 
 ## FAQs
 
 Will NeuralFoil be integrated directly into [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox)?
@@ -169,22 +187,14 @@
 >
 > One advantage of a RANS CFD approach over the NeuralFoil XFoil approach is, of course, transonic modeling. NeuralFoil attempts to get around this a little bit by estimating $C_{p, min}$, which in turn allows you to estimate the critical Mach number. (For an implementation of that, [see here](#extended-features-transonics-post-stall-control-surface-deflections)) But fundamentally, NeuralFoil is likely less accurate in the transonic range because of this. The tradeoff is that the much larger training data set allows NeuralFoil to be more accurate in the subsonic range, where [XFoil is actually usually more accurate than RANS CFD](https://www.sciencedirect.com/science/article/abs/pii/S1270963816300839).
 
 Why not use a neural network trained on wind tunnel data?
 
 > This is a super-cool idea, and I'd love to see someone try it! My guess is that you'd need some kind of morphing wing section (and a way of precisely measuring the shape) in order to get enough data samples to "span" the airfoil design space. Then, you'd just let the wing section sit in the wind tunnel for a few days morphing itself around to collect data, then train a model on that. This would be really awesome, someone should do it!
 
-
-<a name="parameterization-question"></a>
-Why parameterize the airfoil geometry using the CST (Kulfan) parameterization? What exactly does the CST parameterization mean, and how can I convert this parameterization to/from actual airfoil coordinates? Why discretize with 8 CST modes per side? Can NeuralFoil accurately analyze airfoils with thick trailing edges?
-
-> To be written, but in the meantime read:
-> - [D. A. Masters, "Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943)
-> - The seminal paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan, "Universal Parametric Geometry Representation Method"](http://mx1.brendakulfan.com/docs/CST6.pdf)
-
 What's the underlying neural network architecture used in NeuralFoil?
 
 > To be written, but it is essentially a feed-forward neural network with a varying number of total layers and layer width depending on model size. Layer counts and widths were [determined through extensive trial and error](./training/supercloud_job_id_notes.log), in conjunction with observed test- and train-loss values. All layers are dense (fully connected, with weights and biases). All activation functions between layers are $\tanh$, to preserve $C^\infty$-continuity. The number of layers and layer width are as follows:
 >
 > * xxsmall: 2 layers,  32 wide.
 > * xsmall:  3 layers,  32 wide.
 > * small:   3 layers,  48 wide.
@@ -192,15 +202,15 @@
 > * large:   4 layers, 128 wide.
 > * xlarge:  4 layers, 256 wide.
 > * xxlarge: 5 layers, 256 wide.
 > * xxxlarge:5 layers, 512 wide.
 
 ## Acknowledgements
 
-NeuralFoil was trained on MIT Supercloud, a high-performance computing cluster operated by the MIT Lincoln Laboratory Supercomputing Center (LLSC). 
+NeuralFoil was trained on MIT Supercloud, a high-performance computing cluster operated by the MIT Lincoln Laboratory Supercomputing Center (LLSC).
 
 ## License
 
 NeuralFoil is licensed under the MIT license. Please see the [LICENSE](LICENSE.txt) file for details.
 
 ## Citing NeuralFoil
 
@@ -210,8 +220,9 @@
 @misc{neuralfoil,
   author = {Peter Sharpe},
   title = {{NeuralFoil}: An airfoil aerodynamics analysis tool using physics-informed machine learning},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/peterdsharpe/NeuralFoil}},
+}
 ```
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                          [./media/neuralfoil_logo.svg]
 by [Peter Sharpe](https://peterdsharpe.github.io) (
-at] mit [dot] edu>) [!![PyPI](https://img.shields.io/pypi/v/neuralfoil) ]
-(https://pypi.org/project/NeuralFoil/) [![Build Status](https://github.com/
+at] mit [dot] edu>) [![PyPI](https://img.shields.io/pypi/v/neuralfoil)](https:/
+/pypi.org/project/NeuralFoil/) [![Build Status](https://github.com/
 peterdsharpe/NeuralFoil/workflows/Tests/badge.svg)](https://github.com/
 peterdsharpe/NeuralFoil/actions/workflows/run-pytest.yml) [![License: MIT]
 (https://img.shields.io/badge/License-MIT-g.svg)](https://opensource.org/
 licenses/MIT) ----- NeuralFoil is a tool for rapid aerodynamics analysis of
 airfoils, similar to [XFoil](https://web.mit.edu/drela/Public/web/xfoil/).
 Under the hood, NeuralFoil consists of physics-informed neural networks trained
 on [tens of millions of XFoil runs](#geometry-parameterization-and-training-
@@ -29,15 +29,15 @@
 efficient, and easily-understood code-base](./neuralfoil) (less than 500 lines
 of user-facing code). ``` pip install neuralfoil ``` ## Overview NeuralFoil
 comes with 8 different neural network models, with increasing levels of
 complexity:
    "xxsmall" "xsmall" "small" "medium" "large" "xlarge" "xxlarge" "xxxlarge"
 This spectrum offers a tradeoff between accuracy and computational cost. In
 addition to its neural network models, NeuralFoil also has a bonus "Linear
-$C_L$ model" that predicts lift coefficient $C_L$ as a purely-linear function
+$C_L$ model" that predicts lift coefficient $C_L$ as a purely-affine function
 of angle of attack $\alpha$. This model is well-suited for linear lifting-line
 or blade-element-method analyses, where the $C_L(\alpha)$ linearity can be used
 to solve the resulting system of equations "in one shot" as a linear solve,
 rather than a less-numerically-robust iterative nonlinear solve. Using
 NeuralFoil is dead-simple, and also offers several possible "entry points" for
 inputs. Here's an example showing this: ```python import neuralfoil as nf #
 `pip install neuralfoil` import numpy as np aero = nf.get_aero_from_dat_file( #
@@ -116,142 +116,159 @@
 above](#clcd-polar)). So, NeuralFoil's true accuracy compared to experiment may
 differ (in either direction) from the numbers in this table. > > â¡ This
 "maximum overspeed" lets you compute $C_{p,\min}$, which can be used to
 calculate the critical Mach number $M_\mathrm{crit}$. [More details below.]
 (#extended-features-transonics-post-stall-control-surface-deflections) Based on
 these performance numbers, you can select the right tradeoff between accuracy
 and computational cost for your application. In general, I recommend starting
-with the "large" model and adjusting from there. In addition to accuracy vs.
-speed, another consideration when choosing the right model is what you're
-trying to use NeuralFoil for. Larger models will be more complicated ("less
-parsimonious," as the math kids would say), which means that they may have more
-"wiggles" in their outputsâthis might be undesirable for gradient-based
-optimization. On the other hand, larger models will be able to capture a wider
-range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might be
-seen mid-optimization), so larger models could have a benefit in that sense. If
-you try a specific application and have better/worse results with a specific
+with the ["large"](#overview) model and adjusting from there. In addition to
+accuracy vs. speed, another consideration when choosing the right model is what
+you're trying to use NeuralFoil for. Larger models will be more complicated
+("less parsimonious," as the math kids would say), which means that they may
+have more "wiggles" in their outputsâthis might be undesirable for gradient-
+based optimization. On the other hand, larger models will be able to capture a
+wider range of airfoils (e.g., nonsensical, weirdly-shaped airfoils that might
+be seen mid-optimization), so larger models could have a benefit in that sense.
+If you try a specific application and have better/worse results with a specific
 model, let me know by opening a GitHub issue! ## Extended Features (transonics,
 post-stall, control surface deflections) For more sophisticated airfoil
 aerodynamics calculations, consider using NeuralFoil via [AeroSandbox](https://
 github.com/peterdsharpe/AeroSandbox) (specifically, through
 [`asb.Airfoil.get_aero_from_neuralfoil()`](https://github.com/peterdsharpe/
 AeroSandbox/blob/8ad83aa4e4e40c503884c722143b7730c08089fa/aerosandbox/geometry/
 airfoil/airfoil.py#L607)). This provides several advanced features: *
-Compressible aerodynamics, including transonic and supersonic aerodynamics.
+**Compressible aerodynamics**, including transonic and supersonic aerodynamics.
 AeroSandbox will generally get the critical Mach number accurate to within $\pm
 0.01$ or so. Subsonic corrections done using a Laitone correction (a higher-
 order variant of Prandtl-Glauert and Karman-Tsien). Wave drag accuracy is, of
 course, less reliable beyond the drag-divergence Mach number, although it still
 [agrees reasonably closely when compared to RANS CFD](https://github.com/
 peterdsharpe/AeroSandbox/blob/master/studies/WingTransonics/
-compare_methods.py). * Post-stall (i.e., truly 360 degree range of $\alpha$)
-aerodynamics. This is useful for applications like wind turbine blades or
+compare_methods.py). * **Post-stall aerodynamics** (i.e., truly 360 degree
+range of $\alpha$). This is useful for applications like wind turbine blades or
 propeller roots, where the airfoil may be operating at high angles of attack. *
-Control surface deflections. Currently only trailing-edge control surface
+**Control surface deflections**. Currently only trailing-edge control surface
 deflections are supported in AeroSandbox's NeuralFoil interface. ##
 Installation [Install from PyPI](https://pypi.org/project/NeuralFoil/) with
 `pip install neuralfoil`.  To run models, NeuralFoil currently requires minimal
 dependencies: * Python 3.7+ * [NumPy](https://numpy.org/) * [AeroSandbox]
 (https://github.com/peterdsharpe/AeroSandbox) 4.0.10+ Currently, NeuralFoil
 only uses AeroSandbox for airfoil geometry parameterization (i.e., converting
 from a set of points to a CST parameterization, which is solved as an
 optimization problem)âthe actual math is implemented in pure NumPy. Recent
 progress on this CST parameterization-fitting problem has allowed it to be
 recast as a least-squares problem, which is potentially amenable to a pure-
 NumPy implementation. That being said, AeroSandbox provides a bunch of nice
 peripheral utilities (e.g., geometry manipulation, visualization, etc.), so
 it's a nice dependency to have anyway. However, if you'd like to work on a
 pure-NumPy implementation, open an issue and let me know! ## Geometry
-Parameterization and Training Data #### Geometry Parameterization To be
-written, but it's basically an 8-parameter-per-side CST (Kulfan)
+Parameterization and Training Data #### Geometry Parameterization  As a user,
+you can give an airfoil in many different formatsâfor example, as a set of $
+(x,y)$ coordinates, as a .dat file, or as an AeroSandbox `Airfoil` object.
+However, under the hood, NeuralFoil parameterizes the airfoil geometry using
+the CST (Kulfan) parameterization. (You can also directly pass in Kulfan
+parameters if preferred.) The airfoil shape fed into NeuralFoil's neural
+networks is in the form of an 8-parameter-per-side CST (Kulfan)
 parameterization, with Kulfan's added leading-edge-modification (LEM) and
 trailing-edge thickness parameter. This gives a total of (8 * 2 + 1 + 1) = 18
-parameters to describe a given airfoil shape. I'll write more here, but in the
-meantime read: - [D. A. Masters, "Geometric Comparison of Aerofoil Shape
-Parameterization Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/
-10.2514/1.J054943) - The seminal paper on the CST (Kulfan) parameterization
-technique: [Brenda Kulfan, "Universal Parametric Geometry Representation
-Method"](http://mx1.brendakulfan.com/docs/CST6.pdf) #### Training Data To be
-written, but in the meantime [see here](https://github.com/peterdsharpe/
-NeuralFoil/tree/master/training_data). Training data is not (yet) uploaded to
-GitHub, but will be soon - need to figure out Git LFS, as it's many gigabytes.
-Contact me if you need it sooner. ## FAQs Will NeuralFoil be integrated
-directly into [AeroSandbox](https://github.com/peterdsharpe/AeroSandbox)? >
-Yes, absolutely. However, the goal is to keep this NeuralFoil repository also
-available as a stand-alone module, if desired. This simplifies dependencies for
-people using NeuralFoil in other applications (e.g., flight simulation, real-
-time control on embedded systems, etc.), and makes it easier if someone wanted
-to port NeuralFoil to another language (e.g., C++, for use on an Arduino).  Why
-not just use XFoil directly? > XFoil is a truly excellent piece of aerospace
-software engineering and is the gold standard of airfoil analysis, for good
-reason. When its assumptions hold (airfoils in subsonic flow without massive
-separation), its accuracy exceeds that of RANS CFD, yet it has ~1000x lower
-computational cost. XFoil shines in particular for human-in-the-loop airfoil
-design. However, XFoil is not the right tool for all applications, for a few
-reasons: > > - XFoil exhibits hysteresis: you can get slightly different
-solutions (for the same airfoil, $\alpha$, and $Re$) depending on whether you
-sweep $\alpha$ up or down, as Newton iteration is resumed from the last
-converged solution and uniqueness is not guaranteed. This hysteresis can be a
-big problem for design optimization. > - XFoil is not differentiable, in the
-sense that it doesn't tell you how performance changes w.r.t. airfoil shape
-(via, for example, an adjoint). That's okayâNeuralFoil doesn't either, at
-least out-of-the-box. However, the "path to obtain an efficient gradient" is
-very straightforward for NeuralFoil's pure NumPy code, where many excellent
-options exist (e.g., JAX). In contrast, gradient options for Fortran code (the
-language XFoil is in) either don't exist or are significantly less advanced
-(e.g., Tapenade). The most promising option for XFoil is probably [CMPLXFOIL]
-(https://github.com/mdolab/CMPLXFOIL), which computes complex-step
-(effectively, forward-mode) gradients. However, even if you can get a gradient,
-it still may present issues, because... > - XFoil's solutions lack $C^1$-
-continuity. NeuralFoil, by contrast, is guaranteed to be $C^\infty$-continuous
-by construction. This is critical for gradient-based optimization. > - Even if
-one tries to compute gradients of XFoil's outputs by finite-differencing or
-complex-stepping, these gradients are often inaccurate. > - A bit into the
-weeds, but: this comes down to how XFoil handles transition (onset of
-turbulence). XFoil does a cut-cell approach on the transitioning interval, and
-while this specific cut-cell implementation restores $C^0$-continuity (i.e.,
-transition won't truly "jump" from one node to another discretely), gradients
-of the laminar and turbulent BL closure functions still change at the cell
-interface due to the differing BL parameters ($H$ and $Re_\theta$) from node to
-node. This loses $C^1$ continuity, causing a "ragged" polar at the microscopic
-level. In theory $C^1$-continuity could be restored by also blending the BL
-shape variables through the transitioning cell interval, but that unleashes
-some ugly integrals and is not done in XFoil. > - For more on this, see [Adler,
-Gray, and Martins, "To CFD or not to CFD?..."](http://websites.umich.edu/
-~mdolaboratory/pdf/Adler2022c.pdf), Figure 7. > - While XFoil is ~1000x faster
-than RANS CFD, NeuralFoil [can be another ~1000x faster to evaluate than XFoil]
-(#performance). NeuralFoil is also much easier to interface with on a memory
-level than XFoil, which means you won't find yourself I/O bound from file
-reading/writing like you will with XFoil. > - XFoil is not vectorized, which
-exacerbates the speed advantage of a (vectorized) neural network when analyzing
-large batches of airfoil cases simultaneously. > - XFoil is not guaranteed to
-produce a solution. Instead, XFoil often crashes when "ambitious" calculations
-are attempted, rather than producing a less-accurate answer. In some
-applications, that's okay or even desirable; in others, that's a deal-breaker.
-Example applications where this is a problem include: > - Real-time control,
-where one wants to estimate forces (e.g., for a MPC trajectory), but you can't
-have the controller crash if XFoil fails to converge or hangs the CPU. > -
-Flight simulation: similar to real-time control where "a less-accurate answer"
-is much better than "no answer." > - Design optimization, where the optimizer
-needs "an answer" in order to recover from a bad design point and send the
-search back to a reasonable design. > - XFoil can be a serious pain to compile
-from source, which is often required if running on Mac or Linux (i.e., all
-supercomputers, some lab computers). NeuralFoil is pure Python and NumPy, so
-it's easy to install and run anywhere. Why not use a neural network trained on
-RANS CFD instead? > This is a cool idea too, and it has been done (See
-[Bouhlel, He, and Martins, "Scalable gradient-enhanced artificial..."](https://
-link.springer.com/article/10.1007/s00158-020-02488-5))! The fundamental
-challenge here, of course, is the cost of training data. RANS CFD is much more
-expensive than XFoil, so it's much harder to get sufficient training data to
-build a neural network that will generalize well out-of-sample. For example, in
-the linked work by Bouhlel et al., the authors trained a neural network on
-42,000 RANS CFD runs (and they were sweeping over Mach as well, so the data
-becomes even sparser). In contrast, NeuralFoil was trained on tens of millions
-of XFoil runs. Ultimately, this exposes NeuralFoil to a much larger "span" of
-the airfoil design space, which is critical for accurate predictions on out-of-
+parameters to describe a given airfoil shape.
+              [./media/kulfan_parameterization_illustration.svg]
+For more details on this parameterization, or why it is a good choice, read: -
+[D. A. Masters, "Geometric Comparison of Aerofoil Shape Parameterization
+Methods", AIAA Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943)
+- The seminal paper on the CST (Kulfan) parameterization technique: [Brenda
+Kulfan, "Universal Parametric Geometry Representation Method"](http://
+mx1.brendakulfan.com/docs/CST6.pdf) To convert between airfoil coordinates and
+the CST parameterization, use the following functions: ```python from
+aerosandbox.geometry.airfoil.airfoil_families import get_kulfan_parameters,
+get_kulfan_coordinates ``` with documentation [here](https://
+aerosandbox.readthedocs.io/en/master/autoapi/aerosandbox/geometry/airfoil/
+airfoil_families/index.html) or in the source ([here](https://github.com/
+peterdsharpe/AeroSandbox/blob/8ad83aa4e4e40c503884c722143b7730c08089fa/
+aerosandbox/geometry/airfoil/airfoil_families.py#L128), [here](https://
+github.com/peterdsharpe/AeroSandbox/blob/
+8ad83aa4e4e40c503884c722143b7730c08089fa/aerosandbox/geometry/airfoil/
+airfoil_families.py#L265)). #### Training Data To be written, but in the
+meantime [see here](https://github.com/peterdsharpe/NeuralFoil/tree/master/
+training_data). Training data is not (yet) uploaded to GitHub, but will be soon
+- need to figure out Git LFS, as it's many gigabytes. Contact me if you need it
+sooner. ## FAQs Will NeuralFoil be integrated directly into [AeroSandbox]
+(https://github.com/peterdsharpe/AeroSandbox)? > Yes, absolutely. However, the
+goal is to keep this NeuralFoil repository also available as a stand-alone
+module, if desired. This simplifies dependencies for people using NeuralFoil in
+other applications (e.g., flight simulation, real-time control on embedded
+systems, etc.), and makes it easier if someone wanted to port NeuralFoil to
+another language (e.g., C++, for use on an Arduino).  Why not just use XFoil
+directly? > XFoil is a truly excellent piece of aerospace software engineering
+and is the gold standard of airfoil analysis, for good reason. When its
+assumptions hold (airfoils in subsonic flow without massive separation), its
+accuracy exceeds that of RANS CFD, yet it has ~1000x lower computational cost.
+XFoil shines in particular for human-in-the-loop airfoil design. However, XFoil
+is not the right tool for all applications, for a few reasons: > > - XFoil
+exhibits hysteresis: you can get slightly different solutions (for the same
+airfoil, $\alpha$, and $Re$) depending on whether you sweep $\alpha$ up or
+down, as Newton iteration is resumed from the last converged solution and
+uniqueness is not guaranteed. This hysteresis can be a big problem for design
+optimization. > - XFoil is not differentiable, in the sense that it doesn't
+tell you how performance changes w.r.t. airfoil shape (via, for example, an
+adjoint). That's okayâNeuralFoil doesn't either, at least out-of-the-box.
+However, the "path to obtain an efficient gradient" is very straightforward for
+NeuralFoil's pure NumPy code, where many excellent options exist (e.g., JAX).
+In contrast, gradient options for Fortran code (the language XFoil is in)
+either don't exist or are significantly less advanced (e.g., Tapenade). The
+most promising option for XFoil is probably [CMPLXFOIL](https://github.com/
+mdolab/CMPLXFOIL), which computes complex-step (effectively, forward-mode)
+gradients. However, even if you can get a gradient, it still may present
+issues, because... > - XFoil's solutions lack $C^1$-continuity. NeuralFoil, by
+contrast, is guaranteed to be $C^\infty$-continuous by construction. This is
+critical for gradient-based optimization. > - Even if one tries to compute
+gradients of XFoil's outputs by finite-differencing or complex-stepping, these
+gradients are often inaccurate. > - A bit into the weeds, but: this comes down
+to how XFoil handles transition (onset of turbulence). XFoil does a cut-cell
+approach on the transitioning interval, and while this specific cut-cell
+implementation restores $C^0$-continuity (i.e., transition won't truly "jump"
+from one node to another discretely), gradients of the laminar and turbulent BL
+closure functions still change at the cell interface due to the differing BL
+parameters ($H$ and $Re_\theta$) from node to node. This loses $C^1$
+continuity, causing a "ragged" polar at the microscopic level. In theory $C^1$-
+continuity could be restored by also blending the BL shape variables through
+the transitioning cell interval, but that unleashes some ugly integrals and is
+not done in XFoil. > - For more on this, see [Adler, Gray, and Martins, "To CFD
+or not to CFD?..."](http://websites.umich.edu/~mdolaboratory/pdf/
+Adler2022c.pdf), Figure 7. > - While XFoil is ~1000x faster than RANS CFD,
+NeuralFoil [can be another ~1000x faster to evaluate than XFoil](#performance).
+NeuralFoil is also much easier to interface with on a memory level than XFoil,
+which means you won't find yourself I/O bound from file reading/writing like
+you will with XFoil. > - XFoil is not vectorized, which exacerbates the speed
+advantage of a (vectorized) neural network when analyzing large batches of
+airfoil cases simultaneously. > - XFoil is not guaranteed to produce a
+solution. Instead, XFoil often crashes when "ambitious" calculations are
+attempted, rather than producing a less-accurate answer. In some applications,
+that's okay or even desirable; in others, that's a deal-breaker. Example
+applications where this is a problem include: > - Real-time control, where one
+wants to estimate forces (e.g., for a MPC trajectory), but you can't have the
+controller crash if XFoil fails to converge or hangs the CPU. > - Flight
+simulation: similar to real-time control where "a less-accurate answer" is much
+better than "no answer." > - Design optimization, where the optimizer needs "an
+answer" in order to recover from a bad design point and send the search back to
+a reasonable design. > - XFoil can be a serious pain to compile from source,
+which is often required if running on Mac or Linux (i.e., all supercomputers,
+some lab computers). NeuralFoil is pure Python and NumPy, so it's easy to
+install and run anywhere. Why not use a neural network trained on RANS CFD
+instead? > This is a cool idea too, and it has been done (See [Bouhlel, He, and
+Martins, "Scalable gradient-enhanced artificial..."](https://link.springer.com/
+article/10.1007/s00158-020-02488-5))! The fundamental challenge here, of
+course, is the cost of training data. RANS CFD is much more expensive than
+XFoil, so it's much harder to get sufficient training data to build a neural
+network that will generalize well out-of-sample. For example, in the linked
+work by Bouhlel et al., the authors trained a neural network on 42,000 RANS CFD
+runs (and they were sweeping over Mach as well, so the data becomes even
+sparser). In contrast, NeuralFoil was trained on tens of millions of XFoil
+runs. Ultimately, this exposes NeuralFoil to a much larger "span" of the
+airfoil design space, which is critical for accurate predictions on out-of-
 sample airfoils. > > One advantage of a RANS CFD approach over the NeuralFoil
 XFoil approach is, of course, transonic modeling. NeuralFoil attempts to get
 around this a little bit by estimating $C_{p, min}$, which in turn allows you
 to estimate the critical Mach number. (For an implementation of that, [see
 here](#extended-features-transonics-post-stall-control-surface-deflections))
 But fundamentally, NeuralFoil is likely less accurate in the transonic range
 because of this. The tradeoff is that the much larger training data set allows
@@ -259,38 +276,28 @@
 usually more accurate than RANS CFD](https://www.sciencedirect.com/science/
 article/abs/pii/S1270963816300839). Why not use a neural network trained on
 wind tunnel data? > This is a super-cool idea, and I'd love to see someone try
 it! My guess is that you'd need some kind of morphing wing section (and a way
 of precisely measuring the shape) in order to get enough data samples to "span"
 the airfoil design space. Then, you'd just let the wing section sit in the wind
 tunnel for a few days morphing itself around to collect data, then train a
-model on that. This would be really awesome, someone should do it!  Why
-parameterize the airfoil geometry using the CST (Kulfan) parameterization? What
-exactly does the CST parameterization mean, and how can I convert this
-parameterization to/from actual airfoil coordinates? Why discretize with 8 CST
-modes per side? Can NeuralFoil accurately analyze airfoils with thick trailing
-edges? > To be written, but in the meantime read: > - [D. A. Masters,
-"Geometric Comparison of Aerofoil Shape Parameterization Methods", AIAA
-Journal, 2017.](https://arc.aiaa.org/doi/pdf/10.2514/1.J054943) > - The seminal
-paper on the CST (Kulfan) parameterization technique: [Brenda Kulfan,
-"Universal Parametric Geometry Representation Method"](http://
-mx1.brendakulfan.com/docs/CST6.pdf) What's the underlying neural network
-architecture used in NeuralFoil? > To be written, but it is essentially a feed-
-forward neural network with a varying number of total layers and layer width
-depending on model size. Layer counts and widths were [determined through
-extensive trial and error](./training/supercloud_job_id_notes.log), in
-conjunction with observed test- and train-loss values. All layers are dense
-(fully connected, with weights and biases). All activation functions between
-layers are $\tanh$, to preserve $C^\infty$-continuity. The number of layers and
-layer width are as follows: > > * xxsmall: 2 layers, 32 wide. > * xsmall: 3
-layers, 32 wide. > * small: 3 layers, 48 wide. > * medium: 4 layers, 64 wide. >
-* large: 4 layers, 128 wide. > * xlarge: 4 layers, 256 wide. > * xxlarge: 5
-layers, 256 wide. > * xxxlarge:5 layers, 512 wide. ## Acknowledgements
-NeuralFoil was trained on MIT Supercloud, a high-performance computing cluster
-operated by the MIT Lincoln Laboratory Supercomputing Center (LLSC). ## License
-NeuralFoil is licensed under the MIT license. Please see the [LICENSE]
-(LICENSE.txt) file for details. ## Citing NeuralFoil If you use NeuralFoil in
-your research, please cite it as follows: ``` @misc{neuralfoil, author = {Peter
-Sharpe}, title = {{NeuralFoil}: An airfoil aerodynamics analysis tool using
-physics-informed machine learning}, year = {2023}, publisher = {GitHub},
-journal = {GitHub repository}, howpublished = {\url{https://github.com/
-peterdsharpe/NeuralFoil}}, ```
+model on that. This would be really awesome, someone should do it! What's the
+underlying neural network architecture used in NeuralFoil? > To be written, but
+it is essentially a feed-forward neural network with a varying number of total
+layers and layer width depending on model size. Layer counts and widths were
+[determined through extensive trial and error](./training/
+supercloud_job_id_notes.log), in conjunction with observed test- and train-loss
+values. All layers are dense (fully connected, with weights and biases). All
+activation functions between layers are $\tanh$, to preserve $C^\infty$-
+continuity. The number of layers and layer width are as follows: > > * xxsmall:
+2 layers, 32 wide. > * xsmall: 3 layers, 32 wide. > * small: 3 layers, 48 wide.
+> * medium: 4 layers, 64 wide. > * large: 4 layers, 128 wide. > * xlarge: 4
+layers, 256 wide. > * xxlarge: 5 layers, 256 wide. > * xxxlarge:5 layers, 512
+wide. ## Acknowledgements NeuralFoil was trained on MIT Supercloud, a high-
+performance computing cluster operated by the MIT Lincoln Laboratory
+Supercomputing Center (LLSC). ## License NeuralFoil is licensed under the MIT
+license. Please see the [LICENSE](LICENSE.txt) file for details. ## Citing
+NeuralFoil If you use NeuralFoil in your research, please cite it as follows:
+``` @misc{neuralfoil, author = {Peter Sharpe}, title = {{NeuralFoil}: An
+airfoil aerodynamics analysis tool using physics-informed machine learning},
+year = {2023}, publisher = {GitHub}, journal = {GitHub repository},
+howpublished = {\url{https://github.com/peterdsharpe/NeuralFoil}}, } ```
```

### Comparing `NeuralFoil-0.1.7/neuralfoil/CL_linear_regression.py` & `NeuralFoil-0.1.8/neuralfoil/CL_linear_regression.py`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.7/neuralfoil/neuralfoil.py` & `NeuralFoil-0.1.8/neuralfoil/neuralfoil.py`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-large.npz` & `NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-large.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-medium.npz` & `NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-medium.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-small.npz` & `NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-small.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-xlarge.npz` & `NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-xlarge.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-xsmall.npz` & `NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-xsmall.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz` & `NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-xxlarge.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz` & `NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-xxsmall.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.7/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz` & `NeuralFoil-0.1.8/neuralfoil/nn_weights_and_biases/nn-xxxlarge.npz`

 * *Files identical despite different names*

### Comparing `NeuralFoil-0.1.7/setup.py` & `NeuralFoil-0.1.8/setup.py`

 * *Files identical despite different names*

