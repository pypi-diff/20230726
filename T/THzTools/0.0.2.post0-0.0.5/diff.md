# Comparing `tmp/thztools-0.0.2.post0.tar.gz` & `tmp/thztools-0.0.5.tar.gz`

## Comparing `thztools-0.0.2.post0.tar` & `thztools-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,43 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.gitattributes
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/simulation-example.ipynb
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/jupyter-settings.xml
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/misc.xml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/modules.xml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/other.xml
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/thztools.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/vcs.xml
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/envs/environment-dev.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/envs/environment-test.yml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/src/thztools/__about__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/src/thztools/__init__.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/src/thztools/_util.py
--rw-r--r--   0        0        0    28725 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/src/thztools/thztools.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/LICENSE
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/README.md
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/pyproject.toml
--rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 thztools-0.0.2.post0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 thztools-0.0.5/.DS_Store
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 thztools-0.0.5/.gitattributes
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 thztools-0.0.5/simulation-example.ipynb
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/jupyter-settings.xml
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/modules.xml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/other.xml
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/thztools.iml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/vcs.xml
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 thztools-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 thztools-0.0.5/.vscode/settings.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/coverage_html.js
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_03fd280ebf6a0a6e___init___py.html
+-rw-r--r--   0        0        0    46109 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_03fd280ebf6a0a6e_common_py.html
+-rw-r--r--   0        0        0    32102 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_03fd280ebf6a0a6e_diff_tools_py.html
+-rw-r--r--   0        0        0    87482 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_03fd280ebf6a0a6e_messages_py.html
+-rw-r--r--   0        0        0   139772 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_03fd280ebf6a0a6e_pytest_plugin_py.html
+-rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_36ede29a3be77d5b___init___py.html
+-rw-r--r--   0        0        0    35110 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_36ede29a3be77d5b__util_py.html
+-rw-r--r--   0        0        0   321235 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_36ede29a3be77d5b_thztools_py.html
+-rw-r--r--   0        0        0    43443 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_8491cb1bc6f6c073_consistency_test_py.html
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_8491cb1bc6f6c073_test_pytest_py.html
+-rw-r--r--   0        0        0    20570 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_e963af3fa267a6d4__jb_pytest_runner_py.html
+-rw-r--r--   0        0        0   107696 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_e963af3fa267a6d4__jb_runner_tools_py.html
+-rw-r--r--   0        0        0    34575 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_e963af3fa267a6d4__jb_serial_tree_manager_py.html
+-rw-r--r--   0        0        0    42146 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/d_e963af3fa267a6d4__jb_utils_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/favicon_32.png
+-rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/keybd_open.png
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 thztools-0.0.5/htmlReport/style.css
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 thztools-0.0.5/src/thztools/.DS_Store
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 thztools-0.0.5/src/thztools/__about__.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 thztools-0.0.5/src/thztools/__init__.py
+-rw-r--r--   0        0        0    18256 2020-02-02 00:00:00.000000 thztools-0.0.5/src/thztools/thztools.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 thztools-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 thztools-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 thztools-0.0.5/README.md
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 thztools-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 thztools-0.0.5/PKG-INFO
```

### Comparing `thztools-0.0.2.post0/simulation-example.ipynb` & `thztools-0.0.5/simulation-example.ipynb`

 * *Files identical despite different names*

### Comparing `thztools-0.0.2.post0/.idea/thztools.iml` & `thztools-0.0.5/.idea/thztools.iml`

 * *Files identical despite different names*

### Comparing `thztools-0.0.2.post0/.idea/inspectionProfiles/Project_Default.xml` & `thztools-0.0.5/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `thztools-0.0.2.post0/.gitignore` & `thztools-0.0.5/.gitignore`

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,95 @@
-# Local .gitignore
-Untitled.ipynb
-
-# Python .gitignore:
-#	https://github.com/github/gitignore/blob/main/Python.gitignore
-
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Sphinx documentation
-docs/build/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# PyCharm .gitignore:
-#	https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-
-# User-specific stuff
-.idea/**/workspace.xml
-.idea/**/tasks.xml
-.idea/**/usage.statistics.xml
-.idea/**/dictionaries
-.idea/**/shelf
-
-# Sensitive or high-churn files
-.idea/**/dataSources/
-.idea/**/dataSources.ids
-.idea/**/dataSources.local.xml
-.idea/**/sqlDataSources.xml
-.idea/**/dynamic.xml
-.idea/**/uiDesigner.xml
-.idea/**/dbnavigator.xml
-
-# Editor-based Rest Client
-.idea/httpRequests
-
-# MATLAB .gitignore:
-#	https://github.com/github/gitignore/blob/main/Global/MATLAB.gitignore
-
-# Windows default autosave extension
-*.asv
+# Local .gitignore
+Untitled*.ipynb
+
+# Python .gitignore:
+#	https://github.com/github/gitignore/blob/main/Python.gitignore
+
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Sphinx documentation
+docs/build/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# PyCharm .gitignore:
+#	https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+
+# User-specific stuff
+.idea/**/workspace.xml
+.idea/**/tasks.xml
+.idea/**/usage.statistics.xml
+.idea/**/dictionaries
+.idea/**/shelf
+
+# Sensitive or high-churn files
+.idea/**/dataSources/
+.idea/**/dataSources.ids
+.idea/**/dataSources.local.xml
+.idea/**/sqlDataSources.xml
+.idea/**/dynamic.xml
+.idea/**/uiDesigner.xml
+.idea/**/dbnavigator.xml
+
+# Editor-based Rest Client
+.idea/httpRequests
+
+# MATLAB .gitignore:
+#	https://github.com/github/gitignore/blob/main/Global/MATLAB.gitignore
+
+# Windows default autosave extension
+*.asv
+
+# VisualStudioCode .gitignore:
+#      https://github.com/github/gitignore/blob/main/Global/VisualStudioCode.gitignore
+
+.vscode/*
+!.vscode/settings.json
+!.vscode/tasks.json
+!.vscode/launch.json
+!.vscode/extensions.json
+!.vscode/*.code-snippets
+
+# Local History for Visual Studio Code
+.history/
+
+# Built Visual Studio Code Extensions
+*.vsix
```

### Comparing `thztools-0.0.2.post0/LICENSE` & `thztools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thztools-0.0.2.post0/README.md` & `thztools-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# THzTools
-
-Data analysis tools for terahertz time-domain spectroscopy.
-
-This is *alpha* software that is currently under development.
-
-| Information       | Links                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
-|:------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| **Project**       | ![PyPI - Status](https://img.shields.io/pypi/status/thztools) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/thztools) ![GitHub](https://img.shields.io/github/license/dodge-research-group/thztools) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)                                                                                                                                                                                                                                                                                             |
-| **Build**         | ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/sphinx.yml?label=build%3Adocs) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-conda.yml?label=build%3Atests%20(conda)) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-pip.yml?label=build%3Atests%20(pip)) [![codecov](https://codecov.io/gh/dodge-research-group/thztools/branch/dev/graph/badge.svg?token=U8PLKTQ7AH)](https://codecov.io/gh/dodge-research-group/thztools) |
-| **Documentation** | https://dodge-research-group.github.io/thztools/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
-| **Cite**          | L. Mohtashemi et al., *Opt. Express* **29**, 4912 (2021). [(DOI)](https://doi.org/10.1364/OE.417724)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
-
-The original MATLAB code is available at [Zenodo](https://zenodo.org/record/4876388).
+# THzTools
+
+Data analysis tools for terahertz time-domain spectroscopy.
+
+This is *alpha* software that is currently under development.
+
+| Information       | Links                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+|:------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| **Project**       | ![PyPI - Status](https://img.shields.io/pypi/status/thztools) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/thztools) ![GitHub](https://img.shields.io/github/license/dodge-research-group/thztools) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)                                                                                                                                                                                                                                                                                                       |
+| **Build**         | ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/sphinx.yml?label=build%3Adocs) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/pytest-with-coverage.yml?label=build%3Atests%20(conda)) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-pip.yml?label=build%3Atests%20(pip)) [![codecov](https://codecov.io/gh/dodge-research-group/thztools/branch/dev/graph/badge.svg?token=U8PLKTQ7AH)](https://codecov.io/gh/dodge-research-group/thztools) |
+| **Documentation** | https://dodge-research-group.github.io/thztools/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+| **Cite**          | L. Mohtashemi et al., *Opt. Express* **29**, 4912 (2021). [(DOI)](https://doi.org/10.1364/OE.417724)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
+
+The original MATLAB code is available at [Zenodo](https://zenodo.org/record/4876388).
```

### Comparing `thztools-0.0.2.post0/PKG-INFO` & `thztools-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: THzTools
-Version: 0.0.2.post0
+Version: 0.0.5
 Summary: Tools for terahertz time-domain spectroscopy (THz-TDS)
 Project-URL: Documentation, https://dodge-research-group.github.io/thztools/
 Project-URL: Issues, https://github.com/dodge-research-group/thztools/issues
 Project-URL: Source, https://github.com/dodge-research-group/thztools
 Author-email: Steve Dodge <jsdodge@sfu.ca>, Santiago Higuera Quintero <s.higuera@uniandes.edu.co>, Jonathan Posada <jonathan.posada1@udea.edu.co>
 Maintainer-email: Steve Dodge <jsdodge@sfu.ca>
 License-Expression: MIT
@@ -19,27 +19,25 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
-Requires-Dist: jupyter
-Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: scipy
 Description-Content-Type: text/markdown
 
 # THzTools
 
 Data analysis tools for terahertz time-domain spectroscopy.
 
 This is *alpha* software that is currently under development.
 
-| Information       | Links                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
-|:------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| **Project**       | ![PyPI - Status](https://img.shields.io/pypi/status/thztools) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/thztools) ![GitHub](https://img.shields.io/github/license/dodge-research-group/thztools) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)                                                                                                                                                                                                                                                                                             |
-| **Build**         | ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/sphinx.yml?label=build%3Adocs) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-conda.yml?label=build%3Atests%20(conda)) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-pip.yml?label=build%3Atests%20(pip)) [![codecov](https://codecov.io/gh/dodge-research-group/thztools/branch/dev/graph/badge.svg?token=U8PLKTQ7AH)](https://codecov.io/gh/dodge-research-group/thztools) |
-| **Documentation** | https://dodge-research-group.github.io/thztools/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
-| **Cite**          | L. Mohtashemi et al., *Opt. Express* **29**, 4912 (2021). [(DOI)](https://doi.org/10.1364/OE.417724)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
+| Information       | Links                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+|:------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| **Project**       | ![PyPI - Status](https://img.shields.io/pypi/status/thztools) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/thztools) ![GitHub](https://img.shields.io/github/license/dodge-research-group/thztools) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)                                                                                                                                                                                                                                                                                                       |
+| **Build**         | ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/sphinx.yml?label=build%3Adocs) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/pytest-with-coverage.yml?label=build%3Atests%20(conda)) ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/dodge-research-group/thztools/test-pip.yml?label=build%3Atests%20(pip)) [![codecov](https://codecov.io/gh/dodge-research-group/thztools/branch/dev/graph/badge.svg?token=U8PLKTQ7AH)](https://codecov.io/gh/dodge-research-group/thztools) |
+| **Documentation** | https://dodge-research-group.github.io/thztools/                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+| **Cite**          | L. Mohtashemi et al., *Opt. Express* **29**, 4912 (2021). [(DOI)](https://doi.org/10.1364/OE.417724)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
 
-The original MATLAB code is available at [Zenodo](https://zenodo.org/record/4876388).
+The original MATLAB code is available at [Zenodo](https://zenodo.org/record/4876388).
```

