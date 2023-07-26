# Comparing `tmp/qoqo_strawberry_fields-0.1.0.tar.gz` & `tmp/qoqo_strawberry_fields-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoqo_strawberry_fields-0.1.0.tar", last modified: Wed Jul 26 08:59:56 2023, max compression
+gzip compressed data, was "qoqo_strawberry_fields-0.1.1.tar", last modified: Wed Jul 26 12:40:19 2023, max compression
```

## Comparing `qoqo_strawberry_fields-0.1.0.tar` & `qoqo_strawberry_fields-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:59:56.533688 qoqo_strawberry_fields-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:59:56.525688 qoqo_strawberry_fields-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:59:56.525688 qoqo_strawberry_fields-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/.github/workflows/hqs-build-deploy-pure-python.yml
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/.github/workflows/hqs-build-deploy-sphinx-doc-pure-python.yml
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/.github/workflows/hqs-ci-test-pure-python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    74058 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/CLA.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/CONTRIBUTE.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-07-26 08:59:56.533688 qoqo_strawberry_fields-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:59:56.529688 qoqo_strawberry_fields-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)   256743 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/qoqo_Logo_vertical_color.png
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 08:59:56.533688 qoqo_strawberry_fields-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:59:56.521688 qoqo_strawberry_fields-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:59:56.533688 qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields/post_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:59:56.533688 qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-07-26 08:59:56.000000 qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-26 08:59:56.000000 qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 08:59:56.000000 qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-26 08:59:56.000000 qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 08:59:56.000000 qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:59:56.533688 qoqo_strawberry_fields-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/tests/test_paper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-26 08:59:32.000000 qoqo_strawberry_fields-0.1.0/tests/test_simple_circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:40:19.257880 qoqo_strawberry_fields-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:40:19.253880 qoqo_strawberry_fields-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:40:19.253880 qoqo_strawberry_fields-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/.github/workflows/hqs-build-deploy-pure-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/.github/workflows/hqs-build-deploy-sphinx-doc-pure-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/.github/workflows/hqs-ci-test-pure-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    74058 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/CLA.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/CONTRIBUTE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-07-26 12:40:19.257880 qoqo_strawberry_fields-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:40:19.253880 qoqo_strawberry_fields-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)   256743 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/qoqo_Logo_vertical_color.png
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:40:19.257880 qoqo_strawberry_fields-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:40:19.253880 qoqo_strawberry_fields-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:40:19.257880 qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 12:40:19.000000 qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields/post_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:40:19.257880 qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-07-26 12:40:19.000000 qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-26 12:40:19.000000 qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:40:19.000000 qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-26 12:40:19.000000 qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 12:40:19.000000 qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:40:19.257880 qoqo_strawberry_fields-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/tests/test_paper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-26 12:40:00.000000 qoqo_strawberry_fields-0.1.1/tests/test_simple_circuit.py
```

### Comparing `qoqo_strawberry_fields-0.1.0/.github/dependabot.yml` & `qoqo_strawberry_fields-0.1.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `qoqo_strawberry_fields-0.1.0/.github/workflows/hqs-ci-test-pure-python.yml` & `qoqo_strawberry_fields-0.1.1/.github/workflows/hqs-ci-test-pure-python.yml`

 * *Files identical despite different names*

### Comparing `qoqo_strawberry_fields-0.1.0/.gitignore` & `qoqo_strawberry_fields-0.1.1/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
 
+# Version file for dynamic versioning
+*__version__.py
+
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
```

### Comparing `qoqo_strawberry_fields-0.1.0/CLA.pdf` & `qoqo_strawberry_fields-0.1.1/CLA.pdf`

 * *Files identical despite different names*

### Comparing `qoqo_strawberry_fields-0.1.0/CONTRIBUTE.md` & `qoqo_strawberry_fields-0.1.1/CONTRIBUTE.md`

 * *Files identical despite different names*

### Comparing `qoqo_strawberry_fields-0.1.0/LICENSE` & `qoqo_strawberry_fields-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_strawberry_fields-0.1.0/PKG-INFO` & `qoqo_strawberry_fields-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo_strawberry_fields
-Version: 0.1.0
+Version: 0.1.1
 Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 Maintainer-email: Kirsten Bark <kirsten.bark@quantumsimulations.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,8 +204,9 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Requires-Python: >=3.8
 Provides-Extra: tests
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `qoqo_strawberry_fields-0.1.0/README.md` & `qoqo_strawberry_fields-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 <img src="qoqo_Logo_vertical_color.png" alt="qoqo logo" width="300" />
 
 # qoqo-strawberry-fields
 Qoqo-strawberry-fields is a backend for the qoqo quantum computing toolkit that translates qoqo Circuits and Programs to the strawberry-fields toolkit from Xanadu.
 
+This project is supported by [PhoQuant](https://www.quantentechnologien.de/forschung/foerderung/quantencomputer-demonstrationsaufbauten/phoquant.html).
+
 ## General Notes
 
 This software is still in the beta stage. Functions and documentation are not yet complete and breaking changes can occur.
 
 ## Contributing
 
 We welcome contributions to the project. If you want to contribute code, please have a look at CONTRIBUTE.md for our code contribution guidelines.
```

