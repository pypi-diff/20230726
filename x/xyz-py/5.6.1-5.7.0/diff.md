# Comparing `tmp/xyz_py-5.6.1.tar.gz` & `tmp/xyz_py-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyz_py-5.6.1.tar", last modified: Thu May 25 14:01:44 2023, max compression
+gzip compressed data, was "xyz_py-5.7.0.tar", last modified: Wed Jul 26 10:24:18 2023, max compression
```

## Comparing `xyz_py-5.6.1.tar` & `xyz_py-5.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:01:44.319617 xyz_py-5.6.1/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2023-05-25 14:01:25.000000 xyz_py-5.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1303 2023-05-25 14:01:44.318617 xyz_py-5.6.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-05-25 14:01:25.000000 xyz_py-5.6.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-25 14:01:25.000000 xyz_py-5.6.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 14:01:44.319617 xyz_py-5.6.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-05-25 14:01:41.000000 xyz_py-5.6.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:01:44.317617 xyz_py-5.6.1/xyz_py/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-05-25 14:01:25.000000 xyz_py-5.6.1/xyz_py/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7424 2023-05-25 14:01:25.000000 xyz_py-5.6.1/xyz_py/atomic.py
--rw-rw-rw-   0 root         (0) root         (0)    10677 2023-05-25 14:01:25.000000 xyz_py-5.6.1/xyz_py/cli.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-25 14:01:41.000000 xyz_py-5.6.1/xyz_py/version.py
--rw-rw-rw-   0 root         (0) root         (0)    38721 2023-05-25 14:01:25.000000 xyz_py-5.6.1/xyz_py/xyz_py.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:01:44.318617 xyz_py-5.6.1/xyz_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1303 2023-05-25 14:01:44.000000 xyz_py-5.6.1/xyz_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-05-25 14:01:44.000000 xyz_py-5.6.1/xyz_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 14:01:44.000000 xyz_py-5.6.1/xyz_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-25 14:01:44.000000 xyz_py-5.6.1/xyz_py.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-25 14:01:44.000000 xyz_py-5.6.1/xyz_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-25 14:01:44.000000 xyz_py-5.6.1/xyz_py.egg-info/top_level.txt
+drwxr-xr-x   0 jon       (1000) jon       (1000)        0 2023-07-26 10:24:18.907607 xyz_py-5.7.0/
+-rw-r--r--   0 jon       (1000) jon       (1000)    35072 2023-02-07 11:58:54.000000 xyz_py-5.7.0/LICENSE
+-rw-r--r--   0 jon       (1000) jon       (1000)     1303 2023-07-26 10:24:18.907607 xyz_py-5.7.0/PKG-INFO
+-rw-r--r--   0 jon       (1000) jon       (1000)      681 2023-02-07 11:58:54.000000 xyz_py-5.7.0/README.md
+-rw-r--r--   0 jon       (1000) jon       (1000)     1485 2023-07-26 10:17:09.000000 xyz_py-5.7.0/pyproject.toml
+-rw-r--r--   0 jon       (1000) jon       (1000)       38 2023-07-26 10:24:18.907607 xyz_py-5.7.0/setup.cfg
+-rw-r--r--   0 jon       (1000) jon       (1000)     1112 2023-07-26 10:24:07.000000 xyz_py-5.7.0/setup.py
+drwxr-xr-x   0 jon       (1000) jon       (1000)        0 2023-07-26 10:24:18.907607 xyz_py-5.7.0/xyz_py/
+-rw-r--r--   0 jon       (1000) jon       (1000)       84 2023-02-07 11:58:54.000000 xyz_py-5.7.0/xyz_py/__init__.py
+-rw-r--r--   0 jon       (1000) jon       (1000)     8117 2023-07-25 15:27:54.000000 xyz_py-5.7.0/xyz_py/atomic.py
+-rw-r--r--   0 jon       (1000) jon       (1000)    11013 2023-07-25 14:47:33.000000 xyz_py-5.7.0/xyz_py/cli.py
+-rw-r--r--   0 jon       (1000) jon       (1000)       22 2023-07-26 10:24:07.000000 xyz_py-5.7.0/xyz_py/version.py
+-rw-r--r--   0 jon       (1000) jon       (1000)    39512 2023-07-25 15:21:05.000000 xyz_py-5.7.0/xyz_py/xyz_py.py
+drwxr-xr-x   0 jon       (1000) jon       (1000)        0 2023-07-26 10:24:18.907607 xyz_py-5.7.0/xyz_py.egg-info/
+-rw-r--r--   0 jon       (1000) jon       (1000)     1303 2023-07-26 10:24:18.000000 xyz_py-5.7.0/xyz_py.egg-info/PKG-INFO
+-rw-r--r--   0 jon       (1000) jon       (1000)      308 2023-07-26 10:24:18.000000 xyz_py-5.7.0/xyz_py.egg-info/SOURCES.txt
+-rw-r--r--   0 jon       (1000) jon       (1000)        1 2023-07-26 10:24:18.000000 xyz_py-5.7.0/xyz_py.egg-info/dependency_links.txt
+-rw-r--r--   0 jon       (1000) jon       (1000)       43 2023-07-26 10:24:18.000000 xyz_py-5.7.0/xyz_py.egg-info/entry_points.txt
+-rw-r--r--   0 jon       (1000) jon       (1000)       28 2023-07-26 10:24:18.000000 xyz_py-5.7.0/xyz_py.egg-info/requires.txt
+-rw-r--r--   0 jon       (1000) jon       (1000)        7 2023-07-26 10:24:18.000000 xyz_py-5.7.0/xyz_py.egg-info/top_level.txt
```

### Comparing `xyz_py-5.6.1/LICENSE` & `xyz_py-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xyz_py-5.6.1/PKG-INFO` & `xyz_py-5.7.0/xyz_py.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xyz_py
-Version: 5.6.1
+Name: xyz-py
+Version: 5.7.0
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xyz_py-5.6.1/README.md` & `xyz_py-5.7.0/README.md`

 * *Files identical despite different names*

### Comparing `xyz_py-5.6.1/setup.py` & `xyz_py-5.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-__version__ = "5.6.1"
+__version__ = "5.7.0"
 
 setuptools.setup(
     name="xyz_py",
     version=__version__,
     author="Jon Kragskow",
     author_email="jonkragskow@gmail.com",
     description="A package for manipulating xyz files and chemical structures",
```

### Comparing `xyz_py-5.6.1/xyz_py/atomic.py` & `xyz_py-5.7.0/xyz_py/atomic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,87 @@
 
 
+#: s block elements, group 1
 s_block_col_1 = ["Li", "Na", "K", "Rb", "Cs", "Fr"]
+#: s block elements, group 2
 s_block_col_2 = ["Be", "Mg", "Ca", "Sr", "Ba", "Ra"]
 
+#: all s block elements
 s_block = s_block_col_1 + s_block_col_2
 
+#: first row p-block elements
 p_block_row_1 = ["He"]
+#: second row p-block elements
 p_block_row_2 = ["B", "C", "N", "O", "F", "Ne"]
+#: third row p-block elements
 p_block_row_3 = ["Al", "Si", "P", "S", "Cl", "Ar"]
+#: fourth row p-block elements
 p_block_row_4 = ["Ga", "Ge", "As", "Se", "Br", "Kr"]
+#: fifth row p-block elements
 p_block_row_5 = ["In", "Sn", "Sb", "Te", "I", "Xe"]
+#: sixth row p-block elements
 p_block_row_6 = ["Tl", "Pb", "Bi", "Po", "At", "Rn"]
 
+#: all p block elements
 p_block = p_block_row_1 + p_block_row_2 + p_block_row_3 + p_block_row_4
 p_block += p_block_row_5 + p_block_row_6
 
+#: first row d-block elements
 d_block_row_1 = [
     "Sc", "Ti", "V", "Cr", "Mn", "Fe", "Co", "Ni", "Cu", "Zn"
 ]
 
+#: second row d-block elements
 d_block_row_2 = [
     "Y", "Zr", "Nb", "Mo", "Tc", "Ru", "Rh", "Pd", "Ag", "Cd"
 ]
 
+#: third row d-block elements
 d_block_row_3 = [
     "Hf", "Ta", "W", "Re", "Os", "Ir", "Pt", "Ni", "Au", "Hg"
 ]
 
+#; All d-block elements
 d_block = d_block_row_1 + d_block_row_2 + d_block_row_3
 
+#: All transition metals
 transition_metals = d_block
 
+#: first row f-block elements
 f_block_row_1 = [
     "Ce", "Pr", "Nd", "Pm", "Sm", "Eu", "Gd", "Tb", "Dy", "Ho", "Er", "Tm",
     "Yb", "Lu"
 ]
 
+#: All lanthanides
 lanthanides = f_block_row_1
 
+#: second row f-block elements
 f_block_row_2 = [
     "Th", "Pa", "U", "Np", "Pu", "Am", "Cm", "Bk", "Cf", "Es", "Fm", "Md",
     "No", "Lr"
 ]
 
+#: All actinides
 actinides = f_block_row_1
 
+#: All f-block elements
 f_block = f_block_row_1 + f_block_row_2
 
+#: All metals
 metals = s_block + d_block + f_block
 metals += ["Al", "Ge", "Ga", "In", "Sn", "Tl", "Pb", "Bi", "Po"]
 
+#: All non-metals
 non_metals = list(set(p_block).difference(metals)) + ['H']
 
+#: All elements
 elements = s_block + p_block + d_block + f_block + ['H']
 
-# Dictionary of relative atomic masses
+#: Relative atomic masses
 masses = {
     "H": 1.0076, "He": 4.0026, "Li": 6.941, "Be": 9.0122, "B": 10.811,
     "C": 12.0107, "N": 14.0067, "O": 15.9994, "F": 18.9984, "Ne": 20.1797,
     "Na": 22.9897, "Mg": 24.305, "Al": 26.9815, "Si": 28.0855, "P": 30.9738,
     "S": 32.065, "Cl": 35.453, "K": 39.0983, "Ar": 39.948, "Ca": 40.078,
     "Sc": 44.9559, "Ti": 47.867, "V": 50.9415, "Cr": 51.9961, "Mn": 54.938,
     "Fe": 55.845, "Ni": 58.6934, "Co": 58.9332, "Cu": 63.546, "Zn": 65.39,
@@ -75,14 +98,15 @@
     "Tl": 204.3833, "Pb": 207.2, "Bi": 208.9804, "Po": 209, "At": 210,
     "Rn": 222, "Fr": 223, "Ra": 226, "Ac": 227, "Pa": 231.0359, "Th": 232.0381,
     "Np": 237, "U": 238.0289, "Am": 243, "Pu": 244, "Cm": 247, "Bk": 247,
     "Cf": 251, "Es": 252, "Fm": 257, "Md": 258, "No": 259, "Rf": 261,
     "Lr": 262, "Db": 262, "Bh": 264, "Sg": 266, "Mt": 268, "Rg": 272, "Hs": 277
 }
 
+#: Atomic label to atomic number dictionary
 lab_num = {
     "H": 1, "He": 2, "Li": 3, "Be": 4, "B": 5, "C": 6, "N": 7,
     "O": 8, "F": 9, "Ne": 10, "Na": 11, "Mg": 12, "Al": 13,
     "Si": 14, "P": 15, "S": 16, "Cl": 17, "Ar": 18, "K": 19,
     "Ca": 20, "Sc": 21, "Ti": 22, "V": 23, "Cr": 24, "Mn": 25,
     "Fe": 26, "Co": 27, "Ni": 28, "Cu": 29, "Zn": 30, "Ga": 31,
     "Ge": 32, "As": 33, "Se": 34, "Br": 35, "Kr": 36, "Rb": 37,
@@ -98,21 +122,25 @@
     "U": 92, "Np": 93, "Pu": 94, "Am": 95, "Cm": 96, "Bk": 97,
     "Cf": 98, "Es": 99, "Fm": 100, "Md": 101, "No": 102, "Lr": 103,
     "Rf": 104, "Db": 105, "Sg": 106, "Bh": 107, "Hs": 108,
     "Mt": 109, "Ds": 110, "Rg": 111, "Cn": 112, "Nh": 113,
     "Fl": 114, "Mc": 115, "Lv": 116, "Ts": 117, "Og": 118
 }
 
+#: Atomic number to atomic label dictionary
 num_lab = dict(zip(lab_num.values(), lab_num.keys()))
 
-# Atomic radii
-# also called vdW radii
-# https://www.rsc.org/periodic-table/
-# CRC Handbook of Chemistry and Physics, 97th Ed.; Haynes, W. M. Ed. CRC
-# Press/Taylor and Francis: Boca Raton, 2016 (accessed 2022-10-01).
+#: Atomic radii
+#:
+#: Also called vdW radii
+#:
+#: https://www.rsc.org/periodic-table/
+#:
+#: CRC Handbook of Chemistry and Physics, 97th Ed.; Haynes, W. M. Ed. CRC
+#: Press/Taylor and Francis: Boca Raton, 2016 (accessed 2022-10-01).
 atomic_radii = {
     "H": 1.1, "He": 1.4, "Li": 1.82, "Be": 1.53, "B": 1.92, "C": 1.7,
     "N": 1.55, "O": 1.52, "F": 1.47, "Ne": 1.54, "Na": 2.27, "Mg": 1.73,
     "Al": 1.84, "Si": 2.1, "P": 1.8, "S": 1.8, "Cl": 1.75, "Ar": 1.88,
     "K": 2.75, "Ca": 2.31, "Sc": 2.15, "Ti": 2.11, "V": 2.07, "Cr": 2.06,
     "Mn": 2.05, "Fe": 2.04, "Co": 2.0, "Ni": 1.97, "Cu": 1.96, "Zn": 2.01,
     "Ga": 1.87, "Ge": 2.11, "As": 1.85, "Se": 1.9, "Br": 1.85, "Kr": 2.02,
@@ -125,16 +153,17 @@
     "Ta": 2.22, "W": 2.18, "Re": 2.16, "Os": 2.16, "Ir": 2.13, "Pt": 2.13,
     "Au": 2.14, "Hg": 2.23, "Tl": 1.96, "Pb": 2.02, "Bi": 2.07, "Po": 1.97,
     "At": 2.02, "Rn": 2.2, "Fr": 3.48, "Ra": 2.83, "Ac": 2.47, "Th": 2.45,
     "Pa": 2.43, "U": 2.41, "Np": 2.39, "Pu": 2.43, "Am": 2.44, "Cm": 2.45,
     "Bk": 2.44, "Cf": 2.45, "Es": 2.45, "Fm": 2.45, "Md": 2.46, "No": 2.46,
     "Lr": 2.46
 }
-# Covalent radii
-# https://www.rsc.org/periodic-table/
+#: Covalent radii
+#:
+#: https://www.rsc.org/periodic-table/\n
 cov_radii = {
     "H": 0.32, "He": 0.37, "Li": 1.3, "Be": 0.99, "B": 0.84, "C": 0.75,
     "N": 0.71, "O": 0.64, "F": 0.6, "Ne": 0.62, "Na": 1.6, "Mg": 1.4,
     "Al": 1.24, "Si": 1.14, "P": 1.09, "S": 1.04, "Cl": 1.0, "Ar": 1.01,
     "K": 2.0, "Ca": 1.74, "Sc": 1.59, "Ti": 1.48, "V": 1.44, "Cr": 1.3,
     "Mn": 1.29, "Fe": 1.24, "Co": 1.18, "Ni": 1.17, "Cu": 1.22, "Zn": 1.2,
     "Ga": 1.23, "Ge": 1.2, "As": 1.2, "Se": 1.18, "Br": 1.17, "Kr": 1.16,
```

### Comparing `xyz_py-5.6.1/xyz_py/cli.py` & `xyz_py-5.7.0/xyz_py/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -149,33 +149,33 @@
     -------
         None
 
     '''
     labels, coords = xyz_py.load_xyz(uargs.xyz_file)
 
     if uargs.radians:
-        xyz_py.rotate_coords(
+        rotated_coords = xyz_py.rotate_coords(
             coords, uargs.alpha, uargs.beta, uargs.gamma
         )
     else:
-        xyz_py.rotate_coords(
+        rotated_coords = xyz_py.rotate_coords(
             coords,
             uargs.alpha * 180. / np.pi,
             uargs.beta * 180. / np.pi,
             uargs.gamma * 180. / np.pi
         )
 
     if uargs.out_f_name:
         out_f_name = uargs.out_f_name
     else:
         out_f_name = '{}_rotated.xyz'.format(
             os.path.splitext(uargs.xyz_file)[0]
         )
 
-    xyz_py.save_xyz(out_f_name, labels, coords)
+    xyz_py.save_xyz(out_f_name, labels, rotated_coords)
 
     return
 
 
 def overlay_func(uargs):
     '''
     Wrapper for cli call to overlay
@@ -249,20 +249,32 @@
     for key, val in entities_dict.items():
         print('{} : {:d}'.format(key, len(val)))
 
     return
 
 
 def renumber_func(uargs):
+    '''
+    Wrapper for cli call to renumber
+    '''
 
+    # Load labels, coordinates
     l, c = xyz_py.load_xyz(uargs.xyz_file)
 
+    # Load comment line
+    comment = xyz_py.load_xyz_comment(uargs.xyz_file)
+
+    # Remove existing labels
+    l = xyz_py.remove_label_indices(l)
+
+    # Add new labels
     l = xyz_py.add_label_indices(l, style=uargs.style)
 
-    xyz_py.save_xyz(uargs.xyz_file, l, c)
+    # Save new xyz file
+    xyz_py.save_xyz(uargs.xyz_file, l, c, comment=comment)
 
     return
 
 
 def parse_cutoffs(cutoffs):
 
     if len(cutoffs) % 2:
```

### Comparing `xyz_py-5.6.1/xyz_py/xyz_py.py` & `xyz_py-5.7.0/xyz_py/xyz_py.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #! /usr/bin/env python3
 
 '''
 This is the main part of xyz_py
 '''
 
 import numpy as np
+import numpy.typing as npt
 import numpy.linalg as la
 from ase import neighborlist, Atoms
 from ase.geometry.analysis import Analysis
 import copy
 import re
 import scipy.optimize as spo
 import sys
@@ -18,62 +19,44 @@
 from . import version
 from . import atomic
 
 __version__ = version.__version__
 
 
 def load_xyz(f_name: str, atomic_numbers: bool = False,
-             add_indices: bool = False, capitalise: bool = True) -> None:
+             add_indices: bool = False,
+             capitalise: bool = True) -> tuple[list, npt.NDArray]:
     '''
     Load labels and coordinates from a .xyz file
 
     File assumes two header lines, first containing number of atoms
     and second containing a comment or blank, followed by actual data
 
     Parameters
     ----------
-    f_name : str
+    f_name: str
         File name
-    atomic_numbers : bool, default False
+    atomic_numbers: bool, default False
         If True, reads xyz file with atomic numbers and converts to labels
-    add_indices : bool, default False
+    add_indices: bool, default False
         If True, add indices to atomic labels
         (replacing those which may exist already)
-    capitalise : bool, default True
+    capitalise: bool, default True
         If True, capitalise atomic labels
 
     Returns
     -------
     list
         atomic labels
     np.ndarray
         (n_atoms,3) array containing xyz coordinates of each atom
-
-    Raises
-    ------
-    ValueError
-        If the .xyz file has incorrect length, or is missing the number
-        of atoms and comment lines
     '''
 
-    # Check file contains number of atoms on first line
-    with open(f_name, 'r') as f:
-        line = next(f)
-        if len(line.split()) != 1:
-            raise ValueError('.xyz file does not contain number of atoms')
-        else:
-            try:
-                n_atoms = int(line)
-            except ValueError:
-                raise ValueError('.xyz file number of atoms is malformed')
-
-            n_lines = len(f.readlines()) + 1  # + 1 for next
-            if n_atoms + 2 != n_lines:
-
-                raise ValueError('.xyz file length/format is incorrect')
+    # Check xyz file formatting
+    check_xyz(f_name)
 
     if atomic_numbers:
         _numbers = np.loadtxt(
             f_name, skiprows=2, usecols=0, dtype=int, ndmin=1
         )
         _labels = num_to_lab(_numbers.tolist())
     else:
@@ -89,37 +72,106 @@
         _labels = add_label_indices(_labels)
 
     _coords = np.loadtxt(f_name, skiprows=2, usecols=(1, 2, 3), ndmin=2)
 
     return _labels, _coords
 
 
+def load_xyz_comment(f_name: str) -> str:
+    '''
+    Load comment line from an xyz file
+
+    Parameters
+    ----------
+    f_name: str
+        File name
+
+    Returns
+    -------
+    str
+        comment line of xyz file
+    '''
+
+    # Check xyz file formatting
+    check_xyz(f_name)
+
+    with open(f_name, 'r') as f:
+        next(f)
+        comment = next(f)
+
+    comment = comment.rstrip()
+
+    return comment
+
+
+def check_xyz(f_name: str) -> None:
+    '''
+    Checks if .xyz file has correct length and contains two header lines
+    for the number of atoms and an optional comment
+
+    Parameters
+    ----------
+    f_name: str
+        File name
+
+    Returns
+    -------
+    None
+
+    Raises
+    ------
+    ValueError
+        If the .xyz file has incorrect length, or is missing the number
+        of atoms and comment lines
+    '''
+
+    # Check file contains number of atoms on first line
+    with open(f_name, 'r') as f:
+        line = next(f)
+        if len(line.split()) != 1:
+            raise ValueError('.xyz file does not contain number of atoms')
+        else:
+            try:
+                n_atoms = int(line)
+            except ValueError:
+                raise ValueError('.xyz file number of atoms is malformed')
+
+            n_lines = len(f.readlines()) + 1  # + 1 for next
+            if n_atoms + 2 != n_lines:
+                raise ValueError('.xyz file length/format is incorrect')
+
+    return
+
+
 def save_xyz(f_name: str, labels: list, coords: np.ndarray,
              with_numbers: bool = False, verbose: bool = True,
-             mask: list = [], atomic_numbers: bool = False):
+             mask: list = [], atomic_numbers: bool = False,
+             comment: str = '') -> None:
     '''
     Save an xyz file containing labels and coordinates
 
     Parameters
     ----------
-    f_name : str
+    f_name: str
         File name
-    labels : list
+    labels: list
         atomic labels
-    coords : np.ndarray
+    coords: np.ndarray
         list of 3 element lists containing xyz coordinates of each atom
-    with_numbers : bool, default False
+    with_numbers: bool, default False
         If True, add/overwrite numbers to labels before printing
-    verbose : bool, default True
+    verbose: bool, default True
         Print information on filename to screen
-    mask : list, optional
+    mask: list, optional
         n_atom list of 0 (exclude) and 1 (include) indicating which
         atoms to print
-    atomic_numbers : bool, default False
-        If true, will save xyz file with atomic numbers
+    atomic_numbers: bool, default False
+        If True, will save xyz file with atomic numbers
+    comment: str, default ''
+        Comment line printed to 2nd line of .xyz file
 
     Returns
     -------
     None
     '''
 
     # Option to have numbers added
