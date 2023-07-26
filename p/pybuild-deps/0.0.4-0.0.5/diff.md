# Comparing `tmp/pybuild_deps-0.0.4.tar.gz` & `tmp/pybuild_deps-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybuild_deps-0.0.4.tar", max compression
+gzip compressed data, was "pybuild_deps-0.0.5.tar", max compression
```

## Comparing `pybuild_deps-0.0.4.tar` & `pybuild_deps-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    35887 2023-02-02 15:12:24.681567 pybuild_deps-0.0.4/LICENSE
--rw-r--r--   0        0        0     2373 2023-02-02 15:12:24.681567 pybuild_deps-0.0.4/README.md
--rw-r--r--   0        0        0     2275 2023-02-02 15:12:39.413958 pybuild_deps-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       20 2023-02-02 15:12:24.681567 pybuild_deps-0.0.4/src/pybuild_deps/__init__.py
--rw-r--r--   0        0        0      712 2023-02-02 15:12:24.681567 pybuild_deps-0.0.4/src/pybuild_deps/__main__.py
--rw-r--r--   0        0        0     1457 2023-02-02 15:12:24.681567 pybuild_deps-0.0.4/src/pybuild_deps/find_build_dependencies.py
--rw-r--r--   0        0        0     1678 2023-02-02 15:12:24.681567 pybuild_deps-0.0.4/src/pybuild_deps/get_package_source.py
--rw-r--r--   0        0        0      770 2023-02-02 15:12:24.681567 pybuild_deps-0.0.4/src/pybuild_deps/parsers/__init__.py
--rw-r--r--   0        0        0     2781 2023-02-02 15:12:24.681567 pybuild_deps-0.0.4/src/pybuild_deps/parsers/setup_py.py
--rw-r--r--   0        0        0        0 2023-02-02 15:12:24.681567 pybuild_deps-0.0.4/src/pybuild_deps/py.typed
--rw-r--r--   0        0        0     3467 1970-01-01 00:00:00.000000 pybuild_deps-0.0.4/setup.py
--rw-r--r--   0        0        0     3410 1970-01-01 00:00:00.000000 pybuild_deps-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35887 2023-07-26 13:39:56.645321 pybuild_deps-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2373 2023-07-26 13:39:56.645321 pybuild_deps-0.0.5/README.md
+-rw-r--r--   0        0        0     2275 2023-07-26 13:40:08.949394 pybuild_deps-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-07-26 13:39:56.645321 pybuild_deps-0.0.5/src/pybuild_deps/__init__.py
+-rw-r--r--   0        0        0      712 2023-07-26 13:39:56.645321 pybuild_deps-0.0.5/src/pybuild_deps/__main__.py
+-rw-r--r--   0        0        0     1457 2023-07-26 13:39:56.645321 pybuild_deps-0.0.5/src/pybuild_deps/find_build_dependencies.py
+-rw-r--r--   0        0        0     1678 2023-07-26 13:39:56.645321 pybuild_deps-0.0.5/src/pybuild_deps/get_package_source.py
+-rw-r--r--   0        0        0      770 2023-07-26 13:39:56.645321 pybuild_deps-0.0.5/src/pybuild_deps/parsers/__init__.py
+-rw-r--r--   0        0        0     2781 2023-07-26 13:39:56.645321 pybuild_deps-0.0.5/src/pybuild_deps/parsers/setup_py.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:39:56.645321 pybuild_deps-0.0.5/src/pybuild_deps/py.typed
+-rw-r--r--   0        0        0     3410 1970-01-01 00:00:00.000000 pybuild_deps-0.0.5/PKG-INFO
```

### Comparing `pybuild_deps-0.0.4/LICENSE` & `pybuild_deps-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pybuild_deps-0.0.4/README.md` & `pybuild_deps-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pybuild_deps-0.0.4/pyproject.toml` & `pybuild_deps-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybuild-deps"
-version = "0.0.4"
+version = "0.0.5"
 description = "A simple tool for detection of PEP-517 build dependencies."
 authors = ["Bruno Ciconelle <fsouza.bruno@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/bruno-fs/pybuild-deps"
 repository = "https://github.com/bruno-fs/pybuild-deps"
 documentation = "https://pybuild-deps.readthedocs.io"
```

### Comparing `pybuild_deps-0.0.4/src/pybuild_deps/__main__.py` & `pybuild_deps-0.0.5/src/pybuild_deps/__main__.py`

 * *Files identical despite different names*

### Comparing `pybuild_deps-0.0.4/src/pybuild_deps/find_build_dependencies.py` & `pybuild_deps-0.0.5/src/pybuild_deps/find_build_dependencies.py`

 * *Files identical despite different names*

### Comparing `pybuild_deps-0.0.4/src/pybuild_deps/get_package_source.py` & `pybuild_deps-0.0.5/src/pybuild_deps/get_package_source.py`

 * *Files identical despite different names*

### Comparing `pybuild_deps-0.0.4/src/pybuild_deps/parsers/__init__.py` & `pybuild_deps-0.0.5/src/pybuild_deps/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pybuild_deps-0.0.4/src/pybuild_deps/parsers/setup_py.py` & `pybuild_deps-0.0.5/src/pybuild_deps/parsers/setup_py.py`

 * *Files identical despite different names*

### Comparing `pybuild_deps-0.0.4/setup.py` & `pybuild_deps-0.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,97 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pybuild-deps
+Version: 0.0.5
+Summary: A simple tool for detection of PEP-517 build dependencies.
+Home-page: https://github.com/bruno-fs/pybuild-deps
+License: GPL-3.0
+Author: Bruno Ciconelle
+Author-email: fsouza.bruno@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.0.1)
+Requires-Dist: requests
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
+Requires-Dist: xdg
+Project-URL: Changelog, https://github.com/bruno-fs/pybuild-deps/releases
+Project-URL: Documentation, https://pybuild-deps.readthedocs.io
+Project-URL: Repository, https://github.com/bruno-fs/pybuild-deps
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# PyBuild Deps
 