### Comparing `qoqo_strawberry_fields-0.1.0/docs/Makefile` & `qoqo_strawberry_fields-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qoqo_strawberry_fields-0.1.0/docs/conf.py` & `qoqo_strawberry_fields-0.1.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 
 # set __version__
-import tomli
-
-main_version = tomli.load(open("../pyproject.toml", "rb"))["project"]["version"]
+from qoqo_strawberry_fields.__version__ import version_tuple
+main_version = f"{version_tuple[0]}.{version_tuple[1]}"
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `qoqo_strawberry_fields-0.1.0/pyproject.toml` & `qoqo_strawberry_fields-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -30,21 +30,31 @@
     "flake8-bandit",
     "flake8-bugbear",
     "flake8-pydocstyle",
     "flake8-pyproject",
     "mypy",
     "ruff",
 ]
+docs = [
+    "sphinx >= 2.1",
+    "nbsphinx",
+    "pygments",
+    "recommonmark",
+    "myst_parser",
+    "sphinx_rtd_theme",
+    "tomli"
+]
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 version_scheme = "python-simplified-semver"
+write_to = "src/qoqo_strawberry_fields/__version__.py"
 # NOTE: in case the pyproject.toml is **not** located at the root folder of the repository,
 # the 'root' option should provide the **relative** path from the pyproject.tomlto the
 # root folder of the repository.
 # NOTE: the example below **assumes** that the pyproject.toml is in a direct sub-folder
 # of the repositorie's root folder, e.g., as done in several QC stack repositories.
 # root = "../"  # default behavior is root = "./"
```

### Comparing `qoqo_strawberry_fields-0.1.0/qoqo_Logo_vertical_color.png` & `qoqo_strawberry_fields-0.1.1/qoqo_Logo_vertical_color.png`

 * *Files identical despite different names*

### Comparing `qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields/__init__.py` & `qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields/backend.py` & `qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields/backend.py`

 * *Files identical despite different names*

### Comparing `qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields/interface.py` & `qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields/interface.py`

 * *Files identical despite different names*

### Comparing `qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields/post_processing.py` & `qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields/post_processing.py`

 * *Files identical despite different names*

### Comparing `qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields.egg-info/PKG-INFO` & `qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo-strawberry-fields
-Version: 0.1.0
+Version: 0.1.1
 Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 Maintainer-email: Kirsten Bark <kirsten.bark@quantumsimulations.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,8 +204,9 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Requires-Python: >=3.8
 Provides-Extra: tests
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `qoqo_strawberry_fields-0.1.0/src/qoqo_strawberry_fields.egg-info/SOURCES.txt` & `qoqo_strawberry_fields-0.1.1/src/qoqo_strawberry_fields.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 .github/workflows/hqs-build-deploy-sphinx-doc-pure-python.yml
 .github/workflows/hqs-ci-test-pure-python.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/modules.rst
 src/qoqo_strawberry_fields/__init__.py
+src/qoqo_strawberry_fields/__version__.py
 src/qoqo_strawberry_fields/backend.py
 src/qoqo_strawberry_fields/interface.py
 src/qoqo_strawberry_fields/post_processing.py
 src/qoqo_strawberry_fields.egg-info/PKG-INFO
 src/qoqo_strawberry_fields.egg-info/SOURCES.txt
 src/qoqo_strawberry_fields.egg-info/dependency_links.txt
 src/qoqo_strawberry_fields.egg-info/requires.txt
```

### Comparing `qoqo_strawberry_fields-0.1.0/tests/test_paper.py` & `qoqo_strawberry_fields-0.1.1/tests/test_paper.py`

 * *Files identical despite different names*

### Comparing `qoqo_strawberry_fields-0.1.0/tests/test_simple_circuit.py` & `qoqo_strawberry_fields-0.1.1/tests/test_simple_circuit.py`

 * *Files identical despite different names*