@@ -141,17 +193,18 @@
         _labels = remove_label_indices(_labels)
         _numbers = lab_to_num(_labels)
         _identifier = _numbers
     else:
         _identifier = _labels
 
     with open(f_name, 'w') as f:
-        f.write('{:d}\n\n'.format(n_atoms))
-        for it, (ident, trio) in enumerate(zip(_identifier, coords)):
-            f.write('{:5} {:15.7f} {:15.7f} {:15.7f} \n'.format(ident, *trio))
+        f.write(f'{n_atoms:d}\n')
+        f.write(f'{comment}')
+        for ident, trio in zip(_identifier, coords):
+            f.write('\n{:5} {:15.7f} {:15.7f} {:15.7f}'.format(ident, *trio))
 
     if verbose:
         print('New xyz file written to {}'.format(f_name))
 
     return
 
 
@@ -160,15 +213,15 @@
     Remove label indexing from atomic symbols
     indexing is either numbers or numbers followed by letters:
     e.g. H1, H2, H3
     or H1a, H2a, H3a
 
     Parameters
     ----------
-    labels : list
+    labels: list
         atomic labels
 
     Returns
     -------
     list
         atomic labels without indexing
     '''
@@ -189,36 +242,36 @@
 
 def add_label_indices(labels, style='per_element', start_index=1):
     '''
     Add label indexing to atomic symbols - either element or per atom.
 
     Parameters
     ----------
