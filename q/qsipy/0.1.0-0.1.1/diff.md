# Comparing `tmp/qsipy-0.1.0.tar.gz` & `tmp/qsipy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsipy-0.1.0.tar", max compression
+gzip compressed data, was "qsipy-0.1.1.tar", max compression
```

## Comparing `qsipy-0.1.0.tar` & `qsipy-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-07-12 16:08:28.531229 qsipy-0.1.0/README.md
--rw-r--r--   0        0        0      660 2023-07-12 16:08:28.531229 qsipy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       35 2023-07-12 16:09:47.384565 qsipy-0.1.0/src/qsipy/__init__.py
--rw-r--r--   0        0        0    25087 2023-07-25 20:05:19.682971 qsipy-0.1.0/src/qsipy/tfs.py
--rw-r--r--   0        0        0    25521 2023-07-25 20:10:05.862971 qsipy-0.1.0/src/qsipy/tms.py
--rw-r--r--   0        0        0      437 2023-07-12 16:09:47.384565 qsipy-0.1.0/src/qsipy/trigonometry.py
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 qsipy-0.1.0/setup.py
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 qsipy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11723 2023-07-26 10:33:07.970228 qsipy-0.1.1/README.md
+-rw-r--r--   0        0        0      660 2023-07-26 10:43:33.486911 qsipy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-07-12 16:09:47.384565 qsipy-0.1.1/src/qsipy/__init__.py
+-rw-r--r--   0        0        0    25171 2023-07-26 09:56:14.876835 qsipy-0.1.1/src/qsipy/tfs.py
+-rw-r--r--   0        0        0    25700 2023-07-26 10:42:18.940242 qsipy-0.1.1/src/qsipy/tms.py
+-rw-r--r--   0        0        0      437 2023-07-12 16:09:47.384565 qsipy-0.1.1/src/qsipy/trigonometry.py
+-rw-r--r--   0        0        0    12776 1970-01-01 00:00:00.000000 qsipy-0.1.1/setup.py
+-rw-r--r--   0        0        0    12224 1970-01-01 00:00:00.000000 qsipy-0.1.1/PKG-INFO
```

### Comparing `qsipy-0.1.0/pyproject.toml` & `qsipy-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
     name = "qsipy"
-    version = "0.1.0"
+    version = "0.1.1"
     description = "Quantum State Interferometry with PYthon."
     authors = ["Quentin Marolleau <quentin.marolleau@institutoptique.fr>"]
     license = "mit"
     readme = "README.md"
     packages = [{ include = "qsipy", from = "src" }]
 
     [tool.poetry.dependencies]
```

### Comparing `qsipy-0.1.0/src/qsipy/tfs.py` & `qsipy-0.1.1/src/qsipy/tfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 analytical form.
 
 abbreviations:
 --------------
     - ev: Expectation Value
     - vhd: Variance of the Half Difference of the number of particles at the output
         (i.e. our observable)
+    - qe: Quantum efficiency (i.e. the value of η)
 
 general notations:
 ------------------
     - N: the total number of particles in the interferometer. It corresponds to the
         main experimental resource.
     - phi: the phase difference between both arms of the interferometer
     - eta: quantum efficiency of the detectors (between 0 and 1). More generally it may
@@ -452,18 +453,18 @@
 
 
 def optimal_phi_vhd(
     N: int | npt.NDArray[np.int_],
     eta: float | npt.NDArray[np.float_] = 1,
 ) -> float | npt.NDArray[np.float_]:
     """Returns the optimal phase to estimate (minimizing the resolution) during an
-    interferometry experiment using twin-Fock states, detectors with finite quantum
-    efficiency and considering the variance of the difference of particles at the
-    output as the observable of interest. The detectors have a finite quantum efficiency
-    eta.
+    interferometry experiment using a twin-Fock state, detectors with finite quantum
+    efficiency and considering the variance of the half difference of particles detected
+    at the output as the observable of interest. The detectors have a finite quantum
+    efficiency eta.
 
     Parameters
     ----------
     N : int | npt.NDArray[np.int_]
         Total number of particles. The input state being the twin-Fock |N/2,N/2>.
     eta : float | npt.NDArray[np.float_], optional
         Quantum efficiency of the detector, must be between 0 and 1, by default 1.
@@ -509,20 +510,20 @@
 
 
 def phase_uncertainty_at_optimal_phi_vhd(
     N: int | npt.NDArray[np.int_],
     eta: float | npt.NDArray[np.float_] = 1,
 ) -> float | npt.NDArray[np.float_]:
     """Returns the resolution at the optimal phase to estimate during an interferometry
-    experiment using twin-Fock states, detectors with finite quantum efficiency eta and
-    considering the variance of the difference of particles at the output as the
-    observable of interest.
+    experiment using a twin-Fock state, detectors with finite quantum efficiency eta and
+    considering the variance of the half difference of particles detected at the output
+    as the observable of interest.
     This function is therefore just:
 
