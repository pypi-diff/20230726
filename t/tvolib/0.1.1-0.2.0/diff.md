# Comparing `tmp/tvolib-0.1.1.tar.gz` & `tmp/tvolib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvolib-0.1.1.tar", max compression
+gzip compressed data, was "tvolib-0.2.0.tar", max compression
```

## Comparing `tvolib-0.1.1.tar` & `tvolib-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-07-21 18:31:00.565627 tvolib-0.1.1/LICENSE
--rw-r--r--   0        0        0      328 2023-07-21 18:33:40.549771 tvolib-0.1.1/README.md
--rw-r--r--   0        0        0      714 2023-07-21 19:01:41.642711 tvolib-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-21 17:26:07.254703 tvolib-0.1.1/src/tvolib/__init__.py
--rw-r--r--   0        0        0      140 2023-07-21 17:59:10.962967 tvolib-0.1.1/src/tvolib/mpl_utils/__init__.py
--rw-r--r--   0        0        0     2067 2023-07-21 17:33:31.015512 tvolib-0.1.1/src/tvolib/mpl_utils/_draw.py
--rw-r--r--   0        0        0      526 2023-07-21 17:36:32.118900 tvolib-0.1.1/src/tvolib/mpl_utils/_format.py
--rw-r--r--   0        0        0      898 2023-07-21 17:59:57.220123 tvolib-0.1.1/src/tvolib/mpl_utils/_setup.py
--rw-r--r--   0        0        0    25742 2023-07-21 17:47:40.083899 tvolib-0.1.1/src/tvolib/mpl_utils/data/mpl_utils.mplstyle
--rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 tvolib-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-21 18:31:00.565627 tvolib-0.2.0/LICENSE
+-rw-r--r--   0        0        0      307 2023-07-25 22:43:23.561333 tvolib-0.2.0/README.md
+-rw-r--r--   0        0        0      714 2023-07-25 23:50:05.041765 tvolib-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 17:26:07.254703 tvolib-0.2.0/src/tvolib/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-25 19:48:55.445686 tvolib-0.2.0/src/tvolib/mpl_utils/__init__.py
+-rw-r--r--   0        0        0     2103 2023-07-25 19:51:46.873557 tvolib-0.2.0/src/tvolib/mpl_utils/_draw.py
+-rw-r--r--   0        0        0      526 2023-07-25 19:42:33.293735 tvolib-0.2.0/src/tvolib/mpl_utils/_format.py
+-rw-r--r--   0        0        0      898 2023-07-25 19:48:29.873412 tvolib-0.2.0/src/tvolib/mpl_utils/_setup.py
+-rw-r--r--   0        0        0    25742 2023-07-21 17:47:40.083899 tvolib-0.2.0/src/tvolib/mpl_utils/data/mpl_utils.mplstyle
+-rw-r--r--   0        0        0       83 2023-07-25 23:49:44.174619 tvolib-0.2.0/src/tvolib/numeric/__init__.py
+-rw-r--r--   0        0        0     1718 2023-07-25 23:49:09.022374 tvolib-0.2.0/src/tvolib/numeric/interpolate.py
+-rw-r--r--   0        0        0     1488 2023-07-25 22:45:58.568398 tvolib-0.2.0/src/tvolib/numeric/moving.py
+-rw-r--r--   0        0        0      572 2023-07-25 23:04:48.648666 tvolib-0.2.0/src/tvolib/numeric/timing.py
+-rw-r--r--   0        0        0     1201 1970-01-01 00:00:00.000000 tvolib-0.2.0/PKG-INFO
```

### Comparing `tvolib-0.1.1/LICENSE` & `tvolib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tvolib-0.1.1/pyproject.toml` & `tvolib-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tvolib"
-version = "0.1.1"
+version = "0.2.0"
 description = "A personal collection of Python and IDL research tools in Space Plasma Physics."
 authors = ["Tien Vo <tien.a.vo@proton.me>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 packages = [
     { include = "tvolib", from = "src" }
 ]
```

### Comparing `tvolib-0.1.1/src/tvolib/mpl_utils/_draw.py` & `tvolib-0.2.0/src/tvolib/mpl_utils/_draw.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 __all__ = [
     "draw_arrows",
     "draw_earth",
     "draw_multicolored_line",
 ]
 
+import numpy as np
 from matplotlib.collections import LineCollection
 from matplotlib.patches import FancyArrowPatch
 from matplotlib.colors import Normalize
-import numpy as np
 
 
 def draw_arrows(axis, x, y, N=None, color="k"):
