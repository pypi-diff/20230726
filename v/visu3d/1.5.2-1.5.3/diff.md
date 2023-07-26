# Comparing `tmp/visu3d-1.5.2.tar.gz` & `tmp/visu3d-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visu3d-1.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "visu3d-1.5.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `visu3d-1.5.2.tar` & `visu3d-1.5.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-06-29 09:54:22.492458 visu3d-1.5.2/LICENSE
--rw-r--r--   0        0        0     4774 2023-06-29 09:54:22.492458 visu3d-1.5.2/README.md
--rw-r--r--   0        0        0     1868 2023-06-29 09:54:22.548459 visu3d-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     1811 2023-06-29 09:54:22.548459 visu3d-1.5.2/visu3d/__init__.py
--rw-r--r--   0        0        0     2257 2023-06-29 09:54:22.548459 visu3d-1.5.2/visu3d/array_dataclass.py
--rw-r--r--   0        0        0     7000 2023-06-29 09:54:22.548459 visu3d-1.5.2/visu3d/dc_arrays/camera.py
--rw-r--r--   0        0        0    13254 2023-06-29 09:54:22.548459 visu3d-1.5.2/visu3d/dc_arrays/camera_spec.py
--rw-r--r--   0        0        0     4890 2023-06-29 09:54:22.548459 visu3d-1.5.2/visu3d/dc_arrays/point.py
--rw-r--r--   0        0        0     4401 2023-06-29 09:54:22.548459 visu3d-1.5.2/visu3d/dc_arrays/ray.py
--rw-r--r--   0        0        0    17201 2023-06-29 09:54:22.548459 visu3d-1.5.2/visu3d/dc_arrays/transformation.py
--rw-r--r--   0        0        0     1301 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/math/__init__.py
--rw-r--r--   0        0        0     2980 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/math/coord_utils.py
--rw-r--r--   0        0        0     3523 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/math/interp_utils.py
--rw-r--r--   0        0        0     1259 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/math/math_utils.py
--rw-r--r--   0        0        0     7449 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/math/rotation_utils.py
--rw-r--r--   0        0        0     1245 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/plotly/__init__.py
--rw-r--r--   0        0        0     1674 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/plotly/auto_plot.py
--rw-r--r--   0        0        0     4080 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/plotly/fig_config_utils.py
--rw-r--r--   0        0        0    17401 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/plotly/fig_utils.py
--rw-r--r--   0        0        0     2018 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/plotly/traces_builder.py
--rw-r--r--   0        0        0      584 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/utils/__init__.py
--rw-r--r--   0        0        0      777 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/utils/file_utils.py
--rw-r--r--   0        0        0     1281 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/utils/lazy_imports.py
--rw-r--r--   0        0        0     3632 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/utils/np_utils.py
--rw-r--r--   0        0        0     2122 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/utils/py_utils.py
--rw-r--r--   0        0        0     6224 1970-01-01 00:00:00.000000 visu3d-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 16:05:34.775795 visu3d-1.5.3/LICENSE
+-rw-r--r--   0        0        0     5069 2023-07-26 16:05:34.775795 visu3d-1.5.3/README.md
+-rw-r--r--   0        0        0     2020 2023-07-26 16:05:34.843795 visu3d-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1792 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/__init__.py
+-rw-r--r--   0        0        0     2257 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/array_dataclass.py
+-rw-r--r--   0        0        0     7000 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/dc_arrays/camera.py
+-rw-r--r--   0        0        0    13254 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/dc_arrays/camera_spec.py
+-rw-r--r--   0        0        0     4890 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/dc_arrays/point.py
+-rw-r--r--   0        0        0     4401 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/dc_arrays/ray.py
+-rw-r--r--   0        0        0    17156 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/dc_arrays/transformation.py
+-rw-r--r--   0        0        0     1301 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/math/__init__.py
+-rw-r--r--   0        0        0     2980 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/math/coord_utils.py
+-rw-r--r--   0        0        0     3523 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/math/interp_utils.py
+-rw-r--r--   0        0        0     1259 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/math/math_utils.py
+-rw-r--r--   0        0        0     7449 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/math/rotation_utils.py
+-rw-r--r--   0        0        0     1245 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/plotly/__init__.py
+-rw-r--r--   0        0        0     1674 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/plotly/auto_plot.py
+-rw-r--r--   0        0        0     4080 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/plotly/fig_config_utils.py
+-rw-r--r--   0        0        0    17401 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/plotly/fig_utils.py
+-rw-r--r--   0        0        0     2018 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/plotly/traces_builder.py
+-rw-r--r--   0        0        0      584 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/utils/__init__.py
+-rw-r--r--   0        0        0      777 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/utils/file_utils.py
+-rw-r--r--   0        0        0     1281 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/utils/lazy_imports.py
+-rw-r--r--   0        0        0     3632 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/utils/np_utils.py
+-rw-r--r--   0        0        0     2122 2023-07-26 16:05:34.843795 visu3d-1.5.3/visu3d/utils/py_utils.py
+-rw-r--r--   0        0        0     6830 1970-01-01 00:00:00.000000 visu3d-1.5.3/PKG-INFO
```

### Comparing `visu3d-1.5.2/LICENSE` & `visu3d-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/README.md` & `visu3d-1.5.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # visu3d - 3D geometry made easy
 
 [![Unittests](https://github.com/google-research/visu3d/actions/workflows/pytest_and_autopublish.yml/badge.svg)](https://github.com/google-research/visu3d/actions/workflows/pytest_and_autopublish.yml)
 [![PyPI version](https://badge.fury.io/py/visu3d.svg)](https://badge.fury.io/py/visu3d)
+[![Documentation Status](https://readthedocs.org/projects/visu3d/badge/?version=latest)](https://visu3d.readthedocs.io/en/latest/?badge=latest)
 
 `visu3d` is an abstraction layer between Torch/TF/Jax/Numpy and your program.
 It provides:
 
 *   Standard primitives for 3d geometry (`Ray`, `Camera`, `Transform`,...).
     You can combine those standard primitives with your custom ones.
 *   Everything is trivially visualizable with zero boilerplate. Inspect & debug
@@ -144,21 +145,21 @@
 <!-- See [the tutorial]() for more info. -->
 
 </section>
 
 ### Documentation
 
 The best way to get started is to try the Colab tutorials (in the
-[docs/](https://github.com/google-research/visu3d/tree/main/docs/)):
+[documentation](https://visu3d.readthedocs.io/)):
 
-*   [Intro (Colab)](https://colab.research.google.com/github/google-research/visu3d/blob/main/docs/intro.ipynb)
+*   [Intro](https://visu3d.readthedocs.io/en/latest/intro.html) ([Colab](https://colab.research.google.com/github/google-research/visu3d/blob/main/docs/intro.ipynb))
     <!-- {.external} !-->
-*   [Transform (Colab)](https://colab.research.google.com/github/google-research/visu3d/blob/main/docs/transform.ipynb)
+*   [Transform](https://visu3d.readthedocs.io/en/latest/transform.html) ([Colab](https://colab.research.google.com/github/google-research/visu3d/blob/main/docs/transform.ipynb))
     <!-- {.external} !-->
-*   [Create your primitives (Colab)](https://colab.research.google.com/github/google-research/visu3d/blob/main/docs/dataclass.ipynb)
+*   [Create your primitives](https://visu3d.readthedocs.io/en/latest/dataclass.html) ([Colab](https://colab.research.google.com/github/google-research/visu3d/blob/main/docs/dataclass.ipynb))
     <!-- {.external} !-->
 
 Installation:
 
 ```sh
 pip install visu3d
 ```
```

### Comparing `visu3d-1.5.2/pyproject.toml` & `visu3d-1.5.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -34,33 +34,39 @@
 
 # This is set automatically by flit using `etils.__version__`
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://github.com/google-research/visu3d"
 repository = "https://github.com/google-research/visu3d"
+documentation = "https://visu3d.readthedocs.io"
+changelog = "https://github.com/google-research/visu3d/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
 dev = [
     "pytest>=3.4",
     "pytest-xdist",
     # Development deps (linting, formating,...)
     "pylint>=2.6.0",
     "pyink",
     # Lazy deps
     "chex",
     "jax[cpu]",
     "jupyter",
-    # TODO(epot): Restore "tf-nightly", it create segfault during tests
-    "tensorflow",
+    "tf-nightly",
     "tensorflow_datasets",
     "torch",
     "plotly",
     "scipy",
 ]
+docs = [
+    "sphinx-apitree[ext]",
+    "visu3d[dev]",  # Install lazy deps
+    "scipy>=1.10",
+]
 
 [tool.pyink]
 # Formatting configuration to follow Google style-guide
 line-length = 80
 preview = true
 pyink-indentation = 2
 pyink-use-majority-quotes = true
```

### Comparing `visu3d-1.5.2/visu3d/__init__.py` & `visu3d-1.5.3/visu3d/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Visu3d API."""
 
 from __future__ import annotations
 
-# pylint: disable=g-import-not-at-top,g-bad-import-order
+# pylint: disable=g-import-not-at-top,g-bad-import-order,g-importing-member
 
 # Core API
 from visu3d.array_dataclass import DataclassArray
-from visu3d.utils import lazy_imports
 
 from visu3d import math
 from visu3d.math import DEG2RAD
 from visu3d.math import RAD2DEG
 
 # Visualization
 from visu3d import plotly
@@ -45,8 +44,8 @@
 from visu3d.dc_arrays.transformation import custom_transform
 from visu3d.dc_arrays.transformation import Transform
 
 # Updating this will auto-trigger a release on PyPI and GitHub
 # Note:
 # * Make sure to also update the `CHANGELOG.md` before this.
 # * Make sure to also trigger an `etils` release
-__version__ = '1.5.2'
+__version__ = '1.5.3'
```

### Comparing `visu3d-1.5.2/visu3d/array_dataclass.py` & `visu3d-1.5.3/visu3d/array_dataclass.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/dc_arrays/camera.py` & `visu3d-1.5.3/visu3d/dc_arrays/camera.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/dc_arrays/camera_spec.py` & `visu3d-1.5.3/visu3d/dc_arrays/camera_spec.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/dc_arrays/point.py` & `visu3d-1.5.3/visu3d/dc_arrays/point.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/dc_arrays/ray.py` & `visu3d-1.5.3/visu3d/dc_arrays/ray.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/dc_arrays/transformation.py` & `visu3d-1.5.3/visu3d/dc_arrays/transformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,36 +221,36 @@
           'Cannot get `Transform.scale` when x, y, z scale are '
           f'different: {self.scale_xyz}'
       )
 
     xnp = self.xnp
     scale_xyz = xnp.round(self.scale_xyz, decimals=7)
     # TODO(epot): Move into `enp.ops.unique`
-    if xnp is enp.lazy.np:
+    if enp.lazy.is_np_xnp(xnp):
       global_scales = xnp.unique(scale_xyz)
       raise_error = len(global_scales) != 1
-    elif enp.lazy.has_jax and xnp is enp.lazy.jnp:
+    elif enp.lazy.is_jax_xnp(xnp):
       global_scales, global_count = xnp.unique(
           scale_xyz,
           size=1,
           return_counts=True,
       )
 
       # Unfortunately, Jax don't have an easy API to conditionally
       # raise error within a `jax.jit` function
       # This won't have any effect when the function is traced.
       from jax.experimental import checkify  # pytype: disable=import-error  # pylint: disable=g-import-not-at-top
 
       checkify.check(global_count[0] == 3, msg=_err_msg())
 
       raise_error = False
-    elif enp.lazy.has_torch and xnp is enp.lazy.torch:
+    elif enp.lazy.is_torch_xnp(xnp):
       global_scales = enp.lazy.torch.unique(scale_xyz)
       raise_error = len(global_scales) != 1
-    elif enp.lazy.has_tf and xnp is enp.lazy.tnp:
+    elif enp.lazy.is_tf_xnp(xnp):
       global_scales, _ = enp.lazy.tf.unique(scale_xyz)
       raise_error = len(global_scales) != 1
     else:
       raise AssertionError(f'Unknown numpy module {xnp}')
     if raise_error:
       raise ValueError(_err_msg())
     else:
```

### Comparing `visu3d-1.5.2/visu3d/math/__init__.py` & `visu3d-1.5.3/visu3d/math/__init__.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/math/coord_utils.py` & `visu3d-1.5.3/visu3d/math/coord_utils.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/math/interp_utils.py` & `visu3d-1.5.3/visu3d/math/interp_utils.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/math/math_utils.py` & `visu3d-1.5.3/visu3d/math/math_utils.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/math/rotation_utils.py` & `visu3d-1.5.3/visu3d/math/rotation_utils.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/plotly/__init__.py` & `visu3d-1.5.3/visu3d/plotly/__init__.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/plotly/auto_plot.py` & `visu3d-1.5.3/visu3d/plotly/auto_plot.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/plotly/fig_config_utils.py` & `visu3d-1.5.3/visu3d/plotly/fig_config_utils.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/plotly/fig_utils.py` & `visu3d-1.5.3/visu3d/plotly/fig_utils.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/plotly/traces_builder.py` & `visu3d-1.5.3/visu3d/plotly/traces_builder.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/utils/__init__.py` & `visu3d-1.5.3/visu3d/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/utils/file_utils.py` & `visu3d-1.5.3/visu3d/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/utils/lazy_imports.py` & `visu3d-1.5.3/visu3d/utils/lazy_imports.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/utils/np_utils.py` & `visu3d-1.5.3/visu3d/utils/np_utils.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/visu3d/utils/py_utils.py` & `visu3d-1.5.3/visu3d/utils/py_utils.py`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.2/PKG-INFO` & `visu3d-1.5.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visu3d
-Version: 1.5.2
+Version: 1.5.3
 Summary: 3d geometry made easy.
 Keywords: 3d,visu3d,visualization,neural rendering,nerf
 Author-email: Visu3d team <visu3d@google.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -21,27 +21,34 @@
 Requires-Dist: pytest>=3.4 ; extra == "dev"
 Requires-Dist: pytest-xdist ; extra == "dev"
 Requires-Dist: pylint>=2.6.0 ; extra == "dev"
 Requires-Dist: pyink ; extra == "dev"
 Requires-Dist: chex ; extra == "dev"
 Requires-Dist: jax[cpu] ; extra == "dev"
 Requires-Dist: jupyter ; extra == "dev"
-Requires-Dist: tensorflow ; extra == "dev"
+Requires-Dist: tf-nightly ; extra == "dev"
 Requires-Dist: tensorflow_datasets ; extra == "dev"
 Requires-Dist: torch ; extra == "dev"
 Requires-Dist: plotly ; extra == "dev"
 Requires-Dist: scipy ; extra == "dev"
+Requires-Dist: sphinx-apitree[ext] ; extra == "docs"
+Requires-Dist: visu3d[dev] ; extra == "docs"
+Requires-Dist: scipy>=1.10 ; extra == "docs"
+Project-URL: changelog, https://github.com/google-research/visu3d/blob/main/CHANGELOG.md
+Project-URL: documentation, https://visu3d.readthedocs.io
 Project-URL: homepage, https://github.com/google-research/visu3d
 Project-URL: repository, https://github.com/google-research/visu3d
 Provides-Extra: dev
+Provides-Extra: docs
 
 # visu3d - 3D geometry made easy
 
 [![Unittests](https://github.com/google-research/visu3d/actions/workflows/pytest_and_autopublish.yml/badge.svg)](https://github.com/google-research/visu3d/actions/workflows/pytest_and_autopublish.yml)
 [![PyPI version](https://badge.fury.io/py/visu3d.svg)](https://badge.fury.io/py/visu3d)
+[![Documentation Status](https://readthedocs.org/projects/visu3d/badge/?version=latest)](https://visu3d.readthedocs.io/en/latest/?badge=latest)
 
 `visu3d` is an abstraction layer between Torch/TF/Jax/Numpy and your program.
 It provides:
 
 *   Standard primitives for 3d geometry (`Ray`, `Camera`, `Transform`,...).
     You can combine those standard primitives with your custom ones.
 *   Everything is trivially visualizable with zero boilerplate. Inspect & debug
@@ -180,21 +187,21 @@
 <!-- See [the tutorial]() for more info. -->
 
 </section>
 
 ### Documentation
 
 The best way to get started is to try the Colab tutorials (in the
-[docs/](https://github.com/google-research/visu3d/tree/main/docs/)):
+[documentation](https://visu3d.readthedocs.io/)):
 
-*   [Intro (Colab)](https://colab.research.google.com/github/google-research/visu3d/blob/main/docs/intro.ipynb)
+*   [Intro](https://visu3d.readthedocs.io/en/latest/intro.html) ([Colab](https://colab.research.google.com/github/google-research/visu3d/blob/main/docs/intro.ipynb))
     <!-- {.external} !-->
-*   [Transform (Colab)](https://colab.research.google.com/github/google-research/visu3d/blob/main/docs/transform.ipynb)
+*   [Transform](https://visu3d.readthedocs.io/en/latest/transform.html) ([Colab](https://colab.research.google.com/github/google-research/visu3d/blob/main/docs/transform.ipynb))
     <!-- {.external} !-->
-*   [Create your primitives (Colab)](https://colab.research.google.com/github/google-research/visu3d/blob/main/docs/dataclass.ipynb)
+*   [Create your primitives](https://visu3d.readthedocs.io/en/latest/dataclass.html) ([Colab](https://colab.research.google.com/github/google-research/visu3d/blob/main/docs/dataclass.ipynb))
     <!-- {.external} !-->
 
 Installation:
 
 ```sh
 pip install visu3d
 ```
```

