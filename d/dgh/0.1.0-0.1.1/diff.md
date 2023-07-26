# Comparing `tmp/dgh-0.1.0.tar.gz` & `tmp/dgh-0.1.1.tar.gz`

## Comparing `dgh-0.1.0.tar` & `dgh-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,13 @@
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 dgh-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0    10558 2020-02-02 00:00:00.000000 dgh-0.1.0/illustration.pdf
--rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 dgh-0.1.0/illustration.svg
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 dgh-0.1.0/illustration_wide.pdf
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 dgh-0.1.0/illustration_wide_tall.pdf
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 dgh-0.1.0/dgh/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 dgh-0.1.0/dgh/constants.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 dgh-0.1.0/dgh/dgh.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 dgh-0.1.0/dgh/fw.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 dgh-0.1.0/dgh/mappings.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 dgh-0.1.0/dgh/spaces.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dgh-0.1.0/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 dgh-0.1.0/LICENSE
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 dgh-0.1.0/README.md
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dgh-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 dgh-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 dgh-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 dgh-0.1.1/illustration.svg
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 dgh-0.1.1/dgh/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 dgh-0.1.1/dgh/constants.py
+-rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 dgh-0.1.1/dgh/dgh.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 dgh-0.1.1/dgh/fw.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 dgh-0.1.1/dgh/mappings.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 dgh-0.1.1/dgh/spaces.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dgh-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 dgh-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 dgh-0.1.1/README.md
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dgh-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 dgh-0.1.1/PKG-INFO
```

### Comparing `dgh-0.1.0/CHANGELOG.md` & `dgh-0.1.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,48 @@
 # Changelog
 
 <!--next-version-placeholder-->
+## v0.1.1 (Jul 25 2023)
+
+### Feature
+
+- Renamed `ub()` to `upper()`
+
+### Fix
+
+- Corrected random number generator state in the search for best $c$ and its effects on the subsequent computations
+
+### Documentation
+
+- Added link to the paper
+- Added "Basics" section
+- Layout and readability improvements
+
 ## v0.1.0 (Jul 24 2023)
 
 ### Feature
 
-- Added searching for best c as default behavior
-- Added function for random generation of a bi-mapping polytope vertex R
+- Added searching for best $c$ as default behavior
+- Added function for random generation of a bi-mapping polytope vertex $\mathbf{R}$
 - Added `__version__` variable
 - Python >= 3.8 is now required
 
 ### Fix
 
-- Removed convexity-based calculation of c and warm-start sequences of c due to inefficiency
+- Removed convexity-based calculation of $c$ and warm-start sequences of $c$ due to inefficiency
 
 ### Documentation
 
-- Created "Advanced" section where the logic behind parameter c is explained
+- Created "Advanced" section where the logic behind parameter $c$ is explained
 
 ## v0.0.8 (May 11 2023)
 
 ### Feature
 
-- Added f, g to verbose output if returning them
+- Added $(f, g)$ to verbose output if returning the mappings
 
 ### Fix
 
 - Corrected (halved) ub in summary (verbose > 0)
 
 ### Documentation
```

### Comparing `dgh-0.1.0/illustration.svg` & `dgh-0.1.1/illustration.svg`

 * *Files identical despite different names*

### Comparing `dgh-0.1.0/dgh/dgh.py` & `dgh-0.1.1/dgh/dgh.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,31 +20,32 @@
     S_Y_X = S @ _Y_X
 
     dis_S = np.abs(X__Y - S @ Y__X @ S.T + S_Y_X - S_Y_X.T).max()
 
     return dis_S
 
 
