# Comparing `tmp/rgmining_fraudar-0.7.1.tar.gz` & `tmp/rgmining_fraudar-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgmining_fraudar-0.7.1.tar", max compression
+gzip compressed data, was "rgmining_fraudar-0.7.2.tar", max compression
```

## Comparing `rgmining_fraudar-0.7.1.tar` & `rgmining_fraudar-0.7.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    34500 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/COPYING
--rw-r--r--   0        0        0    10703 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/LICENSE-2.0
--rw-r--r--   0        0        0     2044 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/README.rst
--rw-r--r--   0        0        0     1960 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/__init__.py
--rw-r--r--   0        0        0      823 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/__version__.py
--rw-r--r--   0        0        0     2735 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/export/MinTree.py
--rw-r--r--   0        0        0     4490 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/export/README
--rw-r--r--   0        0        0     1737 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/export/__init__.py
--rw-r--r--   0        0        0     9233 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/export/greedy.py
--rw-r--r--   0        0        0     2417 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/export/run_greedy.py
--rw-r--r--   0        0        0     1408 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/export/testMinTree.py
--rw-r--r--   0        0        0     6789 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/graph.py
--rw-r--r--   0        0        0        0 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/py.typed
--rw-r--r--   0        0        0     2093 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 rgmining_fraudar-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    34500 2023-07-26 07:36:21.071410 rgmining_fraudar-0.7.2/COPYING
+-rw-r--r--   0        0        0    10703 2023-07-26 07:36:21.071410 rgmining_fraudar-0.7.2/LICENSE-2.0
+-rw-r--r--   0        0        0     2044 2023-07-26 07:36:21.071410 rgmining_fraudar-0.7.2/README.rst
+-rw-r--r--   0        0        0     1960 2023-07-26 07:36:21.071410 rgmining_fraudar-0.7.2/fraudar/__init__.py
+-rw-r--r--   0        0        0      823 2023-07-26 07:36:21.071410 rgmining_fraudar-0.7.2/fraudar/__version__.py
+-rw-r--r--   0        0        0     2735 2023-07-26 07:36:21.071410 rgmining_fraudar-0.7.2/fraudar/export/MinTree.py
+-rw-r--r--   0        0        0     4490 2023-07-26 07:36:21.071410 rgmining_fraudar-0.7.2/fraudar/export/README
+-rw-r--r--   0        0        0     1737 2023-07-26 07:36:21.071410 rgmining_fraudar-0.7.2/fraudar/export/__init__.py
+-rw-r--r--   0        0        0     9233 2023-07-26 07:36:21.071410 rgmining_fraudar-0.7.2/fraudar/export/greedy.py
+-rw-r--r--   0        0        0     2417 2023-07-26 07:36:21.071410 rgmining_fraudar-0.7.2/fraudar/export/run_greedy.py
+-rw-r--r--   0        0        0     1408 2023-07-26 07:36:21.071410 rgmining_fraudar-0.7.2/fraudar/export/testMinTree.py
+-rw-r--r--   0        0        0     6789 2023-07-26 07:36:21.071410 rgmining_fraudar-0.7.2/fraudar/graph.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:36:21.071410 rgmining_fraudar-0.7.2/fraudar/py.typed
+-rw-r--r--   0        0        0     2094 2023-07-26 07:36:21.071410 rgmining_fraudar-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 rgmining_fraudar-0.7.2/PKG-INFO
```

### Comparing `rgmining_fraudar-0.7.1/COPYING` & `rgmining_fraudar-0.7.2/COPYING`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.1/LICENSE-2.0` & `rgmining_fraudar-0.7.2/LICENSE-2.0`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.1/README.rst` & `rgmining_fraudar-0.7.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -41,11 +41,11 @@
    :target: https://www.gnu.org/copyleft/gpl.html
 .. |Build Status| image:: https://github.com/rgmining/fraudar/actions/workflows/python-lib.yaml/badge.svg
    :target: https://github.com/rgmining/fraudar/actions/workflows/python-lib.yaml
 .. |Maintainability| image:: https://api.codeclimate.com/v1/badges/4c4c3df79b33f65b77cd/maintainability
    :target: https://codeclimate.com/github/rgmining/fraudar/maintainability
 .. |Test Coverage| image:: https://api.codeclimate.com/v1/badges/4c4c3df79b33f65b77cd/test_coverage
    :target: https://codeclimate.com/github/rgmining/fraudar/test_coverage
-.. |Release| image:: https://img.shields.io/badge/release-0.7.1-brightgreen.svg
+.. |Release| image:: https://img.shields.io/badge/release-0.7.2-brightgreen.svg
    :target: https://pypi.org/project/rgmining-fraudar/
 .. |Logo| image:: https://rgmining.github.io/fraudar/_static/image.png
    :target: https://rgmining.github.io/fraudar/
