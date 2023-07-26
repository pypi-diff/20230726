# Comparing `tmp/hypigu-1.3.tar.gz` & `tmp/hypigu-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypigu-1.3.tar", last modified: Fri Jun 24 11:51:39 2022, max compression
+gzip compressed data, was "hypigu-1.4.tar", last modified: Wed Jul 26 08:41:16 2023, max compression
```

## Comparing `hypigu-1.3.tar` & `hypigu-1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-06-24 11:51:39.772154 hypigu-1.3/
--rw-rw-rw-   0        0        0     1097 2022-06-24 11:49:19.000000 hypigu-1.3/LICENSE
--rw-rw-rw-   0        0        0     2640 2022-06-24 11:51:39.772154 hypigu-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1928 2022-06-24 11:49:19.000000 hypigu-1.3/README.md
-drwxrwxrwx   0        0        0        0 2022-06-24 11:51:39.724213 hypigu-1.3/hypigu/
--rw-rw-rw-   0        0        0      563 2022-06-24 11:49:19.000000 hypigu-1.3/hypigu/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-24 11:51:39.770152 hypigu-1.3/hypigu/src/
--rw-rw-rw-   0        0        0     4573 2021-03-08 12:28:42.000000 hypigu-1.3/hypigu/src/Braid.py
--rw-rw-rw-   0        0        0    10240 2021-03-08 12:28:42.000000 hypigu-1.3/hypigu/src/Constructors.py
--rw-rw-rw-   0        0        0     3792 2021-11-03 18:14:41.000000 hypigu-1.3/hypigu/src/Database.py
--rw-rw-rw-   0        0        0    17204 2022-06-24 11:49:19.000000 hypigu-1.3/hypigu/src/GenFunctions.py
--rw-rw-rw-   0        0        0      314 2021-03-08 12:28:42.000000 hypigu-1.3/hypigu/src/Globals.py
--rw-rw-rw-   0        0        0    26894 2021-11-03 18:14:41.000000 hypigu-1.3/hypigu/src/LatticeFlats.py
--rw-rw-rw-   0        0        0        0 2021-03-08 12:28:42.000000 hypigu-1.3/hypigu/src/__init__.py
--rw-rw-rw-   0        0        0    52915 2021-03-08 12:28:42.000000 hypigu-1.3/hypigu/src/init_data.py
-drwxrwxrwx   0        0        0        0 2022-06-24 11:51:39.754152 hypigu-1.3/hypigu.egg-info/
--rw-rw-rw-   0        0        0     2640 2022-06-24 11:51:39.000000 hypigu-1.3/hypigu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2022-06-24 11:51:39.000000 hypigu-1.3/hypigu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-24 11:51:39.000000 hypigu-1.3/hypigu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-06-24 11:51:39.000000 hypigu-1.3/hypigu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2021-03-08 12:28:42.000000 hypigu-1.3/pyproject.toml
--rw-rw-rw-   0        0        0      796 2022-06-24 11:51:39.775153 hypigu-1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 08:41:16.513700 hypigu-1.4/
+-rw-rw-rw-   0        0        0     1097 2023-07-26 08:35:09.000000 hypigu-1.4/LICENSE
+-rw-rw-rw-   0        0        0     2634 2023-07-26 08:41:16.513700 hypigu-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1922 2023-07-26 08:35:09.000000 hypigu-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 08:41:16.488701 hypigu-1.4/hypigu/
+-rw-rw-rw-   0        0        0      569 2023-07-26 08:35:09.000000 hypigu-1.4/hypigu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:41:16.512697 hypigu-1.4/hypigu/src/
+-rw-rw-rw-   0        0        0     4776 2023-07-26 08:35:09.000000 hypigu-1.4/hypigu/src/Braid.py
+-rw-rw-rw-   0        0        0    10183 2023-07-26 08:35:09.000000 hypigu-1.4/hypigu/src/Constructors.py
+-rw-rw-rw-   0        0        0     3790 2023-07-26 08:35:09.000000 hypigu-1.4/hypigu/src/Database.py
+-rw-rw-rw-   0        0        0    17002 2023-07-26 08:35:09.000000 hypigu-1.4/hypigu/src/GenFunctions.py
+-rw-rw-rw-   0        0        0      318 2023-07-26 08:35:09.000000 hypigu-1.4/hypigu/src/Globals.py
+-rw-rw-rw-   0        0        0    21402 2023-07-26 08:35:09.000000 hypigu-1.4/hypigu/src/LatticeFlats.py
+-rw-rw-rw-   0        0        0        0 2022-10-08 07:19:20.000000 hypigu-1.4/hypigu/src/__init__.py
+-rw-rw-rw-   0        0        0    48931 2022-10-10 21:12:31.000000 hypigu-1.4/hypigu/src/init_data.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:41:16.504706 hypigu-1.4/hypigu.egg-info/
+-rw-rw-rw-   0        0        0     2634 2023-07-26 08:41:16.000000 hypigu-1.4/hypigu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-07-26 08:41:16.000000 hypigu-1.4/hypigu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:41:16.000000 hypigu-1.4/hypigu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 08:41:16.000000 hypigu-1.4/hypigu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       89 2022-10-10 21:12:31.000000 hypigu-1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      796 2023-07-26 08:41:16.521698 hypigu-1.4/setup.cfg
```

### Comparing `hypigu-1.3/LICENSE` & `hypigu-1.4/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020--2022 Josh Maglione
+Copyright (c) 2020--2023 Josh Maglione
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hypigu-1.3/PKG-INFO` & `hypigu-1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypigu
-Version: 1.3
+Version: 1.4
 Summary: A SageMath package that provides functions to compute the Igusa local zeta function associated with hyperplane arrangements.
 Home-page: https://joshmaglione.github.io/hypigu/
 Author: Joshua Maglione
 Author-email: joshmaglione@gmail.com
 Project-URL: Bug Tracker, https://github.com/joshmaglione/hypigu/issues
 Keywords: SageMath,hyperplane arrangements,Igusa zeta functions,topological zeta functions,Flag Hilbert--Poincare series
 Classifier: Programming Language :: Python :: 3