-    phase_resolution_difference_finite_qe(optimal_phi_difference(n, eta), n, eta)
+    phase_resolution_difference_finite_qe(optimal_phi_vhd(n, eta), n, eta)
 
     Parameters
     ----------
     N : int | npt.NDArray[np.int_]
         Total number of particles. The input state being the twin-Fock |N/2,N/2>.
     eta : float | npt.NDArray[np.float_], optional
         Quantum efficiency of the detector, must be between 0 and 1, by default 1.
@@ -663,15 +664,15 @@
 
 
 def asymptotic_ratio_phase_uncertainty_to_SQL_at_optimal_phi_vhd(
     eta: float | npt.NDArray[np.float_],
 ) -> float | npt.NDArray[np.float_]:
     """Returns the asymptotic limit (as the number of particles goes to infinity) of the ratio between:
         - the phase uncertainty at the optimal phase and considering the variance of the half difference
-        of particles at the output as the observable of interest
+        of particles detected at the output as the observable of interest
         - the SQL 1/sqrt(eta N).
 
     It only depends on the quantum efficiency of the detectors.
 
     Parameters
     ----------
     eta : float | npt.NDArray[np.float_]
```

### Comparing `qsipy-0.1.0/src/qsipy/tms.py` & `qsipy-0.1.1/src/qsipy/tms.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 analytical form.
 
 abbreviations:
 --------------
     - ev: Expectation Value
     - vhd: Variance of the Half Difference of the number of particles at the output
         (i.e. our observable)
+    - qe: Quantum efficiency (i.e. the value of η)
 
 general notations:
 ------------------
     - N: the average  total number of particles in the interferometer. It corresponds to
     the main experimental resource.
     - phi: the phase difference between both arms of the interferometer
     - eta: quantum efficiency of the detectors (between 0 and 1). More generally it may
@@ -461,18 +462,18 @@
 
 
 def optimal_phi_vhd(
     N: float | npt.NDArray[np.float_],
     eta: float | npt.NDArray[np.float_] = 1,
 ) -> float | npt.NDArray[np.float_]:
     """Returns the optimal phase to estimate (minimizing the resolution) during an
-    interferometry experiment using twin-Fock states, detectors with finite quantum
-    efficiency and considering the variance of the difference of particles at the
-    output as the observable of interest. The detectors have a finite quantum efficiency
-    eta.
+    interferometry experiment using a two-mode squeezed vacuum state, detectors with
+    finite quantum efficiency and considering the variance of the half difference of
+    particles detected at the output as the observable of interest. The detectors have
+    a finite quantum efficiency eta.
 
     Parameters
     ----------
     N : float | npt.NDArray[np.float_]
         Average total number of particles. The input state being the two-mode squeezed vacuum
         state with N/2 particles per mode on average.
     eta : float | npt.NDArray[np.float_], optional
@@ -509,23 +510,23 @@
             )
         ),
     )
 
 
 def phase_uncertainty_at_optimal_phi_vhd(
     N: float | npt.NDArray[np.float_],
-    eta: float | npt.NDArray[np.float_],
+    eta: float | npt.NDArray[np.float_] = 1,
 ) -> float | npt.NDArray[np.float_]:
     """Returns the resolution at the optimal phase to estimate during an interferometry
-    experiment using twin-Fock states, detectors with finite quantum efficiency eta and
-    considering the variance of the difference of particles at the output as the
-    observable of interest.
+    experiment using a two-mode squeezed vacuum state, detectors with finite quantum
+    efficiency eta and considering the variance of the half difference of particles
+    detected at the output as the observable of interest.
     This function is therefore just:
 
-    phase_resolution_difference_finite_qe(optimal_phi_difference(n, eta), n, eta)
+    phase_resolution_difference_finite_qe(optimal_phi_vhd(n, eta), n, eta)
 
     Parameters
     ----------
     N : float | npt.NDArray[np.float_]
         Average total number of particles. The input state being the two-mode squeezed vacuum
         state with N/2 particles per mode on average.
     eta : float | npt.NDArray[np.float_], optional
@@ -533,15 +534,17 @@
 
     Returns
     -------
     float | npt.NDArray[np.float_]
         Optimal resolution.
     """
     nu = N / 2
-    return (
+    return np.where(
+        eta == 1,
+        1 / np.sqrt(N * (N + 2)),
         1
         / (2 * np.sqrt(2) * eta**2 * nu * (1 + nu))
         * np.sqrt(
             eta
             * nu
             * (
                 1
@@ -659,24 +662,24 @@
                                 )
                             )
                         )
                     )
                     / (1 - eta + 10 * (-1 + eta) ** 2 * eta * nu)
                 )
             )
-        )
+        ),
     )
 
 
 def asymptotic_ratio_phase_uncertainty_to_SQL_at_optimal_phi_vhd(
     eta: float | npt.NDArray[np.float_],
 ) -> float | npt.NDArray[np.float_]:
     """Returns the asymptotic limit (as the number of particles goes to infinity) of the ratio between:
         - the phase uncertainty at the optimal phase and considering the variance of the half difference
-        of particles at the output as the observable of interest
+        of particles detected at the output as the observable of interest
         - the SQL 1/sqrt(eta N).
 
     It only depends on the quantum efficiency of the detectors.
 
     Parameters
     ----------
     eta : float | npt.NDArray[np.float_]
```