-def ub(X, Y, c='auto', iter_budget=100, center_start=False, tol=1e-8, return_fg=False,
-       lower=0, validate_tri_ineq=False, verbose=0, rnd=None):
+def upper(X, Y, c='auto', iter_budget=100, center_start=False, tol=1e-8,
+          return_fg=False, lb=0, validate_tri_ineq=False, verbose=0, rnd=None):
     """
     Find upper bound of dGH(X, Y) by minimizing smoothed dis(R) = dis(f, g) over
     the bi-mapping polytope 𝓢 using Frank-Wolfe.
 
     :param X: distance matrix of X (2d-array)
     :param Y: distance matrix of Y (2d-array)
     :param c: exponentiation base ∈ (1, ∞) for smoothing the distortion
         in the first minimization problem (float)
     :param iter_budget: total number of Frank-Wolfe iterations (int)
     :param center_start: whether to try the center of 𝓢 as a starting point first (bool)
     :param tol: tolerance to use when evaluating convergence (float)
     :param return_fg: whether to return the optimal pair of mappings (bool)
-    :param lower: lower bound of dGH(X, Y) to avoid redundant iterations (float)
+    :param lb: lower bound of dGH(X, Y) to avoid redundant iterations (float)
     :param validate_tri_ineq: whether to validate the triangle inequality (bool)
     :param verbose: no output if 0, summary if >0, restarts if >1, iterations if >2
+    :param rnd: random number generator to use for restarts
     :return: dGH(X, Y), f [optional], g [optional]
     """
     # Check that the distances satisfy the metric properties minus the triangle inequality.
     assert (X >= 0).all() and (Y >= 0).all(), 'distance matrices have negative entries'
     assert (np.diag(X) == 0).all() and (np.diag(Y) == 0).all(),\
         'distance matrices have non-zeros on the main diagonal'
     assert (X == X.T).all() and (Y == Y.T).all(), 'distance matrices are not symmetric'
@@ -56,42 +57,49 @@
     n, m = len(X), len(Y)
     rnd = rnd or np.random.RandomState(DEFAULT_SEED)
     best_dis_R = np.inf
 
     # Update lower bound using the radius and diameter differences.
     diam_X, diam_Y = map(diam, [X, Y])
     rad_X, rad_Y = map(rad, [X, Y])
-    lower = max(lower, abs(diam_X - diam_Y)/2, abs(rad_X - rad_Y)/2)
+    lb = max(lb, abs(diam_X - diam_Y)/2, abs(rad_X - rad_Y)/2)
 
     if verbose > 0:
-        print(f'iteration budget {iter_budget} | c={c} | | dGH≥{lower}')
+        print(f'iteration budget {iter_budget} | c={c} | | dGH≥{lb}')
 
     # Search for best c if not specified.
     if c == 'auto':
         # Allocate 50% of iteration budget for the search.
         search_iter_budget_per_c = iter_budget // (2*len(C_SEARCH_GRID))
         search_iter_budget = search_iter_budget_per_c * len(C_SEARCH_GRID)
         iter_budget -= search_iter_budget
 
         # Select c resulting in the smallest upper bound.
+        init_rnd_state = rnd.get_state()
         for c_test in C_SEARCH_GRID:
-            upper, f, g = ub(X, Y, c=c_test, iter_budget=search_iter_budget_per_c,
-                             center_start=center_start, tol=tol, return_fg=True)
-            if upper < best_dis_R/2:
+            rnd.set_state(init_rnd_state)
+            ub, f, g = upper(X, Y, c=c_test, iter_budget=search_iter_budget_per_c,
+                             center_start=center_start, tol=tol, return_fg=True,
+                             lb=lb, rnd=rnd)
+            if ub < best_dis_R/2:
                 c = c_test
+                rnd_state = rnd.get_state()
                 best_f, best_g = f, g
-                best_dis_R = 2*upper
+                best_dis_R = 2*ub
+
+        # Set random number generator to after the search iterations.
+        rnd.set_state(rnd_state)
 
         if verbose > 0:
             print(f'spent {search_iter_budget} iterations to choose c={c}')
 
     # Scale all distances to avoid overflow.
     d_max = max(diam_X, diam_Y)
     X, Y = map(lambda Z: Z.copy() / d_max, [X, Y])
-    lower /= d_max
+    lb /= d_max
 
     # Find minima from new restarts until iteration budget is depleted.
     restart_idx = 0
     fw = make_frank_wolfe_solver(X, Y, c, tol=tol, verbose=verbose)
     while iter_budget > 0:
         # Initialize new restart.
         S0 = center(n, m) if restart_idx == 0 and center_start else rnd_S(n, m, rnd)
@@ -116,15 +124,15 @@
             fg_descr = f' | f={best_f}, g={best_g}' if return_fg else ''
             print(f'restart {restart_idx} ({used_iter} iterations) | '
                   f'½dis(R)={dis_R/2:.4f} | min ½dis(R)={best_dis_R/2:.4f}{fg_descr}')
 
         restart_idx += 1
 
         # Terminate if achieved lower bound.