-    labels : list
+    labels: list
         atomic labels
-    style : str, optional
+    style: str, optional
         {'per_element', 'sequential'}
-            'per_element' : Index by element e.g. Dy1, Dy2, N1, N2, etc.
-            'sequential' : Index the atoms 1->N regardless of element
-    start_index : int
+            'per_element': Index by element e.g. Dy1, Dy2, N1, N2, etc.
+            'sequential': Index the atoms 1->N regardless of element
+    start_index: int
         integer at which indexing will start
 
     Returns
     -------
     list
         atomic labels with indexing
     '''
 
     # remove numbers just in case
     labels_nn = remove_label_indices(labels)
 
     # Just number the atoms 1->N regardless of element
     if style == 'sequential':
         labels_wn = ['{}{:d}'.format(lab, it + start_index)
-                     for (it, lab) in enumerate(labels)]
+                     for (it, lab) in enumerate(labels_nn)]
 
     # Index by element Dy1, Dy2, N1, N2, etc.
     if style == 'per_element':
         # Get list of unique elements
         atoms = set(labels_nn)
         # Create dict to keep track of index of current atom of each element
         atom_count = {atom: start_index for atom in atoms}
@@ -236,15 +289,15 @@
 
 def count_n_atoms(form_str):
     '''
     Count number of atoms in a chemical formula
 
     Parameters
     ----------