@@ -49,15 +49,15 @@
 
 ## Funding 
 
 This package was funded in part by DFG grant [373111162](https://gepris.dfg.de/gepris/projekt/373111162?language=en).
 
 ## Copyright & License
 
-Copyright 2021&ndash;2022 Joshua Maglione.
+Copyright 2020&ndash;2023 Joshua Maglione.
 
 HypIgu is distributed with the MIT License.
 
 ## References 
 
-1. [Joshua Maglione](https://joshmaglione.com/) and [Christopher Voll](https://www.math.uni-bielefeld.de/~voll/). Flag Hilbert&ndash;Poincar&#233; series of hyperplane arrangements and their Igusa zeta functions, 2021. [arXiv:2103:03640](https://arxiv.org/abs/2103.03640).
+1. [Joshua Maglione](https://joshmaglione.com/) and [Christopher Voll](https://www.math.uni-bielefeld.de/~voll/). Flag Hilbert&ndash;Poincar&#233; series of hyperplane arrangements and Igusa zeta functions, 2021. [arXiv:2103:03640](https://arxiv.org/abs/2103.03640).
```

### Comparing `hypigu-1.3/README.md` & `hypigu-1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 ## Funding 
 
 This package was funded in part by DFG grant [373111162](https://gepris.dfg.de/gepris/projekt/373111162?language=en).
 
 ## Copyright & License
 
-Copyright 2021&ndash;2022 Joshua Maglione.
+Copyright 2020&ndash;2023 Joshua Maglione.
 
 HypIgu is distributed with the MIT License.
 
 ## References 
 
-1. [Joshua Maglione](https://joshmaglione.com/) and [Christopher Voll](https://www.math.uni-bielefeld.de/~voll/). Flag Hilbert&ndash;Poincar&#233; series of hyperplane arrangements and their Igusa zeta functions, 2021. [arXiv:2103:03640](https://arxiv.org/abs/2103.03640).
+1. [Joshua Maglione](https://joshmaglione.com/) and [Christopher Voll](https://www.math.uni-bielefeld.de/~voll/). Flag Hilbert&ndash;Poincar&#233; series of hyperplane arrangements and Igusa zeta functions, 2021. [arXiv:2103:03640](https://arxiv.org/abs/2103.03640).
```

### Comparing `hypigu-1.3/hypigu/__init__.py` & `hypigu-1.4/hypigu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #
-#   Copyright 2021 Joshua Maglione 
+#   Copyright 2021--2023 Joshua Maglione 
 #
 #   Distributed under MIT License
 #
 
-__version__ = 1.3
+__version__ = 1.4
 
 from .src.Braid import BraidArrangementIgusa
 from .src.Constructors import CoxeterArrangement, LinialArrangement, ShiArrangement, CatalanArrangement, DirectSum, PolynomialToArrangement, ResonanceArrangement
 from .src.LatticeFlats import LatticeOfFlats
 from .src.GenFunctions import FlagHilbertPoincareSeries, IgusaZetaFunction, CoarseFlagHPSeries, AnalyticZetaFunction, AtomZetaFunction, TopologicalZetaFunction
 from .src.Database import internal_database
```

### Comparing `hypigu-1.3/hypigu/src/Braid.py` & `hypigu-1.4/hypigu/src/Braid.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,91 +1,108 @@
 #
-#   Copyright 2020 Joshua Maglione 
+#   Copyright 2020 Joshua Maglione
 #
 #   Distributed under MIT License
 #
 
 from sage.all import binomial as _binomial
 from sage.all import factorial as _factorial
 from functools import reduce as _reduce
 
 _TABLE_CUTOFF = 3
 
+
 def _Igusa_braid_table(p, t, n, style="standard"):
     if n <= 0:
         return 1
     if n == 1:
         if style == "reduced":
             return 2/(1 - t)
         elif style == "skeleton":
             return (1 + p)/(1 - t)
         else:
             return (1 - p**-1)/(1 - p**-1*t)
-    if n == 2: 
+    if n == 2:
         if style == "reduced":
             return (6 + 6*t)/((1 - t)*(1 - t**3))
         elif style == "skeleton":
             return ((1 + 3*p + 2*p**2) + (2 + 3*p + p**2)*t)/((1 - t)**2)
         else:
             return (1-p**-1)*(1-2*p**-1+2*p**-1*t-p**-2*t)/((1-p**-1*t)*(1-p**-2*t**3))
-    if n == 3: 
+    if n == 3:
         if style == "reduced":
             return (24 + 48*t + 24*t**2 + 48*t**3 + 24*t**4)/((1 - t)*(1 - t**3)*(1 - t**6))
         elif style == "skeleton":
             return ((1 + 6*p + 11*p**2 + 6*p**3) + (11 + 37*p + 37*p**2 + 11*p**3)*t + (6 + 11*p + 6*p**2 + p**3)*t**2)/((1 - t)**3)
         else:
             return p**-6*(1-p**-1)*(p**4*(6-5*p+p**2)-4*p**4*(2-p)*t-p**2*(3-7*p+2*p**2)*t**2+p**2*(2-7*p+3*p**2)*t**3-4*p*(1-2*p)*t**4-(1-5*p+6*p**2)*t**5)/((1-p**-1*t)**2*(1-p**-2*t**3)*(1-p**-3*t**6))
     raise ValueError("Bad n-value.")
 
+
 # Counts the number of set partitions of [L[0] + ... + L[-1]]. So instead of
 # running through all *labeled* partitions, we just run through the partition
 # "shape" and count the number of different labelings.
 def _P(L):
     from sage.all import Set
     # Compute binom(n, p_1)*binom(n - p_1, p_2)*binom(n - p_1 - p_2, p_3)*...
+
     def binom(n, P):
         if len(P) == 1:
             return _binomial(n, P[0])
         else:
             return _binomial(n, P[0]) * binom(n - P[0], P[1:])
-    n = _reduce(lambda x, y: x + y, L)
-    count = lambda n: len(list(filter(lambda x: x == n, L)))
-    S = list(Set(list(L)))
-    d = _reduce(lambda x, y: x*y, map(lambda z: _factorial(count(z)), S))
+    n = sum(L)
+    count = lambda n: len([1 for x in L if x == n])
+    S = list(Set(L))
+    d = _reduce(lambda x, y: x*y, (_factorial(count(z)) for z in S))
     return binom(n, L) // d
 
+
 # Counts the number of edges in a subgraph of the complete graph determined by L
 def _binom_sum(L):
-    binomials = map(lambda z: _binomial(z, 2), L)
-    return _reduce(lambda x, y: x + y, binomials)
+    return sum(_binomial(z, 2) for z in L)
+
+
+def _Poincare(L):
+    """
+    Construct the Poincaré polynomial (in Y) of the braid arrangement
+    in ``|L|-1`` affine space.
 
-# Constructs the Poincare polynomial (in Y) of the braid arrangement in |L|-1
-# affine space.
-def _Poincare(L): 
+    EXAMPLES::
+
+        sage: from hypigu.Braid import _Poincare
+        sage: _Poincare(4)
+    """
     from sage.all import var
     Y = var('Y')
-    factors= map(lambda z: 1 + z*Y, range(1, len(L)))
-    return _reduce(lambda x, y: x*y, factors, 1)
+    factors = (1 + z * Y for z in range(1, len(L)))
+    return _reduce(lambda x, y: x * y, factors, 1)
+
+    # better code using polynomials
+    # from sage.all import PolynomialRing, ZZ
+    # A = PolynomialRing(ZZ, 'Y')
+    # return A.prod(A([1, z]) for z in range(1, len(L)))
+
 
 # Constructs the Igusa integral for the braid arrangement with little repetition
-# of work. 
+# of work.
 def _recursive_crank(p, t, n, known=[], style="standard"):
-    from sage.all import Partitions 
-    if known == []:
-        known = [_Igusa_braid_table(p, t, k, style=style) 
+    from sage.all import Partitions
+    if not known:
+        known = [_Igusa_braid_table(p, t, k, style=style)
             for k in range(_TABLE_CUTOFF + 1)]
     k = len(known) + 1
     Zk = 0
     for L in Partitions(k):
         if len(L) > 1:
             if style == "reduced":
                 L_factors = [_P(L), 1, t**(_binom_sum(L)), _factorial(len(L))]
             else:
                 L_factors = [
-                    _P(L), p**(1-_reduce(lambda x, y: x + y - 1, L)), 
+                    _P(L), p**(1 - _reduce(lambda x, y: x + y - 1, L)),
                     t**(_binom_sum(L)), _Poincare(L)(Y=-p**-1)
                 ]
             lower_integrals = list(map(lambda z: known[z - 1], list(L)))
             L_term = _reduce(lambda x, y: x*y, L_factors + lower_integrals, 1)
             Zk += L_term
     if style == "reduced":
         Zk = Zk/(1 - t**(_binomial(k, 2)))
@@ -93,14 +110,15 @@
         Zk = Zk/(1 - p**(-k + 1)*t**(_binomial(k, 2)))
     known += [Zk]
     if k - 1 < n:
         return _recursive_crank(p, t, n, known=known, style=style)
     else:
         return known[n]
 
+
 def BraidArrangementIgusa(n):
     r"""
     Return the rational function associated to the local Igusa zeta function for
     the n-dimensional essential braid arrangement.
 
     INPUT:
 
@@ -111,16 +129,14 @@
     EXAMPLES:
 
     This example illustrates what to expect ::
 
         sage: Z = BraidArrangementIgusa(2)
         sage: Z
         -(2*t/q - 2/q - t/q^2 + 1)*(1/q - 1)/((t^3/q^2 - 1)*(t/q - 1))
-
     """
     from sage.all import var
     p = var('q')
     t = var('t')
     if n <= _TABLE_CUTOFF:
         return _Igusa_braid_table(p, t, n, style="standard")
     return _recursive_crank(p, t, n, style="standard")
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hypigu-1.3/hypigu/src/Constructors.py` & `hypigu-1.4/hypigu/src/Constructors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,130 +1,139 @@
 #
-#   Copyright 2020 Joshua Maglione 
+#   Copyright 2020 Joshua Maglione
 #
 #   Distributed under MIT License
 #
 
 def _non_Weyl_arrangements(X, n, shift=[0]):
     from functools import reduce
     from sage.all import HyperplaneArrangements, QQ, CoxeterGroup
+
     def add_shift(x):
         return list(map(lambda k: [k] + list(x), shift))
     if X == 'I':
         # Not expecting n <= 2 for type I.
         if n == 3:
             return _arrangements_from_roots("A", 2, shift=shift)
-        if n == 4: 
+        if n == 4:
             return _arrangements_from_roots("B", 2, shift=shift)
         H = HyperplaneArrangements(QQ, tuple(['x0', 'x1']))
         norms = [tuple([1, 0]), tuple([0, 1]), tuple([1, 1]), tuple([1, -1])]
         cval = 2
         for k in range(n - 4):
-            norms.append(tuple([(-1)**(k%2), cval + (k // 2)]))
+            norms.append(tuple([(-1)**(k % 2), cval + (k // 2)]))
     else:
         if n == 2:
             return _non_Weyl_arrangements("I", 5, shift=shift)
         W = CoxeterGroup([X, n])
         H = HyperplaneArrangements(W.base_ring(), tuple(['x' + str(k) for k in range(n)]))
         norms = W.positive_roots()
-    aff_norms = reduce(lambda x, y: x+y, map(lambda x: add_shift(x), norms),[])
+    aff_norms = reduce(lambda x, y: x+y, map(lambda x: add_shift(x), norms), [])
     return H(aff_norms)
-    
+
+
 def _arrangements_from_roots(X, n, shift=[0]):
     from functools import reduce
     from sage.all import HyperplaneArrangements, QQ, RootSystem
     Phi = RootSystem([X, n]).ambient_space()
     d = Phi.dimension()
     H = HyperplaneArrangements(QQ, tuple(['x' + str(i) for i in range(d)]))
     norms = Phi.positive_roots()
+
     def add_shift(x):
         norm = tuple(map(lambda i: QQ(i), x._vector_().list()))
         return list(map(lambda k: [norm, k], shift))
-    aff_norms = reduce(lambda x, y: x+y, map(lambda x: add_shift(x), norms),[])
+    aff_norms = reduce(lambda x, y: x+y, map(lambda x: add_shift(x), norms), [])
     return H(aff_norms)
 
+
 # Verifies that the Coxeter-theoretic data is expected.
 def _Coxeter_check(X, n):
     if n <= 0:
         raise ValueError("Expected a positive rank.")
-    if not X in ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I']:
+    if X not in ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I']:
         raise ValueError(
             "Expected first character to be in {A, B, C, D, E, F, G, H, I}."
         )
     if X in ['E', 'F', 'G', 'H']:
-        if X == 'E' and not n in {6, 7, 8}:
+        if X == 'E' and n not in {6, 7, 8}:
             raise ValueError(
                 "Expected rank to be either 6, 7, or 8."
             )
         if X == 'F' and n != 4:
             raise ValueError(
                 "Expected rank to be 4."
             )
         if X == 'G' and n != 2:
             raise ValueError(
                 "Expected rank to be 2."
             )
-        if X == 'H' and not n in {2, 3, 4}:
+        if X == 'H' and n not in {2, 3, 4}:
             raise ValueError(
                 "Expected rank to be either 2, 3, or 4."
             )
         if X == 'I' and n <= 2:
             raise ValueError(
                 "Expected rank above 2."
             )
     return True
 
-# Parses the Coxeter type input and runs the check for good input. 
+
+# Parses the Coxeter type input and runs the check for good input.
 def _parse_Coxeter_input(name):
-    from sage.all import ZZ
     if isinstance(name, str):
         factors = name.split(' ')
     else:
         factors = list(name)
-        if not isinstance(factors[0], str): 
+        if not isinstance(factors[0], str):
             raise TypeError("Expected ``name`` to be an interable container of strings.")
+
     def convert(s):
         if len(s) <= 1:
             raise ValueError("Cannot parse input: {0}".format(s))
         try:
             n = int(s[1:])
         except ValueError:
             raise ValueError("Cannot parse as integer: {0}".format(s[1:]))
         return tuple([s[0].upper(), n])
     Cox_facts = list(map(convert, factors))
     assert all(map(lambda X: _Coxeter_check(X[0], X[1]), Cox_facts))
     return Cox_facts
 
+
 # Builds the direct sum arrangement of arrangements A and B.
 def _direct_sum(A, B):
     from sage.all import HyperplaneArrangements as HA
     K = A.base_ring()
     d = A.dimension() + B.dimension()
     A_H = map(lambda H: H.coefficients(), A.hyperplanes())
     B_H = map(lambda H: H.coefficients(), B.hyperplanes())
     HH = HA(K, tuple(['x' + str(k) for k in range(d)]))
     A_emb = map(lambda L: L + [0]*(B.dimension()), A_H)
     B_emb = map(lambda L: L[0:1] + [0]*(A.dimension()) + L[1:], B_H)
     return HH(list(A_emb) + list(B_emb))
 
+
 def _basic_wrapper(name, s):
-    from functools import reduce
     factors = _parse_Coxeter_input(name)
+
     def irr_facts(X):
         if X[0] in {'I', 'H'}:
             return _non_Weyl_arrangements(X[0], X[1], shift=s)
         if X == ['D', 1]:
             X = ['A', 1]
         return _arrangements_from_roots(X[0], X[1], shift=s)
     irr_arr = list(map(irr_facts, factors))
     return DirectSum(irr_arr)
 
+
 def _res_arr(n):
     from sage.all import Subsets, HyperplaneArrangements, QQ, Matrix
     Subs = Subsets(range(1, n + 1))
+
     def S_vec(S):
         v = [QQ(0)]*(n+1)
         for s in S:
             v[s] = QQ(1)
         return v
     M = [S_vec(S) for S in Subs if len(S) > 0]
     HH = HyperplaneArrangements(QQ, tuple(['x' + str(k) for k in range(n)]))
@@ -134,15 +143,15 @@
 
 def DirectSum(*args):
     r"""
     Return the direct sum of hyperplane arrangements.
 
     INPUT:
 
-    - An iterable container of hyperplane arrangements. 
+    - An iterable container of hyperplane arrangements.
 
     OUTPUT: the direct sum arrangement given as a hyperplane arrangement.
 
     EXAMPLE:
 
         sage: A = hi.CoxeterArrangement("A1")
         sage: Bool3 = hi.DirectSum(A, A, A)
@@ -154,29 +163,29 @@
     """
 
     from functools import reduce
     if len(args) == 1:
         HPAs = args[0]
     else:
         HPAs = args
-    if len(HPAs) == 1: 
+    if len(HPAs) == 1:
         return HPAs[0]
     else:
         D = _direct_sum(HPAs[0], HPAs[1])
         return reduce(lambda A, B: _direct_sum(A, B), HPAs[2:], D)
 
 
 def CoxeterArrangement(name):
     r"""
     Return the Coxeter arrangement of the prescribed Coxeter type.
 
     INPUT:
 
-    - ``name`` -- an interable container of strings; the Coxeter group 
-        name. The string must include a letter from {A, ..., H} and a 
+    - ``name`` -- an interable container of strings; the Coxeter group
+        name. The string must include a letter from {A, ..., H} and a
         nonnegative integer.
 
     OUTPUT: the Coxeter arrangement given as a hyperplane arrangement.
 
     EXAMPLES:
 
         sage: hi.CoxeterArrangement("B4")
@@ -193,16 +202,16 @@
 
 def ShiArrangement(name):
     r"""
     Return the Shi arrangement of the Coxeter prescribed type.
 
     INPUT:
 
-    - ``name`` -- an interable container of strings; the Coxeter group 
-        name. The string must include a letter from {A, ..., H} and a 
+    - ``name`` -- an interable container of strings; the Coxeter group
+        name. The string must include a letter from {A, ..., H} and a
         nonnegative integer.
 
     OUTPUT: the Shi arrangement given as a hyperplane arrangement.
 
     EXAMPLES:
 
         sage: hi.ShiArrangement("A2")
@@ -219,16 +228,16 @@
 
 def LinialArrangement(name):
     r"""
     Return the Linial arrangement of the prescribed Coxeter type.
 
     INPUT:
 
-    - ``name`` -- an interable container of strings; the Coxeter group 
-        name. The string must include a letter from {A, ..., H} and a 
+    - ``name`` -- an interable container of strings; the Coxeter group
+        name. The string must include a letter from {A, ..., H} and a
         nonnegative integer.
 
     OUTPUT: the Linial arrangement given as a hyperplane arrangement.
 
     EXAMPLES:
 
         sage: hi.LinialArrangement("D4")
@@ -245,16 +254,16 @@
 
 def CatalanArrangement(name):
     r"""
     Return the Catalan arrangement of the prescribed Coxeter type.
 
     INPUT:
 
-    - ``name`` -- an interable container of strings; the Coxeter group 
-        name. The string must include a letter from {A, ..., H} and a 
+    - ``name`` -- an interable container of strings; the Coxeter group
+        name. The string must include a letter from {A, ..., H} and a
         nonnegative integer.
 
     OUTPUT: the Catalan arrangement given as a hyperplane arrangement.
 
     EXAMPLES:
 
         sage: hi.CatalanArrangement("B4")
@@ -264,14 +273,15 @@
         Arrangement of 6 hyperplanes of dimension 4 and rank 2
 
         sage: hi.CatalanArrangement(["D4", "A3"])
         Arrangement of 54 hyperplanes of dimension 8 and rank 7
     """
     return _basic_wrapper(name, [-1, 0, 1])
 
+
 def ResonanceArrangement(n):
     r"""
     Return the rank-n resonance arrangement.
 
     INPUT:
 
     - ``n`` -- a positive integer.
@@ -287,18 +297,19 @@
         Arrangement <x1 | x0 | x0 + x1>
 
         sage: hi.ResonanceArrangement(10)
         Arrangement of 1023 hyperplanes of dimension 10 and rank 10
     """
     return _res_arr(n)
 
+
 def PolynomialToArrangement(f):
     r"""
-    Return the associated hyperplane arrangement of f, the given product of 
-    linear polynomials. 
+    Return the associated hyperplane arrangement of f, the given product of
+    linear polynomials.
 
     INPUT:
 
     - ``f`` -- a polynomial or symbolic expression.
 
     OUTPUT: the hyperplane arrangement associated with the linear factors of f.
 
@@ -311,10 +322,9 @@
         Arrangement <Z | Y | X>
 
         sage: f = 'X*Y*Z*W*(X - Y)*(X - Z)*(Y - W)'
         sage: hi.PolynomialToArrangement(f)
         Arrangement of 7 hyperplanes of dimension 4 and rank 4
     """
     from .GenFunctions import _parse_poly
-    A, M = _parse_poly(f)
+    A, _ = _parse_poly(f)
     return A
-
```

### Comparing `hypigu-1.3/hypigu/src/Database.py` & `hypigu-1.4/hypigu/src/Database.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,22 +38,22 @@
     def save_gen_func(self, P, style, F):
         assert P.rank() > 2
         assert style in ['Igusa', 'skele']
         isit, k = self.has_poset(P)
         if not isit:
             # New poset, so we save it.
             gen_dict = {
-                'Igusa' : None,
-                'skele' : None
+                'Igusa': None,
+                'skele': None
             }
             gen_dict[style] = F
             self.poset_list += [P]
             self.gen_func_list += [gen_dict]
         else:
-            if self.gen_func_list[k][style] == None:
+            if self.gen_func_list[k][style] is None:
                 GFL = self.gen_func_list
                 GFL[k][style] = F
                 self.gen_func_list = GFL
 
 
 def _initialize_main_DB():
     from sage.all import DiGraph, Poset, var
```

### Comparing `hypigu-1.3/hypigu/src/GenFunctions.py` & `hypigu-1.4/hypigu/src/GenFunctions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,111 +1,113 @@
 #
-#   Copyright 2021 Joshua Maglione 
+#   Copyright 2021 Joshua Maglione
 #
 #   Distributed under MIT License
 #
+from sage.all import var
 
 from .Database import internal_database as _data
 from .Globals import __PRINT as _print
 from .Globals import __TIME as _time
 from functools import reduce as _reduce
 
-# A function to return a poincare function.
-def _Poincare_polynomial(L, sub=None):
-    from sage.all import var 
-    if sub == None:
+
+# A function to return a Poincaré function.
+def _Poincare_polynomial(L, sub=None, abs_val=False):
+    if sub is None:
         sub = var('Y')
+
     def poincare(x):
-        pi = L.restriction(x).Poincare_polynomial()
+        pi = L.restriction(x).Poincare_polynomial(abs_val=abs_val)
         try:
-            return pi.subs({pi.variables()[0] : sub})
-        except AttributeError: # In case pi is a constant.
+            return pi.subs({pi.variables()[0]: sub})
+        except AttributeError:  # In case pi is a constant.
             return pi
     return poincare
 
+
 # The complete solutions for small central arrangements of rank <= 2.
 def _small_central(A, style, numerator=False):
-    from sage.all import var
-
     p = var('q')
     t = var('t')
     Y = var('Y')
     T = var('T')
     if A.rank() == 1:
         if style == 'Igusa':
             return (1 - p**-1)/(1 - p**-1*t)
         if style == 'skele':
             if numerator:
-                return 1 + Y 
+                return 1 + Y
             else:
                 return (1 + Y)/(1 - T)
     # Now we assume the rank == 2.
     m = len(A)
     if style == 'Igusa':
         return (1 - p**-1)*(1 - (m - 1)*p**-1 + (m - 1)*p**-1*t - p**-2*t) / ((1 - p**-1*t)*(1 - p**-2*t**m))
     if style == 'skele':
         if numerator:
             return 1 + m*Y + (m-1)*Y**2 + (m-1 + m*Y + Y**2)*T
         else:
             return (1 + m*Y + (m-1)*Y**2 + (m-1 + m*Y + Y**2)*T)/((1 - T)**2)
 
+
 # The direct version of the universal generating function computation.
-def _universal(L, anayltic=False, atom=False):
-    from sage.all import var
+def _universal(L, analytic=False, atom=False):
     from .LatticeFlats import _subposet
 
     # Set up the potential substitutions for T -- as defined in Maglione--Voll.
-    if anayltic:
+    if analytic:
         q = var('q')
         Y = -q**(-1)
         P = L.poset
         t_name = lambda x: var("t" + str(x))
         if atom:
             atoms = P.upper_covers(P.bottom())
+
             def T_data(x):
-                under_poset = _subposet(P, x, lambda z: P.lower_covers(z))
-                elts = filter(lambda y: y in under_poset, atoms)
+                under_poset = _subposet(P, x, P.lower_covers)
+                elts = (y for y in atoms if y in under_poset)
                 ts = map(t_name, elts)
                 return _reduce(lambda x, y: x*y, ts, q**(-P.rank(x)))
         else:
             def T_data(x):
-                under_poset = _subposet(P, x, lambda z: P.lower_covers(z))
+                under_poset = _subposet(P, x, P.lower_covers)
                 elts = list(under_poset._elements)
                 elts.remove(P.bottom())
                 ts = map(t_name, elts)
                 return _reduce(lambda x, y: x*y, ts, q**(-P.rank(x)))
-    else: 
+    else:
         T_data = lambda x: var("T" + str(x))
         Y = var('Y')
 
-    T = {x : T_data(x) for x in L.poset._elements}
-    
+    T = {x: T_data(x) for x in L.poset._elements}
+
     # Base cases for recursion.
     if L.poset.has_top() and L.poset.rank() == 2:
         elts = L.proper_part_poset()._elements
         merge = lambda x, y: x + (1 + Y)**2*T[y]/(1 - T[y])
         one = L.poset.top()
         return _reduce(merge, elts, (1 + Y)*(1 + (len(elts) - 1)*Y))/(1-T[one])
     if L.poset.rank == 1:
         elts = list(L.poset._elements).remove(L.poset.bottom())
         merge = lambda x, y: x + (1 + Y)*T[y]/(1 - T[y])
         return _reduce(merge, elts, 1 + len(elts)*Y)
-    
+
     P = L.proper_part_poset()
     poincare = _Poincare_polynomial(L, sub=Y)
-    recurse = lambda M: _universal(M, anayltic=anayltic, atom=atom)
+    recurse = lambda M: _universal(M, analytic=analytic, atom=atom)
     num_dat = lambda x: poincare(x)*T[x]*recurse(L.subarrangement(x))
     factors = map(num_dat, P._elements)
     HP = _reduce(lambda x, y: x + y, factors, poincare(L.poset.bottom()))
     if L.poset.has_top():
         HP = HP/(1 - T[L.poset.top()])
     return HP
 
+
 def _Igusa_zeta_function(L, DB=True, verbose=_print):
-    from sage.all import var
     from .Constructors import CoxeterArrangement
     from .Braid import BraidArrangementIgusa
     from .LatticeFlats import LatticeOfFlats, _Coxeter_poset_data
 
     P = L.poset
     q = var('q')
     t = var('t')
@@ -116,17 +118,17 @@
         return (1 - q**-1)*(1 - (m-1)*q**-1 + m*(1 - q**-1)*q**-1*t/(1 - q**-1*t))/(1 - q**-2*t**m)
     if P.rank() == 1:
         m = len(P) - 1
         return 1 - m*q**-1 + m*(1 - q**-1)*q**-1*t/(1 - q**-1*t)
 
     if DB:
         zeta = _data.get_gen_func(P, 'Igusa')
-        if zeta != None:
+        if zeta is not None:
             return zeta
-    # We check to see if we have a type A braid arrangement. 
+    # We check to see if we have a type A braid arrangement.
     # We can compute these *extremely* quickly.
     if _Coxeter_poset_data()['A']['hyperplanes'](P.rank()) == len(L.atoms()):
         if _Coxeter_poset_data()['A']['poset'](P.rank()) == len(P):
             B = CoxeterArrangement("A" + str(P.rank()))
             if P.is_isomorphic(LatticeOfFlats(B).poset):
                 return BraidArrangementIgusa(P.rank())
 
@@ -136,22 +138,20 @@
     eq_elt_data = L._combinatorial_eq_elts()
     factors = map(lambda x: x[1]*x_factor(x[0]), eq_elt_data)
     integrals = map(lambda x: _Igusa_zeta_function(x[2], DB=DB), eq_elt_data)
     pi = poincare(P.bottom())
     zeta = _reduce(lambda x, y: x + y[0]*y[1], zip(factors, integrals), 0) + pi
     if P.has_top():
         zeta = zeta/(1 - q**(-P.rank())*t**len(L.atoms()))
-    if DB and P.rank() > 2: 
+    if DB and P.rank() > 2:
         _data.save_gen_func(P, 'Igusa', zeta)
     return zeta
 
 
 def _top_zeta_function_uni(L, DB=True, verbose=_print):
-    from sage.all import var
-
     P = L.poset
     s = var('s')
     C = 1*L.poset.has_top()
 
     # Base cases for recursion.
     if P.has_top() and P.rank() == 2:
         m = len(P) - 2
@@ -171,38 +171,38 @@
     if C == 1:
         zeta = zeta/(P.rank() + len(L.atoms())*s)
 
     return zeta
 
 
 def _top_zeta_function_mul(L, DB=True, verbose=_print, atom=False):
-    from sage.all import var
     from .LatticeFlats import _subposet
 
     P = L.poset
-    C = 1*L.poset.has_top()
+    C = 1 * L.poset.has_top()
 
     s_name = lambda x: var("s" + str(x))
     if atom:
         if atom:
             atoms = P.upper_covers(P.bottom())
+
             def s_data(x):
-                under_poset = _subposet(P, x, lambda z: P.lower_covers(z))
-                elts = filter(lambda y: y in under_poset, atoms)
+                under_poset = _subposet(P, x, P.lower_covers)
+                elts = (y for y in atoms if y in under_poset)
                 ts = map(s_name, elts)
                 return _reduce(lambda x, y: x + y, ts, 0)
     else:
         def s_data(x):
-            under_poset = _subposet(P, x, lambda z: P.lower_covers(z))
+            under_poset = _subposet(P, x, P.lower_covers)
             elts = list(under_poset._elements)
             elts.remove(P.bottom())
             ts = map(s_name, elts)
             return _reduce(lambda x, y: x + y, ts, 0)
 
-    S = {x : s_data(x) for x in P._elements}
+    S = {x: s_data(x) for x in P._elements}
 
     # Base cases for recursion.
     add_em = lambda x, y: x + y
     if P.has_top() and P.rank() == 2:
         atms = P.upper_covers(P.bottom())
         m = len(atms)
         elt_dat = lambda x: 1/(1 + S[x])
@@ -212,281 +212,279 @@
         m = len(atms)
         elt_dat = lambda x: 1/(1 + S[x])
         return _reduce(add_em, map(elt_dat, atms), 1 - m)
 
     poincare = _Poincare_polynomial(L)
     Y = poincare(P.bottom()).variables()[0]
     pi_circ = lambda x: (poincare(x)/(1 + Y)**C).factor().simplify().subs({Y: -1})
-    x_factor = lambda x: pi_circ(x)
+    x_factor = pi_circ
     prop_elts = L.proper_part_poset()._elements
     factors = map(lambda x: x_factor(x), prop_elts)
     integrals = map(lambda x: _top_zeta_function_mul(L.subarrangement(x), DB=DB, atom=atom), prop_elts)
     pi = pi_circ(P.bottom())
     zeta = _reduce(lambda x, y: x + y[0]*y[1], zip(factors, integrals), 0) + pi
     if P.has_top():
         zeta = zeta/(P.rank() + S[P.top()])
 
     return zeta
 
 
-def _comb_skele(L, DB=True, verbose=_print):
-    from sage.all import var
+def _comb_skele(L, abs_val=False, DB=True, verbose=_print):
     P = L.poset
     Y = var('Y')
     T = var('T')
 
-    if P.has_top():
-        if P.rank() == 1:
-            return (1 + Y)/(1 - T)
-        if P.rank() == 2:
-            m = len(P) - 2
-            return (1 + m*Y + (m - 1)*Y**2 + (m - 1 + m*Y + Y**2)*T)/(1 - T)**2
+    if P.rank() == 1:
+        a = len(L.atoms())
+        return (1 + a*Y)/(1 - T)
+    if P.rank() == 2 and P.has_top():
+        m = len(P) - 2
+        return (1 + m*Y + (m - 1)*Y**2 + (m - 1 + m*Y + Y**2)*T)/(1 - T)**2
     if DB:
         if verbose:
             print(_time() + "Checking database.")
         zeta = _data.get_gen_func(P, 'skele')
-        if zeta != None:
+        if zeta is not None:
+            if verbose:
+                print("\tFound it.")
             return zeta
-        if verbose:
-            print("\tDone.")
+        else:
+            if verbose:
+                print("\tDid not find it.")
 
-    poincare = _Poincare_polynomial(L)
-    if verbose: 
+    poincare = _Poincare_polynomial(L, abs_val=abs_val)
+    if verbose:
         print(_time() + "Gleaning structure from poset.")
     eq_elt_data = L._combinatorial_eq_elts()
     if verbose:
         print("\tDone.")
         print(_time() + "Lattice points: {0},  Relevant points: {1}".format(len(P), len(eq_elt_data)))
     factors = map(lambda x: x[1]*T*poincare(x[0]), eq_elt_data)
     if verbose:
         print(_time() + "Recursing...")
-    integrals = map(lambda x: _comb_skele(x[2], DB=DB), eq_elt_data)
+    integrals = map(lambda x: _comb_skele(x[2], DB=DB, abs_val=abs_val, verbose=verbose), eq_elt_data)
     if verbose:
         print(_time() + "Putting everything together...")
     pi = poincare(P.bottom())
     zeta = _reduce(lambda x, y: x + y[0]*y[1], zip(factors, integrals), 0) + pi
     if P.has_top():
         zeta = zeta/(1 - T)
-    if DB and P.rank() > 2: 
+    if DB and P.rank() > 2:
         _data.save_gen_func(P, 'skele', zeta)
-        
+
     return zeta
 
+
 # Given a polynomial, return a hyperplane arrangement equivalent to the linear
-# factors of f. 
-def _parse_poly(f): 
+# factors of f.
+def _parse_poly(f):
     from sage.all import SR, QQ, HyperplaneArrangements, Matrix
-    if type(f) == str:
+    if isinstance(f, str):
         f = SR(f)
     if f.base_ring() == SR:
         L = f.factor_list()
         K = QQ
-    else: 
+    else:
         L = list(f.factor())
         K = f.base_ring()
 
-    L = filter(lambda T: not T[0] in K, L) # Remove constant factors
+    L = filter(lambda T: not T[0] in K, L)  # Remove constant factors
     F, M = list(zip(*L))
 
     # Verify that each polynomial factor is linear
-    is_lin = lambda g: all(map(lambda x: g.degree(x) <= 1, g.variables()))
+    is_lin = lambda g: all(g.degree(x) <= 1 for x in g.variables())
     if not all(map(is_lin, F)):
         raise ValueError("Expected product of linear factors.")
 
     varbs = f.variables()
-    varbs_str = tuple(map(lambda x: str(x), varbs))
+    varbs_str = tuple(str(x) for x in varbs)
     HH = HyperplaneArrangements(K, varbs_str)
 
     def poly_vec(g):
-        c = K(g.subs({x : 0 for x in g.variables()}))
+        c = K(g.subs({x: 0 for x in g.variables()}))
         return tuple([c] + [K(g.coefficient(x)) for x in varbs])
 
     F_vec = tuple(map(poly_vec, F))
     A = HH(Matrix(K, F_vec))
 
     # This scrambles the hyperplanes, so we need to scramble M in the same way.
     A_vec = tuple(map(lambda H: tuple(H.coefficients()), A.hyperplanes()))
-    perm = tuple([F_vec.index(v) for v in A_vec])
+    perm = (F_vec.index(v) for v in A_vec)
     M_new = tuple([M[i] for i in perm])
 
     return A, M_new
 
 
-
-
-def CoarseFlagHPSeries(A=None, lattice_of_flats=None, int_poset=None, matroid=None, numerator=False, verbose=_print):
+def CoarseFlagHPSeries(A=None, lattice_of_flats=None, poset=None, matroid=None, numerator=False, abs_val=False, verbose=_print):
     from .LatticeFlats import LatticeOfFlats
 
-    if matroid == None: 
-        try:
-            if A.is_central() and A.rank() <= 2:
-                return _small_central(A, 'skele', numerator=numerator)
-        except AttributeError:
-            raise TypeError("object is not a hyperplane arrangement.")
-    if lattice_of_flats == None:
+    if lattice_of_flats is None:
         if verbose:
             print("{0}Building lattice of flats".format(_time()))
-        if matroid == None:
-            L = LatticeOfFlats(A, poset=int_poset)
+        if matroid is None and poset is None:
+            L = LatticeOfFlats(A=A)
         else:
-            L = LatticeOfFlats(matroid=matroid)
+            if poset is None:
+                L = LatticeOfFlats(matroid=matroid)
+            else:
+                L = LatticeOfFlats(poset=poset)
     else:
         L = lattice_of_flats
 
     if verbose:
         print("{0}Computing coarse flag Hilbert--Poincare series".format(_time()))
-    cfHP = _comb_skele(L)
-    
+    cfHP = _comb_skele(L, abs_val=abs_val, verbose=verbose)
+
     if numerator:
+        if verbose:
+            print(_time() + "Constructing numerator.")
         D = cfHP.numerator_denominator()[1]
         T = D.variables()[0]
-        if D == (T - 1)**(L.poset.rank()): 
+        if D == (T - 1)**(L.poset.rank()):
             e = -1
-        if D == (1 - T)**(L.poset.rank()): 
+        if D == (1 - T)**(L.poset.rank()):
             e = 1
         return e*(cfHP*D).factor()
-    else: 
-        return cfHP 
+    else:
+        return cfHP
 
 
 def IgusaZetaFunction(X=None, lattice_of_flats=None, int_poset=None, matroid=None, verbose=_print):
     from .LatticeFlats import LatticeOfFlats
-    from sage.all import var
 
-    HPA = True 
-    if matroid == None:
+    HPA = True
+    if matroid is None:
         try:
-            # Check if a hyperplane arrangement. 
+            # Check if a hyperplane arrangement.
             _ = X.hyperplanes()
             A = X
         except AttributeError:
-            # Not an HPA; deal with polynomial input. 
+            # Not an HPA; deal with polynomial input.
             A, M = _parse_poly(X)
             if verbose:
                 print("{0}Constructed a hyperplane arrangement".format(_time()))
-            HPA = False 
+            HPA = False
 
-    if lattice_of_flats == None:
+    if lattice_of_flats is None:
         if verbose:
             print("{0}Building lattice of flats".format(_time()))
-        if matroid == None:
+        if matroid is None:
             L = LatticeOfFlats(A, poset=int_poset)
         else:
             L = LatticeOfFlats(matroid=matroid)
     else:
         L = lattice_of_flats
 
     if not HPA:
         if list(M) == [1]*len(M):
             if verbose:
                 print("{0}Computing Igusa's zeta function".format(_time()))
             return _Igusa_zeta_function(L)
         else:
             if verbose:
                 print("{0}Computing the atom zeta function".format(_time()))
-            Z = _universal(L, anayltic=True, atom=True)
+            Z = _universal(L, analytic=True, atom=True)
             t = var('t')
-            SUB = {var('t' + str(k+1)) : t**(M[k]) for k in range(len(M))}
+            SUB = {var('t' + str(k+1)): t**(M[k]) for k in range(len(M))}
             return Z.subs(SUB)
 
     if verbose:
         print("{0}Computing Igusa's zeta function".format(_time()))
     return _Igusa_zeta_function(L)
 
 
 def TopologicalZetaFunction(X=None, lattice_of_flats=None, int_poset=None, verbose=_print, multivariate=False, atom=False, matroid=None):
     from .LatticeFlats import LatticeOfFlats
-    from sage.all import var
 
-    HPA = True 
-    if matroid == None:
+    HPA = True
+    if matroid is None:
         try:
-            # Check if a hyperplane arrangement. 
+            # Check if a hyperplane arrangement.
             _ = X.hyperplanes()
             A = X
         except AttributeError:
-            # Not an HPA; deal with polynomial input. 
+            # Not an HPA; deal with polynomial input.
             A, M = _parse_poly(X)
             if verbose:
                 print("{0}Constructed a hyperplane arrangement".format(_time()))
-            HPA = False 
+            HPA = False
 
-    if lattice_of_flats == None:
-        if matroid == None:
+    if lattice_of_flats is None:
+        if matroid is None:
             if verbose:
                 print("{0}Building lattice of flats".format(_time()))
             L = LatticeOfFlats(A, poset=int_poset)
-        else: 
+        else:
             L = LatticeOfFlats(matroid=matroid)
     else:
         L = lattice_of_flats
 
     if verbose:
         print("{0}Computing the topological zeta function".format(_time()))
 
     if not HPA:
-        if list(M) == [1]*len(M):
+        if all(m == 1 for m in M):
             return _top_zeta_function_uni(L)
         else:
             Z = _top_zeta_function_mul(L, atom=True)
             s = var('s')
-            SUB = {var('s' + str(k+1)) : M[k]*s for k in range(len(M))}
+            SUB = {var('s' + str(k+1)): M[k]*s for k in range(len(M))}
             return Z.subs(SUB)
 
     if not multivariate:
         return _top_zeta_function_uni(L)
 
     return _top_zeta_function_mul(L, atom=atom)
 
 
 def AnalyticZetaFunction(A=None, lattice_of_flats=None, int_poset=None, matroid=None, verbose=_print):
     from .LatticeFlats import LatticeOfFlats
 
-    if lattice_of_flats == None:
-        if matroid == None:
+    if lattice_of_flats is None:
+        if matroid is None:
             if verbose:
                 print("{0}Building lattice of flats".format(_time()))
             L = LatticeOfFlats(A, poset=int_poset)
-        else: 
+        else:
             L = LatticeOfFlats(matroid=matroid)
     else:
         L = lattice_of_flats
 
     if verbose:
         print("{0}Computing the analytic zeta function".format(_time()))
-    return _universal(L, anayltic=True)
+    return _universal(L, analytic=True)
 
 
 def AtomZetaFunction(A=None, lattice_of_flats=None, int_poset=None, matroid=None, verbose=_print):
     from .LatticeFlats import LatticeOfFlats
 
-    if lattice_of_flats == None:
-        if matroid == None:
+    if lattice_of_flats is None:
+        if matroid is None:
             if verbose:
                 print("{0}Building lattice of flats".format(_time()))
             L = LatticeOfFlats(A, poset=int_poset)
-        else: 
+        else:
             L = LatticeOfFlats(matroid=matroid)
     else:
         L = lattice_of_flats
 
     if verbose:
         print("{0}Computing the atom zeta function".format(_time()))
-    return _universal(L, anayltic=True, atom=True)
+    return _universal(L, analytic=True, atom=True)
 
 
 def FlagHilbertPoincareSeries(A=None, lattice_of_flats=None, int_poset=None, matroid=None, verbose=_print):
     from .LatticeFlats import LatticeOfFlats
 
-    if lattice_of_flats == None:
-        if matroid == None:
+    if lattice_of_flats is None:
+        if matroid is None:
             if verbose:
                 print("{0}Building lattice of flats".format(_time()))
             L = LatticeOfFlats(A, poset=int_poset)
-        else: 
+        else:
             L = LatticeOfFlats(matroid=matroid)
     else:
         L = lattice_of_flats
 
     if verbose:
-        print("{0}Computing the flag Hilbert--Poincare series".format(_time()))
+        print("{0}Computing the flag Hilbert--Poincaré series".format(_time()))
     return _universal(L)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hypigu-1.3/hypigu/src/LatticeFlats.py` & `hypigu-1.4/hypigu/src/LatticeFlats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 #
-#   Copyright 2020 Joshua Maglione 
+#   Copyright 2020 Joshua Maglione
 #
 #   Distributed under MIT License
 #
 
-from functools import reduce as _reduce
+from functools import reduce
 from sage.misc.cachefunc import cached_method
 from .Globals import __TIME as _time
 from .Globals import __NCPUS as _N
 import sage.parallel.decorate as _para
 
 
 def _contract(M, rows):
-    from sage.all import Matrix, identity_matrix
+    from sage.all import Matrix
     K = M.base_ring()
-    Q = [M[k] for k in rows] + [M[k] for k in range(M.nrows()) if not k in rows]
+    Q = [M[k] for k in rows] + [M[k] for k in range(M.nrows()) if k not in rows]
     Q = Matrix(K, Q).transpose()
     top = Q[0]
     E = Q[1:, :].echelon_form()
     rel_E = E[:, :len(rows)]
     out_E = E[:, len(rows):]
     rm = rel_E.pivot_rows()
     # In case we have a non-central arrangement
     for r in rm:
         v = E[r]
         i = list(v).index(1)
         top = top - top[i]*v
-    A = [tuple(list(top)[len(rows):])] + [out_E[k] for k in range(E.nrows()) if not k in rm]
+    A = [tuple(list(top)[len(rows):])] + [out_E[k] for k in range(E.nrows())
+                                          if k not in rm]
     M_out = Matrix(K, A).transpose()
     return M_out
 
+
 # BUILD A WAY TO GET THE LABELS FROM THE CONTRACT MATRIX
 def _get_labels(M, x, rows, L):
     from sage.all import VectorSpace, Set, Matrix
 
     # If non-central, then this is true iff not intersecting.
     not_e1 = lambda v: list(v)[1:] != [0]*(len(v)-1)
 
     # Determine new hyperplanes and group like rows together.
     V = VectorSpace(M.base_ring(), M.ncols())
     lines = []
     labels = []
     for r in range(M.nrows()):
-        v = M[r] 
-        is_new = not_e1(v) 
+        v = M[r]
+        is_new = not_e1(v)
         i = 0
         while i < len(lines) and is_new:
             if v in V.subspace([lines[i]]):
-                is_new = False 
+                is_new = False
                 labels[i] = labels[i].union(Set([r]))
             else:
                 i += 1
         if is_new:
             lines.append(v)
             labels.append(Set([r]))
 
     # Adjust the labels because we are missing rows.
     fix_sets = lambda F: lambda S: Set(list(map(lambda s: F(s), S)))
     for k in rows:
         adjust = lambda i: i + (k <= i)*1
         labels = list(map(fix_sets(adjust), labels))
-    labels = [Set(rows)] + labels 
+    labels = [Set(rows)] + labels
 
     # Adjust the row labels to hyperplane labels
     HL = L.hyperplane_labels
     A = L.hyperplane_arrangement
     HL_lab = lambda i: list(filter(lambda j: HL[j] == A[i], HL.keys()))[0]
     labels = list(map(fix_sets(HL_lab), labels))
 
@@ -80,309 +82,208 @@
         T = S.difference(labels[0])
         new_T = Set([])
         for k in range(len(l_hyp)):
             if l_hyp[k].issubset(T):
                 new_T = new_T.union(Set([new_hyp[k]]))
         return new_T
 
-    return Matrix(lines),last_adj,{new_hyp[i] : i for i in range(len(new_hyp))}
+    return Matrix(lines), last_adj, {new_hyp[i]: i for i in range(len(new_hyp))}
+
 
 def _parse_poset(P):
     global POS, atoms, labs, int_at
     from sage.all import Set
     import sage.parallel.decorate as para
-    
+
     POS = P
     N = _N
     atoms = POS.upper_covers(POS.bottom())
 
     @para.parallel(N)
-    def atom_set(k, shift): 
+    def atom_set(k, shift):
         S = list(POS._elements[1+shift::k])
-        m = lambda x: [x, Set(list(filter(lambda a: POS.le(a, x), atoms)))]
+        m = lambda x: [x, Set(filter(lambda a: POS.le(a, x), atoms))]
         return list(map(m, S))
 
     labs = list(atom_set([(N, k) for k in range(N)]))
-    labs = [[P.bottom(), Set([])]] + _reduce(lambda x, y: x + y[1], labs, [])
-    label_dict = {T[0] : T[1] for T in labs}
+    labs = [[P.bottom(), Set([])]] + reduce(lambda x, y: x + y[1], labs, [])
+    label_dict = {T[0]: T[1] for T in labs}
 
     return label_dict
 
+
 # Can return the subarrangement A_x or restriction A^x simply based on the
-# function F given. For subarrangement use 'lambda z: P.lower_covers(z)' and for
-# restriction use 'lambda z: P.upper_covers(z)'.
+# function F given. For subarrangement use 'P.lower_covers' and for
+# restriction use 'P.upper_covers'.
 def _subposet(P, x, F):
-    from sage.all import Set, Poset
-    elts = Set([])
+    from sage.all import Set
+    elts = Set()
     new_level = Set([x])
     while len(elts.union(new_level)) > len(elts):
         elts = elts.union(new_level)
-        new_level = Set(_reduce(
-            lambda x, y: x+y, 
-            map(F, new_level), 
+        new_level = Set(reduce(
+            lambda x, y: x+y,
+            map(F, new_level),
             []
         ))
-    new_P = P.subposet(elts)
-    return new_P
+    return P.subposet(elts)
 
 
 # Parallel function to build the intersection lattice.
-# Moved to global to prevent accidentally carrying unnecessary data. 
+# Moved to global to prevent accidentally carrying unnecessary data.
 @_para.parallel(_N)
 def build_next(A, S, HYP, LIN):
     from sage.all import exists, Set
     new_level = []
     new_hypcont = []
     if len(S) > 0:
         m = S[0]
     for i in S:
         T = LIN[i - m]
         for j in range(len(A)):
             # Skip the hyperplane already known to contain the intersection.
-            if not j in HYP[i - m]: 
+            if j not in HYP[i - m]:
                 H = A[j]
                 I = H._affine_subspace().intersection(T)
                 # Check if the intersection is trivial.
                 if I is not None:
-                    if I == T: 
+                    if I == T:
                         # This case means that H cap T = T, so we should
                         # record that H contains T.
                         HYP[i - m] = HYP[i - m].union(Set([j]))
                     else:
-                        # Check if we have this intersection already. 
+                        # Check if we have this intersection already.
                         is_in, ind = exists(
-                            range(len(new_level)), 
+                            range(len(new_level)),
                             lambda k: I == new_level[k]
                         )
                         if is_in:
                             # We have the intersection, so we update
-                            # containment info accordingly. 
+                            # containment info accordingly.
                             new_hypcont[ind] = new_hypcont[ind].union(
                                 Set([j]).union(HYP[i - m])
                             )
                         else:
                             # We do not have it, so we update everything.
                             new_level.append(I)
                             new_hypcont.append(HYP[i - m].union(Set([j])))
     return list(zip(new_level, new_hypcont))
 
 
-# We expand on the function in sage, optimizing a little bit. This makes little
-# difference in small ranks but noticeable difference in larger ranks. This is
-# still quite slow. 
-def _para_intersection_poset(A):
-    from sage.geometry.hyperplane_arrangement.affine_subspace import AffineSubspace
-    from sage.all import exists, flatten, Set, QQ, VectorSpace, Poset
-    from .Globals import __SANITY
-
-    N = _N
-    K = A.base_ring()
-    whole_space = AffineSubspace(0, VectorSpace(K, A.dimension()))
-    # L is the ranked list of affine subspaces in L(A).
-    L = [[whole_space], list(map(lambda H: H._affine_subspace(), A))]
-    # hyp_cont is the ranked list describing which hyperplanes contain the
-    # corresponding intersection. 
-    hyp_cont = [[Set([])], [Set([k]) for k in range(len(A))]]
-
-    c = A.is_central()*(-1)
-    for r in range(2, A.rank() + c + 1):
-        print("{1}Working on elements of rank {0}".format(r, _time()))
-        m = len(L[r-1])
-        pmax = lambda k: (k+1)*(m//N) + (k==N-1)*(m%N)
-        pmin = lambda k: k*(m//N)
-        all_input = lambda k: tuple([
-            A, range(pmin(k), pmax(k)), 
-            hyp_cont[r - 1][pmin(k):pmax(k)], L[r - 1][pmin(k):pmax(k)]
-        ])
-        data = list(build_next(
-            [all_input(k) for k in range(N) if pmin(k) != pmax(k)]
-        ))
-        data = _reduce(lambda x, y: x + y[1], data, [])
-        new_lev, new_hyp = list(zip(*data))
-        new_lev = list(new_lev)
-        new_hyp = list(new_hyp)
-        i = 0
-        # Merge the lists down
-        print("{0}Merging the lists from the {1} workers".format(_time(), N))
-        # First we check the affine spaces
-        while i < len(new_lev):
-            U = new_lev[i]
-            B1 = U.linear_part().basis_matrix()
-            p1 = U.point()
-            j = i + 1
-            while j < len(new_lev):
-                V = new_lev[j]
-                B2 = V.linear_part().basis_matrix()
-                p2 = V.point()
-                if B1 == B2 and p1 == p2:
-                    new_lev = new_lev[:j] + new_lev[j+1:]
-                    new_hyp[i] = new_hyp[i].union(new_hyp[j])
-                    new_hyp = new_hyp[:j] + new_hyp[j+1:]
-                else:
-                    j += 1
-            i += 1
-        # Second we check the labels of intersection (don't want duplicates)
-        i = 0
-        while i < len(new_lev):
-            j = i + 1
-            while j < len(new_lev):
-                if new_hyp[i] == new_hyp[j]:
-                    new_lev = new_lev[:j] + new_lev[j+1:]
-                    new_hyp = new_hyp[:j] + new_hyp[j+1:]
-                else:
-                    j += 1
-            i += 1
-        L.append(new_lev)
-        hyp_cont.append(new_hyp)
-
-    # A silly optimization for centrals.
-    if A.is_central() and len(A) > 1:
-        inter = lambda X, Y: X.intersection(Y._affine_subspace())
-        L.append([_reduce(inter, A[1:], A[0]._affine_subspace())])
-        hyp_cont.append([Set(list(range(len(A))))])
-
-    L_flat = list(_reduce(lambda x, y: x + y, L, []))
-    hc_flat = list(_reduce(lambda x, y: x + y, hyp_cont, []))
-
-    # Sanity checks
-    if __SANITY:
-        print("{0}Running sanity check".format(_time()))
-        assert len(L_flat) == len(hc_flat)
-        for i in range(len(hc_flat)):
-            for j in range(i+1, len(hc_flat)): 
-                assert hc_flat[i] != hc_flat[j], "{0} vs {1}".format(i, j)
-        for i in range(len(L_flat)):
-            I = list(map(lambda x: A[x], hc_flat[i]))
-            U = _reduce(lambda x, y: x.intersection(y._affine_subspace()), I, whole_space)
-            assert U == L_flat[i], "{0} vs {1}".format(U, L_flat[i])
-
-    print("{0}Constructing lattice of flats".format(_time()))
-    t = {}
-    for i in range(len(hc_flat)):
-        t[i] = Set(list(map(lambda x: x+1, hc_flat[i])))
-    cmp_fn = lambda p, q: t[p].issubset(t[q])
-    label_dict = {i : t[i] for i in range(len(hc_flat))}
-    get_hyp = lambda i: A[label_dict[i].an_element() - 1]
-    hyp_dict = {i + 1 : get_hyp(i + 1) for i in range(len(A))}
-
-    return [Poset((t, cmp_fn)), label_dict, hyp_dict]
-
-
 # Default SageMath algorithm works well. However 'A.matroid()' seems to remove
-# ordering, which we depend on, so care is needed. 
+# ordering, which we depend on, so care is needed.
 def _lof_from_matroid(A=None, matroid=None):
     from sage.all import Set, Matrix, Matroid, Poset
-    from functools import reduce
-    if A != None:
+    if A is not None:
         rows = list(map(lambda H: H.coefficients()[1:], A.hyperplanes()))
         mat = Matrix(A.base_ring(), rows).transpose()
         M = Matroid(mat)
         n = len(A)
-        lbl_map = lambda S: S 
+        lbl_map = lambda S: S
     else:
         M = matroid.simplify()
         n = len(M.groundset())
         grd_list = list(M.groundset())
-        l_map = {x : grd_list.index(x) for x in grd_list}
+        l_map = {x: grd_list.index(x) for x in grd_list}
         lbl_map = lambda S: frozenset([l_map[x] for x in S])
 
     L = M.lattice_of_flats()
     rank_r = lambda L, r: list(
         map(lbl_map, filter(lambda x: L.rank(x) == r, L._elements))
     )
     rank_1 = [frozenset([k]) for k in range(n)]
     ranks = reduce(
-        lambda x, y: x + y, 
-        [rank_r(L, r) for r in range(2, L.rank() + 1)], 
+        lambda x, y: x + y,
+        [rank_r(L, r) for r in range(2, L.rank() + 1)],
         [L.bottom()] + rank_1
     )
     P = Poset(
-        L, element_labels={x : ranks.index(lbl_map(x)) for x in L._elements}
+        L, element_labels={x: ranks.index(lbl_map(x)) for x in L._elements}
     )
     adj_set = lambda S: Set([x+1 for x in S])
-    label_dict = {i : adj_set(ranks[i]) for i in range(len(L))}
-    if A != None:
-        hyp_dict = {i : A[list(ranks[i])[0]] for i in range(1, n + 1)}
-    else: 
-        hyp_dict = None 
+    label_dict = {i: adj_set(ranks[i]) for i in range(len(L))}
+    if A is not None:
+        hyp_dict = {i: A[list(ranks[i])[0]] for i in range(1, n + 1)}
+    else:
+        hyp_dict = None
     return [P, label_dict, hyp_dict]
 
 
 def _lof_from_affine_matroid(A):
-    from sage.all import Poset, Set 
-    from functools import reduce
+    from sage.all import Poset, Set
     A_coned = A.cone()
     hyps = list(map(lambda H: H.coefficients(), A_coned.hyperplanes()))
     extra = [0, 1] + [0]*(A.dimension())
     i = hyps.index(extra)
     P, L, H = _lof_from_matroid(A_coned)
-    assert (H[i + 1]).coefficients() == extra 
+    assert (H[i + 1]).coefficients() == extra
     new_elts = list(filter(lambda x: not P.le(i + 1, x), P))
     new_elts = reduce(
         lambda x, y: x + y,
         [list(filter(lambda x: P.rank(x) == r, new_elts)) for r in range(2, P.rank() + 1)],
         [0] + [j for j in range(1, len(A_coned) + 1) if j != i + 1]
     )
-    new_names = {x : new_elts.index(x) for x in new_elts}
+    new_names = {x: new_elts.index(x) for x in new_elts}
     adj_set = lambda S: Set([new_names[x] for x in S if x in new_elts])
     P_new = Poset(P.subposet(new_elts), element_labels=new_names)
-    L_new = {new_names[x] : adj_set(L[x]) for x in new_elts}
-    def inv_H(h): 
+    L_new = {new_names[x]: adj_set(L[x]) for x in new_elts}
+
+    def inv_H(h):
         cut = lambda x: x.coefficients()[1:]
-        pair = list(filter(lambda x: cut(x[1]) == h, H.items())) 
+        pair = list(filter(lambda x: cut(x[1]) == h, H.items()))
         return pair[0][0]
-    H_new = {new_names[inv_H(h.coefficients())] : h for h in A}
+    H_new = {new_names[inv_H(h.coefficients())]: h for h in A}
     return [P_new, L_new, H_new]
 
 
 class LatticeOfFlats():
 
-    def __init__(self, A=None, poset=None, flat_labels=None, 
-    hyperplane_labels=None, lazy=False, matroid=None, 
+    def __init__(self, A=None, poset=None, flat_labels=None,
+    hyperplane_labels=None, lazy=False, matroid=None,
     nature_hyperplane_label=True):
         self.hyperplane_arrangement = A
-        self.poset = poset 
+        self.poset = poset
         self.flat_labels = flat_labels
         self.hyperplane_labels = hyperplane_labels
-        if poset != None:
+        if poset is not None:
             assert poset.has_bottom(), "Expected a unique minimal element in poset."
             assert poset.is_graded(), "Expected a graded poset."
             self.poset = poset
         else:
             if not lazy:
-                if A != None: 
+                if A is not None:
                     if A.is_central():
                         P, FL, HL = _lof_from_matroid(A)
                     else:
                         P, FL, HL = _lof_from_affine_matroid(A)
-                else: 
+                else:
                     P, FL, HL = _lof_from_matroid(A=None, matroid=matroid)
                 self.poset = P
                 self.flat_labels = FL
                 self.hyperplane_labels = HL
-        if self.flat_labels == None and not lazy:
+        if self.flat_labels is None and not lazy:
             self.flat_labels = _parse_poset(poset)
-        if self.hyperplane_arrangement != None and self.hyperplane_labels == None and nature_hyperplane_label:
-            self.hyperplane_labels = {i + 1 : A[i] for i in range(len(A))}
+        if self.hyperplane_arrangement is not None and self.hyperplane_labels is None and nature_hyperplane_label:
+            self.hyperplane_labels = {i + 1: A[i] for i in range(len(A))}
 
     def __repr__(self):
         if self.hyperplane_arrangement:
             return "The lattice of flats of:\n{0}\ngiven by:\n{1}".format(self.hyperplane_arrangement, self.poset)
         else:
             return "The lattice of flats of some matroid given by:\n{0}".format(self.poset)
 
     def _save(self, file, var_name='L'):
         from sage.all import Matrix
         HH = self.hyperplane_arrangement.parent()
         A = Matrix(map(lambda H: H.coefficients(), self.hyperplane_arrangement.hyperplanes())).rows()
         CR = tuple(map(lambda T: tuple(T), self.poset.cover_relations()))
         FL = self.flat_labels
         FL_tup = tuple([tuple([x, list(FL[x])]) for x in FL.keys()])
-        del FL 
-        dict_builder = "FL = {x[0] : Set(x[1]) for x in FL_tup}\n"
+        del FL
+        dict_builder = "FL = {x[0]: Set(x[1]) for x in FL_tup}\n"
         with open(file, "w") as F:
             F.write("from sage.all import HyperplaneArrangements, QQ, Poset, Set\n")
             F.write("import hypigu as hi\n")
             F.write("H = HyperplaneArrangements(QQ, {0})\n".format(HH.variable_names()))
             del HH
             F.write("A = H({0})\n".format(A).replace("), ", "),\n"))
             del A
@@ -392,24 +293,23 @@
             F.write("FL_tup = {0}\n".format(FL_tup).replace("), ", "),\n"))
             F.write(dict_builder)
             F.write("del FL_tup\n")
             F.write("{0} = hi.LatticeOfFlats(A, poset=P, flat_labels=FL)\n".format(var_name))
             F.write("del H, A, CR, P, FL\n")
             F.write("print('Loaded a lattice of flats. Variable name: {0}')".format(var_name))
 
-
     def atoms(self):
         return self.poset.upper_covers(self.poset.bottom())
 
     def labels_of_flats(self):
         elt_tup = lambda x: tuple([x, self.flat_labels[x]])
         return list(map(elt_tup, self.poset._elements))
 
     def labels_of_hyperplanes(self):
-        P = self.poset 
+        P = self.poset
         elt_tup = lambda x: tuple([x, self.hyperplane_labels[x]])
         return list(map(elt_tup, P.upper_covers(P.bottom())))
 
     def proper_part_poset(self):
         P = self.poset
         elts = list(P._elements)
         if P.has_top():
@@ -417,178 +317,193 @@
         elts.remove(P.bottom())
         return P.subposet(elts)
 
     def show(self):
         self.poset.show()
 
     def subarrangement(self, x):
-        P = self.poset 
-        if type(x) != set:
+        P = self.poset
+        if not isinstance(x, set):
             assert x in P, "Expected element to be in poset."
-            new_P = _subposet(P, x, lambda z: P.lower_covers(z))
-            new_A = None 
+            new_P = _subposet(P, x, P.lower_covers)
+            new_A = None
             new_FL = None
-            new_HL = None 
+            new_HL = None
             if self.hyperplane_arrangement and self.hyperplane_labels:
                 A = self.hyperplane_arrangement
                 HL = self.hyperplane_labels
                 atoms = new_P.upper_covers(new_P.bottom())
                 keep = list(map(lambda k: HL[k], atoms))
                 new_A = A.parent()(keep)
-                new_HL = {a : HL[a] for a in atoms}
+                new_HL = {a: HL[a] for a in atoms}
             if self.flat_labels:
                 FL = self.flat_labels
-                new_FL = {x : FL[x] for x in new_P._elements}
+                new_FL = {x: FL[x] for x in new_P._elements}
             return LatticeOfFlats(new_A, poset=new_P, flat_labels=new_FL, hyperplane_labels=new_HL)
         else:
-            L = self.flat_labels 
+            L = self.flat_labels
             X = list(filter(lambda y: L[y] == x, P._elements))
             try:
                 return self.subarrangement(X[0])
             except IndexError:
                 raise ValueError("No element labeled by:\n{0}".format(x))
-    
+
     def restriction(self, x):
         from sage.all import Matrix, HyperplaneArrangements
-        P = self.poset 
-        if type(x) != set:
+        P = self.poset
+        if not isinstance(x, set):
             assert x in P, "Expected element to be in poset."
-            new_P = _subposet(P, x, lambda z: P.upper_covers(z))
-            new_A = None 
-            new_HL = None 
+            new_P = _subposet(P, x, P.upper_covers)
+            new_A = None
+            new_HL = None
             if self.hyperplane_arrangement:
                 A = self.hyperplane_arrangement
                 hyp_coeffs = map(lambda H: H.coefficients(), A.hyperplanes())
                 M = Matrix(A.base_ring(), list(hyp_coeffs))
                 rows = sorted(list(map(
-                    lambda H: list(A).index(self.hyperplane_labels[H]), 
+                    lambda H: list(A).index(self.hyperplane_labels[H]),
                     self.flat_labels[x]
                 )))
                 new_M = _contract(M, rows)
                 new_M, lab_func, hyp_dict = _get_labels(new_M, x, rows, self)
                 HH = HyperplaneArrangements(
-                    A.base_ring(), 
+                    A.base_ring(),
                     A.parent().variable_names()[:new_M.ncols()-1]
                 )
                 new_A = HH(new_M)
                 FL = self.flat_labels
-                new_FL = {x : lab_func(FL[x]) for x in new_P._elements}
-                new_HL = {a : new_A[hyp_dict[a]] for a in new_P.upper_covers(new_P.bottom())}
+                new_FL = {x: lab_func(FL[x]) for x in new_P._elements}
+                new_HL = {a: new_A[hyp_dict[a]] for a in new_P.upper_covers(new_P.bottom())}
             else:
                 FL = self.flat_labels
-                new_FL = {y : FL[y].difference(FL[x]) for y in new_P._elements}
+                new_FL = {y: FL[y].difference(FL[x]) for y in new_P._elements}
             return LatticeOfFlats(new_A, poset=new_P, flat_labels=new_FL, hyperplane_labels=new_HL)
         else:
-            L = self.flat_labels 
+            L = self.flat_labels
             X = list(filter(lambda y: L[y] == x, P._elements))
             try:
                 return self.restriction(X[0])
             except IndexError:
                 raise ValueError("No element labeled by:\n{0}".format(x))
-    
+
     def deletion(self, H):
         from sage.all import Set
 
         P = self.poset
         L = self.flat_labels
 
-        if type(H) == set:
-            L = self.flat_labels 
-            X = list(filter(lambda y: L[y] == H, P._elements))
+        if isinstance(H, set):
+            L = self.flat_labels
+            X = [y for y in P._elements if L[y] == H]
             try:
                 return self.deletion(X[0])
             except IndexError:
                 raise ValueError("No element labeled by:\n{0}".format(H))
-            
+
         assert P.rank_function()(H) == 1, "Expected an atom."
 
         if P.has_top():
             coatoms = P.lower_covers(P.top())
         else:
             # not really coatoms... but whatever
             coatoms = P.maximal_elements()
 
         m = len(self.atoms()) - 1
+
         def check(C):
             S = L[C]
-            return bool(len(S) == m and not H in S)
+            return len(S) == m and H not in S
+
         new_top = list(filter(check, coatoms))
 
         if len(new_top) == 1:
-            new_P = _subposet(P, new_top[0], lambda z: P.lower_covers(z))
-            new_FL = {y : L[y] for y in new_P._elements}
+            new_P = _subposet(P, new_top[0], P.lower_covers)
+            new_FL = {y: L[y] for y in new_P._elements}
         else:
             def good_flats(F):
                 S = L[F]
                 if H in S:
                     U = S.difference(Set([H]))
-                    return (U != 0) and (not U in L.values())
+                    return (U != 0) and (U not in L.values())
                 else:
                     return True
             flats = list(filter(good_flats, P._elements))
             new_P = P.subposet(flats)
-            new_FL = {y : L[y].difference(Set([H])) for y in flats}
+            new_FL = {y: L[y].difference(Set([H])) for y in flats}
 
         if self.hyperplane_arrangement:
             HPA = self.hyperplane_arrangement
             HL = self.hyperplane_labels
             A = list(HPA)
             A.remove(HPA[H])
             new_HPA = HPA.parent()(A)
-            new_HL = {x : HL[x] for x in new_P.upper_covers(new_P.bottom())}
+            new_HL = {x: HL[x] for x in new_P.upper_covers(new_P.bottom())}
         else:
             new_HPA = None
             new_HL = None
 
         return LatticeOfFlats(new_HPA, poset=new_P, flat_labels=new_FL, hyperplane_labels=new_HL)
 
     def _lazy_restriction(self, H):
         HPA = self.hyperplane_arrangement
-        assert HPA != None, "Needs underlying hyperplane arrangement."
+        assert HPA is not None, "Needs underlying hyperplane arrangement."
         A = HPA.restriction(HPA[H - 1])
         return LatticeOfFlats(A, lazy=True)
 
     def _lazy_deletion(self, H):
         HPA = self.hyperplane_arrangement
-        assert HPA != None, "Needs underlying hyperplane arrangement."
+        assert HPA is not None, "Needs underlying hyperplane arrangement."
         return LatticeOfFlats(HPA.parent()(HPA[:H-1] + HPA[H:]), lazy=True)
 
     @cached_method
-    def Poincare_polynomial(self):
+    def Poincare_polynomial(self, abs_val=False):
         from sage.all import QQ, PolynomialRing
+        if abs_val not in {True, False}:
+            raise ValueError("abs must be either True or False.")
         PR = PolynomialRing(QQ, 'Y')
         Y = PR.gens()[0]
-        if self.poset != None:
-            P = self.poset 
+        if self.poset is not None:
+            P = self.poset
             atoms = self.atoms()
             if P.rank() == 0:
                 return PR(1)
             if P.rank() == 1:
                 return PR(1 + len(atoms)*Y)
-        else: 
-            # Lazy 
+        else:
+            # Lazy
             A = self.hyperplane_arrangement
-            assert A != None, "Expected either a poset or hyperplane arrangement."
+            assert A is not None, "Expected either a poset or hyperplane arrangement."
             if A.rank() == 0:
                 return PR(1)
             if A.rank() == 1:
                 return PR(1 + len(A)*Y)
-        if self.hyperplane_arrangement != None:
-            try: # Some hyperplane arrangements are bugged in SageMath.
+        if self.hyperplane_arrangement is not None:
+            try:  # Some hyperplane arrangements are bugged in SageMath.
                 D = self._lazy_deletion(1)
                 R = self._lazy_restriction(1)
                 return PR(D.Poincare_polynomial() + Y*R.Poincare_polynomial())
-            except: 
-                pass 
-        chi = self.poset.characteristic_polynomial()
-        q = chi.variables()[0]
-        d = chi.degree(q)
-        return PR((-Y)**d*chi.subs({q : -Y**-1}))
-        
-        
+            except Exception:
+                pass
+        if abs_val:
+            comb_elts = self._combinatorial_eq_elts()
+            rk = P.rank_function()
+            bot = P.bottom()
+            pi = PR(1)
+            if P.has_top():
+                top = P.top()
+                pi += abs(P.moebius_function(bot, top))*Y**(rk(top))
+            for t in comb_elts:
+                pi += abs(P.moebius_function(bot, t[0]))*t[1]*Y**(rk(t[0]))
+            return pi
+        else:
+            chi = P.characteristic_polynomial()
+            q = chi.variables()[0]
+            d = chi.degree(q)
+            return PR((-Y)**d*chi.subs({q: -Y**-1}))
+
     @cached_method
     def _combinatorial_eq_elts(self):
         global POS, P_elts
         import sage.parallel.decorate as para
 
         N = _N
         POS = self.poset
@@ -620,76 +535,26 @@
                     down.append(dow_x)
                     restrict.append(res_x)
                 all_elts = all_elts[1:]
             return list(zip(eq_elts, counts, down, restrict))
 
         # Get the preliminary set of inequivalent elements
         prelim_elts = list(match_elts([(N, k) for k in range(N)]))
-        prelim_elts = _reduce(lambda x, y: x + y[1], prelim_elts, [])
+        prelim_elts = reduce(lambda x, y: x + y[1], prelim_elts, [])
 
-        # Test further to minimize the size. 
+        # Test further to minimize the size.
         equiv_elts = []
-        while len(prelim_elts) > 0:
+        while prelim_elts:
             x = prelim_elts[0]
             match = False
             i = 0
             while not match and i < len(equiv_elts):
                 if x[2].poset.is_isomorphic(equiv_elts[i][2].poset) and x[3].poset.is_isomorphic(equiv_elts[i][3].poset):
                     match = True
                 else:
                     i += 1
             if match:
                 equiv_elts[i][1] += x[1]
             else:
                 equiv_elts.append(list(x))
             prelim_elts = prelim_elts[1:]
         return equiv_elts
-
-
-def _Coxeter_poset_data():
-    # Bell numbers: A000110
-    def A_poset(n):
-        from sage.all import binomial
-        S = [1, 1, 2, 5, 15, 52, 203]
-        while len(S) <= n+1:
-            m = len(S) - 1
-            S.append(_reduce(
-                lambda x, y: x + y[0]*binomial(m, y[1]), zip(S, range(m+1)), 0
-            ))
-        return S[n+1]
-    def S(n, k, m):
-        if k > n or k < 0 : 
-            return 0
-        if n == 0 and k == 0: 
-            return 1
-        return S(n-1, k-1, m) + (m*(k+1)-1)*S(n-1, k, m)
-    def A007405(n): 
-        from sage.all import add
-        return add(S(n, k, 2) for k in (0..n)) # Peter Luschny, May 20 2013
-    # D analog of Bell numbers: A039764
-    Dlist = [1, 1, 4, 15, 72, 403, 2546, 17867, 137528, 1149079, 10335766, 99425087, 1017259964, 11018905667, 125860969266, 1510764243699, 18999827156304, 249687992188015, 3420706820299374, 48751337014396167]
-    table = {
-        'A': {
-            'hyperplanes': lambda n: n*(n+1) // 2,
-            'poset': A_poset
-        },
-        'B': {
-            'hyperplanes': lambda n: n**2,
-            'poset': A007405
-        },
-        'D': {
-            'hyperplanes': lambda n: n**2 - n,
-            'poset': lambda n: Dlist[n]
-        }
-    }
-    return table
-
-def _possibly_Coxeter(P):
-    r = P.rank()
-    hypers = list(filter(lambda x: P.covers(P.bottom(), x), P))
-    m = len(hypers)
-    CPD = _Coxeter_poset_data()
-    for name in ['A', 'B', 'D']:
-        if CPD[name]['hyperplanes'](r) == m:
-            if CPD[name]['poset'](r) == len(P):
-                return [True, name]
-    return [False, None]
```

### Comparing `hypigu-1.3/hypigu/src/init_data.py` & `hypigu-1.4/hypigu/src/init_data.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,3984 +1,3984 @@
-A3_rels = [[0, 1],
- [0, 2],
- [0, 3],
- [0, 4],
- [0, 5],
- [0, 6],
- [0, 7],
- [0, 8],
- [0, 9],
- [0, 10],
- [0, 11],
- [0, 13],
- [0, 12],
- [0, 14],
- [1, 7],
- [1, 8],
- [1, 9],
- [1, 14],
- [2, 7],
- [2, 10],
- [2, 11],
- [2, 14],
- [3, 7],
- [3, 13],
- [3, 12],
- [3, 14],
- [7, 14],
- [4, 8],
- [4, 10],
- [4, 12],
- [4, 14],
- [8, 14],
- [5, 10],
- [5, 13],
- [5, 9],
- [5, 14],
- [10, 14],
- [13, 14],
- [6, 9],
- [6, 11],
- [6, 12],
- [6, 14],
- [9, 14],
- [11, 14],
- [12, 14]]
-
-A4_rels = [[0, 1],
- [0, 2],
- [0, 3],
- [0, 4],
- [0, 5],
- [0, 6],
- [0, 7],
- [0, 8],
- [0, 9],
- [0, 10],
- [0, 11],
- [0, 12],
- [0, 13],
- [0, 14],
- [0, 15],
- [0, 16],
- [0, 17],
- [0, 18],
- [0, 19],
- [0, 20],
- [0, 21],
- [0, 23],
- [0, 22],
- [0, 24],
- [0, 26],
- [0, 25],
- [0, 27],
- [0, 28],
- [0, 29],
- [0, 31],
- [0, 30],
- [0, 32],
- [0, 34],
- [0, 35],
- [0, 33],
- [0, 36],
- [0, 37],
- [0, 38],
- [0, 39],
- [0, 40],
- [0, 42],
- [0, 41],
- [0, 43],
- [0, 44],
- [0, 46],
- [0, 45],
- [0, 49],
- [0, 50],
- [0, 48],
- [0, 47],
- [0, 51],
- [1, 11],
- [1, 12],
- [1, 13],
- [1, 14],
- [1, 15],
- [1, 16],
- [1, 36],
- [1, 37],
- [1, 38],
- [1, 39],
- [1, 40],
- [1, 42],
- [1, 41],
- [1, 51],
- [2, 11],
- [2, 17],
- [2, 18],
- [2, 19],
- [2, 20],
- [2, 21],
- [2, 36],
- [2, 37],
- [2, 38],
- [2, 43],
- [2, 44],
- [2, 46],
- [2, 45],
- [2, 51],
- [3, 11],
- [3, 23],
- [3, 22],
- [3, 24],
- [3, 26],
- [3, 25],
- [3, 36],
- [3, 37],
- [3, 38],
- [3, 49],
- [3, 50],
- [3, 48],
- [3, 47],
- [3, 51],
- [11, 36],
- [11, 37],
- [11, 38],
- [11, 51],
- [4, 12],
- [4, 17],
- [4, 22],
- [4, 27],
- [4, 28],
- [4, 29],
- [4, 36],
- [4, 39],
- [4, 40],
- [4, 43],
- [4, 44],
- [4, 48],
- [4, 47],
- [4, 51],
- [12, 36],
- [12, 39],
- [12, 40],
- [12, 51],
- [5, 17],
- [5, 23],
- [5, 13],
- [5, 31],
- [5, 30],
- [5, 32],
- [5, 36],
- [5, 43],
- [5, 44],
- [5, 49],
- [5, 50],
- [5, 42],
- [5, 41],
- [5, 51],
- [17, 36],
- [17, 43],
- [17, 44],
- [17, 51],
- [23, 36],
- [23, 49],
- [23, 50],
- [23, 51],
- [6, 13],
- [6, 18],
- [6, 22],
- [6, 34],
- [6, 35],
- [6, 33],
- [6, 36],
- [6, 42],
- [6, 41],
- [6, 46],
- [6, 45],
- [6, 48],
- [6, 47],
- [6, 51],
- [13, 36],
- [13, 42],
- [13, 41],
- [13, 51],
- [18, 36],
- [18, 46],
- [18, 45],
- [18, 51],
- [22, 36],
- [22, 48],
- [22, 47],
- [22, 51],
- [36, 51],
- [7, 14],
- [7, 19],
- [7, 24],
- [7, 27],
- [7, 30],
- [7, 33],
- [7, 37],
- [7, 39],
- [7, 41],
- [7, 43],
- [7, 45],
- [7, 49],
- [7, 47],
- [7, 51],
- [14, 37],
- [14, 39],
- [14, 41],
- [14, 51],
- [19, 37],
- [19, 43],
- [19, 45],
- [19, 51],
- [24, 37],
- [24, 49],
- [24, 47],
- [24, 51],
- [37, 51],
- [8, 15],
- [8, 27],
- [8, 31],
- [8, 34],
- [8, 20],
- [8, 25],
- [8, 39],
- [8, 42],
- [8, 38],
- [8, 43],
- [8, 47],
- [8, 50],
- [8, 46],
- [8, 51],
- [15, 39],
- [15, 42],
- [15, 38],
- [15, 51],
- [27, 39],
- [27, 43],
- [27, 47],
- [27, 51],
- [39, 51],
- [31, 42],
- [31, 43],
- [31, 50],
- [31, 51],
- [34, 42],
- [34, 46],
- [34, 47],
- [34, 51],
- [42, 51],
- [9, 20],
- [9, 26],
- [9, 28],
- [9, 30],
- [9, 35],
- [9, 16],
- [9, 43],
- [9, 46],
- [9, 38],
- [9, 49],
- [9, 48],
- [9, 40],
- [9, 41],
- [9, 51],
- [20, 43],
- [20, 46],
- [20, 38],
- [20, 51],
- [26, 49],
- [26, 48],
- [26, 38],
- [26, 51],
- [28, 43],
- [28, 48],
- [28, 40],
- [28, 51],
- [30, 43],
- [30, 49],
- [30, 41],
- [30, 51],
- [43, 51],
- [49, 51],
- [35, 46],
- [35, 48],
- [35, 41],
- [35, 51],
- [46, 51],
- [48, 51],
- [10, 16],
- [10, 21],
- [10, 25],
- [10, 29],
- [10, 32],
- [10, 33],
- [10, 38],
- [10, 40],
- [10, 41],
- [10, 44],
- [10, 45],
- [10, 50],
- [10, 47],
- [10, 51],
- [16, 38],
- [16, 40],
- [16, 41],
- [16, 51],
- [21, 38],
- [21, 44],
- [21, 45],
- [21, 51],
- [25, 38],
- [25, 50],
- [25, 47],
- [25, 51],
- [38, 51],
- [29, 40],
- [29, 44],
- [29, 47],
- [29, 51],
- [40, 51],
- [32, 44],
- [32, 50],
- [32, 41],
- [32, 51],
- [44, 51],
- [50, 51],
- [33, 41],
- [33, 45],
- [33, 47],
- [33, 51],
- [41, 51],
- [45, 51],
- [47, 51]]
-
-A5_rels = [[0, 1],
- [0, 2],
- [0, 3],
- [0, 4],
- [0, 5],
- [0, 6],
- [0, 7],
- [0, 8],
- [0, 9],
- [0, 10],
- [0, 11],
- [0, 12],
- [0, 13],
- [0, 14],
- [0, 15],
- [0, 16],
- [0, 17],
- [0, 18],
- [0, 19],
- [0, 20],
- [0, 21],
- [0, 22],
- [0, 23],
- [0, 24],
- [0, 25],
- [0, 26],
- [0, 27],
- [0, 28],
- [0, 29],
- [0, 30],
- [0, 31],
- [0, 32],
- [0, 33],
- [0, 34],
- [0, 36],
- [0, 35],
- [0, 37],
- [0, 39],
- [0, 38],
- [0, 40],
- [0, 41],
- [0, 43],
- [0, 42],
- [0, 44],
- [0, 45],
- [0, 46],
- [0, 47],
- [0, 48],
- [0, 49],
- [0, 50],
- [0, 52],
- [0, 51],
- [0, 53],
- [0, 54],
- [0, 56],
- [0, 55],
- [0, 57],
- [0, 59],
- [0, 60],
- [0, 58],
- [0, 61],
- [0, 63],
- [0, 64],
- [0, 62],
- [0, 65],
- [0, 66],
- [0, 67],
- [0, 68],
- [0, 70],
- [0, 69],
- [0, 71],
- [0, 72],
- [0, 74],
- [0, 75],
- [0, 73],
- [0, 76],
- [0, 78],
- [0, 79],
- [0, 80],
- [0, 77],
- [0, 81],
- [0, 82],
- [0, 83],
- [0, 84],
- [0, 85],
- [0, 86],
- [0, 87],
- [0, 88],
- [0, 89],
- [0, 90],
- [0, 91],
- [0, 93],
- [0, 92],
- [0, 94],
- [0, 96],
- [0, 95],
- [0, 97],
- [0, 98],
- [0, 99],
- [0, 101],
- [0, 100],
- [0, 102],
- [0, 104],
- [0, 105],
- [0, 103],
- [0, 106],
- [0, 107],
- [0, 108],
- [0, 109],
- [0, 110],
- [0, 112],
- [0, 111],
- [0, 113],
- [0, 115],
- [0, 114],
- [0, 116],
- [0, 117],
- [0, 118],
- [0, 120],
- [0, 119],
- [0, 121],
- [0, 123],
- [0, 124],
- [0, 122],
- [0, 130],
- [0, 131],
- [0, 132],
- [0, 133],
- [0, 134],
- [0, 126],
- [0, 125],
- [0, 127],
- [0, 129],
- [0, 128],
- [0, 135],
- [0, 137],
- [0, 136],
- [0, 142],
- [0, 141],
- [0, 143],
- [0, 139],
- [0, 140],
- [0, 138],
- [0, 144],
- [0, 145],
- [0, 146],
- [0, 148],
- [0, 147],
- [0, 149],
- [0, 151],
- [0, 152],
- [0, 150],
- [0, 156],
- [0, 157],
- [0, 158],
- [0, 154],
- [0, 153],
- [0, 155],
- [0, 161],
- [0, 160],
- [0, 159],
- [0, 165],
- [0, 167],
- [0, 166],
- [0, 170],
- [0, 168],
- [0, 169],
- [0, 163],
- [0, 164],
- [0, 162],
- [0, 171],
- [0, 172],
- [0, 173],
- [0, 174],
- [0, 175],
- [0, 177],
- [0, 176],
- [0, 178],
- [0, 179],
- [0, 181],
- [0, 180],
- [0, 184],
- [0, 185],
- [0, 183],
- [0, 182],
- [0, 186],
- [0, 187],
- [0, 189],
- [0, 188],
- [0, 192],
- [0, 193],
- [0, 191],
- [0, 190],
- [0, 198],
- [0, 199],
- [0, 201],
- [0, 200],
- [0, 196],
- [0, 197],
- [0, 195],
- [0, 194],
- [0, 202],
- [1, 16],
- [1, 17],
- [1, 18],
- [1, 19],
- [1, 20],
- [1, 21],
- [1, 22],
- [1, 23],
- [1, 24],
- [1, 25],
- [1, 81],
- [1, 82],
- [1, 83],
- [1, 84],
- [1, 85],
- [1, 86],
- [1, 87],
- [1, 88],
- [1, 89],
- [1, 90],
- [1, 91],
- [1, 93],
- [1, 92],
- [1, 94],
- [1, 96],
- [1, 95],
- [1, 97],
- [1, 98],
- [1, 99],
- [1, 101],
- [1, 100],
- [1, 102],
- [1, 104],
- [1, 105],
- [1, 103],
- [1, 171],
- [1, 172],
- [1, 173],
- [1, 174],
- [1, 175],
- [1, 177],
- [1, 176],
- [1, 178],
- [1, 179],
- [1, 181],
- [1, 180],
- [1, 184],
- [1, 185],
- [1, 183],
- [1, 182],
- [1, 202],
- [2, 16],
- [2, 26],
- [2, 27],
- [2, 28],
- [2, 29],
- [2, 30],
- [2, 31],
- [2, 32],
- [2, 33],
- [2, 34],
- [2, 81],
- [2, 82],
- [2, 83],
- [2, 84],
- [2, 85],
- [2, 86],
- [2, 106],
- [2, 107],
- [2, 108],
- [2, 109],
- [2, 110],
- [2, 112],
- [2, 111],
- [2, 113],
- [2, 115],
- [2, 114],
- [2, 116],
- [2, 117],
- [2, 118],
- [2, 120],
- [2, 119],
- [2, 121],
- [2, 123],
- [2, 124],
- [2, 122],
- [2, 171],
- [2, 172],
- [2, 173],
- [2, 174],
- [2, 175],
- [2, 177],
- [2, 176],
- [2, 186],
- [2, 187],
- [2, 189],
- [2, 188],
- [2, 192],
- [2, 193],
- [2, 191],
- [2, 190],
- [2, 202],
- [3, 16],
- [3, 36],
- [3, 35],
- [3, 37],
- [3, 39],
- [3, 38],
- [3, 40],
- [3, 41],
- [3, 43],
- [3, 42],
- [3, 81],
- [3, 82],
- [3, 83],
- [3, 84],
- [3, 85],
- [3, 86],
- [3, 130],
- [3, 131],
- [3, 132],
- [3, 133],
- [3, 134],
- [3, 126],
- [3, 125],
- [3, 127],
- [3, 129],
- [3, 128],
- [3, 135],
- [3, 137],
- [3, 136],
- [3, 142],
- [3, 141],
- [3, 143],
- [3, 139],
- [3, 140],
- [3, 138],
- [3, 171],
- [3, 172],
- [3, 173],
- [3, 174],
- [3, 175],
- [3, 177],
- [3, 176],
- [3, 198],
- [3, 199],
- [3, 201],
- [3, 200],
- [3, 196],
- [3, 197],
- [3, 195],
- [3, 194],
- [3, 202],
- [16, 81],
- [16, 82],
- [16, 83],
- [16, 84],
- [16, 85],
- [16, 86],
- [16, 171],
- [16, 172],
- [16, 173],
- [16, 174],
- [16, 175],
- [16, 177],
- [16, 176],
- [16, 202],
- [4, 17],
- [4, 26],
- [4, 35],
- [4, 44],
- [4, 45],
- [4, 46],
- [4, 47],
- [4, 48],
- [4, 49],
- [4, 50],
- [4, 81],
- [4, 87],
- [4, 88],
- [4, 89],
- [4, 90],
- [4, 91],
- [4, 106],
- [4, 107],
- [4, 108],
- [4, 109],
- [4, 110],
- [4, 126],
- [4, 125],
- [4, 127],
- [4, 129],
- [4, 128],
- [4, 144],
- [4, 145],
- [4, 146],
- [4, 148],
- [4, 147],
- [4, 149],
- [4, 151],
- [4, 152],
- [4, 150],
- [4, 171],
- [4, 172],
- [4, 173],
- [4, 178],
- [4, 179],
- [4, 181],
- [4, 180],
- [4, 186],
- [4, 187],
- [4, 189],
- [4, 188],
- [4, 196],
- [4, 197],
- [4, 195],
- [4, 194],
- [4, 202],
- [17, 81],
- [17, 87],
- [17, 88],
- [17, 89],
- [17, 90],
- [17, 91],
- [17, 171],
- [17, 172],
- [17, 173],
- [17, 178],
- [17, 179],
- [17, 181],
- [17, 180],
- [17, 202],
- [5, 26],
- [5, 36],
- [5, 18],
- [5, 52],
- [5, 51],
- [5, 53],
- [5, 54],
- [5, 56],
- [5, 55],
- [5, 57],
- [5, 81],
- [5, 106],
- [5, 107],
- [5, 108],
- [5, 109],
- [5, 110],
- [5, 130],
- [5, 131],
- [5, 132],
- [5, 133],
- [5, 134],
- [5, 93],
- [5, 92],
- [5, 94],
- [5, 96],
- [5, 95],
- [5, 156],
- [5, 157],
- [5, 158],
- [5, 154],
- [5, 153],
- [5, 155],
- [5, 161],
- [5, 160],
- [5, 159],
- [5, 171],
- [5, 172],
- [5, 173],
- [5, 186],
- [5, 187],
- [5, 189],
- [5, 188],
- [5, 198],
- [5, 199],
- [5, 201],
- [5, 200],
- [5, 184],
- [5, 185],
- [5, 183],
- [5, 182],
- [5, 202],
- [26, 81],
- [26, 106],
- [26, 107],
- [26, 108],
- [26, 109],
- [26, 110],
- [26, 171],
- [26, 172],
- [26, 173],
- [26, 186],
- [26, 187],
- [26, 189],
- [26, 188],
- [26, 202],
- [36, 81],
- [36, 130],
- [36, 131],
- [36, 132],
- [36, 133],
- [36, 134],
- [36, 171],
- [36, 172],
- [36, 173],
- [36, 198],
- [36, 199],
- [36, 201],
- [36, 200],
- [36, 202],
- [6, 18],
- [6, 27],
- [6, 35],
- [6, 59],
- [6, 60],
- [6, 58],
- [6, 61],
- [6, 63],
- [6, 64],
- [6, 62],
- [6, 81],
- [6, 93],
- [6, 92],
- [6, 94],
- [6, 96],
- [6, 95],
- [6, 112],
- [6, 111],
- [6, 113],
- [6, 115],
- [6, 114],
- [6, 126],
- [6, 125],
- [6, 127],
- [6, 129],
- [6, 128],
- [6, 165],
- [6, 167],
- [6, 166],
- [6, 170],
- [6, 168],
- [6, 169],
- [6, 163],
- [6, 164],
- [6, 162],
- [6, 171],
- [6, 172],
- [6, 173],
- [6, 184],
- [6, 185],
- [6, 183],
- [6, 182],
- [6, 192],
- [6, 193],
- [6, 191],
- [6, 190],
- [6, 196],
- [6, 197],
- [6, 195],
- [6, 194],
- [6, 202],
- [18, 81],
- [18, 93],
- [18, 92],
- [18, 94],
- [18, 96],
- [18, 95],
- [18, 171],
- [18, 172],
- [18, 173],
- [18, 184],
- [18, 185],
- [18, 183],
- [18, 182],
- [18, 202],
- [27, 81],
- [27, 112],
- [27, 111],
- [27, 113],
- [27, 115],
- [27, 114],
- [27, 171],
- [27, 172],
- [27, 173],
- [27, 192],
- [27, 193],
- [27, 191],
- [27, 190],
- [27, 202],
- [35, 81],
- [35, 126],
- [35, 125],
- [35, 127],
- [35, 129],
- [35, 128],
- [35, 171],
- [35, 172],
- [35, 173],
- [35, 196],
- [35, 197],
- [35, 195],
- [35, 194],
- [35, 202],
- [81, 171],
- [81, 172],
- [81, 173],
- [81, 202],
- [7, 19],
- [7, 28],
- [7, 37],
- [7, 44],
- [7, 51],
- [7, 58],
- [7, 65],
- [7, 66],
- [7, 67],
- [7, 68],
- [7, 82],
- [7, 87],
- [7, 92],
- [7, 97],
- [7, 98],
- [7, 99],
- [7, 106],
- [7, 111],
- [7, 116],
- [7, 117],
- [7, 118],
- [7, 130],
- [7, 125],
- [7, 135],
- [7, 137],
- [7, 136],
- [7, 144],
- [7, 145],
- [7, 146],
- [7, 154],
- [7, 153],
- [7, 155],
- [7, 163],
- [7, 164],
- [7, 162],
- [7, 171],
- [7, 174],
- [7, 175],
- [7, 178],
- [7, 179],
- [7, 183],
- [7, 182],
- [7, 186],
- [7, 187],
- [7, 191],
- [7, 190],
- [7, 198],
- [7, 199],
- [7, 195],
- [7, 194],
- [7, 202],
- [19, 82],
- [19, 87],
- [19, 92],
- [19, 97],
- [19, 98],
- [19, 99],
- [19, 171],
- [19, 174],
- [19, 175],
- [19, 178],
- [19, 179],
- [19, 183],
- [19, 182],
- [19, 202],
- [28, 82],
- [28, 106],
- [28, 111],
- [28, 116],
- [28, 117],
- [28, 118],
- [28, 171],
- [28, 174],
- [28, 175],
- [28, 186],
- [28, 187],
- [28, 191],
- [28, 190],
- [28, 202],
- [37, 82],
- [37, 130],
- [37, 125],
- [37, 135],
- [37, 137],
- [37, 136],
- [37, 171],
- [37, 174],
- [37, 175],
- [37, 198],
- [37, 199],
- [37, 195],
- [37, 194],
- [37, 202],
- [82, 171],
- [82, 174],
- [82, 175],
- [82, 202],
- [8, 20],
- [8, 44],
- [8, 52],
- [8, 59],
- [8, 29],
- [8, 38],
- [8, 70],
- [8, 69],
- [8, 71],
- [8, 72],
- [8, 87],
- [8, 93],
- [8, 83],
- [8, 101],
- [8, 100],
- [8, 102],
- [8, 106],
- [8, 125],
- [8, 144],
- [8, 145],
- [8, 146],
- [8, 131],
- [8, 156],
- [8, 157],
- [8, 158],
- [8, 112],
- [8, 165],
- [8, 167],
- [8, 166],
- [8, 120],
- [8, 119],
- [8, 121],
- [8, 139],
- [8, 140],
- [8, 138],
- [8, 171],
- [8, 178],
- [8, 179],
- [8, 184],
- [8, 185],
- [8, 177],
- [8, 176],
- [8, 186],
- [8, 187],
- [8, 195],
- [8, 194],
- [8, 201],
- [8, 200],
- [8, 192],
- [8, 193],
- [8, 202],
- [20, 87],
- [20, 93],
- [20, 83],
- [20, 101],
- [20, 100],
- [20, 102],
- [20, 171],
- [20, 178],
- [20, 179],
- [20, 184],
- [20, 185],
- [20, 177],
- [20, 176],
- [20, 202],
- [44, 87],
- [44, 106],
- [44, 125],
- [44, 144],
- [44, 145],
- [44, 146],
- [44, 171],
- [44, 178],
- [44, 179],
- [44, 186],
- [44, 187],
- [44, 195],
- [44, 194],
- [44, 202],
- [87, 171],
- [87, 178],
- [87, 179],
- [87, 202],
- [52, 93],
- [52, 106],
- [52, 131],
- [52, 156],
- [52, 157],
- [52, 158],
- [52, 171],
- [52, 184],
- [52, 185],
- [52, 186],
- [52, 187],
- [52, 201],
- [52, 200],
- [52, 202],
- [59, 93],
- [59, 112],
- [59, 125],
- [59, 165],
- [59, 167],
- [59, 166],
- [59, 171],
- [59, 184],
- [59, 185],
- [59, 192],
- [59, 193],
- [59, 195],
- [59, 194],
- [59, 202],
- [93, 171],
- [93, 184],
- [93, 185],
- [93, 202],
- [9, 29],
- [9, 39],
- [9, 45],
- [9, 51],
- [9, 60],
- [9, 21],
- [9, 74],
- [9, 75],
- [9, 73],
- [9, 76],
- [9, 106],
- [9, 112],
- [9, 83],
- [9, 120],
- [9, 119],
- [9, 121],
- [9, 130],
- [9, 126],
- [9, 142],
- [9, 141],
- [9, 143],
- [9, 88],
- [9, 148],
- [9, 147],
- [9, 149],
- [9, 92],
- [9, 154],
- [9, 153],
- [9, 155],
- [9, 170],
- [9, 168],
- [9, 169],
- [9, 104],
- [9, 105],
- [9, 103],
- [9, 171],
- [9, 186],
- [9, 187],
- [9, 192],
- [9, 193],
- [9, 177],
- [9, 176],
- [9, 198],
- [9, 199],
- [9, 196],
- [9, 197],
- [9, 181],
- [9, 180],
- [9, 183],
- [9, 182],
- [9, 202],
- [29, 106],
- [29, 112],
- [29, 83],
- [29, 120],
- [29, 119],
- [29, 121],
- [29, 171],
- [29, 186],
- [29, 187],
- [29, 192],
- [29, 193],
- [29, 177],
- [29, 176],
- [29, 202],
- [39, 130],
- [39, 126],
- [39, 83],
- [39, 142],
- [39, 141],
- [39, 143],
- [39, 171],
- [39, 198],
- [39, 199],
- [39, 196],
- [39, 197],
- [39, 177],
- [39, 176],
- [39, 202],
- [45, 106],
- [45, 126],
- [45, 88],
- [45, 148],
- [45, 147],
- [45, 149],
- [45, 171],
- [45, 186],
- [45, 187],
- [45, 196],
- [45, 197],
- [45, 181],
- [45, 180],
- [45, 202],
- [51, 106],
- [51, 130],
- [51, 92],
- [51, 154],
- [51, 153],
- [51, 155],
- [51, 171],
- [51, 186],
- [51, 187],
- [51, 198],
- [51, 199],
- [51, 183],
- [51, 182],
- [51, 202],
- [106, 171],
- [106, 186],
- [106, 187],
- [106, 202],
- [130, 171],
- [130, 198],
- [130, 199],
- [130, 202],
- [60, 112],
- [60, 126],
- [60, 92],
- [60, 170],
- [60, 168],
- [60, 169],
- [60, 171],
- [60, 192],
- [60, 193],
- [60, 196],
- [60, 197],
- [60, 183],
- [60, 182],
- [60, 202],
- [112, 171],
- [112, 192],
- [112, 193],
- [112, 202],
- [126, 171],
- [126, 196],
- [126, 197],
- [126, 202],
- [10, 21],
- [10, 30],
- [10, 38],
- [10, 46],
- [10, 53],
- [10, 58],
- [10, 78],
- [10, 79],
- [10, 80],
- [10, 77],
- [10, 83],
- [10, 88],
- [10, 92],
- [10, 104],
- [10, 105],
- [10, 103],
- [10, 107],
- [10, 111],
- [10, 123],
- [10, 124],
- [10, 122],
- [10, 131],
- [10, 125],
- [10, 139],
- [10, 140],
- [10, 138],
- [10, 151],
- [10, 152],
- [10, 150],
- [10, 161],
- [10, 160],
- [10, 159],
- [10, 163],
- [10, 164],
- [10, 162],
- [10, 171],
- [10, 177],
- [10, 176],
- [10, 181],
- [10, 180],
- [10, 183],
- [10, 182],
- [10, 189],
- [10, 188],
- [10, 191],
- [10, 190],
- [10, 201],
- [10, 200],
- [10, 195],
- [10, 194],
- [10, 202],
- [21, 83],
- [21, 88],
- [21, 92],
- [21, 104],
- [21, 105],
- [21, 103],
- [21, 171],
- [21, 177],
- [21, 176],
- [21, 181],
- [21, 180],
- [21, 183],
- [21, 182],
- [21, 202],
- [30, 83],
- [30, 107],
- [30, 111],
- [30, 123],
- [30, 124],
- [30, 122],
- [30, 171],
- [30, 177],
- [30, 176],
- [30, 189],
- [30, 188],
- [30, 191],
- [30, 190],
- [30, 202],
- [38, 83],
- [38, 131],
- [38, 125],
- [38, 139],
- [38, 140],
- [38, 138],
- [38, 171],
- [38, 177],
- [38, 176],
- [38, 201],
- [38, 200],
- [38, 195],
- [38, 194],
- [38, 202],
- [83, 171],
- [83, 177],
- [83, 176],
- [83, 202],
- [46, 88],
- [46, 107],
- [46, 125],
- [46, 151],
- [46, 152],
- [46, 150],
- [46, 171],
- [46, 181],
- [46, 180],
- [46, 189],
- [46, 188],
- [46, 195],
- [46, 194],
- [46, 202],
- [88, 171],
- [88, 181],
- [88, 180],
- [88, 202],
- [53, 107],
- [53, 131],
- [53, 92],
- [53, 161],
- [53, 160],
- [53, 159],
- [53, 171],
- [53, 189],
- [53, 188],
- [53, 201],
- [53, 200],
- [53, 183],
- [53, 182],
- [53, 202],
- [107, 171],
- [107, 189],
- [107, 188],
- [107, 202],
- [131, 171],
- [131, 201],
- [131, 200],
- [131, 202],
- [58, 92],
- [58, 111],
- [58, 125],
- [58, 163],
- [58, 164],
- [58, 162],
- [58, 171],
- [58, 183],
- [58, 182],
- [58, 191],
- [58, 190],
- [58, 195],
- [58, 194],
- [58, 202],
- [92, 171],
- [92, 183],
- [92, 182],
- [92, 202],
- [111, 171],
- [111, 191],
- [111, 190],
- [111, 202],
- [125, 171],
- [125, 195],
- [125, 194],
- [125, 202],
- [171, 202],
- [11, 22],
- [11, 31],
- [11, 40],
- [11, 47],
- [11, 54],
- [11, 61],
- [11, 65],
- [11, 69],
- [11, 73],
- [11, 77],
- [11, 84],
- [11, 89],
- [11, 94],
- [11, 97],
- [11, 100],
- [11, 103],
- [11, 108],
- [11, 113],
- [11, 116],
- [11, 119],
- [11, 122],
- [11, 132],
- [11, 127],
- [11, 135],
- [11, 141],
- [11, 138],
- [11, 144],
- [11, 147],
- [11, 150],
- [11, 156],
- [11, 153],
- [11, 159],
- [11, 165],
- [11, 168],
- [11, 162],
- [11, 172],
- [11, 174],
- [11, 176],
- [11, 178],
- [11, 180],
- [11, 184],
- [11, 182],
- [11, 186],
- [11, 188],
- [11, 192],
- [11, 190],
- [11, 198],
- [11, 200],
- [11, 196],
- [11, 194],
- [11, 202],
- [22, 84],
- [22, 89],
- [22, 94],
- [22, 97],
- [22, 100],
- [22, 103],
- [22, 172],
- [22, 174],
- [22, 176],
- [22, 178],
- [22, 180],
- [22, 184],
- [22, 182],
- [22, 202],
- [31, 84],
- [31, 108],
- [31, 113],
- [31, 116],
- [31, 119],
- [31, 122],
- [31, 172],
- [31, 174],
- [31, 176],
- [31, 186],
- [31, 188],
- [31, 192],
- [31, 190],
- [31, 202],
- [40, 84],
- [40, 132],
- [40, 127],
- [40, 135],
- [40, 141],
- [40, 138],
- [40, 172],
- [40, 174],
- [40, 176],
- [40, 198],
- [40, 200],
- [40, 196],
- [40, 194],
- [40, 202],
- [84, 172],
- [84, 174],
- [84, 176],
- [84, 202],
- [47, 89],
- [47, 108],
- [47, 127],
- [47, 144],
- [47, 147],
- [47, 150],
- [47, 172],
- [47, 178],
- [47, 180],
- [47, 186],
- [47, 188],
- [47, 196],
- [47, 194],
- [47, 202],
- [89, 172],
- [89, 178],
- [89, 180],
- [89, 202],
- [54, 108],
- [54, 132],
- [54, 94],
- [54, 156],
- [54, 153],
- [54, 159],
- [54, 172],
- [54, 186],
- [54, 188],
- [54, 198],
- [54, 200],
- [54, 184],
- [54, 182],
- [54, 202],
- [108, 172],
- [108, 186],
- [108, 188],
- [108, 202],
- [132, 172],
- [132, 198],
- [132, 200],
- [132, 202],
- [61, 94],
- [61, 113],
- [61, 127],
- [61, 165],
- [61, 168],
- [61, 162],
- [61, 172],
- [61, 184],
- [61, 182],
- [61, 192],
- [61, 190],
- [61, 196],
- [61, 194],
- [61, 202],
- [94, 172],
- [94, 184],
- [94, 182],
- [94, 202],
- [113, 172],
- [113, 192],
- [113, 190],
- [113, 202],
- [127, 172],
- [127, 196],
- [127, 194],
- [127, 202],
- [172, 202],
- [12, 23],
- [12, 32],
- [12, 41],
- [12, 65],
- [12, 70],
- [12, 74],
- [12, 78],
- [12, 48],
- [12, 55],
- [12, 62],
- [12, 85],
- [12, 97],
- [12, 101],
- [12, 104],
- [12, 90],
- [12, 95],
- [12, 116],
- [12, 120],
- [12, 123],
- [12, 109],
- [12, 114],
- [12, 135],
- [12, 142],
- [12, 139],
- [12, 133],
- [12, 128],
- [12, 144],
- [12, 153],
- [12, 162],
- [12, 157],
- [12, 166],
- [12, 148],
- [12, 169],
- [12, 151],
- [12, 160],
- [12, 174],
- [12, 177],
- [12, 173],
- [12, 178],
- [12, 182],
- [12, 185],
- [12, 181],
- [12, 186],
- [12, 190],
- [12, 193],
- [12, 189],
- [12, 198],
- [12, 194],
- [12, 197],
- [12, 201],
- [12, 202],
- [23, 85],
- [23, 97],
- [23, 101],
- [23, 104],
- [23, 90],
- [23, 95],
- [23, 174],
- [23, 177],
- [23, 173],
- [23, 178],
- [23, 182],
- [23, 185],
- [23, 181],
- [23, 202],
- [32, 85],
- [32, 116],
- [32, 120],
- [32, 123],
- [32, 109],
- [32, 114],
- [32, 174],
- [32, 177],
- [32, 173],
- [32, 186],
- [32, 190],
- [32, 193],
- [32, 189],
- [32, 202],
- [41, 85],
- [41, 135],
- [41, 142],
- [41, 139],
- [41, 133],
- [41, 128],
- [41, 174],
- [41, 177],
- [41, 173],
- [41, 198],
- [41, 194],
- [41, 197],
- [41, 201],
- [41, 202],
- [85, 174],
- [85, 177],
- [85, 173],
- [85, 202],
- [65, 97],
- [65, 116],
- [65, 135],
- [65, 144],
- [65, 153],
- [65, 162],
- [65, 174],
- [65, 178],
- [65, 182],
- [65, 186],
- [65, 190],
- [65, 198],
- [65, 194],
- [65, 202],
- [97, 174],
- [97, 178],
- [97, 182],
- [97, 202],
- [116, 174],
- [116, 186],
- [116, 190],
- [116, 202],
- [135, 174],
- [135, 198],
- [135, 194],
- [135, 202],
- [174, 202],
- [70, 101],
- [70, 120],
- [70, 139],
- [70, 144],
- [70, 157],
- [70, 166],
- [70, 177],
- [70, 178],
- [70, 185],
- [70, 186],
- [70, 193],
- [70, 201],
- [70, 194],
- [70, 202],
- [101, 177],
- [101, 178],
- [101, 185],
- [101, 202],
- [74, 120],
- [74, 142],
- [74, 104],
- [74, 148],
- [74, 153],
- [74, 169],
- [74, 177],
- [74, 186],
- [74, 193],
- [74, 198],
- [74, 197],
- [74, 181],
- [74, 182],
- [74, 202],
- [120, 177],
- [120, 186],
- [120, 193],
- [120, 202],
- [142, 177],
- [142, 198],
- [142, 197],
- [142, 202],
- [78, 104],
- [78, 123],
- [78, 139],
- [78, 151],
- [78, 160],
- [78, 162],
- [78, 177],
- [78, 181],
- [78, 182],
- [78, 189],
- [78, 190],
- [78, 201],
- [78, 194],
- [78, 202],
- [104, 177],
- [104, 181],
- [104, 182],
- [104, 202],
- [123, 177],
- [123, 189],
- [123, 190],
- [123, 202],
- [139, 177],
- [139, 201],
- [139, 194],
- [139, 202],
- [177, 202],
- [13, 24],
- [13, 48],
- [13, 56],
- [13, 63],
- [13, 66],
- [13, 69],
- [13, 75],
- [13, 79],
- [13, 33],
- [13, 42],
- [13, 90],
- [13, 96],
- [13, 98],
- [13, 100],
- [13, 105],
- [13, 86],
- [13, 144],
- [13, 148],
- [13, 151],
- [13, 109],
- [13, 128],
- [13, 156],
- [13, 154],
- [13, 161],
- [13, 134],
- [13, 165],
- [13, 170],
- [13, 163],
- [13, 115],
- [13, 117],
- [13, 136],
- [13, 119],
- [13, 138],
- [13, 143],
- [13, 124],
- [13, 178],
- [13, 181],
- [13, 173],
- [13, 184],
- [13, 183],
- [13, 175],
- [13, 176],
- [13, 186],
- [13, 194],
- [13, 197],
- [13, 189],
- [13, 200],
- [13, 199],
- [13, 192],
- [13, 191],
- [13, 202],
- [24, 90],
- [24, 96],
- [24, 98],
- [24, 100],
- [24, 105],
- [24, 86],
- [24, 178],
- [24, 181],
- [24, 173],
- [24, 184],
- [24, 183],
- [24, 175],
- [24, 176],
- [24, 202],
- [48, 90],
- [48, 144],
- [48, 148],
- [48, 151],
- [48, 109],
- [48, 128],
- [48, 178],
- [48, 181],
- [48, 173],
- [48, 186],
- [48, 194],
- [48, 197],
- [48, 189],
- [48, 202],
- [90, 178],
- [90, 181],
- [90, 173],
- [90, 202],
- [56, 96],
- [56, 156],
- [56, 154],
- [56, 161],
- [56, 109],
- [56, 134],
- [56, 184],
- [56, 183],
- [56, 173],
- [56, 186],
- [56, 200],
- [56, 199],
- [56, 189],
- [56, 202],
- [63, 96],
- [63, 165],
- [63, 170],
- [63, 163],
- [63, 115],
- [63, 128],
- [63, 184],
- [63, 183],
- [63, 173],
- [63, 192],
- [63, 194],
- [63, 197],
- [63, 191],
- [63, 202],
- [96, 184],
- [96, 183],
- [96, 173],
- [96, 202],
- [66, 98],
- [66, 144],
- [66, 154],
- [66, 163],
- [66, 117],
- [66, 136],
- [66, 178],
- [66, 183],
- [66, 175],
- [66, 186],
- [66, 194],
- [66, 199],
- [66, 191],
- [66, 202],
- [98, 178],
- [98, 183],
- [98, 175],
- [98, 202],
- [69, 100],
- [69, 144],
- [69, 156],
- [69, 165],
- [69, 119],
- [69, 138],
- [69, 178],
- [69, 184],
- [69, 176],
- [69, 186],
- [69, 194],
- [69, 200],
- [69, 192],
- [69, 202],
- [100, 178],
- [100, 184],
- [100, 176],
- [100, 202],
- [144, 178],
- [144, 186],
- [144, 194],
- [144, 202],
- [178, 202],
- [156, 184],
- [156, 186],
- [156, 200],
- [156, 202],
- [165, 184],
- [165, 192],
- [165, 194],
- [165, 202],
- [184, 202],
- [75, 148],
- [75, 154],
- [75, 170],
- [75, 105],
- [75, 119],
- [75, 143],
- [75, 181],
- [75, 186],
- [75, 197],
- [75, 183],
- [75, 199],
- [75, 192],
- [75, 176],
- [75, 202],
- [148, 181],
- [148, 186],
- [148, 197],
- [148, 202],
- [154, 183],
- [154, 186],
- [154, 199],
- [154, 202],
- [170, 183],
- [170, 192],
- [170, 197],
- [170, 202],
- [79, 105],
- [79, 151],
- [79, 161],
- [79, 163],
- [79, 124],
- [79, 138],
- [79, 181],
- [79, 183],
- [79, 176],
- [79, 189],
- [79, 194],
- [79, 200],
- [79, 191],
- [79, 202],
- [105, 181],
- [105, 183],
- [105, 176],
- [105, 202],
- [151, 181],
- [151, 189],
- [151, 194],
- [151, 202],
- [181, 202],
- [161, 183],
- [161, 189],
- [161, 200],
- [161, 202],
- [163, 183],
- [163, 191],
- [163, 194],
- [163, 202],
- [183, 202],
- [14, 33],
- [14, 43],
- [14, 49],
- [14, 55],
- [14, 64],
- [14, 67],
- [14, 71],
- [14, 73],
- [14, 80],
- [14, 25],
- [14, 109],
- [14, 115],
- [14, 117],
- [14, 119],
- [14, 124],
- [14, 86],
- [14, 133],
- [14, 129],
- [14, 137],
- [14, 141],
- [14, 140],
- [14, 145],
- [14, 147],
- [14, 152],
- [14, 91],
- [14, 157],
- [14, 153],
- [14, 160],
- [14, 95],
- [14, 167],
- [14, 168],
- [14, 164],
- [14, 99],
- [14, 102],
- [14, 103],
- [14, 186],
- [14, 189],
- [14, 173],
- [14, 192],
- [14, 191],
- [14, 175],
- [14, 176],
- [14, 198],
- [14, 201],
- [14, 196],
- [14, 195],
- [14, 179],
- [14, 180],
- [14, 185],
- [14, 182],
- [14, 202],
- [33, 109],
- [33, 115],
- [33, 117],
- [33, 119],
- [33, 124],
- [33, 86],
- [33, 186],
- [33, 189],
- [33, 173],
- [33, 192],
- [33, 191],
- [33, 175],
- [33, 176],
- [33, 202],
- [43, 133],
- [43, 129],
- [43, 137],
- [43, 141],
- [43, 140],
- [43, 86],
- [43, 198],
- [43, 201],
- [43, 173],
- [43, 196],
- [43, 195],
- [43, 175],
- [43, 176],
- [43, 202],
- [49, 109],
- [49, 129],
- [49, 145],
- [49, 147],
- [49, 152],
- [49, 91],
- [49, 186],
- [49, 189],
- [49, 173],
- [49, 196],
- [49, 195],
- [49, 179],
- [49, 180],
- [49, 202],
- [55, 109],
- [55, 133],
- [55, 157],
- [55, 153],
- [55, 160],
- [55, 95],
- [55, 186],
- [55, 189],
- [55, 173],
- [55, 198],
- [55, 201],
- [55, 185],
- [55, 182],
- [55, 202],
- [109, 186],
- [109, 189],
- [109, 173],
- [109, 202],
- [133, 198],
- [133, 201],
- [133, 173],
- [133, 202],
- [64, 115],
- [64, 129],
- [64, 167],
- [64, 168],
- [64, 164],
- [64, 95],
- [64, 192],
- [64, 191],
- [64, 173],
- [64, 196],
- [64, 195],
- [64, 185],
- [64, 182],
- [64, 202],
- [115, 192],
- [115, 191],
- [115, 173],
- [115, 202],
- [129, 196],
- [129, 195],
- [129, 173],
- [129, 202],
- [67, 117],
- [67, 137],
- [67, 145],
- [67, 153],
- [67, 164],
- [67, 99],
- [67, 186],
- [67, 191],
- [67, 175],
- [67, 198],
- [67, 195],
- [67, 179],
- [67, 182],
- [67, 202],
- [117, 186],
- [117, 191],
- [117, 175],
- [117, 202],
- [137, 198],
- [137, 195],
- [137, 175],
- [137, 202],
- [71, 145],
- [71, 157],
- [71, 167],
- [71, 119],
- [71, 140],
- [71, 102],
- [71, 186],
- [71, 195],
- [71, 179],
- [71, 201],
- [71, 185],
- [71, 192],
- [71, 176],
- [71, 202],
- [145, 186],
- [145, 195],
- [145, 179],
- [145, 202],
- [157, 186],
- [157, 201],
- [157, 185],
- [157, 202],
- [167, 192],
- [167, 195],
- [167, 185],
- [167, 202],
- [73, 119],
- [73, 141],
- [73, 147],
- [73, 153],
- [73, 168],
- [73, 103],
- [73, 186],
- [73, 192],
- [73, 176],
- [73, 198],
- [73, 196],
- [73, 180],
- [73, 182],
- [73, 202],
- [119, 186],
- [119, 192],
- [119, 176],
- [119, 202],
- [141, 198],
- [141, 196],
- [141, 176],
- [141, 202],
- [147, 186],
- [147, 196],
- [147, 180],
- [147, 202],
- [153, 186],
- [153, 198],
- [153, 182],
- [153, 202],
- [186, 202],
- [198, 202],
- [168, 192],
- [168, 196],
- [168, 182],
- [168, 202],
- [192, 202],
- [196, 202],
- [80, 124],
- [80, 140],
- [80, 152],
- [80, 160],
- [80, 164],
- [80, 103],
- [80, 189],
- [80, 191],
- [80, 176],
- [80, 201],
- [80, 195],
- [80, 180],
- [80, 182],
- [80, 202],
- [124, 189],
- [124, 191],
- [124, 176],
- [124, 202],
- [140, 201],
- [140, 195],
- [140, 176],
- [140, 202],
- [152, 189],
- [152, 195],
- [152, 180],
- [152, 202],
- [160, 189],
- [160, 201],
- [160, 182],
- [160, 202],
- [189, 202],
- [201, 202],
- [164, 191],
- [164, 195],
- [164, 182],
- [164, 202],
- [191, 202],
- [195, 202],
- [15, 25],
- [15, 34],
- [15, 42],
- [15, 50],
- [15, 57],
- [15, 62],
- [15, 68],
- [15, 72],
- [15, 76],
- [15, 77],
- [15, 86],
- [15, 91],
- [15, 95],
- [15, 99],
- [15, 102],
- [15, 103],
- [15, 110],
- [15, 114],
- [15, 118],
- [15, 121],
- [15, 122],
- [15, 134],
- [15, 128],
- [15, 136],
- [15, 143],
- [15, 138],
- [15, 146],
- [15, 149],
- [15, 150],
- [15, 158],
- [15, 155],
- [15, 159],
- [15, 166],
- [15, 169],
- [15, 162],
- [15, 173],
- [15, 175],
- [15, 176],
- [15, 179],
- [15, 180],
- [15, 185],
- [15, 182],
- [15, 187],
- [15, 188],
- [15, 193],
- [15, 190],
- [15, 199],
- [15, 200],
- [15, 197],
- [15, 194],
- [15, 202],
- [25, 86],
- [25, 91],
- [25, 95],
- [25, 99],
- [25, 102],
- [25, 103],
- [25, 173],
- [25, 175],
- [25, 176],
- [25, 179],
- [25, 180],
- [25, 185],
- [25, 182],
- [25, 202],
- [34, 86],
- [34, 110],
- [34, 114],
- [34, 118],
- [34, 121],
- [34, 122],
- [34, 173],
- [34, 175],
- [34, 176],
- [34, 187],
- [34, 188],
- [34, 193],
- [34, 190],
- [34, 202],
- [42, 86],
- [42, 134],
- [42, 128],
- [42, 136],
- [42, 143],
- [42, 138],
- [42, 173],
- [42, 175],
- [42, 176],
- [42, 199],
- [42, 200],
- [42, 197],
- [42, 194],
- [42, 202],
- [86, 173],
- [86, 175],
- [86, 176],
- [86, 202],
- [50, 91],
- [50, 110],
- [50, 128],
- [50, 146],
- [50, 149],
- [50, 150],
- [50, 173],
- [50, 179],
- [50, 180],
- [50, 187],
- [50, 188],
- [50, 197],
- [50, 194],
- [50, 202],
- [91, 173],
- [91, 179],
- [91, 180],
- [91, 202],
- [57, 110],
- [57, 134],
- [57, 95],
- [57, 158],
- [57, 155],
- [57, 159],
- [57, 173],
- [57, 187],
- [57, 188],
- [57, 199],
- [57, 200],
- [57, 185],
- [57, 182],
- [57, 202],
- [110, 173],
- [110, 187],
- [110, 188],
- [110, 202],
- [134, 173],
- [134, 199],
- [134, 200],
- [134, 202],
- [62, 95],
- [62, 114],
- [62, 128],
- [62, 166],
- [62, 169],
- [62, 162],
- [62, 173],
- [62, 185],
- [62, 182],
- [62, 193],
- [62, 190],
- [62, 197],
- [62, 194],
- [62, 202],
- [95, 173],
- [95, 185],
- [95, 182],
- [95, 202],
- [114, 173],
- [114, 193],
- [114, 190],
- [114, 202],
- [128, 173],
- [128, 197],
- [128, 194],
- [128, 202],
- [173, 202],
- [68, 99],
- [68, 118],
- [68, 136],
- [68, 146],
- [68, 155],
- [68, 162],
- [68, 175],
- [68, 179],
- [68, 182],
- [68, 187],
- [68, 190],
- [68, 199],
- [68, 194],
- [68, 202],
- [99, 175],
- [99, 179],
- [99, 182],
- [99, 202],
- [118, 175],
- [118, 187],
- [118, 190],
- [118, 202],
- [136, 175],
- [136, 199],
- [136, 194],
- [136, 202],
- [175, 202],
- [72, 102],
- [72, 146],
- [72, 158],
- [72, 166],
- [72, 121],
- [72, 138],
- [72, 179],
- [72, 185],
- [72, 176],
- [72, 187],
- [72, 194],
- [72, 200],
- [72, 193],
- [72, 202],
- [102, 179],
- [102, 185],
- [102, 176],
- [102, 202],
- [146, 179],
- [146, 187],
- [146, 194],
- [146, 202],
- [179, 202],
- [158, 185],
- [158, 187],
- [158, 200],
- [158, 202],
- [166, 185],
- [166, 193],
- [166, 194],
- [166, 202],
- [185, 202],
- [76, 121],
- [76, 143],
- [76, 149],
- [76, 155],
- [76, 169],
- [76, 103],
- [76, 187],
- [76, 193],
- [76, 176],
- [76, 199],
- [76, 197],
- [76, 180],
- [76, 182],
- [76, 202],
- [121, 187],
- [121, 193],
- [121, 176],
- [121, 202],
- [143, 199],
- [143, 197],
- [143, 176],
- [143, 202],
- [149, 187],
- [149, 197],
- [149, 180],
- [149, 202],
- [155, 187],
- [155, 199],
- [155, 182],
- [155, 202],
- [187, 202],
- [199, 202],
- [169, 193],
- [169, 197],
- [169, 182],
- [169, 202],
- [193, 202],
- [197, 202],
- [77, 103],
- [77, 122],
- [77, 138],
- [77, 150],
- [77, 159],
- [77, 162],
- [77, 176],
- [77, 180],
- [77, 182],
- [77, 188],
- [77, 190],
- [77, 200],
- [77, 194],
- [77, 202],
- [103, 176],
- [103, 180],
- [103, 182],
- [103, 202],
- [122, 176],
- [122, 188],
- [122, 190],
- [122, 202],
- [138, 176],
- [138, 200],
- [138, 194],
- [138, 202],
- [176, 202],
- [150, 180],
- [150, 188],
- [150, 194],
- [150, 202],
- [180, 202],
- [159, 188],
- [159, 200],
- [159, 182],
- [159, 202],
- [188, 202],
- [200, 202],
- [162, 182],
- [162, 190],
- [162, 194],
- [162, 202],
- [182, 202],
- [190, 202],
- [194, 202]]
-
-B3_rels = [[0, 1],
- [0, 2],
- [0, 3],
- [0, 4],
- [0, 5],
- [0, 6],
- [0, 7],
- [0, 8],
- [0, 9],
- [0, 10],
- [0, 11],
- [0, 12],
- [0, 13],
- [0, 14],
- [0, 15],
- [0, 16],
- [0, 18],
- [0, 19],
- [0, 17],
- [0, 22],
- [0, 20],
- [0, 21],
- [0, 23],
- [1, 10],
- [1, 11],
- [1, 12],
- [1, 13],
- [1, 23],
- [2, 10],
- [2, 14],
- [2, 15],
- [2, 16],
- [2, 23],
- [3, 10],
- [3, 18],
- [3, 19],
- [3, 17],
- [3, 23],
- [4, 10],
- [4, 22],
- [4, 20],
- [4, 21],
- [4, 23],
- [10, 23],
- [5, 11],
- [5, 14],
- [5, 20],
- [5, 17],
- [5, 23],
- [11, 23],
- [6, 14],
- [6, 18],
- [6, 12],
- [6, 21],
- [6, 23],
- [14, 23],
- [18, 23],
- [7, 15],
- [7, 22],
- [7, 12],
- [7, 17],
- [7, 23],
- [15, 23],
- [22, 23],
- [8, 12],
- [8, 19],
- [8, 20],
- [8, 16],
- [8, 23],
- [12, 23],
- [19, 23],
- [20, 23],
- [9, 13],
- [9, 16],
- [9, 17],
- [9, 21],
- [9, 23],
- [13, 23],
- [16, 23],
- [17, 23],
- [21, 23]]
-
-B4_rels = [[0, 1],
- [0, 2],
- [0, 3],
- [0, 4],
- [0, 5],
- [0, 6],
- [0, 7],
- [0, 8],
- [0, 9],
- [0, 10],
- [0, 11],
- [0, 12],
- [0, 13],
- [0, 14],
- [0, 15],
- [0, 16],
- [0, 17],
- [0, 18],
- [0, 19],
- [0, 20],
- [0, 21],
- [0, 22],
- [0, 23],
- [0, 24],
- [0, 25],
- [0, 26],
- [0, 27],
- [0, 28],
- [0, 29],
- [0, 30],
- [0, 31],
- [0, 32],
- [0, 33],
- [0, 35],
- [0, 36],
- [0, 34],
- [0, 37],
- [0, 39],
- [0, 40],
- [0, 38],
- [0, 41],
- [0, 44],
- [0, 42],
- [0, 43],
- [0, 45],
- [0, 48],
- [0, 46],
- [0, 47],
- [0, 49],
- [0, 50],
- [0, 51],
- [0, 52],
- [0, 53],
- [0, 54],
- [0, 56],
- [0, 55],
- [0, 57],
- [0, 59],
- [0, 58],
- [0, 61],
- [0, 62],
- [0, 63],
- [0, 64],
- [0, 60],
- [0, 66],
- [0, 68],
- [0, 65],
- [0, 69],
- [0, 67],
- [0, 72],
- [0, 73],
- [0, 74],
- [0, 70],
- [0, 71],
- [0, 75],
- [0, 76],
- [0, 77],
- [0, 78],
- [0, 79],
- [0, 80],
- [0, 81],
- [0, 83],
- [0, 84],
- [0, 82],
- [0, 87],
- [0, 85],
- [0, 86],
- [0, 88],
- [0, 89],
- [0, 90],
- [0, 92],
- [0, 93],
- [0, 91],
- [0, 96],
- [0, 94],
- [0, 95],
- [0, 100],
- [0, 101],
- [0, 102],
- [0, 103],
- [0, 104],
- [0, 105],
- [0, 98],
- [0, 99],
- [0, 97],
- [0, 113],
- [0, 114],
- [0, 112],
- [0, 108],
- [0, 106],
- [0, 107],
- [0, 111],
- [0, 109],
- [0, 110],
- [0, 115],
- [1, 17],
- [1, 18],
- [1, 19],
- [1, 20],
- [1, 21],
- [1, 22],
- [1, 23],
- [1, 24],
- [1, 25],
- [1, 75],
- [1, 76],
- [1, 77],
- [1, 78],
- [1, 79],
- [1, 80],
- [1, 81],
- [1, 83],
- [1, 84],
- [1, 82],
- [1, 87],
- [1, 85],
- [1, 86],
- [1, 115],
- [2, 17],
- [2, 26],
- [2, 27],
- [2, 28],
- [2, 29],
- [2, 30],
- [2, 31],
- [2, 32],
- [2, 33],
- [2, 75],
- [2, 76],
- [2, 77],
- [2, 78],
- [2, 88],
- [2, 89],
- [2, 90],
- [2, 92],
- [2, 93],
- [2, 91],
- [2, 96],
- [2, 94],
- [2, 95],
- [2, 115],
- [3, 17],
- [3, 35],
- [3, 36],
- [3, 34],
- [3, 37],
- [3, 39],
- [3, 40],
- [3, 38],
- [3, 41],
- [3, 75],
- [3, 76],
- [3, 77],
- [3, 78],
- [3, 100],
- [3, 101],
- [3, 102],
- [3, 103],
- [3, 104],
- [3, 105],
- [3, 98],
- [3, 99],
- [3, 97],
- [3, 115],
- [4, 17],
- [4, 44],
- [4, 42],
- [4, 43],
- [4, 45],
- [4, 48],
- [4, 46],
- [4, 47],
- [4, 49],
- [4, 75],
- [4, 76],
- [4, 77],
- [4, 78],
- [4, 113],
- [4, 114],
- [4, 112],
- [4, 108],
- [4, 106],
- [4, 107],
- [4, 111],
- [4, 109],
- [4, 110],
- [4, 115],
- [17, 75],
- [17, 76],
- [17, 77],
- [17, 78],
- [17, 115],
- [5, 18],
- [5, 26],
- [5, 42],
- [5, 34],
- [5, 50],
- [5, 51],
- [5, 52],
- [5, 53],
- [5, 54],
- [5, 75],
- [5, 79],
- [5, 80],
- [5, 81],
- [5, 88],
- [5, 89],
- [5, 90],
- [5, 108],
- [5, 106],
- [5, 107],
- [5, 98],
- [5, 99],
- [5, 97],
- [5, 115],
- [18, 75],
- [18, 79],
- [18, 80],
- [18, 81],
- [18, 115],
- [6, 26],
- [6, 35],
- [6, 19],
- [6, 43],
- [6, 56],
- [6, 55],
- [6, 57],
- [6, 59],
- [6, 58],
- [6, 75],
- [6, 88],
- [6, 89],
- [6, 90],
- [6, 100],
- [6, 101],
- [6, 102],
- [6, 83],
- [6, 84],
- [6, 82],
- [6, 111],
- [6, 109],
- [6, 110],
- [6, 115],
- [26, 75],
- [26, 88],
- [26, 89],
- [26, 90],
- [26, 115],
- [35, 75],
- [35, 100],
- [35, 101],
- [35, 102],
- [35, 115],
- [7, 27],
- [7, 44],
- [7, 19],
- [7, 34],
- [7, 61],
- [7, 62],
- [7, 63],
- [7, 64],
- [7, 60],
- [7, 75],
- [7, 92],
- [7, 93],
- [7, 91],
- [7, 113],
- [7, 114],
- [7, 112],
- [7, 83],
- [7, 84],
- [7, 82],
- [7, 98],
- [7, 99],
- [7, 97],
- [7, 115],
- [27, 75],
- [27, 92],
- [27, 93],
- [27, 91],
- [27, 115],
- [44, 75],
- [44, 113],
- [44, 114],
- [44, 112],
- [44, 115],
- [8, 19],
- [8, 36],
- [8, 42],
- [8, 28],
- [8, 66],
- [8, 68],
- [8, 65],
- [8, 69],
- [8, 67],
- [8, 75],
- [8, 83],
- [8, 84],
- [8, 82],
- [8, 103],
- [8, 104],
- [8, 105],
- [8, 108],
- [8, 106],
- [8, 107],
- [8, 96],
- [8, 94],
- [8, 95],
- [8, 115],
- [19, 75],
- [19, 83],
- [19, 84],
- [19, 82],
- [19, 115],
- [36, 75],
- [36, 103],
- [36, 104],
- [36, 105],
- [36, 115],
- [42, 75],
- [42, 108],
- [42, 106],
- [42, 107],
- [42, 115],
- [9, 20],
- [9, 28],
- [9, 34],
- [9, 43],
- [9, 72],
- [9, 73],
- [9, 74],
- [9, 70],
- [9, 71],
- [9, 75],
- [9, 87],
- [9, 85],
- [9, 86],
- [9, 96],
- [9, 94],
- [9, 95],
- [9, 98],
- [9, 99],
- [9, 97],
- [9, 111],
- [9, 109],
- [9, 110],
- [9, 115],
- [20, 75],
- [20, 87],
- [20, 85],
- [20, 86],
- [20, 115],
- [28, 75],
- [28, 96],
- [28, 94],
- [28, 95],
- [28, 115],
- [34, 75],
- [34, 98],
- [34, 99],
- [34, 97],
- [34, 115],
- [43, 75],
- [43, 111],
- [43, 109],
- [43, 110],
- [43, 115],
- [75, 115],
- [10, 21],
- [10, 29],
- [10, 37],
- [10, 45],
- [10, 50],
- [10, 55],
- [10, 65],
- [10, 70],
- [10, 60],
- [10, 76],
- [10, 79],
- [10, 85],
- [10, 82],
- [10, 88],
- [10, 94],
- [10, 91],
- [10, 100],
- [10, 103],
- [10, 97],
- [10, 106],
- [10, 109],
- [10, 112],
- [10, 115],
- [21, 76],
- [21, 79],
- [21, 85],
- [21, 82],
- [21, 115],
- [29, 76],
- [29, 88],
- [29, 94],
- [29, 91],
- [29, 115],
- [37, 76],
- [37, 100],
- [37, 103],
- [37, 97],
- [37, 115],
- [45, 76],
- [45, 106],
- [45, 109],
- [45, 112],
- [45, 115],
- [76, 115],
- [11, 22],
- [11, 50],
- [11, 56],
- [11, 61],
- [11, 66],
- [11, 30],
- [11, 46],
- [11, 38],
- [11, 71],
- [11, 79],
- [11, 83],
- [11, 77],
- [11, 86],
- [11, 88],
- [11, 106],
- [11, 97],
- [11, 101],
- [11, 110],
- [11, 92],
- [11, 113],
- [11, 104],
- [11, 95],
- [11, 115],
- [22, 79],
- [22, 83],
- [22, 77],
- [22, 86],
- [22, 115],
- [50, 79],
- [50, 88],
- [50, 106],
- [50, 97],
- [50, 115],
- [79, 115],
- [56, 83],
- [56, 88],
- [56, 101],
- [56, 110],
- [56, 115],
- [61, 83],
- [61, 92],
- [61, 113],
- [61, 97],
- [61, 115],
- [66, 83],
- [66, 106],
- [66, 104],
- [66, 95],
- [66, 115],
- [83, 115],
- [12, 30],
- [12, 39],
- [12, 51],
- [12, 55],
- [12, 62],
- [12, 72],
- [12, 23],
- [12, 47],
- [12, 67],
- [12, 88],
- [12, 92],
- [12, 77],
- [12, 95],
- [12, 100],
- [12, 98],
- [12, 105],
- [12, 80],
- [12, 107],
- [12, 109],
- [12, 82],
- [12, 114],
- [12, 87],
- [12, 115],
- [30, 88],
- [30, 92],
- [30, 77],
- [30, 95],
- [30, 115],
- [39, 100],
- [39, 98],
- [39, 77],
- [39, 105],
- [39, 115],
- [51, 88],
- [51, 98],
- [51, 80],
- [51, 107],
- [51, 115],
- [55, 88],
- [55, 100],
- [55, 109],
- [55, 82],
- [55, 115],
- [88, 115],
- [100, 115],
- [62, 92],
- [62, 98],
- [62, 114],
- [62, 82],
- [62, 115],
- [92, 115],
- [72, 98],
- [72, 87],
- [72, 109],
- [72, 95],
- [72, 115],
- [98, 115],
- [13, 31],
- [13, 48],
- [13, 52],
- [13, 57],
- [13, 68],
- [13, 73],
- [13, 23],
- [13, 38],
- [13, 60],
- [13, 89],
- [13, 96],
- [13, 77],
- [13, 91],
- [13, 108],
- [13, 111],
- [13, 112],
- [13, 80],
- [13, 97],
- [13, 101],
- [13, 82],
- [13, 104],
- [13, 87],
- [13, 115],
- [31, 89],
- [31, 96],
- [31, 77],
- [31, 91],
- [31, 115],
- [48, 108],
- [48, 111],
- [48, 77],
- [48, 112],
- [48, 115],
- [52, 89],
- [52, 108],
- [52, 80],
- [52, 97],
- [52, 115],
- [57, 89],
- [57, 111],
- [57, 101],
- [57, 82],
- [57, 115],
- [89, 115],
- [68, 108],
- [68, 96],
- [68, 104],
- [68, 82],
- [68, 115],
- [108, 115],
- [73, 96],
- [73, 111],
- [73, 87],
- [73, 97],
- [73, 115],
- [96, 115],
- [111, 115],
- [14, 23],
- [14, 40],
- [14, 46],
- [14, 53],
- [14, 63],
- [14, 65],
- [14, 74],
- [14, 32],
- [14, 58],
- [14, 80],
- [14, 87],
- [14, 77],
- [14, 82],
- [14, 103],
- [14, 99],
- [14, 102],
- [14, 113],
- [14, 106],
- [14, 110],
- [14, 90],
- [14, 93],
- [14, 94],
- [14, 115],
- [23, 80],
- [23, 87],
- [23, 77],
- [23, 82],
- [23, 115],
- [40, 103],
- [40, 99],
- [40, 77],
- [40, 102],
- [40, 115],
- [46, 113],
- [46, 106],
- [46, 77],
- [46, 110],
- [46, 115],
- [53, 80],
- [53, 106],
- [53, 99],
- [53, 90],
- [53, 115],
- [80, 115],
- [63, 113],
- [63, 99],
- [63, 93],
- [63, 82],
- [63, 115],
- [113, 115],
- [65, 103],
- [65, 106],
- [65, 94],
- [65, 82],
- [65, 115],
- [103, 115],
- [106, 115],
- [74, 87],
- [74, 99],
- [74, 94],
- [74, 110],
- [74, 115],
- [87, 115],
- [99, 115],
- [15, 24],
- [15, 32],
- [15, 38],
- [15, 47],
- [15, 59],
- [15, 64],
- [15, 69],
- [15, 70],
- [15, 54],
- [15, 77],
- [15, 84],
- [15, 85],
- [15, 81],
- [15, 93],
- [15, 94],
- [15, 90],
- [15, 101],
- [15, 104],
- [15, 97],
- [15, 114],
- [15, 109],
- [15, 107],
- [15, 115],
- [24, 77],
- [24, 84],
- [24, 85],
- [24, 81],
- [24, 115],
- [32, 77],
- [32, 93],
- [32, 94],
- [32, 90],
- [32, 115],
- [38, 77],
- [38, 101],
- [38, 104],
- [38, 97],
- [38, 115],
- [47, 77],
- [47, 114],
- [47, 109],
- [47, 107],
- [47, 115],
- [77, 115],
- [59, 101],
- [59, 84],
- [59, 109],
- [59, 90],
- [59, 115],
- [101, 115],
- [64, 93],
- [64, 114],
- [64, 84],
- [64, 97],
- [64, 115],
- [93, 115],
- [114, 115],
- [69, 84],
- [69, 104],
- [69, 94],
- [69, 107],
- [69, 115],
- [84, 115],
- [104, 115],
- [70, 85],
- [70, 94],
- [70, 109],
- [70, 97],
- [70, 115],
- [85, 115],
- [94, 115],
- [109, 115],
- [16, 25],
- [16, 33],
- [16, 41],
- [16, 49],
- [16, 54],
- [16, 58],
- [16, 60],
- [16, 67],
- [16, 71],
- [16, 78],
- [16, 81],
- [16, 82],
- [16, 86],
- [16, 90],
- [16, 91],
- [16, 95],
- [16, 102],
- [16, 105],
- [16, 97],
- [16, 112],
- [16, 107],
- [16, 110],
- [16, 115],
- [25, 78],
- [25, 81],
- [25, 82],
- [25, 86],
- [25, 115],
- [33, 78],
- [33, 90],
- [33, 91],
- [33, 95],
- [33, 115],
- [41, 78],
- [41, 102],
- [41, 105],
- [41, 97],
- [41, 115],
- [49, 78],
- [49, 112],
- [49, 107],
- [49, 110],
- [49, 115],
- [78, 115],
- [54, 81],
- [54, 90],
- [54, 107],
- [54, 97],
- [54, 115],
- [81, 115],
- [58, 90],
- [58, 102],
- [58, 82],
- [58, 110],
- [58, 115],
- [90, 115],
- [102, 115],
- [60, 91],
- [60, 112],
- [60, 82],
- [60, 97],
- [60, 115],
- [91, 115],
- [112, 115],
- [67, 82],
- [67, 105],
- [67, 107],
- [67, 95],
- [67, 115],
- [82, 115],
- [105, 115],
- [107, 115],
- [71, 86],
- [71, 95],
- [71, 97],
- [71, 110],
- [71, 115],
- [86, 115],
- [95, 115],
- [97, 115],
- [110, 115]]
-
-D4_rels = [[0, 1],
- [0, 2],
- [0, 3],
- [0, 4],
- [0, 5],
- [0, 6],
- [0, 7],
- [0, 8],
- [0, 9],
- [0, 10],
- [0, 11],
- [0, 12],
- [0, 13],
- [0, 14],
- [0, 15],
- [0, 16],
- [0, 17],
- [0, 18],
- [0, 19],
- [0, 20],
- [0, 21],
- [0, 22],
- [0, 23],
- [0, 24],
- [0, 25],
- [0, 26],
- [0, 27],
- [0, 28],
- [0, 29],
- [0, 30],
- [0, 31],
- [0, 33],
- [0, 32],
- [0, 35],
- [0, 34],
- [0, 37],
- [0, 36],
- [0, 39],
- [0, 38],
- [0, 42],
- [0, 43],
- [0, 40],
- [0, 41],
- [0, 44],
- [0, 45],
- [0, 46],
- [0, 47],
- [0, 48],
- [0, 49],
- [0, 50],
- [0, 51],
- [0, 52],
- [0, 53],
- [0, 54],
- [0, 55],
- [0, 56],
- [0, 57],
- [0, 58],
- [0, 59],
- [0, 60],
- [0, 62],
- [0, 63],
- [0, 61],
- [0, 64],
- [0, 66],
- [0, 67],
- [0, 65],
- [0, 68],
- [0, 69],
- [0, 70],
- [0, 71],
- [1, 13],
- [1, 14],
- [1, 15],
- [1, 16],
- [1, 17],
- [1, 18],
- [1, 19],
- [1, 47],
- [1, 48],
- [1, 49],
- [1, 50],
- [1, 51],
- [1, 52],
- [1, 53],
- [1, 54],
- [1, 55],
- [1, 71],
- [2, 13],
- [2, 20],
- [2, 21],
- [2, 22],
- [2, 23],
- [2, 24],
- [2, 25],
- [2, 47],
- [2, 48],
- [2, 49],
- [2, 50],
- [2, 56],
- [2, 57],
- [2, 58],
- [2, 59],
- [2, 60],
- [2, 71],
- [13, 47],
- [13, 48],
- [13, 49],
- [13, 50],
- [13, 71],
- [3, 14],
- [3, 20],
- [3, 26],
- [3, 27],
- [3, 28],
- [3, 29],
- [3, 30],
- [3, 47],
- [3, 51],
- [3, 52],
- [3, 56],
- [3, 57],
- [3, 62],
- [3, 63],
- [3, 61],
- [3, 64],
- [3, 71],
- [4, 14],
- [4, 31],
- [4, 21],
- [4, 33],
- [4, 32],
- [4, 35],
- [4, 34],
- [4, 47],
- [4, 51],
- [4, 52],
- [4, 66],
- [4, 67],
- [4, 65],
- [4, 58],
- [4, 59],
- [4, 68],
- [4, 71],
- [14, 47],
- [14, 51],
- [14, 52],
- [14, 71],
- [5, 20],
- [5, 31],
- [5, 15],
- [5, 37],
- [5, 36],
- [5, 39],
- [5, 38],
- [5, 47],
- [5, 56],
- [5, 57],
- [5, 66],
- [5, 67],
- [5, 65],
- [5, 53],
- [5, 54],
- [5, 69],
- [5, 71],
- [20, 47],
- [20, 56],
- [20, 57],
- [20, 71],
- [31, 47],
- [31, 66],
- [31, 67],
- [31, 65],
- [31, 71],
- [6, 15],
- [6, 21],
- [6, 26],
- [6, 42],
- [6, 43],
- [6, 40],
- [6, 41],
- [6, 47],
- [6, 53],
- [6, 54],
- [6, 58],
- [6, 59],
- [6, 62],
- [6, 63],
- [6, 61],
- [6, 70],
- [6, 71],
- [15, 47],
- [15, 53],
- [15, 54],
- [15, 71],
- [21, 47],
- [21, 58],
- [21, 59],
- [21, 71],
- [26, 47],
- [26, 62],
- [26, 63],
- [26, 61],
- [26, 71],
- [47, 71],
- [7, 16],
- [7, 22],
- [7, 27],
- [7, 32],
- [7, 36],
- [7, 40],
- [7, 44],
- [7, 48],
- [7, 51],
- [7, 53],
- [7, 55],
- [7, 56],
- [7, 58],
- [7, 60],
- [7, 61],
- [7, 65],
- [7, 71],
- [16, 48],
- [16, 51],
- [16, 53],
- [16, 55],
- [16, 71],
- [22, 48],
- [22, 56],
- [22, 58],
- [22, 60],
- [22, 71],
- [48, 71],
- [8, 27],
- [8, 33],
- [8, 37],
- [8, 17],
- [8, 23],
- [8, 45],
- [8, 41],
- [8, 51],
- [8, 56],
- [8, 61],
- [8, 66],
- [8, 68],
- [8, 59],
- [8, 69],
- [8, 54],
- [8, 49],
- [8, 71],
- [27, 51],
- [27, 56],
- [27, 61],
- [27, 71],
- [33, 66],
- [33, 51],
- [33, 68],
- [33, 59],
- [33, 71],
- [37, 66],
- [37, 56],
- [37, 69],
- [37, 54],
- [37, 71],
- [66, 71],
- [9, 17],
- [9, 28],
- [9, 32],
- [9, 42],
- [9, 46],
- [9, 24],
- [9, 38],
- [9, 51],
- [9, 49],
- [9, 54],
- [9, 62],
- [9, 64],
- [9, 57],
- [9, 58],
- [9, 65],
- [9, 70],
- [9, 71],
- [17, 51],
- [17, 49],
- [17, 54],
- [17, 71],
- [28, 51],
- [28, 62],
- [28, 64],
- [28, 57],
- [28, 71],
- [32, 51],
- [32, 58],
- [32, 65],
- [32, 71],
- [51, 71],
- [42, 62],
- [42, 70],
- [42, 58],
- [42, 54],
- [42, 71],
- [62, 71],
- [10, 23],
- [10, 29],
- [10, 36],
- [10, 43],
- [10, 46],
- [10, 18],
- [10, 34],
- [10, 56],
- [10, 49],
- [10, 59],
- [10, 63],
- [10, 64],
- [10, 52],
- [10, 53],
- [10, 65],
- [10, 70],
- [10, 71],
- [23, 56],
- [23, 49],
- [23, 59],
- [23, 71],
- [29, 56],
- [29, 63],
- [29, 64],
- [29, 52],
- [29, 71],
- [36, 56],
- [36, 53],
- [36, 65],
- [36, 71],
- [56, 71],
- [43, 63],
- [43, 70],
- [43, 53],
- [43, 59],
- [43, 71],
- [63, 71],
- [46, 64],
- [46, 70],
- [46, 49],
- [46, 65],
- [46, 71],
- [64, 71],
- [70, 71],
- [11, 18],
- [11, 24],
- [11, 35],
- [11, 39],
- [11, 40],
- [11, 45],
- [11, 30],
- [11, 53],
- [11, 49],
- [11, 52],
- [11, 58],
- [11, 57],
- [11, 67],
- [11, 68],
- [11, 69],
- [11, 61],
- [11, 71],
- [18, 53],
- [18, 49],
- [18, 52],
- [18, 71],
- [24, 58],
- [24, 49],
- [24, 57],
- [24, 71],
- [35, 67],
- [35, 58],
- [35, 68],
- [35, 52],
- [35, 71],
- [39, 67],
- [39, 53],
- [39, 69],
- [39, 57],
- [39, 71],
- [67, 71],
- [40, 53],
- [40, 58],
- [40, 61],
- [40, 71],
- [53, 71],
- [58, 71],
- [45, 49],
- [45, 68],
- [45, 69],
- [45, 61],
- [45, 71],
- [49, 71],
- [68, 71],
- [69, 71],
- [12, 19],
- [12, 25],
- [12, 30],
- [12, 34],
- [12, 38],
- [12, 41],
- [12, 44],
- [12, 50],
- [12, 52],
- [12, 54],
- [12, 55],
- [12, 57],
- [12, 59],
- [12, 60],
- [12, 61],
- [12, 65],
- [12, 71],
- [19, 50],
- [19, 52],
- [19, 54],
- [19, 55],
- [19, 71],
- [25, 50],
- [25, 57],
- [25, 59],
- [25, 60],
- [25, 71],
- [50, 71],
- [30, 52],
- [30, 57],
- [30, 61],
- [30, 71],
- [34, 52],
- [34, 59],
- [34, 65],
- [34, 71],
- [52, 71],
- [38, 57],
- [38, 54],
- [38, 65],
- [38, 71],
- [57, 71],
- [41, 54],
- [41, 59],
- [41, 61],
- [41, 71],
- [54, 71],
- [59, 71],
- [44, 55],
- [44, 60],
- [44, 61],
- [44, 65],
- [44, 71],
- [55, 71],
- [60, 71],
- [61, 71],
- [65, 71]]
-
-A4_Igusa_n = lambda q, t: -q**11 - 2*q**10*(4*t - 5) + t**11 - (9*t**3 + 6*t**2 - 50*t + 35)*q**9 - (4*t**6 + 12*t**4 - 50*t**3 - 15*t**2 + 100*t - 50)*q**8 - (12*t**7 - 25*t**6 - 6*t**5 - 30*t**4 + 95*t**3 - 70*t + 24)*q**7 - (6*t**9 - 16*t**8 - 30*t**7 + 50*t**6 + 35*t**5 - 70*t**3 + 15*t**2 + 12*t)*q**6 + (12*t**10 + 15*t**9 - 70*t**8 + 35*t**6 + 50*t**5 - 30*t**4 - 16*t**3 + 6*t**2)*q**5 + (24*t**11 - 70*t**10 + 95*t**8 - 30*t**7 - 6*t**6 - 25*t**5 + 12*t**4)*q**4 - (50*t**11 - 100*t**10 + 15*t**9 + 50*t**8 - 12*t**7 - 4*t**5)*q**3 + (35*t**11 - 50*t**10 + 6*t**9 + 9*t**8)*q**2 - 2*(5*t**11 - 4*t**10)*q
-
-A4_Igusa_d = lambda q, t: (t**10 - q**4)*(t**6 - q**3)*(t**3 - q**2)*(q - t)**2
-
-A5_Igusa_n = lambda q, t: 90*q**7*t**23 - 120*q**5*t**25 - 60*q**9*t**20 + 120*q**8*t**21 - 64*q**7*t**22 - 363*q**6*t**23 + 288*q**5*t**24 + 274*q**4*t**25 + 10*q**12*t**16 - 120*q**10*t**18 + 128*q**9*t**19 + 66*q**8*t**20 - 636*q**7*t**21 + 492*q**6*t**22 + 345*q**5*t**23 - 600*q**4*t**24 - 225*q**3*t**25 - 99*q**11*t**16 + 147*q**10*t**17 + 498*q**9*t**18 - 546*q**8*t**19 + 450*q**7*t**20 + 720*q**6*t**21 - 850*q**5*t**22 - 15*q**4*t**23 + 420*q**3*t**24 + 85*q**2*t**25 + 30*q**13*t**13 - 60*q**12*t**14 - 60*q**11*t**15 + 449*q**10*t**16 - 717*q**9*t**17 - 633*q**8*t**18 + 871*q**7*t**19 - 750*q**6*t**20 - 120*q**5*t**21 + 570*q**4*t**22 - 75*q**3*t**23 - 120*q**2*t**24 - 15*q*t**25 + 5*q**15*t**10 + 30*q**14*t**11 - 30*q**13*t**12 - 158*q**12*t**13 + 504*q**11*t**14 - 54*q**10*t**15 - 987*q**9*t**16 + 1275*q**8*t**17 + 105*q**7*t**18 - 765*q**6*t**19 + 330*q**5*t**20 - 120*q**4*t**21 - 166*q**3*t**22 + 18*q**2*t**23 + 12*q*t**24 + t**25 - 51*q**14*t**10 - 162*q**13*t**11 + 261*q**12*t**12 + 174*q**11*t**13 - 1128*q**10*t**14 + 846*q**9*t**15 + 965*q**8*t**16 - 1035*q**7*t**17 + 345*q**6*t**18 + 427*q**5*t**19 - 36*q**4*t**20 + 36*q**3*t**21 + 18*q**2*t**22 + 12*q**14*t**9 + 89*q**13*t**10 + 186*q**12*t**11 - 557*q**11*t**12 + 25*q**10*t**13 + 720*q**9*t**14 - 1120*q**8*t**15 - 366*q**7*t**16 + 378*q**6*t**17 - 243*q**5*t**18 - 129*q**4*t**19 + 14*q**16*t**6 + 48*q**15*t**7 - 48*q**14*t**8 + 16*q**13*t**9 + 345*q**12*t**10 - 90*q**11*t**11 + 255*q**10*t**12 + 255*q**9*t**13 - 90*q**8*t**14 + 345*q**7*t**15 + 16*q**6*t**16 - 48*q**5*t**17 + 48*q**4*t**18 + 14*q**3*t**19 - 129*q**15*t**6 - 243*q**14*t**7 + 378*q**13*t**8 - 366*q**12*t**9 - 1120*q**11*t**10 + 720*q**10*t**11 + 25*q**9*t**12 - 557*q**8*t**13 + 186*q**7*t**14 + 89*q**6*t**15 + 12*q**5*t**16 + 18*q**17*t**3 + 36*q**16*t**4 - 36*q**15*t**5 + 427*q**14*t**6 + 345*q**13*t**7 - 1035*q**12*t**8 + 965*q**11*t**9 + 846*q**10*t**10 - 1128*q**9*t**11 + 174*q**8*t**12 + 261*q**7*t**13 - 162*q**6*t**14 - 51*q**5*t**15 + q**19 + 12*q**18*t + 18*q**17*t**2 - 166*q**16*t**3 - 120*q**15*t**4 + 330*q**14*t**5 - 765*q**13*t**6 + 105*q**12*t**7 + 1275*q**11*t**8 - 987*q**10*t**9 - 54*q**9*t**10 + 504*q**8*t**11 - 158*q**7*t**12 - 30*q**6*t**13 + 30*q**5*t**14 + 5*q**4*t**15 - 15*q**18 - 120*q**17*t - 75*q**16*t**2 + 570*q**15*t**3 - 120*q**14*t**4 - 750*q**13*t**5 + 871*q**12*t**6 - 633*q**11*t**7 - 717*q**10*t**8 + 449*q**9*t**9 - 60*q**8*t**10 - 60*q**7*t**11 + 30*q**6*t**12 + 85*q**17 + 420*q**16*t - 15*q**15*t**2 - 850*q**14*t**3 + 720*q**13*t**4 + 450*q**12*t**5 - 546*q**11*t**6 + 498*q**10*t**7 + 147*q**9*t**8 - 99*q**8*t**9 - 225*q**16 - 600*q**15*t + 345*q**14*t**2 + 492*q**13*t**3 - 636*q**12*t**4 + 66*q**11*t**5 + 128*q**10*t**6 - 120*q**9*t**7 + 10*q**7*t**9 + 274*q**15 + 288*q**14*t - 363*q**13*t**2 - 64*q**12*t**3 + 120*q**11*t**4 - 60*q**10*t**5 - 120*q**14 + 90*q**12*t**2
-
-A5_Igusa_d = lambda q, t: -(t**15 - q**5)*(t**10 - q**4)*(t**6 - q**3)*(t**3 - q**2)**2*(q - t)**3
-
-B3_Igusa_n = lambda q, t: 6*q**5*t**7 + 3*q**4*t**8 - 15*q**3*t**9 - 2*q**7*t**4 + q**6*t**5 + 7*q**5*t**6 - 22*q**4*t**7 + 17*q**3*t**8 + 23*q**2*t**9 - 3*q**7*t**3 + 9*q**6*t**4 - 15*q**5*t**5 - 3*q**4*t**6 + 18*q**3*t**7 - 27*q**2*t**8 - 9*q*t**9 - q**9 - 7*q**8*t + 2*q**7*t**2 + 7*q**6*t**3 - 21*q**5*t**4 + 21*q**4*t**5 - 7*q**3*t**6 - 2*q**2*t**7 + 7*q*t**8 + t**9 + 9*q**8 + 27*q**7*t - 18*q**6*t**2 + 3*q**5*t**3 + 15*q**4*t**4 - 9*q**3*t**5 + 3*q**2*t**6 - 23*q**7 - 17*q**6*t + 22*q**5*t**2 - 7*q**4*t**3 - q**3*t**4 + 2*q**2*t**5 + 15*q**6 - 3*q**5*t - 6*q**4*t**2
-
-B3_Igusa_d = lambda q, t: (t**9 - q**3)*(t**4 - q**2)*(t**3 - q**2)*(q - t)**2
-
+A3_rels = [[0, 1],
+ [0, 2],
+ [0, 3],
+ [0, 4],
+ [0, 5],
+ [0, 6],
+ [0, 7],
+ [0, 8],
+ [0, 9],
+ [0, 10],
+ [0, 11],
+ [0, 13],
+ [0, 12],
+ [0, 14],
+ [1, 7],
+ [1, 8],
+ [1, 9],
+ [1, 14],
+ [2, 7],
+ [2, 10],
+ [2, 11],
+ [2, 14],
+ [3, 7],
+ [3, 13],
+ [3, 12],
+ [3, 14],
+ [7, 14],
+ [4, 8],
+ [4, 10],
+ [4, 12],
+ [4, 14],
+ [8, 14],
+ [5, 10],
+ [5, 13],
+ [5, 9],
+ [5, 14],
+ [10, 14],
+ [13, 14],
+ [6, 9],
+ [6, 11],
+ [6, 12],
+ [6, 14],
+ [9, 14],
+ [11, 14],
+ [12, 14]]
+
+A4_rels = [[0, 1],
+ [0, 2],
+ [0, 3],
+ [0, 4],
+ [0, 5],
+ [0, 6],
+ [0, 7],
+ [0, 8],
+ [0, 9],
+ [0, 10],
+ [0, 11],
+ [0, 12],
+ [0, 13],
+ [0, 14],
+ [0, 15],
+ [0, 16],
+ [0, 17],
+ [0, 18],
+ [0, 19],
+ [0, 20],
+ [0, 21],
+ [0, 23],
+ [0, 22],
+ [0, 24],
+ [0, 26],
+ [0, 25],
+ [0, 27],
+ [0, 28],
+ [0, 29],
+ [0, 31],
+ [0, 30],
+ [0, 32],
+ [0, 34],
+ [0, 35],
+ [0, 33],
+ [0, 36],
+ [0, 37],
+ [0, 38],
+ [0, 39],
+ [0, 40],
+ [0, 42],
+ [0, 41],
+ [0, 43],
+ [0, 44],
+ [0, 46],
+ [0, 45],
+ [0, 49],
+ [0, 50],
+ [0, 48],
+ [0, 47],
+ [0, 51],
+ [1, 11],
+ [1, 12],
+ [1, 13],
+ [1, 14],
+ [1, 15],
+ [1, 16],
+ [1, 36],
+ [1, 37],
+ [1, 38],
+ [1, 39],
+ [1, 40],
+ [1, 42],
+ [1, 41],
+ [1, 51],
+ [2, 11],
+ [2, 17],
+ [2, 18],
+ [2, 19],
+ [2, 20],
+ [2, 21],
+ [2, 36],
+ [2, 37],
+ [2, 38],
+ [2, 43],
+ [2, 44],
+ [2, 46],
+ [2, 45],
+ [2, 51],
+ [3, 11],
+ [3, 23],
+ [3, 22],
+ [3, 24],
+ [3, 26],
+ [3, 25],
+ [3, 36],
+ [3, 37],
+ [3, 38],
+ [3, 49],
+ [3, 50],
+ [3, 48],
+ [3, 47],
+ [3, 51],
+ [11, 36],
+ [11, 37],
+ [11, 38],
+ [11, 51],
+ [4, 12],
+ [4, 17],
+ [4, 22],
+ [4, 27],
+ [4, 28],
+ [4, 29],
+ [4, 36],
+ [4, 39],
+ [4, 40],
+ [4, 43],
+ [4, 44],
+ [4, 48],
+ [4, 47],
+ [4, 51],
+ [12, 36],
+ [12, 39],
+ [12, 40],
+ [12, 51],
+ [5, 17],
+ [5, 23],
+ [5, 13],
+ [5, 31],
+ [5, 30],
+ [5, 32],
+ [5, 36],
+ [5, 43],
+ [5, 44],
+ [5, 49],
+ [5, 50],
+ [5, 42],
+ [5, 41],
+ [5, 51],
+ [17, 36],
+ [17, 43],
+ [17, 44],
+ [17, 51],
+ [23, 36],
+ [23, 49],
+ [23, 50],
+ [23, 51],
+ [6, 13],
+ [6, 18],
+ [6, 22],
+ [6, 34],
+ [6, 35],
+ [6, 33],
+ [6, 36],
+ [6, 42],
+ [6, 41],
+ [6, 46],
+ [6, 45],
+ [6, 48],
+ [6, 47],
+ [6, 51],
+ [13, 36],
+ [13, 42],
+ [13, 41],
+ [13, 51],
+ [18, 36],
+ [18, 46],
+ [18, 45],
+ [18, 51],
+ [22, 36],
+ [22, 48],
+ [22, 47],
+ [22, 51],
+ [36, 51],
+ [7, 14],
+ [7, 19],
+ [7, 24],
+ [7, 27],
+ [7, 30],
+ [7, 33],
+ [7, 37],
+ [7, 39],
+ [7, 41],
+ [7, 43],
+ [7, 45],
+ [7, 49],
+ [7, 47],
+ [7, 51],
+ [14, 37],
+ [14, 39],
+ [14, 41],
+ [14, 51],
+ [19, 37],
+ [19, 43],
+ [19, 45],
+ [19, 51],
+ [24, 37],
+ [24, 49],
+ [24, 47],
+ [24, 51],
+ [37, 51],
+ [8, 15],
+ [8, 27],
+ [8, 31],
+ [8, 34],
+ [8, 20],
+ [8, 25],
+ [8, 39],
+ [8, 42],
+ [8, 38],
+ [8, 43],
+ [8, 47],
+ [8, 50],
+ [8, 46],
+ [8, 51],
+ [15, 39],
+ [15, 42],
+ [15, 38],
+ [15, 51],
+ [27, 39],
+ [27, 43],
+ [27, 47],
+ [27, 51],
+ [39, 51],
+ [31, 42],
+ [31, 43],
+ [31, 50],
+ [31, 51],
+ [34, 42],
+ [34, 46],
+ [34, 47],
+ [34, 51],
+ [42, 51],
+ [9, 20],
+ [9, 26],
+ [9, 28],
+ [9, 30],
+ [9, 35],
+ [9, 16],
+ [9, 43],
+ [9, 46],
+ [9, 38],
+ [9, 49],
+ [9, 48],
+ [9, 40],
+ [9, 41],
+ [9, 51],
+ [20, 43],
+ [20, 46],
+ [20, 38],
+ [20, 51],
+ [26, 49],
+ [26, 48],
+ [26, 38],
+ [26, 51],
+ [28, 43],
+ [28, 48],
+ [28, 40],
+ [28, 51],
+ [30, 43],
+ [30, 49],
+ [30, 41],
+ [30, 51],
+ [43, 51],
+ [49, 51],
+ [35, 46],
+ [35, 48],
+ [35, 41],
+ [35, 51],
+ [46, 51],
+ [48, 51],
+ [10, 16],
+ [10, 21],
+ [10, 25],
+ [10, 29],
+ [10, 32],
+ [10, 33],
+ [10, 38],
+ [10, 40],
+ [10, 41],
+ [10, 44],
+ [10, 45],
+ [10, 50],
+ [10, 47],
+ [10, 51],
+ [16, 38],
+ [16, 40],
+ [16, 41],
+ [16, 51],
+ [21, 38],
+ [21, 44],
+ [21, 45],
+ [21, 51],
+ [25, 38],
+ [25, 50],
+ [25, 47],
+ [25, 51],
+ [38, 51],
+ [29, 40],
+ [29, 44],
+ [29, 47],
+ [29, 51],
+ [40, 51],
+ [32, 44],
+ [32, 50],
+ [32, 41],
+ [32, 51],
+ [44, 51],
+ [50, 51],
+ [33, 41],
+ [33, 45],
+ [33, 47],
+ [33, 51],
+ [41, 51],
+ [45, 51],
+ [47, 51]]
+
+A5_rels = [[0, 1],
+ [0, 2],
+ [0, 3],
+ [0, 4],
+ [0, 5],
+ [0, 6],
+ [0, 7],
+ [0, 8],
+ [0, 9],
+ [0, 10],
+ [0, 11],
+ [0, 12],
+ [0, 13],
+ [0, 14],
+ [0, 15],
+ [0, 16],
+ [0, 17],
+ [0, 18],
+ [0, 19],
+ [0, 20],
+ [0, 21],
+ [0, 22],
+ [0, 23],
+ [0, 24],
+ [0, 25],
+ [0, 26],
+ [0, 27],
+ [0, 28],
+ [0, 29],
+ [0, 30],
+ [0, 31],
+ [0, 32],
+ [0, 33],
+ [0, 34],
+ [0, 36],
+ [0, 35],
+ [0, 37],
+ [0, 39],
+ [0, 38],
+ [0, 40],
+ [0, 41],
+ [0, 43],
+ [0, 42],
+ [0, 44],
+ [0, 45],
+ [0, 46],
+ [0, 47],
+ [0, 48],
+ [0, 49],
+ [0, 50],
+ [0, 52],
+ [0, 51],
+ [0, 53],
+ [0, 54],
+ [0, 56],
+ [0, 55],
+ [0, 57],
+ [0, 59],
+ [0, 60],
+ [0, 58],
+ [0, 61],
+ [0, 63],
+ [0, 64],
+ [0, 62],
+ [0, 65],
+ [0, 66],
+ [0, 67],
+ [0, 68],
+ [0, 70],
+ [0, 69],
+ [0, 71],
+ [0, 72],
+ [0, 74],
+ [0, 75],
+ [0, 73],
+ [0, 76],
+ [0, 78],
+ [0, 79],
+ [0, 80],
+ [0, 77],
+ [0, 81],
+ [0, 82],
+ [0, 83],
+ [0, 84],
+ [0, 85],
+ [0, 86],
+ [0, 87],
+ [0, 88],
+ [0, 89],
+ [0, 90],
+ [0, 91],
+ [0, 93],
+ [0, 92],
+ [0, 94],
+ [0, 96],
+ [0, 95],
+ [0, 97],
+ [0, 98],
+ [0, 99],
+ [0, 101],
+ [0, 100],
+ [0, 102],
+ [0, 104],
+ [0, 105],
+ [0, 103],
+ [0, 106],
+ [0, 107],
+ [0, 108],
+ [0, 109],
+ [0, 110],
+ [0, 112],
+ [0, 111],
+ [0, 113],
+ [0, 115],
+ [0, 114],
+ [0, 116],
+ [0, 117],
+ [0, 118],
+ [0, 120],
+ [0, 119],
+ [0, 121],
+ [0, 123],
+ [0, 124],
+ [0, 122],
+ [0, 130],
+ [0, 131],
+ [0, 132],
+ [0, 133],
+ [0, 134],
+ [0, 126],
+ [0, 125],
+ [0, 127],
+ [0, 129],
+ [0, 128],
+ [0, 135],
+ [0, 137],
+ [0, 136],
+ [0, 142],
+ [0, 141],
+ [0, 143],
+ [0, 139],
+ [0, 140],
+ [0, 138],
+ [0, 144],
+ [0, 145],
+ [0, 146],
+ [0, 148],
+ [0, 147],
+ [0, 149],
+ [0, 151],
+ [0, 152],
+ [0, 150],
+ [0, 156],
+ [0, 157],
+ [0, 158],
+ [0, 154],
+ [0, 153],
+ [0, 155],
+ [0, 161],
+ [0, 160],
+ [0, 159],
+ [0, 165],
+ [0, 167],
+ [0, 166],
+ [0, 170],
+ [0, 168],
+ [0, 169],
+ [0, 163],
+ [0, 164],
+ [0, 162],
+ [0, 171],
+ [0, 172],
+ [0, 173],
+ [0, 174],
+ [0, 175],
+ [0, 177],
+ [0, 176],
+ [0, 178],
+ [0, 179],
+ [0, 181],
+ [0, 180],
+ [0, 184],
+ [0, 185],
+ [0, 183],
+ [0, 182],
+ [0, 186],
+ [0, 187],
+ [0, 189],
+ [0, 188],
+ [0, 192],
+ [0, 193],
+ [0, 191],
+ [0, 190],
+ [0, 198],
+ [0, 199],
+ [0, 201],
+ [0, 200],
+ [0, 196],
+ [0, 197],
+ [0, 195],
+ [0, 194],
+ [0, 202],
+ [1, 16],
+ [1, 17],
+ [1, 18],
+ [1, 19],
+ [1, 20],
+ [1, 21],
+ [1, 22],
+ [1, 23],
+ [1, 24],
+ [1, 25],
+ [1, 81],
+ [1, 82],
+ [1, 83],
+ [1, 84],
+ [1, 85],
+ [1, 86],
+ [1, 87],
+ [1, 88],
+ [1, 89],
+ [1, 90],
+ [1, 91],
+ [1, 93],
+ [1, 92],
+ [1, 94],
+ [1, 96],
+ [1, 95],
+ [1, 97],
+ [1, 98],
+ [1, 99],
+ [1, 101],
+ [1, 100],
+ [1, 102],
+ [1, 104],
+ [1, 105],
+ [1, 103],
+ [1, 171],
+ [1, 172],
+ [1, 173],
+ [1, 174],
+ [1, 175],
+ [1, 177],
+ [1, 176],
+ [1, 178],
+ [1, 179],
+ [1, 181],
+ [1, 180],
+ [1, 184],
+ [1, 185],
+ [1, 183],
+ [1, 182],
+ [1, 202],
+ [2, 16],
+ [2, 26],
+ [2, 27],
+ [2, 28],
+ [2, 29],
+ [2, 30],
+ [2, 31],
+ [2, 32],
+ [2, 33],
+ [2, 34],
+ [2, 81],
+ [2, 82],
+ [2, 83],
+ [2, 84],
+ [2, 85],
+ [2, 86],
+ [2, 106],
+ [2, 107],
+ [2, 108],
+ [2, 109],
+ [2, 110],
+ [2, 112],
+ [2, 111],
+ [2, 113],
+ [2, 115],
+ [2, 114],
+ [2, 116],
+ [2, 117],
+ [2, 118],
+ [2, 120],
+ [2, 119],
+ [2, 121],
+ [2, 123],
+ [2, 124],
+ [2, 122],
+ [2, 171],
+ [2, 172],
+ [2, 173],
+ [2, 174],
+ [2, 175],
+ [2, 177],
+ [2, 176],
+ [2, 186],
+ [2, 187],
+ [2, 189],
+ [2, 188],
+ [2, 192],
+ [2, 193],
+ [2, 191],
+ [2, 190],
+ [2, 202],
+ [3, 16],
+ [3, 36],
+ [3, 35],
+ [3, 37],
+ [3, 39],
+ [3, 38],
+ [3, 40],
+ [3, 41],
+ [3, 43],
+ [3, 42],
+ [3, 81],
+ [3, 82],
+ [3, 83],
+ [3, 84],
+ [3, 85],
+ [3, 86],
+ [3, 130],
+ [3, 131],
+ [3, 132],
+ [3, 133],
+ [3, 134],
+ [3, 126],
+ [3, 125],
+ [3, 127],
+ [3, 129],
+ [3, 128],
+ [3, 135],
+ [3, 137],
+ [3, 136],
+ [3, 142],
+ [3, 141],
+ [3, 143],
+ [3, 139],
+ [3, 140],
+ [3, 138],
+ [3, 171],
+ [3, 172],
+ [3, 173],
+ [3, 174],
+ [3, 175],
+ [3, 177],
+ [3, 176],
+ [3, 198],
+ [3, 199],
+ [3, 201],
+ [3, 200],
+ [3, 196],
+ [3, 197],
+ [3, 195],
+ [3, 194],
+ [3, 202],
+ [16, 81],
+ [16, 82],
+ [16, 83],
+ [16, 84],
+ [16, 85],
+ [16, 86],
+ [16, 171],
+ [16, 172],
+ [16, 173],
+ [16, 174],
+ [16, 175],
+ [16, 177],
+ [16, 176],
+ [16, 202],
+ [4, 17],
+ [4, 26],
+ [4, 35],
+ [4, 44],
+ [4, 45],
+ [4, 46],
+ [4, 47],
+ [4, 48],
+ [4, 49],
+ [4, 50],
+ [4, 81],
+ [4, 87],
+ [4, 88],
+ [4, 89],
+ [4, 90],
+ [4, 91],
+ [4, 106],
+ [4, 107],
+ [4, 108],
+ [4, 109],
+ [4, 110],
+ [4, 126],
+ [4, 125],
+ [4, 127],
+ [4, 129],
+ [4, 128],
+ [4, 144],
+ [4, 145],
+ [4, 146],
+ [4, 148],
+ [4, 147],
+ [4, 149],
+ [4, 151],
+ [4, 152],
+ [4, 150],
+ [4, 171],
+ [4, 172],
+ [4, 173],
+ [4, 178],
+ [4, 179],
+ [4, 181],
+ [4, 180],
+ [4, 186],
+ [4, 187],
+ [4, 189],
+ [4, 188],
+ [4, 196],
+ [4, 197],
+ [4, 195],
+ [4, 194],
+ [4, 202],
+ [17, 81],
+ [17, 87],
+ [17, 88],
+ [17, 89],
+ [17, 90],
+ [17, 91],
+ [17, 171],
+ [17, 172],
+ [17, 173],
+ [17, 178],
+ [17, 179],
+ [17, 181],
+ [17, 180],
+ [17, 202],
+ [5, 26],
+ [5, 36],
+ [5, 18],
+ [5, 52],
+ [5, 51],
+ [5, 53],
+ [5, 54],
+ [5, 56],
+ [5, 55],
+ [5, 57],
+ [5, 81],
+ [5, 106],
+ [5, 107],
+ [5, 108],
+ [5, 109],
+ [5, 110],
+ [5, 130],
+ [5, 131],
+ [5, 132],
+ [5, 133],
+ [5, 134],
+ [5, 93],
+ [5, 92],
+ [5, 94],
+ [5, 96],
+ [5, 95],
+ [5, 156],
+ [5, 157],
+ [5, 158],
+ [5, 154],
+ [5, 153],
+ [5, 155],
+ [5, 161],
+ [5, 160],
+ [5, 159],
+ [5, 171],
+ [5, 172],
+ [5, 173],
+ [5, 186],
+ [5, 187],
+ [5, 189],
+ [5, 188],
+ [5, 198],
+ [5, 199],
+ [5, 201],
+ [5, 200],
+ [5, 184],
+ [5, 185],
+ [5, 183],
+ [5, 182],
+ [5, 202],
+ [26, 81],
+ [26, 106],
+ [26, 107],
+ [26, 108],
+ [26, 109],
+ [26, 110],
+ [26, 171],
+ [26, 172],
+ [26, 173],
+ [26, 186],
+ [26, 187],
+ [26, 189],
+ [26, 188],
+ [26, 202],
+ [36, 81],
+ [36, 130],
+ [36, 131],
+ [36, 132],
+ [36, 133],
+ [36, 134],
+ [36, 171],
+ [36, 172],
+ [36, 173],
+ [36, 198],
+ [36, 199],
+ [36, 201],
+ [36, 200],
+ [36, 202],
+ [6, 18],
+ [6, 27],
+ [6, 35],
+ [6, 59],
+ [6, 60],
+ [6, 58],
+ [6, 61],
+ [6, 63],
+ [6, 64],
+ [6, 62],
+ [6, 81],
+ [6, 93],
+ [6, 92],
+ [6, 94],
+ [6, 96],
+ [6, 95],
+ [6, 112],
+ [6, 111],
+ [6, 113],
+ [6, 115],
+ [6, 114],
+ [6, 126],
+ [6, 125],
+ [6, 127],
+ [6, 129],
+ [6, 128],
+ [6, 165],
+ [6, 167],
+ [6, 166],
+ [6, 170],
+ [6, 168],
+ [6, 169],
+ [6, 163],
+ [6, 164],
+ [6, 162],
+ [6, 171],
+ [6, 172],
+ [6, 173],
+ [6, 184],
+ [6, 185],
+ [6, 183],
+ [6, 182],
+ [6, 192],
+ [6, 193],
+ [6, 191],
+ [6, 190],
+ [6, 196],
+ [6, 197],
+ [6, 195],
+ [6, 194],
+ [6, 202],
+ [18, 81],
+ [18, 93],
+ [18, 92],
+ [18, 94],
+ [18, 96],
+ [18, 95],
+ [18, 171],
+ [18, 172],
+ [18, 173],
+ [18, 184],
+ [18, 185],
+ [18, 183],
+ [18, 182],
+ [18, 202],
+ [27, 81],
+ [27, 112],
+ [27, 111],
+ [27, 113],
+ [27, 115],
+ [27, 114],
+ [27, 171],
+ [27, 172],
+ [27, 173],
+ [27, 192],
+ [27, 193],
+ [27, 191],
+ [27, 190],
+ [27, 202],
+ [35, 81],
+ [35, 126],
+ [35, 125],
+ [35, 127],
+ [35, 129],
+ [35, 128],
+ [35, 171],
+ [35, 172],
+ [35, 173],
+ [35, 196],
+ [35, 197],
+ [35, 195],
+ [35, 194],
+ [35, 202],
+ [81, 171],
+ [81, 172],
+ [81, 173],
+ [81, 202],
+ [7, 19],
+ [7, 28],
+ [7, 37],
+ [7, 44],
+ [7, 51],
+ [7, 58],
+ [7, 65],
+ [7, 66],
+ [7, 67],
+ [7, 68],
+ [7, 82],
+ [7, 87],
+ [7, 92],
+ [7, 97],
+ [7, 98],
+ [7, 99],
+ [7, 106],
+ [7, 111],
+ [7, 116],
+ [7, 117],
+ [7, 118],
+ [7, 130],
+ [7, 125],
+ [7, 135],
+ [7, 137],
+ [7, 136],
+ [7, 144],
+ [7, 145],
+ [7, 146],
+ [7, 154],
+ [7, 153],
+ [7, 155],
+ [7, 163],
+ [7, 164],
+ [7, 162],
+ [7, 171],
+ [7, 174],
+ [7, 175],
+ [7, 178],
+ [7, 179],
+ [7, 183],
+ [7, 182],
+ [7, 186],
+ [7, 187],
+ [7, 191],
+ [7, 190],
+ [7, 198],
+ [7, 199],
+ [7, 195],
+ [7, 194],
+ [7, 202],
+ [19, 82],
+ [19, 87],
+ [19, 92],
+ [19, 97],
+ [19, 98],
+ [19, 99],
+ [19, 171],
+ [19, 174],
+ [19, 175],
+ [19, 178],
+ [19, 179],
+ [19, 183],
+ [19, 182],
+ [19, 202],
+ [28, 82],
+ [28, 106],
+ [28, 111],
+ [28, 116],
+ [28, 117],
+ [28, 118],
+ [28, 171],
+ [28, 174],
+ [28, 175],
+ [28, 186],
+ [28, 187],
+ [28, 191],
+ [28, 190],
+ [28, 202],
+ [37, 82],
+ [37, 130],
+ [37, 125],
+ [37, 135],
+ [37, 137],
+ [37, 136],
+ [37, 171],
+ [37, 174],
+ [37, 175],
+ [37, 198],
+ [37, 199],
+ [37, 195],
+ [37, 194],
+ [37, 202],
+ [82, 171],
+ [82, 174],
+ [82, 175],
+ [82, 202],
+ [8, 20],
+ [8, 44],
+ [8, 52],
+ [8, 59],
+ [8, 29],
+ [8, 38],
+ [8, 70],
+ [8, 69],
+ [8, 71],
+ [8, 72],
+ [8, 87],
+ [8, 93],
+ [8, 83],
+ [8, 101],
+ [8, 100],
+ [8, 102],
+ [8, 106],
+ [8, 125],
+ [8, 144],
+ [8, 145],
+ [8, 146],
+ [8, 131],
+ [8, 156],
+ [8, 157],
+ [8, 158],
+ [8, 112],
+ [8, 165],
+ [8, 167],
+ [8, 166],
+ [8, 120],
+ [8, 119],
+ [8, 121],
+ [8, 139],
+ [8, 140],
+ [8, 138],
+ [8, 171],
+ [8, 178],
+ [8, 179],
+ [8, 184],
+ [8, 185],
+ [8, 177],
+ [8, 176],
+ [8, 186],
+ [8, 187],
+ [8, 195],
+ [8, 194],
+ [8, 201],
+ [8, 200],
+ [8, 192],
+ [8, 193],
+ [8, 202],
+ [20, 87],
+ [20, 93],
+ [20, 83],
+ [20, 101],
+ [20, 100],
+ [20, 102],
+ [20, 171],
+ [20, 178],
+ [20, 179],
+ [20, 184],
+ [20, 185],
+ [20, 177],
+ [20, 176],
+ [20, 202],
+ [44, 87],
+ [44, 106],
+ [44, 125],
+ [44, 144],
+ [44, 145],
+ [44, 146],
+ [44, 171],
+ [44, 178],
+ [44, 179],
+ [44, 186],
+ [44, 187],
+ [44, 195],
+ [44, 194],
+ [44, 202],
+ [87, 171],
+ [87, 178],
+ [87, 179],
+ [87, 202],
+ [52, 93],
+ [52, 106],
+ [52, 131],
+ [52, 156],
+ [52, 157],
+ [52, 158],
+ [52, 171],
+ [52, 184],
+ [52, 185],
+ [52, 186],
+ [52, 187],
+ [52, 201],
+ [52, 200],
+ [52, 202],
+ [59, 93],
+ [59, 112],
+ [59, 125],
+ [59, 165],
+ [59, 167],
+ [59, 166],
+ [59, 171],
+ [59, 184],
+ [59, 185],
+ [59, 192],
+ [59, 193],
+ [59, 195],
+ [59, 194],
+ [59, 202],
+ [93, 171],
+ [93, 184],
+ [93, 185],
+ [93, 202],
+ [9, 29],
+ [9, 39],
+ [9, 45],
+ [9, 51],
+ [9, 60],
+ [9, 21],
+ [9, 74],
+ [9, 75],
+ [9, 73],
+ [9, 76],
+ [9, 106],
+ [9, 112],
+ [9, 83],
+ [9, 120],
+ [9, 119],
+ [9, 121],
+ [9, 130],
+ [9, 126],
+ [9, 142],
+ [9, 141],
+ [9, 143],
+ [9, 88],
+ [9, 148],
+ [9, 147],
+ [9, 149],
+ [9, 92],
+ [9, 154],
+ [9, 153],
+ [9, 155],
+ [9, 170],
+ [9, 168],
+ [9, 169],
+ [9, 104],
+ [9, 105],
+ [9, 103],
+ [9, 171],
+ [9, 186],
+ [9, 187],
+ [9, 192],
+ [9, 193],
+ [9, 177],
+ [9, 176],
+ [9, 198],
+ [9, 199],
+ [9, 196],
+ [9, 197],
+ [9, 181],
+ [9, 180],
+ [9, 183],
+ [9, 182],
+ [9, 202],
+ [29, 106],
+ [29, 112],
+ [29, 83],
+ [29, 120],
+ [29, 119],
+ [29, 121],
+ [29, 171],
+ [29, 186],
+ [29, 187],
+ [29, 192],
+ [29, 193],
+ [29, 177],
+ [29, 176],
+ [29, 202],
+ [39, 130],
+ [39, 126],
+ [39, 83],
+ [39, 142],
+ [39, 141],
+ [39, 143],
+ [39, 171],
+ [39, 198],
+ [39, 199],
+ [39, 196],
+ [39, 197],
+ [39, 177],
+ [39, 176],
+ [39, 202],
+ [45, 106],
+ [45, 126],
+ [45, 88],
+ [45, 148],
+ [45, 147],
+ [45, 149],
+ [45, 171],
+ [45, 186],
+ [45, 187],
+ [45, 196],
+ [45, 197],
+ [45, 181],
+ [45, 180],
+ [45, 202],
+ [51, 106],
+ [51, 130],
+ [51, 92],
+ [51, 154],
+ [51, 153],
+ [51, 155],
+ [51, 171],
+ [51, 186],
+ [51, 187],
+ [51, 198],
+ [51, 199],
+ [51, 183],
+ [51, 182],
+ [51, 202],
+ [106, 171],
+ [106, 186],
+ [106, 187],
+ [106, 202],
+ [130, 171],
+ [130, 198],
+ [130, 199],
+ [130, 202],
+ [60, 112],
+ [60, 126],
+ [60, 92],
+ [60, 170],
+ [60, 168],
+ [60, 169],
+ [60, 171],
+ [60, 192],
+ [60, 193],
+ [60, 196],
+ [60, 197],
+ [60, 183],
+ [60, 182],
+ [60, 202],
+ [112, 171],
+ [112, 192],
+ [112, 193],
+ [112, 202],
+ [126, 171],
+ [126, 196],
+ [126, 197],
+ [126, 202],
+ [10, 21],
+ [10, 30],
+ [10, 38],
+ [10, 46],
+ [10, 53],
+ [10, 58],
+ [10, 78],
+ [10, 79],
+ [10, 80],
+ [10, 77],
+ [10, 83],
+ [10, 88],
+ [10, 92],
+ [10, 104],
+ [10, 105],
+ [10, 103],
+ [10, 107],
+ [10, 111],
+ [10, 123],
+ [10, 124],
+ [10, 122],
+ [10, 131],
+ [10, 125],
+ [10, 139],
+ [10, 140],
+ [10, 138],
+ [10, 151],
+ [10, 152],
+ [10, 150],
+ [10, 161],
+ [10, 160],
+ [10, 159],
+ [10, 163],
+ [10, 164],
+ [10, 162],
+ [10, 171],
+ [10, 177],
+ [10, 176],
+ [10, 181],
+ [10, 180],
+ [10, 183],
+ [10, 182],
+ [10, 189],
+ [10, 188],
+ [10, 191],
+ [10, 190],
+ [10, 201],
+ [10, 200],
+ [10, 195],
+ [10, 194],
+ [10, 202],
+ [21, 83],
+ [21, 88],
+ [21, 92],
+ [21, 104],
+ [21, 105],
+ [21, 103],
+ [21, 171],
+ [21, 177],
+ [21, 176],
+ [21, 181],
+ [21, 180],
+ [21, 183],
+ [21, 182],
+ [21, 202],
+ [30, 83],
+ [30, 107],
+ [30, 111],
+ [30, 123],
+ [30, 124],
+ [30, 122],
+ [30, 171],
+ [30, 177],
+ [30, 176],
+ [30, 189],
+ [30, 188],
+ [30, 191],
+ [30, 190],
+ [30, 202],
+ [38, 83],
+ [38, 131],
+ [38, 125],
+ [38, 139],
+ [38, 140],
+ [38, 138],
+ [38, 171],
+ [38, 177],
+ [38, 176],
+ [38, 201],
+ [38, 200],
+ [38, 195],
+ [38, 194],
+ [38, 202],
+ [83, 171],
+ [83, 177],
+ [83, 176],
+ [83, 202],
+ [46, 88],
+ [46, 107],
+ [46, 125],
+ [46, 151],
+ [46, 152],
+ [46, 150],
+ [46, 171],
+ [46, 181],
+ [46, 180],
+ [46, 189],
+ [46, 188],
+ [46, 195],
+ [46, 194],
+ [46, 202],
+ [88, 171],
+ [88, 181],
+ [88, 180],
+ [88, 202],
+ [53, 107],
+ [53, 131],
+ [53, 92],
+ [53, 161],
+ [53, 160],
+ [53, 159],
+ [53, 171],
+ [53, 189],
+ [53, 188],
+ [53, 201],
+ [53, 200],
+ [53, 183],
+ [53, 182],
+ [53, 202],
+ [107, 171],
+ [107, 189],
+ [107, 188],
+ [107, 202],
+ [131, 171],
+ [131, 201],
+ [131, 200],
+ [131, 202],
+ [58, 92],
+ [58, 111],
+ [58, 125],
+ [58, 163],
+ [58, 164],
+ [58, 162],
+ [58, 171],
+ [58, 183],
+ [58, 182],
+ [58, 191],
+ [58, 190],
+ [58, 195],
+ [58, 194],
+ [58, 202],
+ [92, 171],
+ [92, 183],
+ [92, 182],
+ [92, 202],
+ [111, 171],
+ [111, 191],
+ [111, 190],
+ [111, 202],
+ [125, 171],
+ [125, 195],
+ [125, 194],
+ [125, 202],
+ [171, 202],
+ [11, 22],
+ [11, 31],
+ [11, 40],
+ [11, 47],
+ [11, 54],
+ [11, 61],
+ [11, 65],
+ [11, 69],
+ [11, 73],
+ [11, 77],
+ [11, 84],
+ [11, 89],
+ [11, 94],
+ [11, 97],
+ [11, 100],
+ [11, 103],
+ [11, 108],
+ [11, 113],
+ [11, 116],
+ [11, 119],
+ [11, 122],
+ [11, 132],
+ [11, 127],
+ [11, 135],
+ [11, 141],
+ [11, 138],
+ [11, 144],
+ [11, 147],
+ [11, 150],
+ [11, 156],
+ [11, 153],
+ [11, 159],
+ [11, 165],
+ [11, 168],
+ [11, 162],
+ [11, 172],
+ [11, 174],
+ [11, 176],
+ [11, 178],
+ [11, 180],
+ [11, 184],
+ [11, 182],
+ [11, 186],
+ [11, 188],
+ [11, 192],
+ [11, 190],
+ [11, 198],
+ [11, 200],
+ [11, 196],
+ [11, 194],
+ [11, 202],
+ [22, 84],
+ [22, 89],
+ [22, 94],
+ [22, 97],
+ [22, 100],
+ [22, 103],
+ [22, 172],
+ [22, 174],
+ [22, 176],
+ [22, 178],
+ [22, 180],
+ [22, 184],
+ [22, 182],
+ [22, 202],
+ [31, 84],
+ [31, 108],
+ [31, 113],
+ [31, 116],
+ [31, 119],
+ [31, 122],
+ [31, 172],
+ [31, 174],
+ [31, 176],
+ [31, 186],
+ [31, 188],
+ [31, 192],
+ [31, 190],
+ [31, 202],
+ [40, 84],
+ [40, 132],
+ [40, 127],
+ [40, 135],
+ [40, 141],
+ [40, 138],
+ [40, 172],
+ [40, 174],
+ [40, 176],
+ [40, 198],
+ [40, 200],
+ [40, 196],
+ [40, 194],
+ [40, 202],
+ [84, 172],
+ [84, 174],
+ [84, 176],
+ [84, 202],
+ [47, 89],
+ [47, 108],
+ [47, 127],
+ [47, 144],
+ [47, 147],
+ [47, 150],
+ [47, 172],
+ [47, 178],
+ [47, 180],
+ [47, 186],
+ [47, 188],
+ [47, 196],
+ [47, 194],
+ [47, 202],
+ [89, 172],
+ [89, 178],
+ [89, 180],
+ [89, 202],
+ [54, 108],
+ [54, 132],
+ [54, 94],
+ [54, 156],
+ [54, 153],
+ [54, 159],
+ [54, 172],
+ [54, 186],
+ [54, 188],
+ [54, 198],
+ [54, 200],
+ [54, 184],
+ [54, 182],
+ [54, 202],
+ [108, 172],
+ [108, 186],
+ [108, 188],
+ [108, 202],
+ [132, 172],
+ [132, 198],
+ [132, 200],
+ [132, 202],
+ [61, 94],
+ [61, 113],
+ [61, 127],
+ [61, 165],
+ [61, 168],
+ [61, 162],
+ [61, 172],
+ [61, 184],
+ [61, 182],
+ [61, 192],
+ [61, 190],
+ [61, 196],
+ [61, 194],
+ [61, 202],
+ [94, 172],
+ [94, 184],
+ [94, 182],
+ [94, 202],
+ [113, 172],
+ [113, 192],
+ [113, 190],
+ [113, 202],
+ [127, 172],
+ [127, 196],
+ [127, 194],
+ [127, 202],
+ [172, 202],
+ [12, 23],
+ [12, 32],
+ [12, 41],
+ [12, 65],
+ [12, 70],
+ [12, 74],
+ [12, 78],
+ [12, 48],
+ [12, 55],
+ [12, 62],
+ [12, 85],
+ [12, 97],
+ [12, 101],
+ [12, 104],
+ [12, 90],
+ [12, 95],
+ [12, 116],
+ [12, 120],
+ [12, 123],
+ [12, 109],
+ [12, 114],
+ [12, 135],
+ [12, 142],
+ [12, 139],
+ [12, 133],
+ [12, 128],
+ [12, 144],
+ [12, 153],
+ [12, 162],
+ [12, 157],
+ [12, 166],
+ [12, 148],
+ [12, 169],
+ [12, 151],
+ [12, 160],
+ [12, 174],
+ [12, 177],
+ [12, 173],
+ [12, 178],
+ [12, 182],
+ [12, 185],
+ [12, 181],
+ [12, 186],
+ [12, 190],
+ [12, 193],
+ [12, 189],
+ [12, 198],
+ [12, 194],
+ [12, 197],
+ [12, 201],
+ [12, 202],
+ [23, 85],
+ [23, 97],
+ [23, 101],
+ [23, 104],
+ [23, 90],
+ [23, 95],
+ [23, 174],
+ [23, 177],
+ [23, 173],
+ [23, 178],
+ [23, 182],
+ [23, 185],
+ [23, 181],
+ [23, 202],
+ [32, 85],
+ [32, 116],
+ [32, 120],
+ [32, 123],
+ [32, 109],
+ [32, 114],
+ [32, 174],
+ [32, 177],
+ [32, 173],
+ [32, 186],
+ [32, 190],
+ [32, 193],
+ [32, 189],
+ [32, 202],
+ [41, 85],
+ [41, 135],
+ [41, 142],
+ [41, 139],
+ [41, 133],
+ [41, 128],
+ [41, 174],
+ [41, 177],
+ [41, 173],
+ [41, 198],
+ [41, 194],
+ [41, 197],
+ [41, 201],
+ [41, 202],
+ [85, 174],
+ [85, 177],
+ [85, 173],
+ [85, 202],
+ [65, 97],
+ [65, 116],
+ [65, 135],
+ [65, 144],
+ [65, 153],
+ [65, 162],
+ [65, 174],
+ [65, 178],
+ [65, 182],
+ [65, 186],
+ [65, 190],
+ [65, 198],
+ [65, 194],
+ [65, 202],
+ [97, 174],
+ [97, 178],
+ [97, 182],
+ [97, 202],
+ [116, 174],
+ [116, 186],
+ [116, 190],
+ [116, 202],
+ [135, 174],
+ [135, 198],
+ [135, 194],
+ [135, 202],
+ [174, 202],
+ [70, 101],
+ [70, 120],
+ [70, 139],
+ [70, 144],
+ [70, 157],
+ [70, 166],
+ [70, 177],
+ [70, 178],
+ [70, 185],
+ [70, 186],
+ [70, 193],
+ [70, 201],
+ [70, 194],
+ [70, 202],
+ [101, 177],
+ [101, 178],
+ [101, 185],
+ [101, 202],
+ [74, 120],
+ [74, 142],
+ [74, 104],
+ [74, 148],
+ [74, 153],
+ [74, 169],
+ [74, 177],
+ [74, 186],
+ [74, 193],
+ [74, 198],
+ [74, 197],
+ [74, 181],
+ [74, 182],
+ [74, 202],
+ [120, 177],
+ [120, 186],
+ [120, 193],
+ [120, 202],
+ [142, 177],
+ [142, 198],
+ [142, 197],
+ [142, 202],
+ [78, 104],
+ [78, 123],
+ [78, 139],
+ [78, 151],
+ [78, 160],
+ [78, 162],
+ [78, 177],
+ [78, 181],
+ [78, 182],
+ [78, 189],
+ [78, 190],
+ [78, 201],
+ [78, 194],
+ [78, 202],
+ [104, 177],
+ [104, 181],
+ [104, 182],
+ [104, 202],
+ [123, 177],
+ [123, 189],
+ [123, 190],
+ [123, 202],
+ [139, 177],
+ [139, 201],
+ [139, 194],
+ [139, 202],
+ [177, 202],
+ [13, 24],
+ [13, 48],
+ [13, 56],
+ [13, 63],
+ [13, 66],
+ [13, 69],
+ [13, 75],
+ [13, 79],
+ [13, 33],
+ [13, 42],
+ [13, 90],
+ [13, 96],
+ [13, 98],
+ [13, 100],
+ [13, 105],
+ [13, 86],
+ [13, 144],
+ [13, 148],
+ [13, 151],
+ [13, 109],
+ [13, 128],
+ [13, 156],
+ [13, 154],
+ [13, 161],
+ [13, 134],
+ [13, 165],
+ [13, 170],
+ [13, 163],
+ [13, 115],
+ [13, 117],
+ [13, 136],
+ [13, 119],
+ [13, 138],
+ [13, 143],
+ [13, 124],
+ [13, 178],
+ [13, 181],
+ [13, 173],
+ [13, 184],
+ [13, 183],
+ [13, 175],
+ [13, 176],
+ [13, 186],
+ [13, 194],
+ [13, 197],
+ [13, 189],
+ [13, 200],
+ [13, 199],
+ [13, 192],
+ [13, 191],
+ [13, 202],
+ [24, 90],
+ [24, 96],
+ [24, 98],
+ [24, 100],
+ [24, 105],
+ [24, 86],
+ [24, 178],
+ [24, 181],
+ [24, 173],
+ [24, 184],
+ [24, 183],
+ [24, 175],
+ [24, 176],
+ [24, 202],
+ [48, 90],
+ [48, 144],
+ [48, 148],
+ [48, 151],
+ [48, 109],
+ [48, 128],
+ [48, 178],
+ [48, 181],
+ [48, 173],
+ [48, 186],
+ [48, 194],
+ [48, 197],
+ [48, 189],
+ [48, 202],
+ [90, 178],
+ [90, 181],
+ [90, 173],
+ [90, 202],
+ [56, 96],
+ [56, 156],
+ [56, 154],
+ [56, 161],
+ [56, 109],
+ [56, 134],
+ [56, 184],
+ [56, 183],
+ [56, 173],
+ [56, 186],
+ [56, 200],
+ [56, 199],
+ [56, 189],
+ [56, 202],
+ [63, 96],
+ [63, 165],
+ [63, 170],
+ [63, 163],
+ [63, 115],
+ [63, 128],
+ [63, 184],
+ [63, 183],
+ [63, 173],
+ [63, 192],
+ [63, 194],
+ [63, 197],
+ [63, 191],
+ [63, 202],
+ [96, 184],
+ [96, 183],
+ [96, 173],
+ [96, 202],
+ [66, 98],
+ [66, 144],
+ [66, 154],
+ [66, 163],
+ [66, 117],
+ [66, 136],
+ [66, 178],
+ [66, 183],
+ [66, 175],
+ [66, 186],
+ [66, 194],
+ [66, 199],
+ [66, 191],
+ [66, 202],
+ [98, 178],
+ [98, 183],
+ [98, 175],
+ [98, 202],
+ [69, 100],
+ [69, 144],
+ [69, 156],
+ [69, 165],
+ [69, 119],
+ [69, 138],
+ [69, 178],
+ [69, 184],
+ [69, 176],
+ [69, 186],
+ [69, 194],
+ [69, 200],
+ [69, 192],
+ [69, 202],
+ [100, 178],
+ [100, 184],
+ [100, 176],
+ [100, 202],
+ [144, 178],
+ [144, 186],
+ [144, 194],
+ [144, 202],
+ [178, 202],
+ [156, 184],
+ [156, 186],
+ [156, 200],
+ [156, 202],
+ [165, 184],
+ [165, 192],
+ [165, 194],
+ [165, 202],
+ [184, 202],
+ [75, 148],
+ [75, 154],
+ [75, 170],
+ [75, 105],
+ [75, 119],
+ [75, 143],
+ [75, 181],
+ [75, 186],
+ [75, 197],
+ [75, 183],
+ [75, 199],
+ [75, 192],
+ [75, 176],
+ [75, 202],
+ [148, 181],
+ [148, 186],
+ [148, 197],
+ [148, 202],
+ [154, 183],
+ [154, 186],
+ [154, 199],
+ [154, 202],
+ [170, 183],
+ [170, 192],
+ [170, 197],
+ [170, 202],
+ [79, 105],
+ [79, 151],
+ [79, 161],
+ [79, 163],
+ [79, 124],
+ [79, 138],
+ [79, 181],
+ [79, 183],
+ [79, 176],
+ [79, 189],
+ [79, 194],
+ [79, 200],
+ [79, 191],
+ [79, 202],
+ [105, 181],
+ [105, 183],
+ [105, 176],
+ [105, 202],
+ [151, 181],
+ [151, 189],
+ [151, 194],
+ [151, 202],
+ [181, 202],
+ [161, 183],
+ [161, 189],
+ [161, 200],
+ [161, 202],
+ [163, 183],
+ [163, 191],
+ [163, 194],
+ [163, 202],
+ [183, 202],
+ [14, 33],
+ [14, 43],
+ [14, 49],
+ [14, 55],
+ [14, 64],
+ [14, 67],
+ [14, 71],
+ [14, 73],
+ [14, 80],
+ [14, 25],
+ [14, 109],
+ [14, 115],
+ [14, 117],
+ [14, 119],
+ [14, 124],
+ [14, 86],
+ [14, 133],
+ [14, 129],
+ [14, 137],
+ [14, 141],
+ [14, 140],
+ [14, 145],
+ [14, 147],
+ [14, 152],
+ [14, 91],
+ [14, 157],
+ [14, 153],
+ [14, 160],
+ [14, 95],
+ [14, 167],
+ [14, 168],
+ [14, 164],
+ [14, 99],
+ [14, 102],
+ [14, 103],
+ [14, 186],
+ [14, 189],
+ [14, 173],
+ [14, 192],
+ [14, 191],
+ [14, 175],
+ [14, 176],
+ [14, 198],
+ [14, 201],
+ [14, 196],
+ [14, 195],
+ [14, 179],
+ [14, 180],
+ [14, 185],
+ [14, 182],
+ [14, 202],
+ [33, 109],
+ [33, 115],
+ [33, 117],
+ [33, 119],
+ [33, 124],
+ [33, 86],
+ [33, 186],
+ [33, 189],
+ [33, 173],
+ [33, 192],
+ [33, 191],
+ [33, 175],
+ [33, 176],
+ [33, 202],
+ [43, 133],
+ [43, 129],
+ [43, 137],
+ [43, 141],
+ [43, 140],
+ [43, 86],
+ [43, 198],
+ [43, 201],
+ [43, 173],
+ [43, 196],
+ [43, 195],
+ [43, 175],
+ [43, 176],
+ [43, 202],
+ [49, 109],
+ [49, 129],
+ [49, 145],
+ [49, 147],
+ [49, 152],
+ [49, 91],
+ [49, 186],
+ [49, 189],
+ [49, 173],
+ [49, 196],
+ [49, 195],
+ [49, 179],
+ [49, 180],
+ [49, 202],
+ [55, 109],
+ [55, 133],
+ [55, 157],
+ [55, 153],
+ [55, 160],
+ [55, 95],
+ [55, 186],
+ [55, 189],
+ [55, 173],
+ [55, 198],
+ [55, 201],
+ [55, 185],
+ [55, 182],
+ [55, 202],
+ [109, 186],
+ [109, 189],
+ [109, 173],
+ [109, 202],
+ [133, 198],
+ [133, 201],
+ [133, 173],
+ [133, 202],
+ [64, 115],
+ [64, 129],
+ [64, 167],
+ [64, 168],
+ [64, 164],
+ [64, 95],
+ [64, 192],
+ [64, 191],
+ [64, 173],
+ [64, 196],
+ [64, 195],
+ [64, 185],
+ [64, 182],
+ [64, 202],
+ [115, 192],
+ [115, 191],
+ [115, 173],
+ [115, 202],
+ [129, 196],
+ [129, 195],
+ [129, 173],
+ [129, 202],
+ [67, 117],
+ [67, 137],
+ [67, 145],
+ [67, 153],
+ [67, 164],
+ [67, 99],
+ [67, 186],
+ [67, 191],
+ [67, 175],
+ [67, 198],
+ [67, 195],
+ [67, 179],
+ [67, 182],
+ [67, 202],
+ [117, 186],
+ [117, 191],
+ [117, 175],
+ [117, 202],
+ [137, 198],
+ [137, 195],
+ [137, 175],
+ [137, 202],
+ [71, 145],
+ [71, 157],
+ [71, 167],
+ [71, 119],
+ [71, 140],
+ [71, 102],
+ [71, 186],
+ [71, 195],
+ [71, 179],
+ [71, 201],
+ [71, 185],
+ [71, 192],
+ [71, 176],
+ [71, 202],
+ [145, 186],
+ [145, 195],
+ [145, 179],
+ [145, 202],
+ [157, 186],
+ [157, 201],
+ [157, 185],
+ [157, 202],
+ [167, 192],
+ [167, 195],
+ [167, 185],
+ [167, 202],
+ [73, 119],
+ [73, 141],
+ [73, 147],
+ [73, 153],
+ [73, 168],
+ [73, 103],
+ [73, 186],
+ [73, 192],
+ [73, 176],
+ [73, 198],
+ [73, 196],
+ [73, 180],
+ [73, 182],
+ [73, 202],
+ [119, 186],
+ [119, 192],
+ [119, 176],
+ [119, 202],
+ [141, 198],
+ [141, 196],
+ [141, 176],
+ [141, 202],
+ [147, 186],
+ [147, 196],
+ [147, 180],
+ [147, 202],
+ [153, 186],
+ [153, 198],
+ [153, 182],
+ [153, 202],
+ [186, 202],
+ [198, 202],
+ [168, 192],
+ [168, 196],
+ [168, 182],
+ [168, 202],
+ [192, 202],
+ [196, 202],
+ [80, 124],
+ [80, 140],
+ [80, 152],
+ [80, 160],
+ [80, 164],
+ [80, 103],
+ [80, 189],
+ [80, 191],
+ [80, 176],
+ [80, 201],
+ [80, 195],
+ [80, 180],
+ [80, 182],
+ [80, 202],
+ [124, 189],
+ [124, 191],
+ [124, 176],
+ [124, 202],
+ [140, 201],
+ [140, 195],
+ [140, 176],
+ [140, 202],
+ [152, 189],
+ [152, 195],
+ [152, 180],
+ [152, 202],
+ [160, 189],
+ [160, 201],
+ [160, 182],
+ [160, 202],
+ [189, 202],
+ [201, 202],
+ [164, 191],
+ [164, 195],
+ [164, 182],
+ [164, 202],
+ [191, 202],
+ [195, 202],
+ [15, 25],
+ [15, 34],
+ [15, 42],
+ [15, 50],
+ [15, 57],
+ [15, 62],
+ [15, 68],
+ [15, 72],
+ [15, 76],
+ [15, 77],
+ [15, 86],
+ [15, 91],
+ [15, 95],
+ [15, 99],
+ [15, 102],
+ [15, 103],
+ [15, 110],
+ [15, 114],
+ [15, 118],
+ [15, 121],
+ [15, 122],
+ [15, 134],
+ [15, 128],
+ [15, 136],
+ [15, 143],
+ [15, 138],
+ [15, 146],
+ [15, 149],
+ [15, 150],
+ [15, 158],
+ [15, 155],
+ [15, 159],
+ [15, 166],
+ [15, 169],
+ [15, 162],
+ [15, 173],
+ [15, 175],
+ [15, 176],
+ [15, 179],
+ [15, 180],
+ [15, 185],
+ [15, 182],
+ [15, 187],
+ [15, 188],
+ [15, 193],
+ [15, 190],
+ [15, 199],
+ [15, 200],
+ [15, 197],
+ [15, 194],
+ [15, 202],
+ [25, 86],
+ [25, 91],
+ [25, 95],
+ [25, 99],
+ [25, 102],
+ [25, 103],
+ [25, 173],
+ [25, 175],
+ [25, 176],
+ [25, 179],
+ [25, 180],
+ [25, 185],
+ [25, 182],
+ [25, 202],
+ [34, 86],
+ [34, 110],
+ [34, 114],
+ [34, 118],
+ [34, 121],
+ [34, 122],
+ [34, 173],
+ [34, 175],
+ [34, 176],
+ [34, 187],
+ [34, 188],
+ [34, 193],
+ [34, 190],
+ [34, 202],
+ [42, 86],
+ [42, 134],
+ [42, 128],
+ [42, 136],
+ [42, 143],
+ [42, 138],
+ [42, 173],
+ [42, 175],
+ [42, 176],
+ [42, 199],
+ [42, 200],
+ [42, 197],
+ [42, 194],
+ [42, 202],
+ [86, 173],
+ [86, 175],
+ [86, 176],
+ [86, 202],
+ [50, 91],
+ [50, 110],
+ [50, 128],
+ [50, 146],
+ [50, 149],
+ [50, 150],
+ [50, 173],
+ [50, 179],
+ [50, 180],
+ [50, 187],
+ [50, 188],
+ [50, 197],
+ [50, 194],
+ [50, 202],
+ [91, 173],
+ [91, 179],
+ [91, 180],
+ [91, 202],
+ [57, 110],
+ [57, 134],
+ [57, 95],
+ [57, 158],
+ [57, 155],
+ [57, 159],
+ [57, 173],
+ [57, 187],
+ [57, 188],
+ [57, 199],
+ [57, 200],
+ [57, 185],
+ [57, 182],
+ [57, 202],
+ [110, 173],
+ [110, 187],
+ [110, 188],
+ [110, 202],
+ [134, 173],
+ [134, 199],
+ [134, 200],
+ [134, 202],
+ [62, 95],
+ [62, 114],
+ [62, 128],
+ [62, 166],
+ [62, 169],
+ [62, 162],
+ [62, 173],
+ [62, 185],
+ [62, 182],
+ [62, 193],
+ [62, 190],
+ [62, 197],
+ [62, 194],
+ [62, 202],
+ [95, 173],
+ [95, 185],
+ [95, 182],
+ [95, 202],
+ [114, 173],
+ [114, 193],
+ [114, 190],
+ [114, 202],
+ [128, 173],
+ [128, 197],
+ [128, 194],
+ [128, 202],
+ [173, 202],
+ [68, 99],
+ [68, 118],
+ [68, 136],
+ [68, 146],
+ [68, 155],
+ [68, 162],
+ [68, 175],
+ [68, 179],
+ [68, 182],
+ [68, 187],
+ [68, 190],
+ [68, 199],
+ [68, 194],
+ [68, 202],
+ [99, 175],
+ [99, 179],
+ [99, 182],
+ [99, 202],
+ [118, 175],
+ [118, 187],
+ [118, 190],
+ [118, 202],
+ [136, 175],
+ [136, 199],
+ [136, 194],
+ [136, 202],
+ [175, 202],
+ [72, 102],
+ [72, 146],
+ [72, 158],
+ [72, 166],
+ [72, 121],
+ [72, 138],
+ [72, 179],
+ [72, 185],
+ [72, 176],
+ [72, 187],
+ [72, 194],
+ [72, 200],
+ [72, 193],
+ [72, 202],
+ [102, 179],
+ [102, 185],
+ [102, 176],
+ [102, 202],
+ [146, 179],
+ [146, 187],
+ [146, 194],
+ [146, 202],
+ [179, 202],
+ [158, 185],
+ [158, 187],
+ [158, 200],
+ [158, 202],
+ [166, 185],
+ [166, 193],
+ [166, 194],
+ [166, 202],
+ [185, 202],
+ [76, 121],
+ [76, 143],
+ [76, 149],
+ [76, 155],
+ [76, 169],
+ [76, 103],
+ [76, 187],
+ [76, 193],
+ [76, 176],
+ [76, 199],
+ [76, 197],
+ [76, 180],
+ [76, 182],
+ [76, 202],
+ [121, 187],
+ [121, 193],
+ [121, 176],
+ [121, 202],
+ [143, 199],
+ [143, 197],
+ [143, 176],
+ [143, 202],
+ [149, 187],
+ [149, 197],
+ [149, 180],
+ [149, 202],
+ [155, 187],
+ [155, 199],
+ [155, 182],
+ [155, 202],
+ [187, 202],
+ [199, 202],
+ [169, 193],
+ [169, 197],
+ [169, 182],
+ [169, 202],
+ [193, 202],
+ [197, 202],
+ [77, 103],
+ [77, 122],
+ [77, 138],
+ [77, 150],
+ [77, 159],
+ [77, 162],
+ [77, 176],
+ [77, 180],
+ [77, 182],
+ [77, 188],
+ [77, 190],
+ [77, 200],
+ [77, 194],
+ [77, 202],
+ [103, 176],
+ [103, 180],
+ [103, 182],
+ [103, 202],
+ [122, 176],
+ [122, 188],
+ [122, 190],
+ [122, 202],
+ [138, 176],
+ [138, 200],
+ [138, 194],
+ [138, 202],
+ [176, 202],
+ [150, 180],
+ [150, 188],
+ [150, 194],
+ [150, 202],
+ [180, 202],
+ [159, 188],
+ [159, 200],
+ [159, 182],
+ [159, 202],
+ [188, 202],
+ [200, 202],
+ [162, 182],
+ [162, 190],
+ [162, 194],
+ [162, 202],
+ [182, 202],
+ [190, 202],
+ [194, 202]]
+
+B3_rels = [[0, 1],
+ [0, 2],
+ [0, 3],
+ [0, 4],
+ [0, 5],
+ [0, 6],
+ [0, 7],
+ [0, 8],
+ [0, 9],
+ [0, 10],
+ [0, 11],
+ [0, 12],
+ [0, 13],
+ [0, 14],
+ [0, 15],
+ [0, 16],
+ [0, 18],
+ [0, 19],
+ [0, 17],
+ [0, 22],
+ [0, 20],
+ [0, 21],
+ [0, 23],
+ [1, 10],
+ [1, 11],
+ [1, 12],
+ [1, 13],
+ [1, 23],
+ [2, 10],
+ [2, 14],
+ [2, 15],
+ [2, 16],
+ [2, 23],
+ [3, 10],
+ [3, 18],
+ [3, 19],
+ [3, 17],
+ [3, 23],
+ [4, 10],
+ [4, 22],
+ [4, 20],
+ [4, 21],
+ [4, 23],
+ [10, 23],
+ [5, 11],
+ [5, 14],
+ [5, 20],
+ [5, 17],
+ [5, 23],
+ [11, 23],
+ [6, 14],
+ [6, 18],
+ [6, 12],
+ [6, 21],
+ [6, 23],
+ [14, 23],
+ [18, 23],
+ [7, 15],
+ [7, 22],
+ [7, 12],
+ [7, 17],
+ [7, 23],
+ [15, 23],
+ [22, 23],
+ [8, 12],
+ [8, 19],
+ [8, 20],
+ [8, 16],
+ [8, 23],
+ [12, 23],
+ [19, 23],
+ [20, 23],
+ [9, 13],
+ [9, 16],
+ [9, 17],
+ [9, 21],
+ [9, 23],
+ [13, 23],
+ [16, 23],
+ [17, 23],
+ [21, 23]]
+
+B4_rels = [[0, 1],
+ [0, 2],
+ [0, 3],
+ [0, 4],
+ [0, 5],
+ [0, 6],
+ [0, 7],
+ [0, 8],
+ [0, 9],
+ [0, 10],
+ [0, 11],
+ [0, 12],
+ [0, 13],
+ [0, 14],
+ [0, 15],
+ [0, 16],
+ [0, 17],
+ [0, 18],
+ [0, 19],
+ [0, 20],
+ [0, 21],
+ [0, 22],
+ [0, 23],
+ [0, 24],
+ [0, 25],
+ [0, 26],
+ [0, 27],
+ [0, 28],
+ [0, 29],
+ [0, 30],
+ [0, 31],
+ [0, 32],
+ [0, 33],
+ [0, 35],
+ [0, 36],
+ [0, 34],
+ [0, 37],
+ [0, 39],
+ [0, 40],
+ [0, 38],
+ [0, 41],
+ [0, 44],
+ [0, 42],
+ [0, 43],
+ [0, 45],
+ [0, 48],
+ [0, 46],
+ [0, 47],
+ [0, 49],
+ [0, 50],
+ [0, 51],
+ [0, 52],
+ [0, 53],
+ [0, 54],
+ [0, 56],
+ [0, 55],
+ [0, 57],
+ [0, 59],
+ [0, 58],
+ [0, 61],
+ [0, 62],
+ [0, 63],
+ [0, 64],
+ [0, 60],
+ [0, 66],
+ [0, 68],
+ [0, 65],
+ [0, 69],
+ [0, 67],
+ [0, 72],
+ [0, 73],
+ [0, 74],
+ [0, 70],
+ [0, 71],
+ [0, 75],
+ [0, 76],
+ [0, 77],
+ [0, 78],
+ [0, 79],
+ [0, 80],
+ [0, 81],
+ [0, 83],
+ [0, 84],
+ [0, 82],
+ [0, 87],
+ [0, 85],
+ [0, 86],
+ [0, 88],
+ [0, 89],
+ [0, 90],
+ [0, 92],
+ [0, 93],
+ [0, 91],
+ [0, 96],
+ [0, 94],
+ [0, 95],
+ [0, 100],
+ [0, 101],
+ [0, 102],
+ [0, 103],
+ [0, 104],
+ [0, 105],
+ [0, 98],
+ [0, 99],
+ [0, 97],
+ [0, 113],
+ [0, 114],
+ [0, 112],
+ [0, 108],
+ [0, 106],
+ [0, 107],
+ [0, 111],
+ [0, 109],
+ [0, 110],
+ [0, 115],
+ [1, 17],
+ [1, 18],
+ [1, 19],
+ [1, 20],
+ [1, 21],
+ [1, 22],
+ [1, 23],
+ [1, 24],
+ [1, 25],
+ [1, 75],
+ [1, 76],
+ [1, 77],
+ [1, 78],
+ [1, 79],
+ [1, 80],
+ [1, 81],
+ [1, 83],
+ [1, 84],
+ [1, 82],
+ [1, 87],
+ [1, 85],
+ [1, 86],
+ [1, 115],
+ [2, 17],
+ [2, 26],
+ [2, 27],
+ [2, 28],
+ [2, 29],
+ [2, 30],
+ [2, 31],
+ [2, 32],
+ [2, 33],
+ [2, 75],
+ [2, 76],
+ [2, 77],
+ [2, 78],
+ [2, 88],
+ [2, 89],
+ [2, 90],
+ [2, 92],
+ [2, 93],
+ [2, 91],
+ [2, 96],
+ [2, 94],
+ [2, 95],
+ [2, 115],
+ [3, 17],
+ [3, 35],
+ [3, 36],
+ [3, 34],
+ [3, 37],
+ [3, 39],
+ [3, 40],
+ [3, 38],
+ [3, 41],
+ [3, 75],
+ [3, 76],
+ [3, 77],
+ [3, 78],
+ [3, 100],
+ [3, 101],
+ [3, 102],
+ [3, 103],
+ [3, 104],
+ [3, 105],
+ [3, 98],
+ [3, 99],
+ [3, 97],
+ [3, 115],
+ [4, 17],
+ [4, 44],
+ [4, 42],
+ [4, 43],
+ [4, 45],
+ [4, 48],
+ [4, 46],
+ [4, 47],
+ [4, 49],
+ [4, 75],
+ [4, 76],
+ [4, 77],
+ [4, 78],
+ [4, 113],
+ [4, 114],
+ [4, 112],
+ [4, 108],
+ [4, 106],
+ [4, 107],
+ [4, 111],
+ [4, 109],
+ [4, 110],
+ [4, 115],
+ [17, 75],
+ [17, 76],
+ [17, 77],
+ [17, 78],
+ [17, 115],
+ [5, 18],
+ [5, 26],
+ [5, 42],
+ [5, 34],
+ [5, 50],
+ [5, 51],
+ [5, 52],
+ [5, 53],
+ [5, 54],
+ [5, 75],
+ [5, 79],
+ [5, 80],
+ [5, 81],
+ [5, 88],
+ [5, 89],
+ [5, 90],
+ [5, 108],
+ [5, 106],
+ [5, 107],
+ [5, 98],
+ [5, 99],
+ [5, 97],
+ [5, 115],
+ [18, 75],
+ [18, 79],
+ [18, 80],
+ [18, 81],
+ [18, 115],
+ [6, 26],
+ [6, 35],
+ [6, 19],
+ [6, 43],
+ [6, 56],
+ [6, 55],
+ [6, 57],
+ [6, 59],
+ [6, 58],
+ [6, 75],
+ [6, 88],
+ [6, 89],
+ [6, 90],
+ [6, 100],
+ [6, 101],
+ [6, 102],
+ [6, 83],
+ [6, 84],
+ [6, 82],
+ [6, 111],
+ [6, 109],
+ [6, 110],
+ [6, 115],
+ [26, 75],
+ [26, 88],
+ [26, 89],
+ [26, 90],
+ [26, 115],
+ [35, 75],
+ [35, 100],
+ [35, 101],
+ [35, 102],
+ [35, 115],
+ [7, 27],
+ [7, 44],
+ [7, 19],
+ [7, 34],
+ [7, 61],
+ [7, 62],
+ [7, 63],
+ [7, 64],
+ [7, 60],
+ [7, 75],
+ [7, 92],
+ [7, 93],
+ [7, 91],
+ [7, 113],
+ [7, 114],
+ [7, 112],
+ [7, 83],
+ [7, 84],
+ [7, 82],
+ [7, 98],
+ [7, 99],
+ [7, 97],
+ [7, 115],
+ [27, 75],
+ [27, 92],
+ [27, 93],
+ [27, 91],
+ [27, 115],
+ [44, 75],
+ [44, 113],
+ [44, 114],
+ [44, 112],
+ [44, 115],
+ [8, 19],
+ [8, 36],
+ [8, 42],
+ [8, 28],
+ [8, 66],
+ [8, 68],
+ [8, 65],
+ [8, 69],
+ [8, 67],
+ [8, 75],
+ [8, 83],
+ [8, 84],
+ [8, 82],
+ [8, 103],
+ [8, 104],
+ [8, 105],
+ [8, 108],
+ [8, 106],
+ [8, 107],
+ [8, 96],
+ [8, 94],
+ [8, 95],
+ [8, 115],
+ [19, 75],
+ [19, 83],
+ [19, 84],
+ [19, 82],
+ [19, 115],
+ [36, 75],
+ [36, 103],
+ [36, 104],
+ [36, 105],
+ [36, 115],
+ [42, 75],
+ [42, 108],
+ [42, 106],
+ [42, 107],
+ [42, 115],
+ [9, 20],
+ [9, 28],
+ [9, 34],
+ [9, 43],
+ [9, 72],
+ [9, 73],
+ [9, 74],
+ [9, 70],
+ [9, 71],
+ [9, 75],
+ [9, 87],
+ [9, 85],
+ [9, 86],
+ [9, 96],
+ [9, 94],
+ [9, 95],
+ [9, 98],
+ [9, 99],
+ [9, 97],
+ [9, 111],
+ [9, 109],
+ [9, 110],
+ [9, 115],
+ [20, 75],
+ [20, 87],
+ [20, 85],
+ [20, 86],
+ [20, 115],
+ [28, 75],
+ [28, 96],
+ [28, 94],
+ [28, 95],
+ [28, 115],
+ [34, 75],
+ [34, 98],
+ [34, 99],
+ [34, 97],
+ [34, 115],
+ [43, 75],
+ [43, 111],
+ [43, 109],
+ [43, 110],
+ [43, 115],
+ [75, 115],
+ [10, 21],
+ [10, 29],
+ [10, 37],
+ [10, 45],
+ [10, 50],
+ [10, 55],
+ [10, 65],
+ [10, 70],
+ [10, 60],
+ [10, 76],
+ [10, 79],
+ [10, 85],
+ [10, 82],
+ [10, 88],
+ [10, 94],
+ [10, 91],
+ [10, 100],
+ [10, 103],
+ [10, 97],
+ [10, 106],
+ [10, 109],
+ [10, 112],
+ [10, 115],
+ [21, 76],
+ [21, 79],
+ [21, 85],
+ [21, 82],
+ [21, 115],
+ [29, 76],
+ [29, 88],
+ [29, 94],
+ [29, 91],
+ [29, 115],
+ [37, 76],
+ [37, 100],
+ [37, 103],
+ [37, 97],
+ [37, 115],
+ [45, 76],
+ [45, 106],
+ [45, 109],
+ [45, 112],
+ [45, 115],
+ [76, 115],
+ [11, 22],
+ [11, 50],
+ [11, 56],
+ [11, 61],
+ [11, 66],
+ [11, 30],
+ [11, 46],
+ [11, 38],
+ [11, 71],
+ [11, 79],
+ [11, 83],
+ [11, 77],
+ [11, 86],
+ [11, 88],
+ [11, 106],
+ [11, 97],
+ [11, 101],
+ [11, 110],
+ [11, 92],
+ [11, 113],
+ [11, 104],
+ [11, 95],
+ [11, 115],
+ [22, 79],
+ [22, 83],
+ [22, 77],
+ [22, 86],
+ [22, 115],
+ [50, 79],
+ [50, 88],
+ [50, 106],
+ [50, 97],
+ [50, 115],
+ [79, 115],
+ [56, 83],
+ [56, 88],
+ [56, 101],
+ [56, 110],
+ [56, 115],
+ [61, 83],
+ [61, 92],
+ [61, 113],
+ [61, 97],
+ [61, 115],
+ [66, 83],
+ [66, 106],
+ [66, 104],
+ [66, 95],
+ [66, 115],
+ [83, 115],
+ [12, 30],
+ [12, 39],
+ [12, 51],
+ [12, 55],
+ [12, 62],
+ [12, 72],
+ [12, 23],
+ [12, 47],
+ [12, 67],
+ [12, 88],
+ [12, 92],
+ [12, 77],
+ [12, 95],
+ [12, 100],
+ [12, 98],
+ [12, 105],
+ [12, 80],
+ [12, 107],
+ [12, 109],
+ [12, 82],
+ [12, 114],
+ [12, 87],
+ [12, 115],
+ [30, 88],
+ [30, 92],
+ [30, 77],
+ [30, 95],
+ [30, 115],
+ [39, 100],
+ [39, 98],
+ [39, 77],
+ [39, 105],
+ [39, 115],
+ [51, 88],
+ [51, 98],
+ [51, 80],
+ [51, 107],
+ [51, 115],
+ [55, 88],
+ [55, 100],
+ [55, 109],
+ [55, 82],
+ [55, 115],
+ [88, 115],
+ [100, 115],
+ [62, 92],
+ [62, 98],
+ [62, 114],
+ [62, 82],
+ [62, 115],
+ [92, 115],
+ [72, 98],
+ [72, 87],
+ [72, 109],
+ [72, 95],
+ [72, 115],
+ [98, 115],
+ [13, 31],
+ [13, 48],
+ [13, 52],
+ [13, 57],
+ [13, 68],
+ [13, 73],
+ [13, 23],
+ [13, 38],
+ [13, 60],
+ [13, 89],
+ [13, 96],
+ [13, 77],
+ [13, 91],
+ [13, 108],
+ [13, 111],
+ [13, 112],
+ [13, 80],
+ [13, 97],
+ [13, 101],
+ [13, 82],
+ [13, 104],
+ [13, 87],
+ [13, 115],
+ [31, 89],
+ [31, 96],
+ [31, 77],
+ [31, 91],
+ [31, 115],
+ [48, 108],
+ [48, 111],
+ [48, 77],
+ [48, 112],
+ [48, 115],
+ [52, 89],
+ [52, 108],
+ [52, 80],
+ [52, 97],
+ [52, 115],
+ [57, 89],
+ [57, 111],
+ [57, 101],
+ [57, 82],
+ [57, 115],
+ [89, 115],
+ [68, 108],
+ [68, 96],
+ [68, 104],
+ [68, 82],
+ [68, 115],
+ [108, 115],
+ [73, 96],
+ [73, 111],
+ [73, 87],
+ [73, 97],
+ [73, 115],
+ [96, 115],
+ [111, 115],
+ [14, 23],
+ [14, 40],
+ [14, 46],
+ [14, 53],
+ [14, 63],
+ [14, 65],
+ [14, 74],
+ [14, 32],
+ [14, 58],
+ [14, 80],
+ [14, 87],
+ [14, 77],
+ [14, 82],
+ [14, 103],
+ [14, 99],
+ [14, 102],
+ [14, 113],
+ [14, 106],
+ [14, 110],
+ [14, 90],
+ [14, 93],
+ [14, 94],
+ [14, 115],
+ [23, 80],
+ [23, 87],
+ [23, 77],
+ [23, 82],
+ [23, 115],
+ [40, 103],
+ [40, 99],
+ [40, 77],
+ [40, 102],
+ [40, 115],
+ [46, 113],
+ [46, 106],
+ [46, 77],
+ [46, 110],
+ [46, 115],
+ [53, 80],
+ [53, 106],
+ [53, 99],
+ [53, 90],
+ [53, 115],
+ [80, 115],
+ [63, 113],
+ [63, 99],
+ [63, 93],
+ [63, 82],
+ [63, 115],
+ [113, 115],
+ [65, 103],
+ [65, 106],
+ [65, 94],
+ [65, 82],
+ [65, 115],
+ [103, 115],
+ [106, 115],
+ [74, 87],
+ [74, 99],
+ [74, 94],
+ [74, 110],
+ [74, 115],
+ [87, 115],
+ [99, 115],
+ [15, 24],
+ [15, 32],
+ [15, 38],
+ [15, 47],
+ [15, 59],
+ [15, 64],
+ [15, 69],
+ [15, 70],
+ [15, 54],
+ [15, 77],
+ [15, 84],
+ [15, 85],
+ [15, 81],
+ [15, 93],
+ [15, 94],
+ [15, 90],
+ [15, 101],
+ [15, 104],
+ [15, 97],
+ [15, 114],
+ [15, 109],
+ [15, 107],
+ [15, 115],
+ [24, 77],
+ [24, 84],
+ [24, 85],
+ [24, 81],
+ [24, 115],
+ [32, 77],
+ [32, 93],
+ [32, 94],
+ [32, 90],
+ [32, 115],
+ [38, 77],
+ [38, 101],
+ [38, 104],
+ [38, 97],
+ [38, 115],
+ [47, 77],
+ [47, 114],
+ [47, 109],
+ [47, 107],
+ [47, 115],
+ [77, 115],
+ [59, 101],
+ [59, 84],
+ [59, 109],
+ [59, 90],
+ [59, 115],
+ [101, 115],
+ [64, 93],
+ [64, 114],
+ [64, 84],
+ [64, 97],
+ [64, 115],
+ [93, 115],
+ [114, 115],
+ [69, 84],
+ [69, 104],
+ [69, 94],
+ [69, 107],
+ [69, 115],
+ [84, 115],
+ [104, 115],
+ [70, 85],
+ [70, 94],
+ [70, 109],
+ [70, 97],
+ [70, 115],
+ [85, 115],
+ [94, 115],
+ [109, 115],
+ [16, 25],
+ [16, 33],
+ [16, 41],
+ [16, 49],
+ [16, 54],
+ [16, 58],
+ [16, 60],
+ [16, 67],
+ [16, 71],
+ [16, 78],
+ [16, 81],
+ [16, 82],
+ [16, 86],
+ [16, 90],
+ [16, 91],
+ [16, 95],
+ [16, 102],
+ [16, 105],
+ [16, 97],
+ [16, 112],
+ [16, 107],
+ [16, 110],
+ [16, 115],
+ [25, 78],
+ [25, 81],
+ [25, 82],
+ [25, 86],
+ [25, 115],
+ [33, 78],
+ [33, 90],
+ [33, 91],
+ [33, 95],
+ [33, 115],
+ [41, 78],
+ [41, 102],
+ [41, 105],
+ [41, 97],
+ [41, 115],
+ [49, 78],
+ [49, 112],
+ [49, 107],
+ [49, 110],
+ [49, 115],
+ [78, 115],
+ [54, 81],
+ [54, 90],
+ [54, 107],
+ [54, 97],
+ [54, 115],
+ [81, 115],
+ [58, 90],
+ [58, 102],
+ [58, 82],
+ [58, 110],
+ [58, 115],
+ [90, 115],
+ [102, 115],
+ [60, 91],
+ [60, 112],
+ [60, 82],
+ [60, 97],
+ [60, 115],
+ [91, 115],
+ [112, 115],
+ [67, 82],
+ [67, 105],
+ [67, 107],
+ [67, 95],
+ [67, 115],
+ [82, 115],
+ [105, 115],
+ [107, 115],
+ [71, 86],
+ [71, 95],
+ [71, 97],
+ [71, 110],
+ [71, 115],
+ [86, 115],
+ [95, 115],
+ [97, 115],
+ [110, 115]]
+
+D4_rels = [[0, 1],
+ [0, 2],
+ [0, 3],
+ [0, 4],
+ [0, 5],
+ [0, 6],
+ [0, 7],
+ [0, 8],
+ [0, 9],
+ [0, 10],
+ [0, 11],
+ [0, 12],
+ [0, 13],
+ [0, 14],
+ [0, 15],
+ [0, 16],
+ [0, 17],
+ [0, 18],
+ [0, 19],
+ [0, 20],
+ [0, 21],
+ [0, 22],
+ [0, 23],
+ [0, 24],
+ [0, 25],
+ [0, 26],
+ [0, 27],
+ [0, 28],
+ [0, 29],
+ [0, 30],
+ [0, 31],
+ [0, 33],
+ [0, 32],
+ [0, 35],
+ [0, 34],
+ [0, 37],
+ [0, 36],
+ [0, 39],
+ [0, 38],
+ [0, 42],
+ [0, 43],
+ [0, 40],
+ [0, 41],
+ [0, 44],
+ [0, 45],
+ [0, 46],
+ [0, 47],
+ [0, 48],
+ [0, 49],
+ [0, 50],
+ [0, 51],
+ [0, 52],
+ [0, 53],
+ [0, 54],
+ [0, 55],
+ [0, 56],
+ [0, 57],
+ [0, 58],
+ [0, 59],
+ [0, 60],
+ [0, 62],
+ [0, 63],
+ [0, 61],
+ [0, 64],
+ [0, 66],
+ [0, 67],
+ [0, 65],
+ [0, 68],
+ [0, 69],
+ [0, 70],
+ [0, 71],
+ [1, 13],
+ [1, 14],
+ [1, 15],
+ [1, 16],
+ [1, 17],
+ [1, 18],
+ [1, 19],
+ [1, 47],
+ [1, 48],
+ [1, 49],
+ [1, 50],
+ [1, 51],
+ [1, 52],
+ [1, 53],
+ [1, 54],
+ [1, 55],
+ [1, 71],
+ [2, 13],
+ [2, 20],
+ [2, 21],
+ [2, 22],
+ [2, 23],
+ [2, 24],
+ [2, 25],
+ [2, 47],
+ [2, 48],
+ [2, 49],
+ [2, 50],
+ [2, 56],
+ [2, 57],
+ [2, 58],
+ [2, 59],
+ [2, 60],
+ [2, 71],
+ [13, 47],
+ [13, 48],
+ [13, 49],
+ [13, 50],
+ [13, 71],
+ [3, 14],
+ [3, 20],
+ [3, 26],
+ [3, 27],
+ [3, 28],
+ [3, 29],
+ [3, 30],
+ [3, 47],
+ [3, 51],
+ [3, 52],
+ [3, 56],
+ [3, 57],
+ [3, 62],
+ [3, 63],
+ [3, 61],
+ [3, 64],
+ [3, 71],
+ [4, 14],
+ [4, 31],
+ [4, 21],
+ [4, 33],
+ [4, 32],
+ [4, 35],
+ [4, 34],
+ [4, 47],
+ [4, 51],
+ [4, 52],
+ [4, 66],
+ [4, 67],
+ [4, 65],
+ [4, 58],
+ [4, 59],
+ [4, 68],
+ [4, 71],
+ [14, 47],
+ [14, 51],
+ [14, 52],
+ [14, 71],
+ [5, 20],
+ [5, 31],
+ [5, 15],
+ [5, 37],
+ [5, 36],
+ [5, 39],
+ [5, 38],
+ [5, 47],
+ [5, 56],
+ [5, 57],
+ [5, 66],
+ [5, 67],
+ [5, 65],
+ [5, 53],
+ [5, 54],
+ [5, 69],
+ [5, 71],
+ [20, 47],
+ [20, 56],
+ [20, 57],
+ [20, 71],
+ [31, 47],
+ [31, 66],
+ [31, 67],
+ [31, 65],
+ [31, 71],
+ [6, 15],
+ [6, 21],
+ [6, 26],
+ [6, 42],
+ [6, 43],
+ [6, 40],
+ [6, 41],
+ [6, 47],
+ [6, 53],
+ [6, 54],
+ [6, 58],
+ [6, 59],
+ [6, 62],
+ [6, 63],
+ [6, 61],
+ [6, 70],
+ [6, 71],
+ [15, 47],
+ [15, 53],
+ [15, 54],
+ [15, 71],
+ [21, 47],
+ [21, 58],
+ [21, 59],
+ [21, 71],
+ [26, 47],
+ [26, 62],
+ [26, 63],
+ [26, 61],
+ [26, 71],
+ [47, 71],
+ [7, 16],
+ [7, 22],
+ [7, 27],
+ [7, 32],
+ [7, 36],
+ [7, 40],
+ [7, 44],
+ [7, 48],
+ [7, 51],
+ [7, 53],
+ [7, 55],
+ [7, 56],
+ [7, 58],
+ [7, 60],
+ [7, 61],
+ [7, 65],
+ [7, 71],
+ [16, 48],
+ [16, 51],
+ [16, 53],
+ [16, 55],
+ [16, 71],
+ [22, 48],
+ [22, 56],
+ [22, 58],
+ [22, 60],
+ [22, 71],
+ [48, 71],
+ [8, 27],
+ [8, 33],
+ [8, 37],
+ [8, 17],
+ [8, 23],
+ [8, 45],
+ [8, 41],
+ [8, 51],
+ [8, 56],
+ [8, 61],
+ [8, 66],
+ [8, 68],
+ [8, 59],
+ [8, 69],
+ [8, 54],
+ [8, 49],
+ [8, 71],
+ [27, 51],
+ [27, 56],
+ [27, 61],
+ [27, 71],
+ [33, 66],
+ [33, 51],
+ [33, 68],
+ [33, 59],
+ [33, 71],
+ [37, 66],
+ [37, 56],
+ [37, 69],
+ [37, 54],
+ [37, 71],
+ [66, 71],
+ [9, 17],
+ [9, 28],
+ [9, 32],
+ [9, 42],
+ [9, 46],
+ [9, 24],
+ [9, 38],
+ [9, 51],
+ [9, 49],
+ [9, 54],
+ [9, 62],
+ [9, 64],
+ [9, 57],
+ [9, 58],
+ [9, 65],
+ [9, 70],
+ [9, 71],
+ [17, 51],
+ [17, 49],
+ [17, 54],
+ [17, 71],
+ [28, 51],
+ [28, 62],
+ [28, 64],
+ [28, 57],
+ [28, 71],
+ [32, 51],
+ [32, 58],
+ [32, 65],
+ [32, 71],
+ [51, 71],
+ [42, 62],
+ [42, 70],
+ [42, 58],
+ [42, 54],
+ [42, 71],
+ [62, 71],
+ [10, 23],
+ [10, 29],
+ [10, 36],
+ [10, 43],
+ [10, 46],
+ [10, 18],
+ [10, 34],
+ [10, 56],
+ [10, 49],
+ [10, 59],
+ [10, 63],
+ [10, 64],
+ [10, 52],
+ [10, 53],
+ [10, 65],
+ [10, 70],
+ [10, 71],
+ [23, 56],
+ [23, 49],
+ [23, 59],
+ [23, 71],
+ [29, 56],
+ [29, 63],
+ [29, 64],
+ [29, 52],
+ [29, 71],
+ [36, 56],
+ [36, 53],
+ [36, 65],
+ [36, 71],
+ [56, 71],
+ [43, 63],
+ [43, 70],
+ [43, 53],
+ [43, 59],
+ [43, 71],
+ [63, 71],
+ [46, 64],
+ [46, 70],
+ [46, 49],
+ [46, 65],
+ [46, 71],
+ [64, 71],
+ [70, 71],
+ [11, 18],
+ [11, 24],
+ [11, 35],
+ [11, 39],
+ [11, 40],
+ [11, 45],
+ [11, 30],
+ [11, 53],
+ [11, 49],
+ [11, 52],
+ [11, 58],
+ [11, 57],
+ [11, 67],
+ [11, 68],
+ [11, 69],
+ [11, 61],
+ [11, 71],
+ [18, 53],
+ [18, 49],
+ [18, 52],
+ [18, 71],
+ [24, 58],
+ [24, 49],
+ [24, 57],
+ [24, 71],
+ [35, 67],
+ [35, 58],
+ [35, 68],
+ [35, 52],
+ [35, 71],
+ [39, 67],
+ [39, 53],
+ [39, 69],
+ [39, 57],
+ [39, 71],
+ [67, 71],
+ [40, 53],
+ [40, 58],
+ [40, 61],
+ [40, 71],
+ [53, 71],
+ [58, 71],
+ [45, 49],
+ [45, 68],
+ [45, 69],
+ [45, 61],
+ [45, 71],
+ [49, 71],
+ [68, 71],
+ [69, 71],
+ [12, 19],
+ [12, 25],
+ [12, 30],
+ [12, 34],
+ [12, 38],
+ [12, 41],
+ [12, 44],
+ [12, 50],
+ [12, 52],
+ [12, 54],
+ [12, 55],
+ [12, 57],
+ [12, 59],
+ [12, 60],
+ [12, 61],
+ [12, 65],
+ [12, 71],
+ [19, 50],
+ [19, 52],
+ [19, 54],
+ [19, 55],
+ [19, 71],
+ [25, 50],
+ [25, 57],
+ [25, 59],
+ [25, 60],
+ [25, 71],
+ [50, 71],
+ [30, 52],
+ [30, 57],
+ [30, 61],
+ [30, 71],
+ [34, 52],
+ [34, 59],
+ [34, 65],
+ [34, 71],
+ [52, 71],
+ [38, 57],
+ [38, 54],
+ [38, 65],
+ [38, 71],
+ [57, 71],
+ [41, 54],
+ [41, 59],
+ [41, 61],
+ [41, 71],
+ [54, 71],
+ [59, 71],
+ [44, 55],
+ [44, 60],
+ [44, 61],
+ [44, 65],
+ [44, 71],
+ [55, 71],
+ [60, 71],
+ [61, 71],
+ [65, 71]]
+
+A4_Igusa_n = lambda q, t: -q**11 - 2*q**10*(4*t - 5) + t**11 - (9*t**3 + 6*t**2 - 50*t + 35)*q**9 - (4*t**6 + 12*t**4 - 50*t**3 - 15*t**2 + 100*t - 50)*q**8 - (12*t**7 - 25*t**6 - 6*t**5 - 30*t**4 + 95*t**3 - 70*t + 24)*q**7 - (6*t**9 - 16*t**8 - 30*t**7 + 50*t**6 + 35*t**5 - 70*t**3 + 15*t**2 + 12*t)*q**6 + (12*t**10 + 15*t**9 - 70*t**8 + 35*t**6 + 50*t**5 - 30*t**4 - 16*t**3 + 6*t**2)*q**5 + (24*t**11 - 70*t**10 + 95*t**8 - 30*t**7 - 6*t**6 - 25*t**5 + 12*t**4)*q**4 - (50*t**11 - 100*t**10 + 15*t**9 + 50*t**8 - 12*t**7 - 4*t**5)*q**3 + (35*t**11 - 50*t**10 + 6*t**9 + 9*t**8)*q**2 - 2*(5*t**11 - 4*t**10)*q
+
+A4_Igusa_d = lambda q, t: (t**10 - q**4)*(t**6 - q**3)*(t**3 - q**2)*(q - t)**2
+
+A5_Igusa_n = lambda q, t: 90*q**7*t**23 - 120*q**5*t**25 - 60*q**9*t**20 + 120*q**8*t**21 - 64*q**7*t**22 - 363*q**6*t**23 + 288*q**5*t**24 + 274*q**4*t**25 + 10*q**12*t**16 - 120*q**10*t**18 + 128*q**9*t**19 + 66*q**8*t**20 - 636*q**7*t**21 + 492*q**6*t**22 + 345*q**5*t**23 - 600*q**4*t**24 - 225*q**3*t**25 - 99*q**11*t**16 + 147*q**10*t**17 + 498*q**9*t**18 - 546*q**8*t**19 + 450*q**7*t**20 + 720*q**6*t**21 - 850*q**5*t**22 - 15*q**4*t**23 + 420*q**3*t**24 + 85*q**2*t**25 + 30*q**13*t**13 - 60*q**12*t**14 - 60*q**11*t**15 + 449*q**10*t**16 - 717*q**9*t**17 - 633*q**8*t**18 + 871*q**7*t**19 - 750*q**6*t**20 - 120*q**5*t**21 + 570*q**4*t**22 - 75*q**3*t**23 - 120*q**2*t**24 - 15*q*t**25 + 5*q**15*t**10 + 30*q**14*t**11 - 30*q**13*t**12 - 158*q**12*t**13 + 504*q**11*t**14 - 54*q**10*t**15 - 987*q**9*t**16 + 1275*q**8*t**17 + 105*q**7*t**18 - 765*q**6*t**19 + 330*q**5*t**20 - 120*q**4*t**21 - 166*q**3*t**22 + 18*q**2*t**23 + 12*q*t**24 + t**25 - 51*q**14*t**10 - 162*q**13*t**11 + 261*q**12*t**12 + 174*q**11*t**13 - 1128*q**10*t**14 + 846*q**9*t**15 + 965*q**8*t**16 - 1035*q**7*t**17 + 345*q**6*t**18 + 427*q**5*t**19 - 36*q**4*t**20 + 36*q**3*t**21 + 18*q**2*t**22 + 12*q**14*t**9 + 89*q**13*t**10 + 186*q**12*t**11 - 557*q**11*t**12 + 25*q**10*t**13 + 720*q**9*t**14 - 1120*q**8*t**15 - 366*q**7*t**16 + 378*q**6*t**17 - 243*q**5*t**18 - 129*q**4*t**19 + 14*q**16*t**6 + 48*q**15*t**7 - 48*q**14*t**8 + 16*q**13*t**9 + 345*q**12*t**10 - 90*q**11*t**11 + 255*q**10*t**12 + 255*q**9*t**13 - 90*q**8*t**14 + 345*q**7*t**15 + 16*q**6*t**16 - 48*q**5*t**17 + 48*q**4*t**18 + 14*q**3*t**19 - 129*q**15*t**6 - 243*q**14*t**7 + 378*q**13*t**8 - 366*q**12*t**9 - 1120*q**11*t**10 + 720*q**10*t**11 + 25*q**9*t**12 - 557*q**8*t**13 + 186*q**7*t**14 + 89*q**6*t**15 + 12*q**5*t**16 + 18*q**17*t**3 + 36*q**16*t**4 - 36*q**15*t**5 + 427*q**14*t**6 + 345*q**13*t**7 - 1035*q**12*t**8 + 965*q**11*t**9 + 846*q**10*t**10 - 1128*q**9*t**11 + 174*q**8*t**12 + 261*q**7*t**13 - 162*q**6*t**14 - 51*q**5*t**15 + q**19 + 12*q**18*t + 18*q**17*t**2 - 166*q**16*t**3 - 120*q**15*t**4 + 330*q**14*t**5 - 765*q**13*t**6 + 105*q**12*t**7 + 1275*q**11*t**8 - 987*q**10*t**9 - 54*q**9*t**10 + 504*q**8*t**11 - 158*q**7*t**12 - 30*q**6*t**13 + 30*q**5*t**14 + 5*q**4*t**15 - 15*q**18 - 120*q**17*t - 75*q**16*t**2 + 570*q**15*t**3 - 120*q**14*t**4 - 750*q**13*t**5 + 871*q**12*t**6 - 633*q**11*t**7 - 717*q**10*t**8 + 449*q**9*t**9 - 60*q**8*t**10 - 60*q**7*t**11 + 30*q**6*t**12 + 85*q**17 + 420*q**16*t - 15*q**15*t**2 - 850*q**14*t**3 + 720*q**13*t**4 + 450*q**12*t**5 - 546*q**11*t**6 + 498*q**10*t**7 + 147*q**9*t**8 - 99*q**8*t**9 - 225*q**16 - 600*q**15*t + 345*q**14*t**2 + 492*q**13*t**3 - 636*q**12*t**4 + 66*q**11*t**5 + 128*q**10*t**6 - 120*q**9*t**7 + 10*q**7*t**9 + 274*q**15 + 288*q**14*t - 363*q**13*t**2 - 64*q**12*t**3 + 120*q**11*t**4 - 60*q**10*t**5 - 120*q**14 + 90*q**12*t**2
+
+A5_Igusa_d = lambda q, t: -(t**15 - q**5)*(t**10 - q**4)*(t**6 - q**3)*(t**3 - q**2)**2*(q - t)**3
+
+B3_Igusa_n = lambda q, t: 6*q**5*t**7 + 3*q**4*t**8 - 15*q**3*t**9 - 2*q**7*t**4 + q**6*t**5 + 7*q**5*t**6 - 22*q**4*t**7 + 17*q**3*t**8 + 23*q**2*t**9 - 3*q**7*t**3 + 9*q**6*t**4 - 15*q**5*t**5 - 3*q**4*t**6 + 18*q**3*t**7 - 27*q**2*t**8 - 9*q*t**9 - q**9 - 7*q**8*t + 2*q**7*t**2 + 7*q**6*t**3 - 21*q**5*t**4 + 21*q**4*t**5 - 7*q**3*t**6 - 2*q**2*t**7 + 7*q*t**8 + t**9 + 9*q**8 + 27*q**7*t - 18*q**6*t**2 + 3*q**5*t**3 + 15*q**4*t**4 - 9*q**3*t**5 + 3*q**2*t**6 - 23*q**7 - 17*q**6*t + 22*q**5*t**2 - 7*q**4*t**3 - q**3*t**4 + 2*q**2*t**5 + 15*q**6 - 3*q**5*t - 6*q**4*t**2
+
+B3_Igusa_d = lambda q, t: (t**9 - q**3)*(t**4 - q**2)*(t**3 - q**2)*(q - t)**2
+
```

### Comparing `hypigu-1.3/hypigu.egg-info/PKG-INFO` & `hypigu-1.4/hypigu.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypigu
-Version: 1.3
+Version: 1.4
 Summary: A SageMath package that provides functions to compute the Igusa local zeta function associated with hyperplane arrangements.
 Home-page: https://joshmaglione.github.io/hypigu/
 Author: Joshua Maglione
 Author-email: joshmaglione@gmail.com
 Project-URL: Bug Tracker, https://github.com/joshmaglione/hypigu/issues
 Keywords: SageMath,hyperplane arrangements,Igusa zeta functions,topological zeta functions,Flag Hilbert--Poincare series
 Classifier: Programming Language :: Python :: 3
@@ -49,15 +49,15 @@
 
 ## Funding 
 
 This package was funded in part by DFG grant [373111162](https://gepris.dfg.de/gepris/projekt/373111162?language=en).
 
 ## Copyright & License
 
-Copyright 2021&ndash;2022 Joshua Maglione.
+Copyright 2020&ndash;2023 Joshua Maglione.
 
 HypIgu is distributed with the MIT License.
 
 ## References 
 
-1. [Joshua Maglione](https://joshmaglione.com/) and [Christopher Voll](https://www.math.uni-bielefeld.de/~voll/). Flag Hilbert&ndash;Poincar&#233; series of hyperplane arrangements and their Igusa zeta functions, 2021. [arXiv:2103:03640](https://arxiv.org/abs/2103.03640).
+1. [Joshua Maglione](https://joshmaglione.com/) and [Christopher Voll](https://www.math.uni-bielefeld.de/~voll/). Flag Hilbert&ndash;Poincar&#233; series of hyperplane arrangements and Igusa zeta functions, 2021. [arXiv:2103:03640](https://arxiv.org/abs/2103.03640).
```

### Comparing `hypigu-1.3/setup.cfg` & `hypigu-1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 7970 6967 750d 0a76 6572 7369   = hypigu..versi
-00000020: 6f6e 203d 2031 2e33 0d0a 6175 7468 6f72  on = 1.3..author
+00000020: 6f6e 203d 2031 2e34 0d0a 6175 7468 6f72  on = 1.4..author
 00000030: 203d 204a 6f73 6875 6120 4d61 676c 696f   = Joshua Maglio
 00000040: 6e65 0d0a 6175 7468 6f72 5f65 6d61 696c  ne..author_email
 00000050: 203d 206a 6f73 686d 6167 6c69 6f6e 6540   = joshmaglione@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2041 2053 6167 654d  iption = A SageM
 00000080: 6174 6820 7061 636b 6167 6520 7468 6174  ath package that
 00000090: 2070 726f 7669 6465 7320 6675 6e63 7469   provides functi
```

