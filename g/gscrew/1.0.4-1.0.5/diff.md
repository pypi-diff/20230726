# Comparing `tmp/gscrew-1.0.4.tar.gz` & `tmp/gscrew-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gscrew-1.0.4.tar", last modified: Tue Jul 25 22:56:18 2023, max compression
+gzip compressed data, was "gscrew-1.0.5.tar", last modified: Wed Jul 26 15:24:32 2023, max compression
```

## Comparing `gscrew-1.0.4.tar` & `gscrew-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:56:18.599240 gscrew-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 22:56:07.000000 gscrew-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-25 22:56:18.599240 gscrew-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-25 22:56:07.000000 gscrew-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:56:18.599240 gscrew-1.0.4/gscrew/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 22:56:07.000000 gscrew-1.0.4/gscrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21562 2023-07-25 22:56:07.000000 gscrew-1.0.4/gscrew/geometric_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-25 22:56:07.000000 gscrew-1.0.4/gscrew/screw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:56:18.599240 gscrew-1.0.4/gscrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-25 22:56:18.000000 gscrew-1.0.4/gscrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-25 22:56:18.000000 gscrew-1.0.4/gscrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 22:56:18.000000 gscrew-1.0.4/gscrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 22:56:18.000000 gscrew-1.0.4/gscrew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 22:56:18.000000 gscrew-1.0.4/gscrew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-25 22:56:07.000000 gscrew-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 22:56:07.000000 gscrew-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 22:56:18.599240 gscrew-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 22:56:07.000000 gscrew-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:24:32.445619 gscrew-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 15:24:22.000000 gscrew-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-26 15:24:32.445619 gscrew-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-26 15:24:22.000000 gscrew-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:24:32.445619 gscrew-1.0.5/gscrew/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 15:24:22.000000 gscrew-1.0.5/gscrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22515 2023-07-26 15:24:22.000000 gscrew-1.0.5/gscrew/geometric_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-07-26 15:24:22.000000 gscrew-1.0.5/gscrew/screw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:24:32.445619 gscrew-1.0.5/gscrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-26 15:24:32.000000 gscrew-1.0.5/gscrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-26 15:24:32.000000 gscrew-1.0.5/gscrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:24:32.000000 gscrew-1.0.5/gscrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 15:24:32.000000 gscrew-1.0.5/gscrew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 15:24:32.000000 gscrew-1.0.5/gscrew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-26 15:24:22.000000 gscrew-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 15:24:22.000000 gscrew-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:24:32.445619 gscrew-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 15:24:22.000000 gscrew-1.0.5/setup.py
```

### Comparing `gscrew-1.0.4/LICENSE` & `gscrew-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gscrew-1.0.4/PKG-INFO` & `gscrew-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscrew
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
 Author: Antoine Royer, Loris Delafosse
 Project-URL: Homepage, https://github.com/Shadow15510/GScrew
 Project-URL: Documentation, http://gscrew.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gscrew-1.0.4/README.md` & `gscrew-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gscrew-1.0.4/gscrew/geometric_algebra.py` & `gscrew-1.0.5/gscrew/geometric_algebra.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,19 +51,16 @@
             dimensional one. 
         """
         self.dim = dim
         self.nb_blades = 2 ** dim
 
         self.blades_by_grade = [binomial_coefficient(dim, i) for i in range(dim + 1)]
 
-        ids = []
-        for i in range(self.nb_blades):
-            ids.append((to_array(i, dim), i.bit_count(), i))
-
-        self.blades_ids = [i[0] for i in sorted(ids, key=lambda x: x[1])]
+        ids = list(range(self.nb_blades))
+        self.blades_ids = sorted(ids, key=lambda elmnt: elmnt.bit_count())
 
         self.blades = {}
         self.__generate_blades()
 
     def __repr__(self):
         """Returns the string representation of the geometric algebra.
 