-    form_str : str
+    form_str: str
         chemical formula string
 
     Returns
     -------
     int
         number of atoms in chemical formula
     '''
@@ -259,17 +312,17 @@
 def index_elements(labels, shift=0):
     '''
     Return dictionary of element (keys) and indices (values) from list
     of labels
 
     Parameters
     ----------
-    labels : list
+    labels: list
         atomic labels
-    shift : int, optional
+    shift: int, optional
         additive shift to apply to all indices
 
     Returns
     -------
     dict
         element (keys) and indices (values)
     '''
@@ -289,15 +342,15 @@
 
 def count_elements(labels):
     '''
     Count number of each element in a list of elements
 
     Parameters
     ----------
-    labels : list
+    labels: list
         atomic labels
     Returns
     -------
     dict
         dictionary of elements (keys) and counts (vals)
     '''
 
@@ -316,15 +369,15 @@
 
 def get_formula(labels):
     '''
     Generates empirical formula in alphabetical order given a list of labels
 
     Parameters
     ----------
-    labels : list
+    labels: list
         atomic labels
     Returns
     -------
     str
         Empirical formula in alphabetical order
     '''
 
@@ -337,15 +390,15 @@
 
 def formstr_to_formdict(form_str):
     '''
     Converts formula string into dictionary of {atomic label:quantity} pairs
 
     Parameters
     ----------
