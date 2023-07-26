# Comparing `tmp/tad_dftd3-0.1.3.tar.gz` & `tmp/tad_dftd3-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tad_dftd3-0.1.3.tar", last modified: Thu Jun 22 14:13:53 2023, max compression
+gzip compressed data, was "tad_dftd3-0.1.4.tar", last modified: Wed Jul 26 06:04:17 2023, max compression
```

## Comparing `tad_dftd3-0.1.3.tar` & `tad_dftd3-0.1.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:53.497841 tad_dftd3-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-06-22 14:13:53.497841 tad_dftd3-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-22 14:13:53.501841 tad_dftd3-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:53.493842 tad_dftd3-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:53.497841 tad_dftd3-0.1.3/src/tad_dftd3/
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:53.497841 tad_dftd3-0.1.3/src/tad_dftd3/damping/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/damping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/damping/atm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/damping/rational.py
--rw-r--r--   0 runner    (1001) docker     (123)    75725 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/disp.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/ncoord.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   893128 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/reference-c6.npy
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:53.497841 tad_dftd3-0.1.3/src/tad_dftd3/util/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/util/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/util/grad.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/src/tad_dftd3/util/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:53.497841 tad_dftd3-0.1.3/src/tad_dftd3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-06-22 14:13:53.000000 tad_dftd3-0.1.3/src/tad_dftd3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-22 14:13:53.000000 tad_dftd3-0.1.3/src/tad_dftd3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:13:53.000000 tad_dftd3-0.1.3/src/tad_dftd3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-22 14:13:53.000000 tad_dftd3-0.1.3/src/tad_dftd3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 14:13:53.000000 tad_dftd3-0.1.3/src/tad_dftd3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:13:53.497841 tad_dftd3-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/tests/test_dftd3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/tests/test_disp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-22 14:13:44.000000 tad_dftd3-0.1.3/tests/test_ncoord.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:17.908684 tad_dftd3-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-07-26 06:04:17.908684 tad_dftd3-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-26 06:04:17.908684 tad_dftd3-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:17.896684 tad_dftd3-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:17.904684 tad_dftd3-0.1.4/src/tad_dftd3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:17.904684 tad_dftd3-0.1.4/src/tad_dftd3/damping/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/damping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/damping/atm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/damping/rational.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75727 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/ncoord.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   893128 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/reference-c6.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:17.904684 tad_dftd3-0.1.4/src/tad_dftd3/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/util/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/util/grad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/src/tad_dftd3/util/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:17.904684 tad_dftd3-0.1.4/src/tad_dftd3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-07-26 06:04:17.000000 tad_dftd3-0.1.4/src/tad_dftd3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-26 06:04:17.000000 tad_dftd3-0.1.4/src/tad_dftd3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 06:04:17.000000 tad_dftd3-0.1.4/src/tad_dftd3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-26 06:04:17.000000 tad_dftd3-0.1.4/src/tad_dftd3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 06:04:17.000000 tad_dftd3-0.1.4/src/tad_dftd3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 06:04:17.908684 tad_dftd3-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/tests/test_dftd3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/tests/test_disp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-26 06:04:08.000000 tad_dftd3-0.1.4/tests/test_ncoord.py
```

### Comparing `tad_dftd3-0.1.3/LICENSE` & `tad_dftd3-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.3/PKG-INFO` & `tad_dftd3-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad_dftd3
-Version: 0.1.3
+Version: 0.1.4
 Summary: Torch autodiff DFT-D3 implementation
 License: Apache-2.0
 Project-URL: Documentation, https://tad-dftd3.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/dftd3/tad-dftd3
 Project-URL: Tracker, https://github.com/dftd3/tad-dftd3/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tad_dftd3-0.1.3/README.rst` & `tad_dftd3-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.3/pyproject.toml` & `tad_dftd3-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.3/setup.cfg` & `tad_dftd3-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.3/setup.py` & `tad_dftd3-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/__init__.py` & `tad_dftd3-0.1.4/src/tad_dftd3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 tensor([-0.0124292, -0.0045002])
 >>> print(energy[0] - 2*energy[1])
 tensor(-0.0034288)
 """
 import torch
 
 from . import damping, data, disp, model, ncoord, reference
-from .typing import (
+from ._typing import (
     DD,
     CountingFunction,
     DampingFunction,
     Dict,
     Optional,
     Tensor,
     WeightingFunction,
```

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/__version__.py` & `tad_dftd3-0.1.4/src/tad_dftd3/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Version module for tad_dftd3.
 """
 import torch
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 __torch_version__ = torch.__version__
```

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/constants.py` & `tad_dftd3-0.1.4/src/tad_dftd3/constants.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/damping/__init__.py` & `tad_dftd3-0.1.4/src/tad_dftd3/damping/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/damping/atm.py` & `tad_dftd3-0.1.4/src/tad_dftd3/damping/atm.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     {\left(r_\text{AB} r_\text{BC} r_\text{AC} \right)^3} \\
     f_\text{damp} &=
     \dfrac{1}{1+ 6 \left(\overline{R}_\text{ABC}\right)^{-16}}
 """
 import torch
 
 from .. import defaults
-from ..typing import DD, Tensor
+from .._typing import DD, Tensor
 from ..util import cdist, real_pairs, real_triples
 
 
 def dispersion_atm(
     numbers: Tensor,
     positions: Tensor,
     c6: Tensor,
@@ -80,17 +80,19 @@
     rs9 = rs9.type(positions.dtype).to(positions.device)
     alp = alp.type(positions.dtype).to(positions.device)
 
     cutoff2 = cutoff * cutoff
     srvdw = rs9 * rvdw
 
     mask_pairs = real_pairs(numbers, diagonal=False)
-    mask_triples = real_triples(numbers, diagonal=False)
+    mask_triples = real_triples(numbers, self=False)
 
     eps = torch.tensor(torch.finfo(positions.dtype).eps, **dd)
+    zero = torch.tensor(0.0, **dd)
+    one = torch.tensor(1.0, **dd)
 
     # C9_ABC = s9 * sqrt(|C6_AB * C6_AC * C6_BC|)
     c9 = s9 * torch.sqrt(
         torch.clamp(
             torch.abs(c6.unsqueeze(-1) * c6.unsqueeze(-2) * c6.unsqueeze(-3)), min=eps
         )
     )
@@ -116,17 +118,33 @@
     r2jk = distances.unsqueeze(-3)
     r2 = r2ij * r2ik * r2jk
     r1 = torch.sqrt(r2)
     # add epsilon to avoid zero division later
     r3 = torch.where(mask_triples, r1 * r2, eps)
     r5 = torch.where(mask_triples, r2 * r3, eps)
 
-    fdamp = 1.0 / (1.0 + 6.0 * (r0 / r1) ** ((alp + 2.0) / 3.0))
+    # dividing by tiny numbers leads to huge numbers, which result in NaN's
+    # upon exponentiation in the subsequent step
+    mask = real_triples(numbers, self=False)
+    base = r0 / torch.where(mask_triples, r1, one)
+
+    # to fix the previous mask, we mask again (not strictly necessary because
+    # `ang` is also masked and we later multiply with `ang`)
+    fdamp = torch.where(
+        mask_triples,
+        1.0 / (1.0 + 6.0 * base ** ((alp + 2.0) / 3.0)),
+        zero,
+    )
+
+    s = torch.where(
+        mask,
+        (r2ij + r2jk - r2ik) * (r2ij - r2jk + r2ik) * (-r2ij + r2jk + r2ik),
+        zero,
+    )
 
-    s = (r2ij + r2jk - r2ik) * (r2ij - r2jk + r2ik) * (-r2ij + r2jk + r2ik)
     ang = torch.where(
         mask_triples * (r2ij <= cutoff2) * (r2jk <= cutoff2) * (r2jk <= cutoff2),
         0.375 * s / r5 + 1.0 / r3,
         torch.tensor(0.0, **dd),
     )
 
     energy = ang * fdamp * c9
```

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/damping/rational.py` & `tad_dftd3-0.1.4/src/tad_dftd3/damping/rational.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     f^n_{\text{damp}}\left(R_0^{\text{AB}}\right) =
     \dfrac{R^n_{\text{AB}}}{R^n_{\text{AB}} +
     \left( a_1 R_0^{\text{AB}} + a_2 \right)^n}
 """
 import torch
 
 from .. import defaults
-from ..typing import DD, Dict, Tensor
+from .._typing import DD, Dict, Tensor
 
 
 def rational_damping(
     order: int,
     distances: Tensor,
     qq: Tensor,
     param: Dict[str, Tensor],
```

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/data.py` & `tad_dftd3-0.1.4/src/tad_dftd3/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ===========
 
 Data arrays for atomic constants like covalent radii or van-der-Waals radii.
 """
 import torch
 
 from . import constants