-        if best_dis_R <= lower:
+        if best_dis_R <= lb:
             break
 
     if verbose > 0:
         print(f'proved dGH≤{best_dis_R/2} after {restart_idx} restarts')
 
     res = (best_dis_R/2, best_f, best_g) if return_fg else best_dis_R/2
```

### Comparing `dgh-0.1.0/dgh/fw.py` & `dgh-0.1.1/dgh/fw.py`

 * *Files identical despite different names*

### Comparing `dgh-0.1.0/dgh/mappings.py` & `dgh-0.1.1/dgh/mappings.py`

 * *Files identical despite different names*

### Comparing `dgh-0.1.0/dgh/spaces.py` & `dgh-0.1.1/dgh/spaces.py`

 * *Files identical despite different names*

### Comparing `dgh-0.1.0/LICENSE` & `dgh-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dgh-0.1.0/README.md` & `dgh-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,90 @@
 # dGH
 
-Computes the Gromov–Hausdorff distance $$d_\text{GH}(X, Y) = \frac{1}{2}\inf_{f:X\to Y, g:Y\to X} \text{dis}\Big(\\{(x, f(x)): x \in X\\} \cup \\{(g(y), y): y \in Y\\}\Big),$$ where $\text{dis}(R) = \sup_{(x, y), (x', y') \in R} |d_X(x, x') - d_Y(y, y')|$ for $R \subseteq X \times Y,$ by solving its parametric relaxation whose solutions are guaranteed to deliver $d_\text{GH}(X, Y)$ for sufficiently large value of the parameter $c$. The quadratic relaxation with affine constraints is solved using the Frank–Wolfe algorithm in $O(n^3)$ time per its iteration, where $n = |X| + |Y|$ is the total number of points. Even when the algorithm fails to find a global minimum, the resulting solution provides an upper bound for $d_\text{GH}(X, Y)$.
+Given the distance matrices of some metric spaces $X$ and $Y$, estimates the Gromov–Hausdorff distance $$d_\text{GH}(X, Y) = \frac{1}{2}\inf_{f:X\to Y, g:Y\to X} \text{dis}\Big(\\{(x, f(x)): x \in X\\} \cup \\{(g(y), y): y \in Y\\}\Big),$$ where $$\text{dis}(R) = \sup_{(x, y), (x', y') \in R} |d_X(x, x') - d_Y(y, y')|$$ for $R \subseteq X \times Y$.
 