-    form_string : str
+    form_string: str
         Chemical formula as string
 
     Returns
     -------
     dict
         dictionary of {atomic label:quantity} pairs
     '''
@@ -379,17 +432,17 @@
 def formdict_to_formstr(form_dict, include_one=False):
     '''
     Converts dictionary of {atomic label:quantity} pairs into
     a single formula string in alphabetical order
 
     Parameters
     ----------
-    form_dict : dict
+    form_dict: dict
         dictionary of {atomic label:quantity} pairs
-    include_one : bool, default False
+    include_one: bool, default False
         Include 1 in final chemical formula e.g. C1H4
 
     Returns
     -------
     str
         Chemical formula as string in alphabetical order
     '''
@@ -425,15 +478,15 @@
 
 def contains_metal(form_string):
     '''
     Indicates if a metal is found in a chemical formula string
 
     Parameters
     ----------
-    form_string : str
+    form_string: str
         Chemical formula as string
 
     Returns
     -------
     bool
         True if metal found, else False
     '''
@@ -449,21 +502,21 @@
 
 def combine_xyz(labels_1, labels_2, coords_1, coords_2):
     '''
     Combine two sets of labels and coordinates
 
     Parameters
     ----------
-    labels_1 : list
+    labels_1: list
         Atomic labels
-    coords_1 : list
+    coords_1: list
         xyz coordinates as (n_atoms, 3) array
-    labels_2 : list
+    labels_2: list
         Atomic labels
-    coords_2 : list
+    coords_2: list
         xyz coordinates as (n_atoms, 3) array
 
     Returns
     -------
     list
         Combined atomic labels
     np.ndarray
@@ -481,19 +534,19 @@
 
 def get_neighborlist(labels, coords, adjust_cutoff={}):
     '''
     Calculate ASE neighbourlist based on covalent radii
 
     Parameters
     ----------
-    labels : list
+    labels: list
         Atomic labels
-    coords : np.ndarray
+    coords: np.ndarray
         xyz coordinates as (n_atoms, 3) array
-    adjust_cutoff : dict, optional
+    adjust_cutoff: dict, optional
         dictionary of atoms (keys) and new cutoffs (values)
 
     Returns
     -------
     ASE neighbourlist object
         Neighbourlist for system
     '''
@@ -528,38 +581,41 @@
 
 def get_adjacency(labels, coords, adjust_cutoff={}):
     '''
     Calculate adjacency matrix using ASE based on covalent radii.
 
     Parameters
     ----------
-    labels : list
+    labels: list
         Atomic labels
-    coords : np.ndarray
+    coords: np.ndarray
         xyz coordinates as (n_atoms, 3) array
-    adjust_cutoff : dict, optional
+    adjust_cutoff: dict, optional
         dictionary of atoms (keys) and new cutoffs (values)
-    save : bool, default False
-        If true save to file given by `f_name`
-    f_name : str, default 'adjacency.dat'
+    save: bool, default False
+        If True save to file given by `f_name`
+    f_name: str, default 'adjacency.dat'
         If save true, this name is used for the file containing the adjacency
         matrix
 
     Returns
     -------
     np.array
         Adjacency matrix with same order as labels/coords
     '''
 
     # Remove labels if present
     labels_nn = remove_label_indices(labels)
 
     # Get ASE neighbourlist object
-    neigh_list = get_neighborlist(labels_nn, coords,
-                                  adjust_cutoff=adjust_cutoff)
+    neigh_list = get_neighborlist(
+        labels_nn,
+        coords,
+        adjust_cutoff=adjust_cutoff
+    )
 
     # Create adjacency matrix
     adjacency = neigh_list.get_connectivity_matrix(sparse=False)
 
     return adjacency
 
 