```

### Comparing `rgmining_fraudar-0.7.1/fraudar/__init__.py` & `rgmining_fraudar-0.7.2/fraudar/__init__.py`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.1/fraudar/__version__.py` & `rgmining_fraudar-0.7.2/fraudar/__version__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with rgmining-fraudar. If not, see <http://www.gnu.org/licenses/>.
 #
 from typing import Final
 
-__version__: Final = "0.7.1"
+__version__: Final = "0.7.2"
```

### Comparing `rgmining_fraudar-0.7.1/fraudar/export/MinTree.py` & `rgmining_fraudar-0.7.2/fraudar/export/MinTree.py`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.1/fraudar/export/README` & `rgmining_fraudar-0.7.2/fraudar/export/README`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.1/fraudar/export/__init__.py` & `rgmining_fraudar-0.7.2/fraudar/export/__init__.py`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.1/fraudar/export/greedy.py` & `rgmining_fraudar-0.7.2/fraudar/export/greedy.py`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.1/fraudar/export/run_greedy.py` & `rgmining_fraudar-0.7.2/fraudar/export/run_greedy.py`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.1/fraudar/export/testMinTree.py` & `rgmining_fraudar-0.7.2/fraudar/export/testMinTree.py`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.1/fraudar/graph.py` & `rgmining_fraudar-0.7.2/fraudar/graph.py`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.1/pyproject.toml` & `rgmining_fraudar-0.7.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rgmining-fraudar"
-version = "0.7.1"
+version = "0.7.2"
 description = "A wrapper of Fraudar algorithm for Review graph mining project"
 license = "GPL-3.0-only"
 authors = ["Junpei Kawamoto <kawamoto.junpei@gmail.com>"]
 readme = "README.rst"
 homepage = "https://rgmining.github.io/fraudar/"
 repository = "https://github.com/rgmining/fraudar"
 documentation = "https://rgmining.github.io/fraudar/"
@@ -24,35 +24,35 @@
 packages = [
     { include = "fraudar" },
 ]
 include = ["COPYING", "LICENSE-2.0"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-numpy = "^1.24.1"
-scikit-learn = "^1.2.0"
+numpy = "^1.25.1"
+scikit-learn = "^1.3.0"
 
 [tool.poetry.group.dev.dependencies]
 bump2version = "^1.0.1"
 pre-commit = "^2.21.0"
 isort = "^5.10.1"
 flake8 = "^6.0.0"
 black = "^22.1.0"
-pytest = "^7.1.1"
+pytest = "^7.4.0"
 mypy = "^0.991"
 pytest-cov = "^4.0.0"
-pytest-mock = "^3.7.0"
-tox = "^4.2.3"
+pytest-mock = "^3.11.1"
+tox = "^4.6.4"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^5.3.0"
-sphinx-rtd-theme = "^1.1.1"
+sphinx-rtd-theme = "^1.2.2"
 sphinx-autobuild = "^2021.3.14"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `rgmining_fraudar-0.7.1/PKG-INFO` & `rgmining_fraudar-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgmining-fraudar
-Version: 0.7.1
+Version: 0.7.2
 Summary: A wrapper of Fraudar algorithm for Review graph mining project
 Home-page: https://rgmining.github.io/fraudar/
 License: GPL-3.0-only
 Keywords: review,graph,mining,algorithm,kdd,fraudar
 Author: Junpei Kawamoto
 Author-email: kawamoto.junpei@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -15,16 +15,16 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: numpy (>=1.24.1,<2.0.0)
-Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
+Requires-Dist: numpy (>=1.25.1,<2.0.0)
+Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
 Project-URL: Documentation, https://rgmining.github.io/fraudar/
 Project-URL: Repository, https://github.com/rgmining/fraudar
 Description-Content-Type: text/x-rst
 
 A wrapper of FRAUDAR algorithm
 ==============================
 
@@ -68,12 +68,12 @@
    :target: https://www.gnu.org/copyleft/gpl.html
 .. |Build Status| image:: https://github.com/rgmining/fraudar/actions/workflows/python-lib.yaml/badge.svg
    :target: https://github.com/rgmining/fraudar/actions/workflows/python-lib.yaml
 .. |Maintainability| image:: https://api.codeclimate.com/v1/badges/4c4c3df79b33f65b77cd/maintainability
    :target: https://codeclimate.com/github/rgmining/fraudar/maintainability
 .. |Test Coverage| image:: https://api.codeclimate.com/v1/badges/4c4c3df79b33f65b77cd/test_coverage
    :target: https://codeclimate.com/github/rgmining/fraudar/test_coverage
-.. |Release| image:: https://img.shields.io/badge/release-0.7.1-brightgreen.svg
+.. |Release| image:: https://img.shields.io/badge/release-0.7.2-brightgreen.svg
    :target: https://pypi.org/project/rgmining-fraudar/
 .. |Logo| image:: https://rgmining.github.io/fraudar/_static/image.png
    :target: https://rgmining.github.io/fraudar/
```