-from .typing import Tensor
+from ._typing import Tensor
 
 # fmt: off
 covalent_rad_2009 = constants.ANGSTROM_TO_BOHR * torch.tensor([
     0.00,  # None
     0.32,0.46,  # H,He
     1.20,0.94,0.77,0.75,0.71,0.63,0.64,0.67,  # Li-Ne
     1.40,1.25,1.13,1.04,1.10,1.02,0.99,0.96,  # Na-Ar
@@ -4565,15 +4565,15 @@
         4.3462,
         4.3265,
         4.4341,
     ]
 )  # fmt: off
 
 
-def _load_vdw_rad_d3(dtype: torch.dtype = torch.float) -> Tensor:
+def _load_vdw_rad_d3(dtype: torch.dtype = torch.double) -> Tensor:
     # pylint: disable=import-outside-toplevel
     import math
 
     n_element = (math.isqrt(8 * _vdw_rad_d3.shape[0] + 1) - 1) // 2
 
     rad = torch.zeros((n_element, n_element), dtype=dtype)
     for i in range(1, n_element):
```

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/defaults.py` & `tad_dftd3-0.1.4/src/tad_dftd3/defaults.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/disp.py` & `tad_dftd3-0.1.4/src/tad_dftd3/disp.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 >>> torch.set_printoptions(precision=7)
 >>> print(torch.sum(energy[0] - energy[1] - energy[2]))  # energy in Hartree
 tensor(-0.0003964)
 """
 import torch
 
 from . import data, defaults
+from ._typing import DD, Any, DampingFunction, Dict, Optional, Tensor
 from .damping import dispersion_atm, rational_damping
-from .typing import DD, Any, DampingFunction, Dict, Optional, Tensor
 from .util import cdist, real_pairs
 
 
 def dispersion(
     numbers: Tensor,
     positions: Tensor,
     param: Dict[str, Tensor],
```

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/exception.py` & `tad_dftd3-0.1.4/src/tad_dftd3/exception.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/model.py` & `tad_dftd3-0.1.4/src/tad_dftd3/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,24 +37,20 @@
 >>> print(c6)
 tensor([[10.4130478,  5.4368815,  5.4368815],
         [ 5.4368811,  3.0930152,  3.0930152],
         [ 5.4368811,  3.0930152,  3.0930152]])
 """
 import torch
 
+from ._typing import Any, Tensor, WeightingFunction
 from .reference import Reference
-from .typing import Any, Tensor, WeightingFunction
 from .util import real_atoms
 
 
-def atomic_c6(
-    numbers: Tensor,
-    weights: Tensor,
-    reference: Reference,
-) -> Tensor:
+def atomic_c6(numbers: Tensor, weights: Tensor, reference: Reference) -> Tensor:
     """
     Calculate atomic dispersion coefficients.
 
     Parameters
     ----------
     numbers : Tensor
         The atomic numbers of the atoms in the system.
