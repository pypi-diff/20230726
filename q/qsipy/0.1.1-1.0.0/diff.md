# Comparing `tmp/qsipy-0.1.1.tar.gz` & `tmp/qsipy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsipy-0.1.1.tar", max compression
+gzip compressed data, was "qsipy-1.0.0.tar", max compression
```

## Comparing `qsipy-0.1.1.tar` & `qsipy-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11723 2023-07-26 10:33:07.970228 qsipy-0.1.1/README.md
--rw-r--r--   0        0        0      660 2023-07-26 10:43:33.486911 qsipy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       35 2023-07-12 16:09:47.384565 qsipy-0.1.1/src/qsipy/__init__.py
--rw-r--r--   0        0        0    25171 2023-07-26 09:56:14.876835 qsipy-0.1.1/src/qsipy/tfs.py
--rw-r--r--   0        0        0    25700 2023-07-26 10:42:18.940242 qsipy-0.1.1/src/qsipy/tms.py
--rw-r--r--   0        0        0      437 2023-07-12 16:09:47.384565 qsipy-0.1.1/src/qsipy/trigonometry.py
--rw-r--r--   0        0        0    12776 1970-01-01 00:00:00.000000 qsipy-0.1.1/setup.py
--rw-r--r--   0        0        0    12224 1970-01-01 00:00:00.000000 qsipy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    12188 2023-07-26 11:37:21.770331 qsipy-1.0.0/README.md
+-rw-r--r--   0        0        0      660 2023-07-26 11:37:21.773664 qsipy-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-07-26 11:37:21.773664 qsipy-1.0.0/src/qsipy/__init__.py
+-rw-r--r--   0        0        0    25171 2023-07-26 11:37:21.773664 qsipy-1.0.0/src/qsipy/tfs.py
+-rw-r--r--   0        0        0    25700 2023-07-26 11:37:21.773664 qsipy-1.0.0/src/qsipy/tms.py
+-rw-r--r--   0        0        0      437 2023-07-26 11:37:21.773664 qsipy-1.0.0/src/qsipy/trigonometry.py
+-rw-r--r--   0        0        0    13274 1970-01-01 00:00:00.000000 qsipy-1.0.0/setup.py
+-rw-r--r--   0        0        0    12689 1970-01-01 00:00:00.000000 qsipy-1.0.0/PKG-INFO
```

### Comparing `qsipy-0.1.1/README.md` & `qsipy-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,34 @@
 ## Quick context explanation
 
 The scheme of the experiment that we aer considering is represented with the figure below:
 ![scheme_experiment](images/schematic_exp.png)
 * **twin Fock** or **two-mode squeezed** states are used as *input* in a Mach-Zehnder interferometer ;
 * the detection suffers from a **non-unit quantum efficiency** $\eta$ ;
 * experimentalists are interested in the measurement of the phase difference $\phi$ between the two arms ;
-* the observable $\hat{O}$ that one use to perform a measurement is the **square** of the *half difference* of particles detected at both output ports $\hat{c}_1$ and $\hat{c}_2$, whose expectation value is actually the **variance** of the *half difference* of particles detected[^1]:
-    $$\hat{O} = \frac{1}{4} \left( \hat{N}_{c_2} - \hat{N}_{c_1} \right)^2$$
+* the observable $\hat{O}$ that one use to perform a measurement is the **square** of the *half difference* of particles detected at both output ports $\hat{c}_1$ and $\hat{c}_2$, whose expectation value is actually the **variance** of the *half difference* of particles detected (cf. note below):
+
+```math
+\hat{O} = \frac{1}{4} \left( \hat{N}_{c_2} - \hat{N}_{c_1} \right)^2
+```
+
 * detailed explanation about the derivation of the formulae are given in the [supplemental material](link) of the article ;
 
-[^1]: indeed, $\langle \hat{N}_{c_2} - \hat{N}_{c_1} \rangle = 0$, and therefore  $4 \times \mathrm{Var} \left[ \hat{O} \right] =  \left\langle \left(\hat{N}_{c_2} - \hat{N}_{c_1}\right)^2 \right\rangle - \left\langle \hat{N}_{c_2} - \hat{N}_{c_1} \right\rangle^2 = \left\langle \left(\hat{N}_{c_2} - \hat{N}_{c_1}\right)^2 \right\rangle$
+(note): indeed, 
+
+```math
+\langle\hat{N}_{c_2}-\hat{N}_{c_1}\rangle=0
+```
+
+and therefore 
+
+```math
+4\times\mathrm{Var}\left[\hat{O}\right]=\left\langle\left(\hat{N}_{c_2}-\hat{N}_{c_1}\right)^2\right\rangle-\left\langle\hat{N}_{c_2}-\hat{N}_{c_1}\right\rangle^2=\left\langle\left(\hat{N}_{c_2}-\hat{N}_{c_1}\right)^2\right\rangle
+```
+
 ---
 
 ## Installation
 
 #### Method 1: download from PyPI (recommended for users)
 This package is published in the PyPI repository, it can be added to any Python environment with
 the oneliner:
@@ -36,14 +51,18 @@
 no compilation is needed. The functions of interest are defined in two separate modules:
 * `src/qsipy/tfs.py` $\Rightarrow$ for the functions related to the *twin Fock states*
 * `src/qsipy/tms.py` $\Rightarrow$ for the functions related to the *two-mode squeezed vacuum states* 
 ---
 
 ## Examples
 
+**N.B.** the gain in decibels (relatively to the standard quantum limit) are defined as such:
+
+$$ G = 20 \log \left[ \sqrt{\eta N} \, \Delta \phi \right]$$ 
+
 #### 1. Phase uncertainty $\Delta \phi$ as a function of the measured phase difference
 
 The following figure shows the **ratio** between the **phase sensitivity** achieved with those two quantum states **and the shot-noise**. The quantum efficiency is set to $\eta = 0.95$. It shows in particular that interferometry [below the standard quantum limit (SQL)](https://arxiv.org/abs/1405.7703) can be obtained in specific ranges of phase differences $\phi$.
 
 ![tf_vs_tms](images/FIG_tf_vs_tms/qsipy_tf_vs_tms.png)
 
 The source code generating this figure [can be found here](images/FIG_tf_vs_tms/qsipy_tf_vs_tms.py).
@@ -58,14 +77,19 @@
 ![optimal_phi](images/FIG_optimal_phi/qsipy_optimal_phi.png)
 
 The source code generating this figure [can be found here](images/FIG_optimal_phi/qsipy_optimal_phi.py).
 
 #### 3. Asymptotic behaviour of the phase uncertainty
 
 Knowing the optimal phase $\phi_0$ to estimate, one can study the asymptotic behaviour of $\Delta \phi_0 = \left.\Delta \phi\right|_{\phi=\phi_0}$. One can therefore check that as soon as $\eta \neq 1$, $\Delta \phi_0$ has a $\mathcal{O}(N^{-1/2})$ scaling, therefore overtaking the standard quantum limit only by a constant factor.
+Here is a visualization of this asymptotic behaviour in the case $\eta = 0.95$
+
+![asymptotic_behaviour](images/FIG_asymptotic_behaviour/qsipy_asymptotic_behaviour.png)
+
+The source code generating this figure [can be found here](images/FIG_asymptotic_behaviour/qsipy_asymptotic_behaviour.py).
 
 ---
 
 ## User guide
 
 Currently the package is organized in two main modules `tfs` and `tms`, containing essentially the same functions, but considering either *twin Fock* or *two-mode squeezed* states at the input.
```

### Comparing `qsipy-0.1.1/pyproject.toml` & `qsipy-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
     name = "qsipy"
-    version = "0.1.1"
+    version = "1.0.0"
     description = "Quantum State Interferometry with PYthon."
     authors = ["Quentin Marolleau <quentin.marolleau@institutoptique.fr>"]
     license = "mit"
     readme = "README.md"
     packages = [{ include = "qsipy", from = "src" }]
 
     [tool.poetry.dependencies]
```

### Comparing `qsipy-0.1.1/src/qsipy/tfs.py` & `qsipy-1.0.0/src/qsipy/tfs.py`

 * *Files identical despite different names*

### Comparing `qsipy-0.1.1/src/qsipy/tms.py` & `qsipy-1.0.0/src/qsipy/tms.py`

 * *Files identical despite different names*

### Comparing `qsipy-0.1.1/setup.py` & `qsipy-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.25.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'qsipy',
-    'version': '0.1.1',
+    'version': '1.0.0',
     'description': 'Quantum State Interferometry with PYthon.',
-    'long_description': '# Python package about interferometry using two-mode quantum states\n\n## This package provides functions that return various physical quantities related to interferometry experiments using twin Fock states $|n,n\\rangle$ or two-mode squeezed vacuum states\n\n### Functions contained in this package are derived in [this article](link)\n* DOI: *paper published soon*\n---\n\n## Quick context explanation\n\nThe scheme of the experiment that we aer considering is represented with the figure below:\n![scheme_experiment](images/schematic_exp.png)\n* **twin Fock** or **two-mode squeezed** states are used as *input* in a Mach-Zehnder interferometer ;\n* the detection suffers from a **non-unit quantum efficiency** $\\eta$ ;\n* experimentalists are interested in the measurement of the phase difference $\\phi$ between the two arms ;\n* the observable $\\hat{O}$ that one use to perform a measurement is the **square** of the *half difference* of particles detected at both output ports $\\hat{c}_1$ and $\\hat{c}_2$, whose expectation value is actually the **variance** of the *half difference* of particles detected[^1]:\n    $$\\hat{O} = \\frac{1}{4} \\left( \\hat{N}_{c_2} - \\hat{N}_{c_1} \\right)^2$$\n* detailed explanation about the derivation of the formulae are given in the [supplemental material](link) of the article ;\n\n[^1]: indeed, $\\langle \\hat{N}_{c_2} - \\hat{N}_{c_1} \\rangle = 0$, and therefore  $4 \\times \\mathrm{Var} \\left[ \\hat{O} \\right] =  \\left\\langle \\left(\\hat{N}_{c_2} - \\hat{N}_{c_1}\\right)^2 \\right\\rangle - \\left\\langle \\hat{N}_{c_2} - \\hat{N}_{c_1} \\right\\rangle^2 = \\left\\langle \\left(\\hat{N}_{c_2} - \\hat{N}_{c_1}\\right)^2 \\right\\rangle$\n---\n\n## Installation\n\n#### Method 1: download from PyPI (recommended for users)\nThis package is published in the PyPI repository, it can be added to any Python environment with\nthe oneliner:\n`pip install qsipy`\n\nOr with any other Python packaging and dependency manager, such as poetry:\n`poetry add qsipy`\n\n#### Method 2: cloning from the source (for contributers)\n\nYou may also clone this project and use it right away. Since it is only Python scripts\nno compilation is needed. The functions of interest are defined in two separate modules:\n* `src/qsipy/tfs.py` $\\Rightarrow$ for the functions related to the *twin Fock states*\n* `src/qsipy/tms.py` $\\Rightarrow$ for the functions related to the *two-mode squeezed vacuum states* \n---\n\n## Examples\n\n#### 1. Phase uncertainty $\\Delta \\phi$ as a function of the measured phase difference\n\nThe following figure shows the **ratio** between the **phase sensitivity** achieved with those two quantum states **and the shot-noise**. The quantum efficiency is set to $\\eta = 0.95$. It shows in particular that interferometry [below the standard quantum limit (SQL)](https://arxiv.org/abs/1405.7703) can be obtained in specific ranges of phase differences $\\phi$.\n\n![tf_vs_tms](images/FIG_tf_vs_tms/qsipy_tf_vs_tms.png)\n\nThe source code generating this figure [can be found here](images/FIG_tf_vs_tms/qsipy_tf_vs_tms.py).\n\n#### 2. Maps of the optimal $\\phi_0$ to measure, and sub-shot-noise domains\n\nThe example 1. exhibited the fact that (for given quantum efficiency $\\eta$ and number of particles $N$) there is an optimal phase difference $\\phi_0$ to measure, in order to minimize the measurement uncertainty $\\Delta \\phi$. One can plot the maps of those optimal phases in the $(\\eta,N)$ plane, and identify the regions where sub-shot-noise interferometry may be performed.\n\n* `TF` stands for *twin Fock* state\n* `TMS` stands for *two-mode squeezed vacuum* state\n\n![optimal_phi](images/FIG_optimal_phi/qsipy_optimal_phi.png)\n\nThe source code generating this figure [can be found here](images/FIG_optimal_phi/qsipy_optimal_phi.py).\n\n#### 3. Asymptotic behaviour of the phase uncertainty\n\nKnowing the optimal phase $\\phi_0$ to estimate, one can study the asymptotic behaviour of $\\Delta \\phi_0 = \\left.\\Delta \\phi\\right|_{\\phi=\\phi_0}$. One can therefore check that as soon as $\\eta \\neq 1$, $\\Delta \\phi_0$ has a $\\mathcal{O}(N^{-1/2})$ scaling, therefore overtaking the standard quantum limit only by a constant factor.\n\n---\n\n## User guide\n\nCurrently the package is organized in two main modules `tfs` and `tms`, containing essentially the same functions, but considering either *twin Fock* or *two-mode squeezed* states at the input.\n\n**Important abbreviations:** for the sake of compactness we use the following abbreviation in the names of the functions provided by `qsipy`:\n* `ev` stands for *"expectation value"*\n* `vhd` stands for *"variance of the half difference"*\n* `qe` stands for *"quantum efficiency"* (i.e. the value of $\\eta$)\n\nHere is the listing of the useful functions that one can use, calling `tfs.`*myfunction*\nor `tfs.`*myfunction*:\n\n#### Most important functions\n\n```python\ndef phase_uncertainty_vhd(\n    phi: float | npt.NDArray[np.float_],\n    N: float | npt.NDArray[np.float_],\n    eta: float | npt.NDArray[np.float_] = 1,\n) -> float | npt.NDArray[np.float_]:\n    """Returns the phase uncertainty during an interferometry experiment using\n        - twin-Fock or two-mode squeezed states at the input (depending from which module\n            the function has been called);\n        - considering the variance of the half difference of particles detected at the\n            output as the observable of interest;\n\n    This function only calls either "phase_uncertainty_vhd_perfect_qe" or\n    "phase_uncertainty_vhd_finite_qe", depending on the value of eta that it is set as\n    argument.\n\n    Parameters\n    ----------\n    phi : float | npt.NDArray[np.float_]\n        Phase difference between both arms of the interferometer.\n    N : float | npt.NDArray[np.float_]\n        Total number of particles.\n    eta : float | npt.NDArray[np.float_], optional\n        Quantum efficiency of the detector, must be between 0 and 1, by default 1.\n\n    Returns\n    -------\n    float | npt.NDArray[np.float_]\n        Phase uncertainty.\n    """\n```\n\n```python\ndef optimal_phi_vhd(\n    N: float | npt.NDArray[np.float_],\n    eta: float | npt.NDArray[np.float_] = 1,\n) -> float | npt.NDArray[np.float_]:\n    """Returns the optimal phase to estimate (minimizing the resolution) during an\n    interferometry experiment using detectors with finite quantum efficiency and\n    considering the variance of the half difference of particles detected at the output\n    as the observable of interest. The detectors have a finite quantum efficiency eta.\n\n    Parameters\n    ----------\n    N : float | npt.NDArray[np.float_]\n        Total number of particles.\n    eta : float | npt.NDArray[np.float_], optional\n        Quantum efficiency of the detector, must be between 0 and 1, by default 1.\n\n    Returns\n    -------\n    float | npt.NDArray[np.float_]\n        Optimal phase to estimate experimentally.\n    """\n```\n\n```python\ndef phase_uncertainty_at_optimal_phi_vhd(\n    N: float | npt.NDArray[np.float_],\n    eta: float | npt.NDArray[np.float_] = 1,\n) -> float | npt.NDArray[np.float_]:\n    """Returns the resolution at the optimal phase to estimate during an interferometry\n    experiment using detectors with finite quantum efficiency eta and considering the\n    variance of the difference of particles at the output as the observable of interest.\n    This function is therefore just:\n\n    phase_resolution_difference_finite_qe(optimal_phi_vhd(n, eta), n, eta)\n\n    Parameters\n    ----------\n    N : float | npt.NDArray[np.float_]\n        Total number of particles.\n    eta : float | npt.NDArray[np.float_], optional\n        Quantum efficiency of the detector, must be between 0 and 1, by default 1.\n\n    Returns\n    -------\n    float | npt.NDArray[np.float_]\n        Optimal resolution.\n    """\n```\n\n#### Functions with more specific usage\n\n```python\ndef ev_vhd(\n    phi: float | npt.NDArray[np.float_],\n    N: float | npt.NDArray[np.float_],\n    eta: float | npt.NDArray[np.float_] = 1,\n) -> float | npt.NDArray[np.float_]:\n    """Returns the expectation value of the variance of the half difference of number of\n    particles detected at both output ports of the interferometer.\n    Since the expectation value of the difference itself is zero, the variance is\n    actually equal to the expectation value of the square of the difference.\n\n    This function only calls either "ev_vhd_perfect_qe" or "ev_vhd_finite_qe", depending\n    on the value of eta that it is set as argument.\n\n    Parameters\n    ----------\n    phi : float | npt.NDArray[np.float_]\n        Phase difference between both arms of the interferometer.\n    N : float | npt.NDArray[np.float_]\n        Average total number of particles in the interferometer.\n    eta : float | npt.NDArray[np.float_], optional\n        Quantum efficiency of the detector, must be between 0 and 1, by default 1.\n\n    Returns\n    -------\n    float | npt.NDArray[np.float_]\n        Expectation value: <(1/4) * (N_output1 - N_output2) ** 2>\n    """\n```\n\n```python\ndef ev_vhd_squared(\n    phi: float | npt.NDArray[np.float_],\n    N: float | npt.NDArray[np.float_],\n    eta: float | npt.NDArray[np.float_] = 1,\n) -> float | npt.NDArray[np.float_]:\n    """Returns the expectation value of the power four of the half difference of number\n    of particles detected at both output ports of the interferometer.\n\n    This function only calls either "ev_vhd_squared_perfect_qe" or\n    "ev_vhd_squared_finite_qe", depending on the value of eta that it is set as\n    argument.\n\n    Parameters\n    ----------\n    phi : float | npt.NDArray[np.float_]\n        Phase difference between both arms of the interferometer.\n    N : float | npt.NDArray[np.float_]\n        Total number of particles.\n    eta : float | npt.NDArray[np.float_], optional\n        Quantum efficiency of the detector, must be between 0 and 1, by default 1.\n\n    Returns\n    -------\n    float | npt.NDArray[np.float_]\n        Expectation value: <(1/16) * (N_output1 - N_output2) ** 4>\n    """\n```\n\n```python\ndef fluctuations_vhd(\n    phi: float | npt.NDArray[np.float_],\n    N: float | npt.NDArray[np.float_],\n    eta: float | npt.NDArray[np.float_] = 1,\n) -> float | npt.NDArray[np.float_]:\n    """Returns the quantum fluctuations of the variance of the half difference of number\n    of particles detected at both output ports of the interferometer.\n\n    This function only calls either "fluctuations_vhd_perfect_qe" or\n    "fluctuations_vhd_finite_qe", depending on the value of eta that it is set as\n    argument.\n\n    Parameters\n    ----------\n    phi : float | npt.NDArray[np.float_]\n        Phase difference between both arms of the interferometer.\n    N : float | npt.NDArray[np.float_]\n        Total number of particles.\n    eta : float | npt.NDArray[np.float_], optional\n        Quantum efficiency of the detector, must be between 0 and 1, by default 1.\n\n    Returns\n    -------\n    float | npt.NDArray[np.float_]\n        Expectation value: <Sqrt[Var( Var{ (1/2) * (N_output1 - N_output2) } )]>\n    """\n```\n\n```python\ndef asymptotic_ratio_phase_uncertainty_to_SQL_at_optimal_phi_vhd(\n    eta: float | npt.NDArray[np.float_],\n) -> float | npt.NDArray[np.float_]:\n    """Returns the asymptotic limit (as the number of particles goes to infinity) of the ratio between:\n        - the phase uncertainty at the optimal phase and considering the variance of the half difference\n        of particles detected at the output as the observable of interest\n        - the SQL 1/sqrt(eta N).\n\n    It only depends on the quantum efficiency of the detectors.\n\n    Parameters\n    ----------\n    eta : float | npt.NDArray[np.float_]\n        Quantum efficiency of the detector, must be between 0 and 1.\n\n    Returns\n    -------\n    float | npt.NDArray[np.float_]\n        Optimal phase uncertainty to SQL ratio in the asymptotic limit of N.\n    """\n```\n',
+    'long_description': '# Python package about interferometry using two-mode quantum states\n\n## This package provides functions that return various physical quantities related to interferometry experiments using twin Fock states $|n,n\\rangle$ or two-mode squeezed vacuum states\n\n### Functions contained in this package are derived in [this article](link)\n* DOI: *paper published soon*\n---\n\n## Quick context explanation\n\nThe scheme of the experiment that we aer considering is represented with the figure below:\n![scheme_experiment](images/schematic_exp.png)\n* **twin Fock** or **two-mode squeezed** states are used as *input* in a Mach-Zehnder interferometer ;\n* the detection suffers from a **non-unit quantum efficiency** $\\eta$ ;\n* experimentalists are interested in the measurement of the phase difference $\\phi$ between the two arms ;\n* the observable $\\hat{O}$ that one use to perform a measurement is the **square** of the *half difference* of particles detected at both output ports $\\hat{c}_1$ and $\\hat{c}_2$, whose expectation value is actually the **variance** of the *half difference* of particles detected (cf. note below):\n\n```math\n\\hat{O} = \\frac{1}{4} \\left( \\hat{N}_{c_2} - \\hat{N}_{c_1} \\right)^2\n```\n\n* detailed explanation about the derivation of the formulae are given in the [supplemental material](link) of the article ;\n\n(note): indeed, \n\n```math\n\\langle\\hat{N}_{c_2}-\\hat{N}_{c_1}\\rangle=0\n```\n\nand therefore \n\n```math\n4\\times\\mathrm{Var}\\left[\\hat{O}\\right]=\\left\\langle\\left(\\hat{N}_{c_2}-\\hat{N}_{c_1}\\right)^2\\right\\rangle-\\left\\langle\\hat{N}_{c_2}-\\hat{N}_{c_1}\\right\\rangle^2=\\left\\langle\\left(\\hat{N}_{c_2}-\\hat{N}_{c_1}\\right)^2\\right\\rangle\n```\n\n---\n\n## Installation\n\n#### Method 1: download from PyPI (recommended for users)\nThis package is published in the PyPI repository, it can be added to any Python environment with\nthe oneliner:\n`pip install qsipy`\n\nOr with any other Python packaging and dependency manager, such as poetry:\n`poetry add qsipy`\n\n#### Method 2: cloning from the source (for contributers)\n\nYou may also clone this project and use it right away. Since it is only Python scripts\nno compilation is needed. The functions of interest are defined in two separate modules:\n* `src/qsipy/tfs.py` $\\Rightarrow$ for the functions related to the *twin Fock states*\n* `src/qsipy/tms.py` $\\Rightarrow$ for the functions related to the *two-mode squeezed vacuum states* \n---\n\n## Examples\n\n**N.B.** the gain in decibels (relatively to the standard quantum limit) are defined as such:\n\n$$ G = 20 \\log \\left[ \\sqrt{\\eta N} \\, \\Delta \\phi \\right]$$ \n\n#### 1. Phase uncertainty $\\Delta \\phi$ as a function of the measured phase difference\n\nThe following figure shows the **ratio** between the **phase sensitivity** achieved with those two quantum states **and the shot-noise**. The quantum efficiency is set to $\\eta = 0.95$. It shows in particular that interferometry [below the standard quantum limit (SQL)](https://arxiv.org/abs/1405.7703) can be obtained in specific ranges of phase differences $\\phi$.\n\n![tf_vs_tms](images/FIG_tf_vs_tms/qsipy_tf_vs_tms.png)\n\nThe source code generating this figure [can be found here](images/FIG_tf_vs_tms/qsipy_tf_vs_tms.py).\n\n#### 2. Maps of the optimal $\\phi_0$ to measure, and sub-shot-noise domains\n\nThe example 1. exhibited the fact that (for given quantum efficiency $\\eta$ and number of particles $N$) there is an optimal phase difference $\\phi_0$ to measure, in order to minimize the measurement uncertainty $\\Delta \\phi$. One can plot the maps of those optimal phases in the $(\\eta,N)$ plane, and identify the regions where sub-shot-noise interferometry may be performed.\n\n* `TF` stands for *twin Fock* state\n* `TMS` stands for *two-mode squeezed vacuum* state\n\n![optimal_phi](images/FIG_optimal_phi/qsipy_optimal_phi.png)\n\nThe source code generating this figure [can be found here](images/FIG_optimal_phi/qsipy_optimal_phi.py).\n\n#### 3. Asymptotic behaviour of the phase uncertainty\n\nKnowing the optimal phase $\\phi_0$ to estimate, one can study the asymptotic behaviour of $\\Delta \\phi_0 = \\left.\\Delta \\phi\\right|_{\\phi=\\phi_0}$. One can therefore check that as soon as $\\eta \\neq 1$, $\\Delta \\phi_0$ has a $\\mathcal{O}(N^{-1/2})$ scaling, therefore overtaking the standard quantum limit only by a constant factor.\nHere is a visualization of this asymptotic behaviour in the case $\\eta = 0.95$\n\n![asymptotic_behaviour](images/FIG_asymptotic_behaviour/qsipy_asymptotic_behaviour.png)\n\nThe source code generating this figure [can be found here](images/FIG_asymptotic_behaviour/qsipy_asymptotic_behaviour.py).\n\n---\n\n## User guide\n\nCurrently the package is organized in two main modules `tfs` and `tms`, containing essentially the same functions, but considering either *twin Fock* or *two-mode squeezed* states at the input.\n\n**Important abbreviations:** for the sake of compactness we use the following abbreviation in the names of the functions provided by `qsipy`:\n* `ev` stands for *"expectation value"*\n* `vhd` stands for *"variance of the half difference"*\n* `qe` stands for *"quantum efficiency"* (i.e. the value of $\\eta$)\n\nHere is the listing of the useful functions that one can use, calling `tfs.`*myfunction*\nor `tfs.`*myfunction*:\n\n#### Most important functions\n\n```python\ndef phase_uncertainty_vhd(\n    phi: float | npt.NDArray[np.float_],\n    N: float | npt.NDArray[np.float_],\n    eta: float | npt.NDArray[np.float_] = 1,\n) -> float | npt.NDArray[np.float_]:\n    """Returns the phase uncertainty during an interferometry experiment using\n        - twin-Fock or two-mode squeezed states at the input (depending from which module\n            the function has been called);\n        - considering the variance of the half difference of particles detected at the\n            output as the observable of interest;\n\n    This function only calls either "phase_uncertainty_vhd_perfect_qe" or\n    "phase_uncertainty_vhd_finite_qe", depending on the value of eta that it is set as\n    argument.\n\n    Parameters\n    ----------\n    phi : float | npt.NDArray[np.float_]\n        Phase difference between both arms of the interferometer.\n    N : float | npt.NDArray[np.float_]\n        Total number of particles.\n    eta : float | npt.NDArray[np.float_], optional\n        Quantum efficiency of the detector, must be between 0 and 1, by default 1.\n\n    Returns\n    -------\n    float | npt.NDArray[np.float_]\n        Phase uncertainty.\n    """\n```\n\n```python\ndef optimal_phi_vhd(\n    N: float | npt.NDArray[np.float_],\n    eta: float | npt.NDArray[np.float_] = 1,\n) -> float | npt.NDArray[np.float_]:\n    """Returns the optimal phase to estimate (minimizing the resolution) during an\n    interferometry experiment using detectors with finite quantum efficiency and\n    considering the variance of the half difference of particles detected at the output\n    as the observable of interest. The detectors have a finite quantum efficiency eta.\n\n    Parameters\n    ----------\n    N : float | npt.NDArray[np.float_]\n        Total number of particles.\n    eta : float | npt.NDArray[np.float_], optional\n        Quantum efficiency of the detector, must be between 0 and 1, by default 1.\n\n    Returns\n    -------\n    float | npt.NDArray[np.float_]\n        Optimal phase to estimate experimentally.\n    """\n```\n\n```python\ndef phase_uncertainty_at_optimal_phi_vhd(\n    N: float | npt.NDArray[np.float_],\n    eta: float | npt.NDArray[np.float_] = 1,\n) -> float | npt.NDArray[np.float_]:\n    """Returns the resolution at the optimal phase to estimate during an interferometry\n    experiment using detectors with finite quantum efficiency eta and considering the\n    variance of the difference of particles at the output as the observable of interest.\n    This function is therefore just:\n\n    phase_resolution_difference_finite_qe(optimal_phi_vhd(n, eta), n, eta)\n\n    Parameters\n    ----------\n    N : float | npt.NDArray[np.float_]\n        Total number of particles.\n    eta : float | npt.NDArray[np.float_], optional\n        Quantum efficiency of the detector, must be between 0 and 1, by default 1.\n\n    Returns\n    -------\n    float | npt.NDArray[np.float_]\n        Optimal resolution.\n    """\n```\n\n#### Functions with more specific usage\n\n```python\ndef ev_vhd(\n    phi: float | npt.NDArray[np.float_],\n    N: float | npt.NDArray[np.float_],\n    eta: float | npt.NDArray[np.float_] = 1,\n) -> float | npt.NDArray[np.float_]:\n    """Returns the expectation value of the variance of the half difference of number of\n    particles detected at both output ports of the interferometer.\n    Since the expectation value of the difference itself is zero, the variance is\n    actually equal to the expectation value of the square of the difference.\n\n    This function only calls either "ev_vhd_perfect_qe" or "ev_vhd_finite_qe", depending\n    on the value of eta that it is set as argument.\n\n    Parameters\n    ----------\n    phi : float | npt.NDArray[np.float_]\n        Phase difference between both arms of the interferometer.\n    N : float | npt.NDArray[np.float_]\n        Average total number of particles in the interferometer.\n    eta : float | npt.NDArray[np.float_], optional\n        Quantum efficiency of the detector, must be between 0 and 1, by default 1.\n\n    Returns\n    -------\n    float | npt.NDArray[np.float_]\n        Expectation value: <(1/4) * (N_output1 - N_output2) ** 2>\n    """\n```\n\n```python\ndef ev_vhd_squared(\n    phi: float | npt.NDArray[np.float_],\n    N: float | npt.NDArray[np.float_],\n    eta: float | npt.NDArray[np.float_] = 1,\n) -> float | npt.NDArray[np.float_]:\n    """Returns the expectation value of the power four of the half difference of number\n    of particles detected at both output ports of the interferometer.\n\n    This function only calls either "ev_vhd_squared_perfect_qe" or\n    "ev_vhd_squared_finite_qe", depending on the value of eta that it is set as\n    argument.\n\n    Parameters\n    ----------\n    phi : float | npt.NDArray[np.float_]\n        Phase difference between both arms of the interferometer.\n    N : float | npt.NDArray[np.float_]\n        Total number of particles.\n    eta : float | npt.NDArray[np.float_], optional\n        Quantum efficiency of the detector, must be between 0 and 1, by default 1.\n\n    Returns\n    -------\n    float | npt.NDArray[np.float_]\n        Expectation value: <(1/16) * (N_output1 - N_output2) ** 4>\n    """\n```\n\n```python\ndef fluctuations_vhd(\n    phi: float | npt.NDArray[np.float_],\n    N: float | npt.NDArray[np.float_],\n    eta: float | npt.NDArray[np.float_] = 1,\n) -> float | npt.NDArray[np.float_]:\n    """Returns the quantum fluctuations of the variance of the half difference of number\n    of particles detected at both output ports of the interferometer.\n\n    This function only calls either "fluctuations_vhd_perfect_qe" or\n    "fluctuations_vhd_finite_qe", depending on the value of eta that it is set as\n    argument.\n\n    Parameters\n    ----------\n    phi : float | npt.NDArray[np.float_]\n        Phase difference between both arms of the interferometer.\n    N : float | npt.NDArray[np.float_]\n        Total number of particles.\n    eta : float | npt.NDArray[np.float_], optional\n        Quantum efficiency of the detector, must be between 0 and 1, by default 1.\n\n    Returns\n    -------\n    float | npt.NDArray[np.float_]\n        Expectation value: <Sqrt[Var( Var{ (1/2) * (N_output1 - N_output2) } )]>\n    """\n```\n\n```python\ndef asymptotic_ratio_phase_uncertainty_to_SQL_at_optimal_phi_vhd(\n    eta: float | npt.NDArray[np.float_],\n) -> float | npt.NDArray[np.float_]:\n    """Returns the asymptotic limit (as the number of particles goes to infinity) of the ratio between:\n        - the phase uncertainty at the optimal phase and considering the variance of the half difference\n        of particles detected at the output as the observable of interest\n        - the SQL 1/sqrt(eta N).\n\n    It only depends on the quantum efficiency of the detectors.\n\n    Parameters\n    ----------\n    eta : float | npt.NDArray[np.float_]\n        Quantum efficiency of the detector, must be between 0 and 1.\n\n    Returns\n    -------\n    float | npt.NDArray[np.float_]\n        Optimal phase uncertainty to SQL ratio in the asymptotic limit of N.\n    """\n```\n',
     'author': 'Quentin Marolleau',
     'author_email': 'quentin.marolleau@institutoptique.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `qsipy-0.1.1/PKG-INFO` & `qsipy-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsipy
-Version: 0.1.1
+Version: 1.0.0
 Summary: Quantum State Interferometry with PYthon.
 License: MIT
 Author: Quentin Marolleau
 Author-email: quentin.marolleau@institutoptique.fr
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,19 +24,34 @@
 ## Quick context explanation
 
 The scheme of the experiment that we aer considering is represented with the figure below:
 ![scheme_experiment](images/schematic_exp.png)
 * **twin Fock** or **two-mode squeezed** states are used as *input* in a Mach-Zehnder interferometer ;
 * the detection suffers from a **non-unit quantum efficiency** $\eta$ ;
 * experimentalists are interested in the measurement of the phase difference $\phi$ between the two arms ;
-* the observable $\hat{O}$ that one use to perform a measurement is the **square** of the *half difference* of particles detected at both output ports $\hat{c}_1$ and $\hat{c}_2$, whose expectation value is actually the **variance** of the *half difference* of particles detected[^1]:
-    $$\hat{O} = \frac{1}{4} \left( \hat{N}_{c_2} - \hat{N}_{c_1} \right)^2$$
+* the observable $\hat{O}$ that one use to perform a measurement is the **square** of the *half difference* of particles detected at both output ports $\hat{c}_1$ and $\hat{c}_2$, whose expectation value is actually the **variance** of the *half difference* of particles detected (cf. note below):
+
+```math
+\hat{O} = \frac{1}{4} \left( \hat{N}_{c_2} - \hat{N}_{c_1} \right)^2
+```
+
 * detailed explanation about the derivation of the formulae are given in the [supplemental material](link) of the article ;
 
-[^1]: indeed, $\langle \hat{N}_{c_2} - \hat{N}_{c_1} \rangle = 0$, and therefore  $4 \times \mathrm{Var} \left[ \hat{O} \right] =  \left\langle \left(\hat{N}_{c_2} - \hat{N}_{c_1}\right)^2 \right\rangle - \left\langle \hat{N}_{c_2} - \hat{N}_{c_1} \right\rangle^2 = \left\langle \left(\hat{N}_{c_2} - \hat{N}_{c_1}\right)^2 \right\rangle$
+(note): indeed, 
+
+```math
+\langle\hat{N}_{c_2}-\hat{N}_{c_1}\rangle=0
+```
+
+and therefore 
+
+```math
+4\times\mathrm{Var}\left[\hat{O}\right]=\left\langle\left(\hat{N}_{c_2}-\hat{N}_{c_1}\right)^2\right\rangle-\left\langle\hat{N}_{c_2}-\hat{N}_{c_1}\right\rangle^2=\left\langle\left(\hat{N}_{c_2}-\hat{N}_{c_1}\right)^2\right\rangle
+```
+
 ---
 
 ## Installation
 
 #### Method 1: download from PyPI (recommended for users)
 This package is published in the PyPI repository, it can be added to any Python environment with
 the oneliner:
@@ -51,14 +66,18 @@
 no compilation is needed. The functions of interest are defined in two separate modules:
 * `src/qsipy/tfs.py` $\Rightarrow$ for the functions related to the *twin Fock states*
 * `src/qsipy/tms.py` $\Rightarrow$ for the functions related to the *two-mode squeezed vacuum states* 
 ---
 
 ## Examples
 
+**N.B.** the gain in decibels (relatively to the standard quantum limit) are defined as such:
+
+$$ G = 20 \log \left[ \sqrt{\eta N} \, \Delta \phi \right]$$ 
+
 #### 1. Phase uncertainty $\Delta \phi$ as a function of the measured phase difference
 
 The following figure shows the **ratio** between the **phase sensitivity** achieved with those two quantum states **and the shot-noise**. The quantum efficiency is set to $\eta = 0.95$. It shows in particular that interferometry [below the standard quantum limit (SQL)](https://arxiv.org/abs/1405.7703) can be obtained in specific ranges of phase differences $\phi$.
 
 ![tf_vs_tms](images/FIG_tf_vs_tms/qsipy_tf_vs_tms.png)
 
 The source code generating this figure [can be found here](images/FIG_tf_vs_tms/qsipy_tf_vs_tms.py).
@@ -73,14 +92,19 @@
 ![optimal_phi](images/FIG_optimal_phi/qsipy_optimal_phi.png)
 
 The source code generating this figure [can be found here](images/FIG_optimal_phi/qsipy_optimal_phi.py).
 
 #### 3. Asymptotic behaviour of the phase uncertainty
 
 Knowing the optimal phase $\phi_0$ to estimate, one can study the asymptotic behaviour of $\Delta \phi_0 = \left.\Delta \phi\right|_{\phi=\phi_0}$. One can therefore check that as soon as $\eta \neq 1$, $\Delta \phi_0$ has a $\mathcal{O}(N^{-1/2})$ scaling, therefore overtaking the standard quantum limit only by a constant factor.
+Here is a visualization of this asymptotic behaviour in the case $\eta = 0.95$
+
+![asymptotic_behaviour](images/FIG_asymptotic_behaviour/qsipy_asymptotic_behaviour.png)
+
+The source code generating this figure [can be found here](images/FIG_asymptotic_behaviour/qsipy_asymptotic_behaviour.py).
 
 ---
 
 ## User guide
 
 Currently the package is organized in two main modules `tfs` and `tms`, containing essentially the same functions, but considering either *twin Fock* or *two-mode squeezed* states at the input.
```