@@ -124,15 +121,15 @@
         """
         first_index = sum(self.blades_by_grade[:grade])
         last_index = first_index + self.blades_by_grade[grade]
         return first_index, last_index - 1
 
 
 class MultiVector:
-    """An element of the geometric algebra.
+    r"""An element of the geometric algebra.
 
     The following operators have been overloaded:
 
     * the addition
       ``self + other``
 
     * the substraction
@@ -143,28 +140,53 @@
 
     * the outer product
       ``self ^ other``
 
     * the inner product
       ``self | other``
 
+    * the scalar division
+      ``self / scalar``
+
+    Some others manipulations are available:
+
+    * the projection on grade k
+      ``my_multivector(k)``
+    
+    * the norm
+      ``abs(my_multivector)``
+
+    * the inversion
+      ``my_multivector.inverse()``
+
+    * the reversion :math:`A^{\dagger}`
+      ``~my_multivector``
+
+    * the dual calculation
+      ``my_multivector.dual()``
+
+    * the grade involution
+      ``my_multivector.grade_involution()``
+
     Attributes
     ----------
     geo_alg : GeometricAlgebra
         The geometric algebra to which the multivector belongs.
     value : np.array
         The coefficients on each basis blade.
 
     Methods
     -------
     .. automethod:: __init__
     .. automethod:: __call__
     .. automethod:: __getitem__
-    .. automethod:: norm
+    .. automethod:: copy
+    .. automethod:: dual
     .. automethod:: grade_involution
+    .. automethod:: inverse
 
     Exemples
     --------
     Let's show you a complete exemple of a manipulation of MultiVector.
     You must start by importing the module::
 
         >>> import geometric_algebra as ga
@@ -206,16 +228,31 @@
             if isinstance(value, (int, float)):
                 new_value = np.zeros(geo_alg.nb_blades)
                 new_value[0] = value
             else:
                 new_value = np.array(value)
             self.value = new_value
 
+        self.precision = 5
+
+    def __abs__(self):
+        """Computes the norm of the multivector.
+
+        Returns
+        -------
+        out : float
+            The norm of the multivector"""
+        result = 0
+        for component in self.value:
+            result += abs(component ** 2)
+
+        return math.sqrt(result)
+
     def __add__(self, other):
-        """Compute the addition ``self + other``.
+        """Computes the addition ``self + other``.
 
         Parameters
         ----------
         other : MultiVector, scalar
             The MultiVector or scalar to add up.
 
         Returns
@@ -225,29 +262,29 @@
 
         Raises
         ------
         TypeError
             If ``other`` is neither a scalar nor a MultiVector instance.
         """
         new_value = self.value.copy()
-        if isinstance(other, (int, float)):
+        if np.isscalar(other):
             new_value[0] += other
 
         elif isinstance(other, MultiVector):
             new_value += other.value
 
         else:
             raise TypeError(f"other must be a scalar or a MultiVector instance instead of "\
                     f"{type(other)}"
                 )
 
         return MultiVector(self.geo_alg, new_value)
 
     def __call__(self, *grades):
-        """Project the multivector on the basis blades of given grades.
+        """Projects the multivector on the basis blades of given grades.
 
         Parameters
         ----------
         *grades
             The grades on which the multivector will be project.
 
         Returns
@@ -272,28 +309,28 @@
         for grade in grades:
             first_index, last_index = self.geo_alg.get_grade(grade)
             for index in range(first_index, last_index + 1):
                 new_value[index] = self.value[index]
         return MultiVector(self.geo_alg, new_value)
 
     def __eq__(self, other):
-        """Test the equality between two multivectors.
+        """Tests the equality between two multivectors.
 
         Parameters
         ----------
         other : MultiVector
             The other multivector.
 
         Returns
         -------
         out : bool
             This method will return ``True`` if all the components of the two multivectors are
             equals. 
         """
-        if isinstance(other, (int, float)):
+        if np.isscalar(other):
             return self[0] == other
         return (self.value == other.value).all()
 
     def __getitem__(self, index: int):
         """Returns the component at the given index.
 
         Parameters