@@ -128,19 +124,19 @@
 
     # Due to the exponentiation, `norms` and `weights` may become very small.
     # This may cause problems for the division by `norms`. It may occur that
     # `weights` and `norms` are equal, in which case the result should be
     # exactly one. This might, however, not be the case and ultimately cause
     # larger deviations in the final values.
     #
-    # If the values become even smaller, we may have to evaluate this portion
-    # in double precision to retain the correct results. This must be done in
-    # the D4 variant because the weighting functions contains higher powers,
-    # which lead to values down to 1e-300.
-    dcn = reference.cn[numbers] - cn.unsqueeze(-1)
+    # This must be done in the D4 variant because the weighting functions
+    # contains higher powers, which lead to values down to 1e-300.
+    # Since there are also cases in D3, we have to evaluate this portion
+    # in double precision to retain the correct results and avoid nan's.
+    dcn = (reference.cn[numbers] - cn.unsqueeze(-1)).type(torch.double)
     weights = torch.where(
         mask,
         weighting_function(dcn, **kwargs),
         torch.tensor(0.0, device=dcn.device, dtype=dcn.dtype),  # not eps!
     )
 
     # Nevertheless, we must avoid zero division here in batched calculations.
@@ -155,8 +151,8 @@
     # We solve this issue by using a mask from the atoms and only add a small
     # value, where the actual padding zeros are.
     norms = torch.where(
         real_atoms(numbers),
         torch.sum(weights, dim=-1),
         torch.tensor(torch.finfo(dcn.dtype).eps, device=cn.device, dtype=dcn.dtype),
     )