@@ -571,29 +627,29 @@
     '''
     Calculate list of atoms between which there is a bond.
     Using ASE. Only unique bonds are retained.
     e.g. 0-1 and not 1-0
 
     Parameters
     ----------
-    labels : list
+    labels: list
         Atomic labels
-    coords : np.ndarray
+    coords: np.ndarray
         xyz coordinates as (n_atoms, 3) array in Angstrom
-    neigh_list : ASE neighbourlist object, optional
+    neigh_list: ASE neighbourlist object, optional
         neighbourlist of system
-    f_name : str, 'bonds.dat'
+    f_name: str, 'bonds.dat'
         filename to save bond list to
-    save : bool, default False
+    save: bool, default False
         Save bond list to file
-    verbose : bool, default True
+    verbose: bool, default True
         Print number of bonds to screen
-    style : str, {'indices','labels'}
-            indices : Bond list contains atom number
-            labels  : Bond list contains atom label
+    style: str, {'indices','labels'}
+            indices: Bond list contains atom number
+            labels : Bond list contains atom label
 
     Returns
     -------
     list[list[int | str]]
         list of lists of unique bonds (atom pairs)
     '''
 
@@ -608,29 +664,29 @@
     '''
     Calculate list of atoms between which there is a bond.
     Using ASE. Only unique bonds are retained.
     e.g. 0-1 and not 1-0
 
     Parameters
     ----------
-    labels : list
+    labels: list
         Atomic labels
-    coords : np.ndarray
+    coords: np.ndarray
         xyz coordinates as (n_atoms, 3) array in Angstrom
-    neigh_list : ASE neighbourlist object, optional
+    neigh_list: ASE neighbourlist object, optional
         neighbourlist of system
-    f_name : str, 'bonds.dat'
+    f_name: str, 'bonds.dat'
         filename to save bond list to
-    save : bool, default False
+    save: bool, default False
         Save bond list to file
-    verbose : bool, default True
+    verbose: bool, default True
         Print number of bonds to screen
-    style : str, {'indices','labels'}
-            indices : Bond list contains atom number
-            labels  : Bond list contains atom label
+    style: str, {'indices','labels'}
+            indices: Bond list contains atom number
+            labels : Bond list contains atom label
 
     Returns
     -------
     list[list[int | str]]
         list of lists of unique bonds (atom pairs)
     np.ndarray
         Bond length in Angstrom
@@ -648,17 +704,17 @@
 
     # Get object containing analysis of molecular structure
     ana = Analysis(mol, nl=neigh_list)
 
     # Get bonds from ASE
     # Returns: list of lists of lists containing UNIQUE bonds
     # Defined as
-    # Atom 1 : [bonded atom, bonded atom], ...
-    # Atom 2 : [bonded atom, bonded atom], ...
-    # Atom n : [bonded atom, bonded atom], ...
+    # Atom 1: [bonded atom, bonded atom], ...
+    # Atom 2: [bonded atom, bonded atom], ...
+    # Atom n: [bonded atom, bonded atom], ...
     # Where only the right hand side is in the list
     is_bonded_to = ana.unique_bonds
 
     # Remove weird outer list wrapping the entire thing twice...
     is_bonded_to = is_bonded_to[0]
     # Create list of bonds (atom pairs) by appending lhs of above
     # definition to each element of the rhs
@@ -704,30 +760,30 @@
     '''
     Calculate list of atoms between which there is a bond angle.
     Using ASE. Only unique angles are retained.
     e.g. 0-1-2 but not 2-1-0
 
     Parameters
     ----------
-    labels : list
+    labels: list
         Atomic labels
-    coords : np.ndarray
+    coords: np.ndarray
         xyz coordinates as (n_atoms, 3) array
-    neigh_list : ASE neighbourlist object, optional
+    neigh_list: ASE neighbourlist object, optional
         neighbourlist of system
-    f_name : str, default 'angles.dat'
+    f_name: str, default 'angles.dat'
         filename to save angle list to
-    save : bool, default False
+    save: bool, default False
         Save angle list to file
-    verbose : bool, default True
+    verbose: bool, default True
         Print number of angles to screen
-    style : str, {'indices','labels'}
-            indices : Angle list contains atom number
-            labels  : Angle list contains atom label
-            values  : Angle list is values in degrees
+    style: str, {'indices','labels'}
+            indices: Angle list contains atom number
+            labels : Angle list contains atom label
+            values : Angle list is values in degrees
 
     Returns
     -------
     list[list[int | str | float]]
         list of lists of unique angles (atom trios)
     '''
 
@@ -742,29 +798,29 @@
                 style='labels'):
     '''
     Calculate all angles using ASE. Only unique angles are retained.
     e.g. 0-1-2 but not 2-1-0
 
     Parameters
     ----------
-    labels : list
+    labels: list
         Atomic labels
-    coords : np.ndarray
+    coords: np.ndarray
         xyz coordinates as (n_atoms, 3) array
-    neigh_list : ASE neighbourlist object, optional
+    neigh_list: ASE neighbourlist object, optional
         neighbourlist of system
-    f_name : str, default 'angles.dat'
+    f_name: str, default 'angles.dat'
         filename to save angle list to
-    save : bool, default False
+    save: bool, default False
         Save angle list to file
-    verbose : bool, default True
+    verbose: bool, default True
         Print number of angles to screen
-    style : str, {'indices','labels'}
-            indices : Angle labels are atom number
-            labels  : Angle labels are atom label
+    style: str, {'indices','labels'}
+            indices: Angle labels are atom number
+            labels : Angle labels are atom label
 
     Returns
     -------
     list[list[int | str]]
         list of lists of unique angles (atom trios) as labels or indices
     np.ndarray
         Angles in degrees
@@ -782,17 +838,17 @@
 
     # Get object containing analysis of molecular structure
     ana = Analysis(mol, nl=neigh_list)
 
     # Get angles from ASE
     # Returns: list of lists of lists containing UNIQUE angles
     # Defined as
-    # Atom 1 : [[atom,atom], [atom,atom]], ...
-    # Atom 2 : [[atom,atom], [atom,atom]], ...
-    # Atom n : [[atom,atom], [atom,atom]], ...
+    # Atom 1: [[atom,atom], [atom,atom]], ...
+    # Atom 2: [[atom,atom], [atom,atom]], ...
+    # Atom n: [[atom,atom], [atom,atom]], ...
     # Where only the right hand side is in the list
     is_angled_to = ana.unique_angles
 
     # Remove weird outer list wrapping the entire thing twice...
     is_angled_to = is_angled_to[0]
     # Create list of angles (atom trios) by appending lhs of above
     # definition to each element of the rhs