@@ -304,16 +341,30 @@
         Returns
         -------
         out : float
             The desired component.
         """
         return self.value[index]
 
+    def __invert__(self):
+        """Computes the reversion of the multivector ``~self``.
+
+        Returns
+        -------
+        new_mv : MultiVector
+            The result of the reversion
+        """
+        new_mv = MultiVector(self.geo_alg)
+        for k in range(self.geo_alg.dim + 1):
+            new_mv += (-1) ** ((k**2 - k)/2) * self(k)
+
+        return new_mv
+
     def __mul__(self, other):
-        """Compute the geometrical product ``self * other``.
+        """Computes the geometrical product ``self * other``.
 
         Parameters
         ----------
         other : MultiVector, scalar
             The MultiVector or scalar to multiply.
 
         Returns
@@ -322,15 +373,15 @@
             The result of the geometrical product.
 
         Raises
         ------
         TypeError
             If ``other`` is neither a scalar nor a MultiVector instance.
         """
-        if isinstance(other, (int, float)):
+        if np.isscalar(other):
             return MultiVector(self.geo_alg, self.value * other)
 
         if not isinstance(other, MultiVector):
             raise TypeError(f"other must be a scalar or a MultiVector instance instead of "\
                     f"{type(other)}"
                 )
 
@@ -360,27 +411,33 @@
         Parameters
         ----------
         other : MultiVector
             The other MultiVector.
 
         Returns
         -------
-        out : MultiVector
+        new_mv : MultiVector
             The result of the inner product.
 
         Raises
         ------
         TypeError
             If ``other`` isn't a MultiVector instance.
         """
         if not isinstance(other, MultiVector):
             raise TypeError(f"other must be a scalar or a MultiVector instance instead of "\
                     f"{type(other)}"
                 )
-        return sum(self.value * other.value)
+
+        new_mv = MultiVector(self.geo_alg)
+        for gd1 in range(1, self.geo_alg.dim + 1):
+            for gd2 in range(1, self.geo_alg.dim + 1):
+                new_mv += (self(gd1) * other(gd2))(abs(gd2 - gd1))
+
+        return new_mv
 
     __radd__ = __add__
 
     def __repr__(self):
         """Returns the string representation of the MultiVector.
 
         Returns
@@ -419,15 +476,15 @@
             The result of the geometrical product.
 
         Raises
         ------
         TypeError
             If ``other`` is neither a scalar nor a MultiVector instance.
         """
-        if isinstance(other, (int, float)):
+        if np.isscalar(other):
             return MultiVector(self.geo_alg, other * self.value)
 
         if not isinstance(other, MultiVector):
             raise TypeError(f"other must be a scalar or a MultiVector instance instead of "\
                     f"{type(other)}"
                 )
 
@@ -456,15 +513,15 @@
 
         Raises
         ------
         TypeError
             If ``other`` is neither a scalar nor a MultiVector instance.
         """
         new_value = np.zeros(self.geo_alg.nb_blades)
-        if isinstance(other, (int, float)):
+        if np.isscalar(other):
             new_value[0] = other - self.value[0]
             new_value[1:] -= self.value[1:]
 
         elif isinstance(other, MultiVector):
             new_value = other.value.copy()
             new_value -= self.value
 
@@ -489,15 +546,15 @@
             The result of the outer product.
 
         Raises
         ------
         TypeError
             If ``other`` is neither a scalar nor a MultiVector instance.
         """
-        if isinstance(other, (int, float)):
+        if np.isscalar(other):
             return other * self
 
         if not isinstance(other, MultiVector):
             raise TypeError(f"other must be a scalar or a MultiVector instance instead of "\
                     f"{type(other)}"
                 )
 
@@ -522,27 +579,56 @@
 
         Raises
         ------
         TypeError
             If ``other`` is neither a scalar nor a MultiVector instance.
         """
         new_value = self.value.copy()
-        if isinstance(other, (int, float)):
+        if np.isscalar(other):
             new_value[0] -= other
 
         elif isinstance(other, MultiVector):
             new_value -= other.value
 
         else:
             raise TypeError(f"other must be a scalar or a MultiVector instance instead of "\
                     f"{type(other)}"
                 )
 
         return MultiVector(self.geo_alg, new_value)
 