-    return weights / norms.unsqueeze(-1)
+    return (weights / norms.unsqueeze(-1)).type(cn.dtype)
```

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/ncoord.py` & `tad_dftd3-0.1.4/src/tad_dftd3/ncoord.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 tensor([[2.9901006, 0.9977214, 0.9977214, 0.9977214, 0.0000000, 0.0000000],
         [3.0059586, 1.0318390, 3.0268824, 1.0061584, 1.0036336, 0.9989871],
         [3.0093639, 2.0046251, 1.0187057, 0.9978270, 1.0069743, 0.0000000]])
 """
 import torch
 
 from . import data
-from .typing import DD, Any, CountingFunction, Optional, Tensor
+from ._typing import DD, Any, CountingFunction, Optional, Tensor
 from .util import cdist, real_pairs
 
 
 def exp_count(r: Tensor, r0: Tensor, kcn: float = 16.0) -> Tensor:
     """
     Exponential counting function for coordination number contributions.
```

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/reference-c6.npy` & `tad_dftd3-0.1.4/src/tad_dftd3/reference-c6.npy`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/reference.py` & `tad_dftd3-0.1.4/src/tad_dftd3/reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 This module defines the reference systems for the D3 model to compute the
 C6 dispersion coefficients.
 """
 import os.path as op
 
 import torch
 
-from .typing import Any, NoReturn, Optional, Tensor
+from ._typing import Any, NoReturn, Optional, Tensor
 
 
 def _load_cn(
-    dtype: torch.dtype = torch.float, device: Optional[torch.device] = None
+    dtype: torch.dtype = torch.double, device: Optional[torch.device] = None
 ) -> Tensor:
     return torch.tensor(
         [
             [-1.0000, -1.0000, -1.0000, -1.0000, -1.0000],  # None
             [+0.9118, +0.0000, -1.0000, -1.0000, -1.0000],  # H
             [+0.0000, -1.0000, -1.0000, -1.0000, -1.0000],  # He
             [+0.0000, +0.9865, -1.0000, -1.0000, -1.0000],  # Li
@@ -129,15 +129,15 @@
         ],
         device=device,
         dtype=dtype,
     )
 
 
 def _load_c6(
-    dtype: torch.dtype = torch.float, device: Optional[torch.device] = None
+    dtype: torch.dtype = torch.double, device: Optional[torch.device] = None
 ) -> Tensor:
     """
     Load reference C6 coefficients from file and fill them into a tensor
     """
 
     # pylint: disable=import-outside-toplevel
     import math
@@ -146,15 +146,15 @@
 
     path = op.join(op.dirname(__file__), "reference-c6.npy")
     ref = torch.from_numpy(np.load(path)).type(dtype).to(device)
 
     n_element = (math.isqrt(8 * ref.shape[0] + 1) - 1) // 2 + 1
     n_reference = ref.shape[-1]
     c6 = torch.zeros(
-        (n_element, n_element, n_reference, n_reference), dtype=dtype, device=device
+        (n_element, n_element, n_reference, n_reference), dtype=ref.dtype, device=device
     )
 
     for i in range(1, n_element):
         for j in range(1, n_element):
             ij = i * (i - 1) // 2 + j - 1 if j < i else j * (j - 1) // 2 + i - 1
             c6[i, j, :, :] = ref[ij, :, :].T if j < i else ref[ij, :, :]
 
@@ -184,22 +184,21 @@
         cn: Optional[Tensor] = None,
         c6: Optional[Tensor] = None,
         device: Optional[torch.device] = None,
         dtype: Optional[torch.dtype] = None,
     ):
         if cn is None:
             cn = _load_cn(
-                dtype if dtype is not None else torch.float,
+                dtype=dtype if dtype is not None else torch.double,
                 device=device,
             )
         self.cn = cn
         if c6 is None:
             c6 = _load_c6(
-                dtype if dtype is not None else torch.float,
-                device=device,
+                dtype=dtype if dtype is not None else torch.double, device=device
             )
         self.c6 = c6
 
         self.__dtype = self.c6.dtype
         self.__device = self.c6.device
 
         if any(tensor.device != self.device for tensor in (self.cn, self.c6)):
```

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/typing.py` & `tad_dftd3-0.1.4/src/tad_dftd3/_typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     NoReturn,
     Optional,