-A manuscript describing the underlying theory is currently in preparation.
+The distance is estimated from above by solving its parametric relaxation whose solutions are guaranteed to deliver $d_\text{GH}(X, Y)$ for sufficiently large value of the parameter $c$. The quadratic relaxation with affine constraints is solved using the Frank–Wolfe algorithm in $O(n^3)$ time per its iteration, where $n = \max\{|X|, |Y|\}$ is the number of points in the larger space. Even if the algorithm fails to find $d_\text{GH}(X, Y)$ exactly, the resulting solution provides its upper bound.
+
+A detailed description of the relaxation, its optimality guarantees and optimization landscape, and the approach to solving it can be found in [Computing the Gromov–Hausdorff distance using first-order methods](https://arxiv.org/pdf/2307.13660.pdf).
 
 ## Quickstart
 
-Installing the package from Python Package Index:
+To install the package from Python Package Index:
 
 ```$ pip install dgh```
 
-Computing $d_\text{GH}(X, Y)$ where $X$ is the vertices of a tall narrow rectangle and $Y$ is the vertices of a small equilateral triangle together with a remote point from it (see illustration):
+Consider an example in which $X$ is comprised by the vertices of a $1 \times 10$ rectangle and $Y$ — by the vertices of a unit equilateral triangle together with a point that is 10 away fom them (see illustration).
 
 <p align="center">
     <img src="https://github.com/vlad-oles/dgh/blob/main/illustration.svg" alt="Illustration of the example" width="300"/>
 </p>
 
+To create their distance matrices (in which the (i,j)-th entry contains the distance between the i-th and j-th points of the space):
+
 ```
 import numpy as np
-import dgh
 
-# Set distance matrix for the rectangle.
 X = np.array([[0, 1, 10, 10],
               [0, 0, 10, 10],
               [0, 0, 0, 1],
               [0, 0, 0, 0]])
 X += X.T
 
-# Set distance matrix for the triangle and a remote point.
 Y = np.array([[0, 1, 1, 10],
               [0, 0, 1, 10],
               [0, 0, 0, 10],
               [0, 0, 0, 0]])
 Y += Y.T
+```
+
+To compute (an upper bound of) their Gromov--Hausdorff distance $d_\text{GH}(X, Y)$:
+
+```
+import dgh
 
-# Find an upper bound of the Gromov–Hausdorff distance. In this case, dGH(X, Y) = 0.5.
-dGH = dgh.ub(X, Y)
+dGH = dgh.upper(X, Y)
 ```
 
-Increasing the budget of Frank–Wolfe iterations, and thus the number of restarts, allocated for the search (the default budget is 100):
+In this case, the distance is computed exactly as $d_\text{GH}(X, Y)=\frac{1}{2}$. 
+
+## Basics
 
-```dGH = dgh.ub(X, Y, iter_budget=1000)```
+By default, the computational budget allocated for the search is 100 Frank–Wolfe iterations. Bigger budget means more random restarts (and/or better convergence) and therefore the accuracy. To set the budget:
 
-Obtaining the mappings $f:X\to Y, g:Y\to X$ (as arrays s.t. $f_i = j \Leftrightarrow f(x_i) = y_j$) that deliver the found minimum:
+```dGH = dgh.upper(X, Y, iter_budget=my_budget)```
 
-```dGH, f, g = dgh.ub(X, Y, return_fg=True)```
+To obtain the mappings $f:X\to Y, g:Y\to X$ (as arrays s.t. $f_i = j \Leftrightarrow f(x_i) = y_j$) that deliver the found minimum:
+
+```dGH, f, g = dgh.upper(X, Y, return_fg=True)```
 
 ## Advanced
 The performance can be improved by explicitly specifying the relaxation parameter $c \in (1, \infty)$. Small $c$ makes the relaxation easier to solve, but its solutions are more likely to deliver the Gromov–Hausdorff distance when $c$ is large.
 
-By default, the method allocates half of the iteration budget to select the best value of $c$ for $(X, Y)$ from $1+10^{-4}, 1+10^{-2},\ldots,1+10^8$, and then spends the remaining half on refining the Gromov–Hausdorff distance using this $c$. Revealing the value of $c$ selected after the search:
+By default, the method allocates half of the iteration budget to select the best value of $c$ for $(X, Y)$ from $1+10^{-4}, 1+10^{-2},\ldots,1+10^8$, and then spends the remaining half on refining the Gromov–Hausdorff distance using this $c$.
+
+To reveal the value of $c$ selected after the search:
 
-```dgh.ub(X, Y, verbose=1)```
+```dgh.upper(X, Y, verbose=1)```
 
-Explicitly providing $c$ to the method (to avoid search and/or to test for better accuracy):
+To compute for specific value of $c$ (to avoid spending iterations on the search and/or to test for better accuracy):
 
-```dGH = dgh.ub(X, Y, c=my_c)```
+```dGH = dgh.upper(X, Y, c=my_c)```
 
 
 ## Contributing
 If you found a bug or want to suggest an enhancement, you can create a [GitHub Issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue). Alternatively, you can email vlad.oles (at) proton (dot) me.
 
 ## License
 dGH is released under the MIT license.
+
+## Research
+To cite dGH, you can use the following:
+<blockquote>
+<p>Oles, V. (2023). Computing the Gromov–Hausdorff distance using first-order methods. <i>arXiv preprint arXiv:2307.13660</i>.</p>
+</blockquote>
+<pre><code>@article{oles2023computing,
+  title={Computing the Gromov--Hausdorff distance using first-order methods},
+  author={Oles, Vladyslav},
+  journal={arXiv preprint arXiv:2307.13660},
+  year={2023}
+}
+</code></pre>
```

### Comparing `dgh-0.1.0/pyproject.toml` & `dgh-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dgh"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Vladyslav Oles", email="vlad.oles@proton.me"},
 ]
 description = "Computing the Gromov–Hausdorff distance"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