+    def __truediv__(self, other):
+        """Compute the division ``self / other``.
+
+        Parameters
+        ----------
+        other : MultiVector, scalar
+            The MultiVector or scalar to divide.
+
+        Returns
+        -------
+        out : MultiVector
+            The result of the division.
+
+        Raises
+        ------
+        TypeError
+            If ``other`` is neither a scalar nor a MultiVector instance.
+        """
+        if np.isscalar(other):
+            new_value = self.value / other
+            return MultiVector(self.geo_alg, new_value)
+
+        if not isinstance(other, MultiVector):
+            raise TypeError(f"other must be a scalar or a MultiVector instance instead of "\
+                    f"{type(other)}"
+                )
+
+        return MultiVector(self.geo_alg)
+
     def __xor__(self, other):
         """Compute the outer product ``self ^ other``.
 
         Parameters
         ----------
         other : MultiVector, scalar
             The MultiVector or scalar to multiply.
@@ -553,15 +639,15 @@
             The result of the outer product.
 
         Raises
         ------
         TypeError
             If ``other`` is neither a scalar nor a MultiVector instance.
         """
-        if isinstance(other, (int, float)):
+        if np.isscalar(other):
             return self * other
 
         if not isinstance(other, MultiVector):
             raise TypeError(f"other must be a scalar or a MultiVector instance instead of "\
                     f"{type(other)}"
                 )
 
@@ -581,59 +667,96 @@
 
         Returns
         -------
         out : tuple
             A tuple of the form: ``(index, sign)`` where ``index`` is the index of the
             resulting basis blade and ``sign`` the sign of the result.
         """
-        array = [
-                i^j for i, j in
-                zip(self.geo_alg.blades_ids[index1], self.geo_alg.blades_ids[index2])
-            ]
-
-        new_index = self.geo_alg.blades_ids.index(array)
-        sign = get_sign(self.geo_alg.blades_ids[index1], self.geo_alg.blades_ids[index2])
-        return new_index, sign
+        new_index = self.geo_alg.blades_ids[index1] ^ self.geo_alg.blades_ids[index2]
+        sign = self.__get_sign(self.geo_alg.blades_ids[index1], self.geo_alg.blades_ids[index2])
+        return self.geo_alg.blades_ids[new_index], sign
+
+    def __get_sign(self, index1: int, index2: int):
+        """Calculate the sign of the geometric product between the given basis blades.
+
+        Parameters
+        ----------
+        index1 : int
+            The index of the first basis blade.
+        index2 : int
+            The index of the second basis blade.
+
+        Returns
+        -------
+        out : int
+            The sign of the geometric product between the two basis blades.
+        """
+        index1 //= 2
+        n_swap = 0
+        while index1:
+            n_swap += (index1 & index2).bit_count()
+            index1 //= 2
+        n_swap += 1
+        return 2 * (n_swap % 2) - 1
+
 
     def copy(self):
         """Create a deep copy of the instance.
 
         Returns
         -------
         out : MultiVector
             The copy of the instance.
         """
         return MultiVector(self.geo_alg, self.value.copy())
 
-    def norm(self):
-        """Compute the norm of the multivector.
-
-        Returns
-        -------
-        out : float
-            The norm of the multivector"""
-        result = 0
-        for component in self.value:
-            result += abs(component ** 2)
-
-        return math.sqrt(result)
-
     def grade_involution(self):
         """Compute the grade involution of the multivector.
 
         Returns
         -------
         new_mv : MultiVector
             The result of the grade involution.
         """
         new_mv = MultiVector(self.geo_alg)
         for i in range(self.geo_alg.dim + 1):
             new_mv += (-1)**i * self(i)
         return new_mv
 
+    def inverse(self):
+        """Compute the inverse of a given multivector.
+
+        Returns
+        -------
+        out : MultiVector
+            The inverted multivector.
+        """
+        system = np.zeros((self.geo_alg.nb_blades, self.geo_alg.nb_blades))
+        for i in range(self.geo_alg.nb_blades):
+            column = (self * tuple(self.geo_alg.blades.values())[i]).value
+            for j in range(self.geo_alg.nb_blades):
+                if column[j] > 1e-10 or column[j] < -1e-10:
+                    system[j, i] = column[j]
+
+        new_value = list(map(
+                lambda x: round(x, self.precision),
+                np.linalg.solve(system, tuple(self.geo_alg.blades.values())[0].value)
+            ))
+        return MultiVector(self.geo_alg, new_value)
+
+    def dual(self):
+        """Compute the dual multivector.
+
+        Returns
+        -------
+        out : MultiVector
+            The dual.
+        """
+        return self * tuple(self.geo_alg.blades.values())[-1].inverse()
+
 
 def binomial_coefficient(n: int, k: int):
     """Compute the binomial coefficient nCk.
     
     Parameters
     ----------
     n : int