+    Protocol,
     Tuple,
     TypedDict,
     Union,
 )
 
 import torch
 from torch import Tensor
```

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/util/distance.py` & `tad_dftd3-0.1.4/src/tad_dftd3/util/distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 Utility functions: Distance
 ===========================
 
 Functions for calculating the cartesian distance of two vectors.
 """
 import torch
 
-from ..typing import Optional, Tensor
+from .._typing import Optional, Tensor
 
 __all__ = ["cdist"]
 
 
 def euclidean_dist_quadratic_expansion(x: Tensor, y: Tensor) -> Tensor:
     """
     Computation of euclidean distance matrix via quadratic expansion (sum of
```

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/util/grad.py` & `tad_dftd3-0.1.4/src/tad_dftd3/util/grad.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ===========================
 
 Utilities for calculating gradients and Hessians.
 """
 import torch
 
 from ..__version__ import __torch_version__
-from ..typing import Any, Callable, Tensor, Tuple
+from .._typing import Any, Callable, Tensor, Tuple
 
 __all__ = ["jac", "hessian"]
 
 
 if __torch_version__ < (2, 0, 0):  # type: ignore # pragma: no cover
     try:
         from functorch import jacrev  # type: ignore
```

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3/util/misc.py` & `tad_dftd3-0.1.4/src/tad_dftd3/util/misc.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,36 +17,97 @@
 =======================
 
 Utilities for working with tensors as well as translating between element
 symbols and atomic numbers.
 """
 import torch
 
-from ..typing import List, Optional, Size, Tensor, TensorOrTensors, Union
+from .._typing import List, Optional, Size, Tensor, TensorOrTensors, Union
 
 __all__ = ["real_atoms", "real_pairs", "real_triples", "pack", "to_number"]
 
 
 def real_atoms(numbers: Tensor) -> Tensor:
+    """
+    Create a mask for atoms, discerning padding and actual atoms.
+    Padding value is zero.
+
+    Parameters
+    ----------
+    numbers : Tensor
+        Atomic numbers for all atoms.
+
+    Returns
+    -------
+    Tensor
+        Mask for atoms that discerns padding and real atoms.
+    """
     return numbers != 0
 
 
 def real_pairs(numbers: Tensor, diagonal: bool = False) -> Tensor:
+    """
+    Create a mask for pairs of atoms from atomic numbers, discerning padding
+    and actual atoms. Padding value is zero.
+
+    Parameters
+    ----------
+    numbers : Tensor
+        Atomic numbers for all atoms.
+    diagonal : bool, optional
+        Flag for also writing `False` to the diagonal, i.e., to all pairs
+        with the same indices. Defaults to `False`, i.e., writing False
+        to the diagonal.
+
+    Returns
+    -------
+    Tensor
+        Mask for atom pairs that discerns padding and real atoms.
+    """
     real = real_atoms(numbers)
     mask = real.unsqueeze(-2) * real.unsqueeze(-1)
     if diagonal is False:
         mask *= ~torch.diag_embed(torch.ones_like(real))
     return mask
 
 
-def real_triples(numbers: Tensor, diagonal: bool = False) -> Tensor:
+def real_triples(
+    numbers: torch.Tensor, diagonal: bool = False, self: bool = True
+) -> Tensor:
+    """
+    Create a mask for triples from atomic numbers. Padding value is zero.
+
+    Parameters
+    ----------
+    numbers : torch.Tensor
+        Atomic numbers for all atoms.
+    diagonal : bool, optional
+        Flag for also writing `False` to the space diagonal, i.e., to all
+        triples with the same indices. Defaults to `False`, i.e., writing False
+        to the diagonal.
+    self : bool, optional
+        Flag for also writing `False` to all triples where at least two indices
+        are identical. Defaults to `True`, i.e., not writing `False`.
+
+    Returns
+    -------
+    Tensor
+        Mask for triples.
+    """
     real = real_pairs(numbers, diagonal=True)
     mask = real.unsqueeze(-3) * real.unsqueeze(-2) * real.unsqueeze(-1)