-    r"""Draws arrows along a path on the axis"""
+    r"""Draws arrows along a path on the axis
+    """
     N = len(x) // 5 if N is None else N
     d = len(x) // (N + 1)
 
     idx = np.arange(d, len(x), d)
     for i in idx:
         ar = FancyArrowPatch(
             (x[i - 1], y[i - 1]),
@@ -24,15 +25,16 @@
             mutation_scale=20,
             color=color,
         )
         axis.add_patch(ar)
 
 
 def draw_earth(axis, R=1, N=50, zorder=999):
-    r"""Draws the Earth on the axis (with shading indicating day/night)"""
+    r"""Draws the Earth on the axis (with shading indicating day/night)
+    """
     # Nightside
     theta = np.linspace(np.pi / 2, 3 * np.pi / 2, N)
     Xn = R * np.cos(theta)
     Yn = R * np.sin(theta)
     Xn = np.append(Xn, Xn[0])
     Yn = np.append(Yn, Yn[0])
     # Dayside
@@ -44,18 +46,18 @@
     # Plot
     axis.plot(Xd, Yd, "-k", zorder=zorder)
     axis.plot(Xn, Yn, "-k", zorder=zorder)
     axis.fill(Xd, Yd, color="w")
     axis.fill(Xn, Yn, color="k")
 
 
-def draw_multicolored_line(
-    axis, x, y, c, cmap="jet", vmin=None, vmax=None, set_lim=False, **kwargs
-):
-    r"""Draws a line with colors on a scale determined by c"""
+def draw_multicolored_line(axis, x, y, c, cmap="jet",
+                           vmin=None, vmax=None, set_lim=False, **kwargs):
+    r"""Draws a line with colors on a scale determined by c
+    """
 
     vmin = c.min() if vmin is None else vmin
     vmax = c.max() if vmax is None else vmax
 
     points = np.array([x, y]).T.reshape(-1, 1, 2)
     segments = np.concatenate([points[:-1], points[1:]], axis=1)
     norm = Normalize(vmin, vmax)
```

### Comparing `tvolib-0.1.1/src/tvolib/mpl_utils/_format.py` & `tvolib-0.2.0/src/tvolib/mpl_utils/_format.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __all__ = [
     "add_colorbar",
     "format_datetime_axis",
 ]
 
-from mpl_toolkits.axes_grid1 import make_axes_locatable
 import matplotlib.dates as mdates
+from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 
 def add_colorbar(axis, where="right", pad=0.05, size="2%"):
     r"""Adds colorbar next to an axis"""
     divider = make_axes_locatable(axis)
     return divider.append_axes(where, size=size, pad=pad)
```

### Comparing `tvolib-0.1.1/src/tvolib/mpl_utils/_setup.py` & `tvolib-0.2.0/src/tvolib/mpl_utils/_setup.py`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 __all__ = ["setup"]
 
-from importlib.resources import files
-import matplotlib.pyplot as plt
-import matplotlib as mpl
 import tempfile
 import atexit
 import shutil
 import os
+import matplotlib.pyplot as plt
+import matplotlib as mpl
+from importlib.resources import files
 
 
 def _checkdep_usetex(s):
     return s and shutil.which("tex")
 
 
 def setup(tex=False, cache=False, **kw):
```

### Comparing `tvolib-0.1.1/src/tvolib/mpl_utils/data/mpl_utils.mplstyle` & `tvolib-0.2.0/src/tvolib/mpl_utils/data/mpl_utils.mplstyle`

 * *Files identical despite different names*

### Comparing `tvolib-0.1.1/PKG-INFO` & `tvolib-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvolib
-Version: 0.1.1
+Version: 0.2.0
 Summary: A personal collection of Python and IDL research tools in Space Plasma Physics.
 Home-page: https://github.com/tien-vo/tvolib
 License: GPL-3.0-or-later
 Author: Tien Vo
 Author-email: tien.a.vo@proton.me
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -19,18 +19,18 @@
 Requires-Dist: numpy
 Requires-Dist: scipy
 Project-URL: Repository, https://github.com/tien-vo/tvolib
 Description-Content-Type: text/markdown
 
 # About
 
-This is a personal collection of Python and IDL routines for my research in Space Plasma Physics, organized
-into packages. Some are more well-documented than others. Please use them at your discretion.
+This is a personal collection of Python and IDL routines for my research
+in Space Plasma Physics, organized into packages. Some are more
+well-documented than others. Please use them at your discretion.
 
 ## Installation
 
+Ensure `micromamba` is recognized in PATH. Then just run
 ```
-conda create --name tvolib --file conda-linux-64.lock
-conda activate tvolib
-poetry install
+make install
 ```
```