@@ -653,99 +776,7 @@
     k = min(k, n - k)
 
     coeff = 1
     for i in range(k):
         coeff = coeff * (n - i) // (i + 1)
 
     return coeff
-
-def to_array(integer: int, nb_bit: int):
-    """Convert an integer into an array of bits.
-
-    Parameters
-    ----------
-    integer : int
-        The integer to convert into an array.
-    nb_bit : int
-        The number of bits over which to express ``integer``.
-
-    Returns
-    -------
-    array : np.array
-        The array of bits.
-
-    Raises
-    ------
-    ValueError
-        If the integer can't be expressed on ``nb_bit`` bits.
-
-    Exemples
-    --------
-    For exemple, the decimal number 5 is expressed as 101 in base 2, if we want to have an array of
-    4 bits, the function will return ``np.array([0, 1, 0, 1])``::
-
-        >>> to_array(5, 4)
-        array([0, 1, 0, 1])
-        >>> to_array(7, 3)
-        array([1, 1, 1])
-    """
-    if integer >= 2 ** nb_bit:
-        raise ValueError(f"{integer} can't be expressed on {nb_bit} bits")
-
-    array = list(map(int, bin(integer)[2:]))
-    while len(array) < nb_bit:
-        array.insert(0, 0)
-    return array
-
-
-def get_index(array_like, search_element: np.array):
-    """Search the index of ``search_element`` into ``array_like``.
-
-    Parameters
-    ----------
-    array_like
-        A list or a tuple of NumPy arrays.
-    search_element : np.array
-        The researched array
-
-    Returns
-    -------
-    index : int
-        The index of ``search_element`` in ``array_like``.
-
-    Raises
-    ------
-    ValueError
-        If ``search_element`` is not in ``array_like``.
-    """
-    return np.where(search_element == array_like)
-
-    # for index, value in enumerate(array_like):
-    #     if (value == search_element).all():
-    #         return index
-    # raise ValueError(f"{rslt} not in {array_like.__class__.__name__}")
-
-
-def get_sign(array1: np.array, array2: np.array):
-    """Calculate the sign of the geometric product between the given basis blades.
-
-    Parameters
-    ----------
-    array1 : np.array
-        The array form of the first basis blade.
-    array2 : np.array
-        The array form of the second basis blade.
-
-    Returns
-    -------
-    out : int
-        The sign of the geometric product between the two basis blades.
-    """    
-    id1 = int("0b" + "".join(map(str, array1)), 2) // 2
-    id2 = int("0b" + "".join(map(str, array2)), 2)
-
-    n_swap = 0
-    while id1:
-        n_swap += (id1 & id2).bit_count()
-        id1 //= 2
-    n_swap += 1
-    return 2 * (n_swap % 2) - 1
```

### Comparing `gscrew-1.0.4/gscrew/screw.py` & `gscrew-1.0.5/gscrew/screw.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,16 +48,14 @@
 
     Methods
     -------
     .. automethod:: __init__
     .. automethod:: change_point
     .. automethod:: show
     """
-    classname = "ScrewBase"
-
     def __init__(self, ref_point, direction, moment):
         """Constructor method.
 
         Parameters
         ----------
         ref_point : MultiVector
             The point of reference of the (co)screw