+
     if diagonal is False:
         mask *= ~torch.diag_embed(torch.ones_like(real))
+
+    if self is False:
+        mask *= ~torch.diag_embed(torch.ones_like(real), offset=0, dim1=-3, dim2=-2)
+        mask *= ~torch.diag_embed(torch.ones_like(real), offset=0, dim1=-3, dim2=-1)
+        mask *= ~torch.diag_embed(torch.ones_like(real), offset=0, dim1=-2, dim2=-1)
+
     return mask
 
 
 def pack(
     tensors: TensorOrTensors,
     axis: int = 0,
     value: Union[int, float] = 0,
```

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3.egg-info/PKG-INFO` & `tad_dftd3-0.1.4/src/tad_dftd3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tad-dftd3
-Version: 0.1.3
+Version: 0.1.4
 Summary: Torch autodiff DFT-D3 implementation
 License: Apache-2.0
 Project-URL: Documentation, https://tad-dftd3.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/dftd3/tad-dftd3
 Project-URL: Tracker, https://github.com/dftd3/tad-dftd3/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tad_dftd3-0.1.3/src/tad_dftd3.egg-info/SOURCES.txt` & `tad_dftd3-0.1.4/src/tad_dftd3.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 LICENSE
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 src/tad_dftd3/__init__.py
 src/tad_dftd3/__version__.py
+src/tad_dftd3/_typing.py
 src/tad_dftd3/constants.py
 src/tad_dftd3/data.py
 src/tad_dftd3/defaults.py
 src/tad_dftd3/disp.py
 src/tad_dftd3/exception.py
 src/tad_dftd3/model.py
 src/tad_dftd3/ncoord.py
 src/tad_dftd3/py.typed
 src/tad_dftd3/reference-c6.npy
 src/tad_dftd3/reference.py
-src/tad_dftd3/typing.py
 src/tad_dftd3.egg-info/PKG-INFO
 src/tad_dftd3.egg-info/SOURCES.txt
 src/tad_dftd3.egg-info/dependency_links.txt
 src/tad_dftd3.egg-info/requires.txt
 src/tad_dftd3.egg-info/top_level.txt
 src/tad_dftd3/damping/__init__.py
 src/tad_dftd3/damping/atm.py
```

### Comparing `tad_dftd3-0.1.3/tests/test_dftd3.py` & `tad_dftd3-0.1.4/tests/test_dftd3.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.3/tests/test_disp.py` & `tad_dftd3-0.1.4/tests/test_disp.py`

 * *Files identical despite different names*

### Comparing `tad_dftd3-0.1.3/tests/test_model.py` & `tad_dftd3-0.1.4/tests/test_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
 
 def test_reference_fail() -> None:
     c6 = reference._load_c6()  # pylint: disable=protected-access
 
     # wrong dtype
     with pytest.raises(RuntimeError):
-        reference.Reference(c6=c6.type(torch.float64))
+        reference.Reference(c6=c6.type(torch.float16))
 
     # wrong device
     if torch.cuda.is_available() is True:
         with pytest.raises(RuntimeError):
             reference.Reference(c6=c6.to(torch.device("cuda")))
 
     # wrong shape
@@ -168,9 +168,9 @@
         reference.Reference(
             cn=torch.rand((4, 4), dtype=torch.float32),
             c6=c6.type(torch.float32),
         )
 
     assert (
         repr(reference.Reference())
-        == "Reference(n_element=95, n_reference=5, dtype=torch.float32, device=cpu)"
+        == "Reference(n_element=95, n_reference=5, dtype=torch.float64, device=cpu)"
     )
```

### Comparing `tad_dftd3-0.1.3/tests/test_ncoord.py` & `tad_dftd3-0.1.4/tests/test_ncoord.py`

 * *Files identical despite different names*