@@ -837,29 +893,29 @@
     '''
     Calculate and list of atoms between which there is a dihedral.
     Using ASE. Only unique dihedrals are retained.
     e.g. 0-1-2-3 but not 3-2-1-0
 
     Parameters
     ----------
-    labels : list
+    labels: list
         Atomic labels
-    coords : np.ndarray
+    coords: np.ndarray
         xyz coordinates as (n_atoms, 3) array
-    neigh_list : ASE neighbourlist object, optional
+    neigh_list: ASE neighbourlist object, optional
         neighbourlist of system
-    f_name : str, default 'dihedrals.dat'
+    f_name: str, default 'dihedrals.dat'
         filename to save angle list to
-    save : bool, default False
+    save: bool, default False
         Save angle list to file
-    verbose : bool, default True
+    verbose: bool, default True
         Print number of dihedrals to screen
-    style : str, {'indices','labels'}
-            indices : Dihedral list contains atom number
-            labels  : Dihedral list contains atom label
+    style: str, {'indices','labels'}
+            indices: Dihedral list contains atom number
+            labels : Dihedral list contains atom label
 
     Returns
     -------
     list[list[int | str]]
         list of lists of unique dihedrals (atom quads)
     '''
     dihedrals, _ = find_dihedrals(
@@ -874,29 +930,29 @@
     '''
     Calculate and list of atoms between which there is a dihedral.
     Using ASE. Only unique dihedrals are retained.
     e.g. 0-1-2-3 but not 3-2-1-0
 
     Parameters
     ----------
-    labels : list
+    labels: list
         Atomic labels
-    coords : np.ndarray
+    coords: np.ndarray
         xyz coordinates as (n_atoms, 3) array
-    neigh_list : ASE neighbourlist object, optional
+    neigh_list: ASE neighbourlist object, optional
         neighbourlist of system
-    f_name : str, default 'dihedrals.dat'
+    f_name: str, default 'dihedrals.dat'
         filename to save angle list to
-    save : bool, default False
+    save: bool, default False
         Save angle list to file
-    verbose : bool, default True
+    verbose: bool, default True
         Print number of dihedrals to screen
-    style : str, {'indices','labels'}
-            indices : Dihedral list contains atom number
-            labels  : Dihedral list contains atom label
+    style: str, {'indices','labels'}
+            indices: Dihedral list contains atom number
+            labels : Dihedral list contains atom label
 
     Returns
     -------
     list[list[int | str]]
         list of lists of unique dihedrals (atom quads)
     np.ndarray
         Dihedral angles in degrees
@@ -914,17 +970,17 @@
 
     # Get object containing analysis of molecular structure
     ana = Analysis(mol, nl=neigh_list)
 
     # Get dihedrals from ASE
     # Returns: list of lists of lists containing UNIQUE dihedrals
     # Defined as
-    # Atom 1 : [[atom,atom,atom], [atom,atom,atom]], ...
-    # Atom 2 : [[atom,atom,atom], [atom,atom,atom]], ...
-    # Atom n : [[atom,atom,atom], [atom,atom,atom]], ...
+    # Atom 1: [[atom,atom,atom], [atom,atom,atom]], ...
+    # Atom 2: [[atom,atom,atom], [atom,atom,atom]], ...
+    # Atom n: [[atom,atom,atom], [atom,atom,atom]], ...
     # Where only the right hand side is in the list
     is_dihedraled_to = ana.unique_dihedrals
 
     # Remove weird outer list wrapping the entire thing twice...
     is_dihedraled_to = is_dihedraled_to[0]
     # Create list of dihedrals (atom quads) by appending lhs of above
     # definition to each element of the rhs
@@ -967,15 +1023,15 @@
 
 def lab_to_num(labels):
     '''
     Convert atomic label to atomic number
 
     Parameters
     ----------
-    labels : list[str]
+    labels: list[str]
         Atomic labels
 
     Returns
     -------
     list[int]
         Atomic numbers
     '''
@@ -989,17 +1045,17 @@
 
 def num_to_lab(numbers, numbered=True):
     '''
     Convert atomic number to atomic labels
 
     Parameters
     ----------
-    numbers : list[int]
+    numbers: list[int]
         Atomic numbers
-    numbered : bool, optional
+    numbered: bool, optional
         Add indexing number to end of atomic labels
 
     Returns
     -------
     list[str]
         Atomic labels
     '''
@@ -1016,15 +1072,15 @@
 
 def reflect_coords(coords):
     '''
     Reflect coordinates through xy plane
 
     Parameters
     ----------
-    coords : np.ndarray
+    coords: np.ndarray
         xyz coordinates as (n_atoms, 3) array
 
     Returns
     -------
     np.ndarray
         xyz coordinates as (n_atoms, 3) array
 
@@ -1058,29 +1114,29 @@
 def find_entities(labels, coords, adjust_cutoff={}):
     '''
     Finds formulae of entities given in labels and coords using adjacency
     matrix
 
     Parameters
     ----------
-    labels : list[str]
+    labels: list[str]
         atomic labels
-    coords : np.ndarray
+    coords: np.ndarray
         xyz coordinates of each atom as (n_atoms, 3) array
-    adjust_cutoff : dict, optional
+    adjust_cutoff: dict, optional
         dictionary of atoms (keys) and new cutoffs (values) used in generating
         adjacency matrix
 
     Returns
     -------
     dict[str:list[list[int]]]
-        keys = molecular formula,
+        keys = molecular formula\n
         vals = list of lists, where each list contains the indices of a single
-                occurrence of the `key`, and the indices match the order given
-                in `labels` and `coords`
+        \noccurrence of the `key`, and the indices match the order given\n
+        in `labels` and `coords`
     '''
 
     # Remove label numbers if present
     labels_nn = remove_label_indices(labels)
 
     # Generate adjacency matrix using ASE
     adjacency = get_adjacency(labels_nn, coords, adjust_cutoff=adjust_cutoff)
@@ -1093,26 +1149,26 @@
 
 def find_entities_from_adjacency(labels_nn, adjacency):
     '''
     Finds formulae of entities given in labels and adjacency matrix
 
     Parameters
     ----------
-    labels : list[str]
+    labels: list[str]
         atomic labels
-    adjacency : np.ndarray
+    adjacency: np.ndarray
         Adjacency matrix (0,1) with same order as labels
 
     Returns
     -------
     dict[str:list[list[int]]]
-        keys = molecular formula,
+        keys = molecular formula\n
         vals = list of lists, where each list contains the indices of a single
-                occurrence of the `key`, and the indices match the order given
-                in `labels` and `coords`
+        \noccurrence of the `key`, and the indices match the order given\n
+        in `labels` and `coords`
     '''
 
     # Count number of atoms
     n_atoms = len(labels_nn)
 
     # Set current fragment as start atom
     curr_frag = {0}
@@ -1164,17 +1220,17 @@
     '''
     Calculates RMSD between two structures
     RMSD = sqrt(mean(deviations**2))
     Where deviations are defined as norm([x1,y1,z1]-[x2,y2,z2])
 
     Parameters
     ----------
-    coords_1 : np.ndarray
+    coords_1: np.ndarray
         xyz coordinates as (n_atoms, 3) array
-    coords_2 : np.ndarray
+    coords_2: np.ndarray
         xyz coordinates as (n_atoms, 3) array
 
     Returns
     -------
     float
         Root mean square of norms of deviation between two structures
     '''
@@ -1196,36 +1252,36 @@
 
     return rmsd
 
 
 def calculate_rmsd(coords_1, coords_2, mask_1=[], mask_2=[], order_1=[],
                    order_2=[]):
     '''
-    Calculates RMSD between two structures
-    RMSD = sqrt(mean(deviations**2))
-    Where deviations are defined as norm([x1,y1,z1]-[x2,y2,z2])
+    Calculates RMSD between two structures\n
+    RMSD = sqrt(mean(deviations**2))\n
+    Where deviations are defined as norm([x1,y1,z1]-[x2,y2,z2])\n
     If coords_1 and coords_2 are not the same length, then a mask array can be
-    provided for either/both and is applied prior to the calculation
+    \nprovided for either/both and is applied prior to the calculation\n
     coords_1 and coords_2 can also be reordered if new orders are specified
-        - note this occurs BEFORE masking
+    - note this occurs BEFORE masking
 
     Parameters
     ----------
-    coords_1 : np.ndarray
+    coords_1: np.ndarray
         xyz coordinates as (n_atoms, 3) array
-    coords_2 : np.ndarray
+    coords_2: np.ndarray
         xyz coordinates as (n_atoms, 3) array
 
-    mask_1 : list
+    mask_1: list
         list of 0 (exclude) and 1 (include) for each element in coords_1
-    mask_2 : list
+    mask_2: list
         list of 0 (exclude) and 1 (include) for each element in coords_2
-    order_1 : list
+    order_1: list
         list of new indices for coords_1 - applied BEFORE masking
-    order_2 : list
+    order_2: list
         list of new indices for coords_2 - applied BEFORE masking
 
     Returns
     -------
     float
         Root mean square of norms of deviation between two structures
     '''
@@ -1262,21 +1318,21 @@
 def rotate_coords(coords, alpha, beta, gamma):
     '''
     Rotates coordinates by alpha, beta, gamma using the zyz convention
     https://easyspin.org/easyspin/documentation/eulerangles.html
 
     Parameters
     ----------
-    coords : np.ndarray
+    coords: np.ndarray
         xyz coordinates as (n_atoms, 3) array
-    alpha : float
+    alpha: float
         alpha angle in radians
-    beta : float
+    beta: float
         beta  angle in radians
-    gamma : float
+    gamma: float
         gamma angle in radians
 
     Returns
     -------
     np.ndarray
         xyz coordinates as (n_atoms, 3) array after rotation
         in same order as input coordinates
@@ -1315,25 +1371,25 @@
     If coords_1 and coords_2 are not the same length, then a mask array can be
     provided for either/both and is applied prior to the calculation
     coords_1 and coords_2 can also be reordered if new orders are specified
     **note reordering occurs before masking**
 
     Parameters
     ----------
-    coords_1 : np.ndarray
+    coords_1: np.ndarray
         xyz coordinates as (n_atoms, 3) array
-    coords_2 : np.ndarray
+    coords_2: np.ndarray
         xyz coordinates as (n_atoms, 3) array
-    mask_1 : list[int]
+    mask_1: list[int]
         0 (exclude) or 1 (include) for each element in coords_1
-    mask_2 : list[int]
+    mask_2: list[int]
         0 (exclude) or 1 (include) for each element in coords_2
-    order_1 : list[int]
+    order_1: list[int]
         new indices for coords_1 - applied BEFORE masking
-    order_2 : list[int]
+    order_2: list[int]
         new indices for coords_2 - applied BEFORE masking
 
     Returns
     -------
     float
         Root mean square of norms of deviation between two structures
     float
@@ -1387,19 +1443,19 @@
     '''
     Rotates coords_1 by alpha, beta, gamma using the zyz convention
     https://easyspin.org/easyspin/documentation/eulerangles.html
     then calcualtes the rmsd between coords_1 and coords_2
 
     Parameters
     ----------
-    coords_1 : np.ndarray
+    coords_1: np.ndarray
         xyz coordinates as (n_atoms, 3) array of first system
-    coords_2 : np.ndarray
+    coords_2: np.ndarray
         xyz coordinates as (n_atoms, 3) array of second system
-    angs : list[float]
+    angs: list[float]
         alpha, beta, gamma in radians
 
     Returns
     -------
     np.ndarray
         xyz coordinates as (n_atoms, 3) array after rotation
         in same order as input coordinates
@@ -1416,17 +1472,17 @@
 
 def calculate_com(labels, coords):
     '''
     Calculates centre-of-mass using relative atomic masses
 
     Parameters
     ----------
-    labels : list
+    labels: list
         list of atomic labels
-    coords : np.ndarray
+    coords: np.ndarray
         xyz coordinates as (n_atoms, 3) array
 
     Returns
     -------
     np.ndarray
         xyz coordinates of centre of mass as (3) array
     '''
```

### Comparing `xyz_py-5.6.1/xyz_py.egg-info/PKG-INFO` & `xyz_py-5.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xyz-py
-Version: 5.6.1
+Name: xyz_py
+Version: 5.7.0
 Summary: A package for manipulating xyz files and chemical structures
 Home-page: https://gitlab.com/jonkragskow/xyz_py
 Author: Jon Kragskow
 Author-email: jonkragskow@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/jonkragskow/xyz_py/-/issues
 Project-URL: Documentation, https://jonkragskow.gitlab.io/xyz_py
 Classifier: Programming Language :: Python :: 3
```