-packages = \
-['pybuild_deps', 'pybuild_deps.parsers']
+[![PyPI](https://img.shields.io/pypi/v/pybuild-deps.svg)][pypi status]
+[![Status](https://img.shields.io/pypi/status/pybuild-deps.svg)][pypi status]
+[![Python Version](https://img.shields.io/pypi/pyversions/pybuild-deps)][pypi status]
+[![License](https://img.shields.io/pypi/l/pybuild-deps)][license]
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8.0.1', 'requests', 'xdg']
-
-extras_require = \
-{':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
-
-entry_points = \
-{'console_scripts': ['pybuild-deps = pybuild_deps.__main__:cli']}
-
-setup_kwargs = {
-    'name': 'pybuild-deps',
-    'version': '0.0.4',
-    'description': 'A simple tool for detection of PEP-517 build dependencies.',
-    'long_description': "# PyBuild Deps\n\n[![PyPI](https://img.shields.io/pypi/v/pybuild-deps.svg)][pypi status]\n[![Status](https://img.shields.io/pypi/status/pybuild-deps.svg)][pypi status]\n[![Python Version](https://img.shields.io/pypi/pyversions/pybuild-deps)][pypi status]\n[![License](https://img.shields.io/pypi/l/pybuild-deps)][license]\n\n[![Read the documentation at https://pybuild-deps.readthedocs.io/](https://img.shields.io/readthedocs/pybuild-deps/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/bruno-fs/pybuild-deps/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/bruno-fs/pybuild-deps/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi status]: https://pypi.org/project/pybuild-deps/\n[read the docs]: https://pybuild-deps.readthedocs.io/\n[tests]: https://github.com/bruno-fs/pybuild-deps/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/bruno-fs/pybuild-deps\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- TODO\n\n## Requirements\n\n- TODO\n\n## Installation\n\nYou can install _PyBuild Deps_ via [pip] from [PyPI]:\n\n```console\n$ pip install pybuild-deps\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [GPL 3.0 license][license],\n_PyBuild Deps_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/bruno-fs/pybuild-deps/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/bruno-fs/pybuild-deps/blob/main/LICENSE\n[contributor guide]: https://github.com/bruno-fs/pybuild-deps/blob/main/CONTRIBUTING.md\n[command-line reference]: https://pybuild-deps.readthedocs.io/en/latest/usage.html\n",
-    'author': 'Bruno Ciconelle',
-    'author_email': 'fsouza.bruno@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/bruno-fs/pybuild-deps',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+[![Read the documentation at https://pybuild-deps.readthedocs.io/](https://img.shields.io/readthedocs/pybuild-deps/latest.svg?label=Read%20the%20Docs)][read the docs]
+[![Tests](https://github.com/bruno-fs/pybuild-deps/workflows/Tests/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/bruno-fs/pybuild-deps/branch/main/graph/badge.svg)][codecov]
 
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+
+[pypi status]: https://pypi.org/project/pybuild-deps/
+[read the docs]: https://pybuild-deps.readthedocs.io/
+[tests]: https://github.com/bruno-fs/pybuild-deps/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/bruno-fs/pybuild-deps
+[pre-commit]: https://github.com/pre-commit/pre-commit
+[black]: https://github.com/psf/black
+
+## Features
+
+- TODO
+
+## Requirements
+
+- TODO
+
+## Installation
+
+You can install _PyBuild Deps_ via [pip] from [PyPI]:
+
+```console
+$ pip install pybuild-deps
+```
+
+## Usage
+
+Please see the [Command-line Reference] for details.
+
+## Contributing
+
+Contributions are very welcome.
+To learn more, see the [Contributor Guide].
+
+## License
+
+Distributed under the terms of the [GPL 3.0 license][license],
+_PyBuild Deps_ is free and open source software.
+
+## Issues
+
+If you encounter any problems,
+please [file an issue] along with a detailed description.
+
+## Credits
+
+This project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
+
+[@cjolowicz]: https://github.com/cjolowicz
+[pypi]: https://pypi.org/
+[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+[file an issue]: https://github.com/bruno-fs/pybuild-deps/issues
+[pip]: https://pip.pypa.io/
+
+<!-- github-only -->
+
+[license]: https://github.com/bruno-fs/pybuild-deps/blob/main/LICENSE
+[contributor guide]: https://github.com/bruno-fs/pybuild-deps/blob/main/CONTRIBUTING.md
+[command-line reference]: https://pybuild-deps.readthedocs.io/en/latest/usage.html
 
-setup(**setup_kwargs)
```