@@ -82,35 +80,44 @@
         """Allow to display the (co)Screw at its reference point.
 
         Returns
         -------
         out : str
             The string representation of the (co)Screw.
         """
-        return f"{self.classname}(\n\tdirection={self.direction}\n\tmoment={self.moment}\n)"
+        name = self.__class__.__name__
+        return f"{name}(\n\tdirection={self.direction}\n\tmoment={self.moment}\n)"
 
     def change_point(self, new_point):
-        """Computes and returns the (co)screw on the new reference point.
+        """Computes and returns the (co)screw on the new reference point. The formula changes
+        according to the type of screw.
 
         Parameters
         ----------
         new_point : MultiVector
             The new point.
 
         Returns
         -------
-        out : (co)Screw
-            The (co)screw on ``new_point``.
+        out : (Co)Screw
+            The screw on ``new_point``.
         """
+        new_moment = self.moment
+        if self.__class__.__name__ == "Screw":
+            new_moment = self.moment - ((new_point - self.ref_point) ^ self.direction)
+        elif self.__class__.__name__ == "CoScrew":
+            new_moment = self.moment - (self.direction | (new_point - self.ref_point))
+
         return self.__class__(
                 new_point,
                 self.direction,
-                self.moment - ((new_point - self.ref_point) ^ self.direction)
+                new_moment
             )
 
+
     def show(self, new_point=None):
         """Print the (co)screw on a given point.
 
         Parameters
         ----------
         new_point : MultiVector, optionnal
             The point on which the (co)screw should be shown. If no point was given, it shows the
@@ -132,20 +139,22 @@
 
     * the right-handed addition
       ``other + self``
 
     * the outer product of screws
       ``self ^ other``
 
+    Methods
+    -------
+    .. automethod:: change_point
+
     See also
     --------
     This class inherits from the ScrewBase one.
     """
-    classname = "Screw"
-
     def __add__(self, other):
         """The addition ``self + other``.
 
         Parameters
         ----------
         other : Screw
             The screw to be add up.
@@ -215,21 +224,23 @@
       ``self + other``
 
     * the right-handed addition
       ``other + self``
 
     * the product between a scalar and a coscrew
       ``scalar * self``
+    
+    Methods
+    -------
+    .. automethod:: change_point
 
     See also
     --------
     This class inherits from the ScrewBase one.
     """
-    classname = "CoScrew"
-
     def __add__(self, other):
         """The addition ``self + other``.
 
         Parameters
         ----------
         other : CoScrew
             The coscrew to be add up.
@@ -278,14 +289,15 @@
 
         return CoScrew(
                 self.ref_point,
                 scalar * self.direction,
                 scalar * self.moment
             )
 
+
 def comoment(coscrew: CoScrew, screw: Screw):
     """Compute the comoment between a coscrew and a screw.
 
     Parameters
     ----------
     coscrew : CoScrew
         The coscrew.
@@ -293,9 +305,9 @@
         The screw.
 
     Returns
     -------
     out : MultiVector
         The comoment between the given coscrew and the screw.
     """
-    return (-coscrew.direction.grade_involution() * screw.moment.grade_involution()
-            + screw.direction * coscrew.moment)(0)
+    return ((-coscrew.direction.grade_involution() * screw.moment.grade_involution())(0)
+            + (screw.direction * coscrew.moment)(0))
```

### Comparing `gscrew-1.0.4/gscrew.egg-info/PKG-INFO` & `gscrew-1.0.5/gscrew.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscrew
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python module to manipulate Screws and Coscrews with geometrics algebra (Clifford's Algebra).
 Author: Antoine Royer, Loris Delafosse
 Project-URL: Homepage, https://github.com/Shadow15510/GScrew
 Project-URL: Documentation, http://gscrew.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gscrew-1.0.4/pyproject.toml` & `gscrew-1.0.5/pyproject.toml`

 * *Files identical despite different names*

