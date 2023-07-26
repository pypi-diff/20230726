# Comparing `tmp/problem_bank_helpers-0.1.9.tar.gz` & `tmp/problem_bank_helpers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "problem_bank_helpers-0.1.9.tar", max compression
+gzip compressed data, was "problem_bank_helpers-0.2.0.tar", max compression
```

## Comparing `problem_bank_helpers-0.1.9.tar` & `problem_bank_helpers-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,20 @@
--rwxr-xr-x   0        0        0        1 2021-06-14 01:41:43.016309 problem_bank_helpers-0.1.9/LICENSE
--rw-r--r--   0        0        0     1244 2021-06-14 01:41:43.033405 problem_bank_helpers-0.1.9/README.md
--rw-r--r--   0        0        0      783 2022-01-02 06:27:06.219645 problem_bank_helpers-0.1.9/pyproject.toml
--rw-r--r--   0        0        0       59 2022-01-02 06:27:22.047869 problem_bank_helpers-0.1.9/src/problem_bank_helpers/__init__.py
--rw-r--r--   0        0        0    10554 2022-01-02 05:50:00.099601 problem_bank_helpers-0.1.9/src/problem_bank_helpers/problem_bank_helpers.py
--rw-r--r--   0        0        0     2069 2022-01-02 06:29:41.919962 problem_bank_helpers-0.1.9/setup.py
--rw-r--r--   0        0        0     2040 2022-01-02 06:29:41.920435 problem_bank_helpers-0.1.9/PKG-INFO
+-rwxr-xr-x   0        0        0        1 2021-06-14 01:41:43.016309 problem_bank_helpers-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1244 2021-06-14 01:41:43.033405 problem_bank_helpers-0.2.0/README.md
+-rw-r--r--   0        0        0       44 2023-06-30 00:13:15.868563 problem_bank_helpers-0.2.0/data/animals.csv
+-rw-r--r--   0        0        0        0 2023-07-26 04:00:06.482196 problem_bank_helpers-0.2.0/data/empty.csv
+-rw-r--r--   0        0        0       61 2023-06-30 00:13:15.869185 problem_bank_helpers-0.2.0/data/jumpers.csv
+-rw-r--r--   0        0        0       84 2023-06-30 00:13:15.869706 problem_bank_helpers-0.2.0/data/manual_vehicles.csv
+-rw-r--r--   0        0        0      248 2023-06-30 00:13:15.870015 problem_bank_helpers-0.2.0/data/metals.csv
+-rw-r--r--   0        0        0       75 2023-06-30 00:13:15.870268 problem_bank_helpers-0.2.0/data/names.csv
+-rw-r--r--   0        0        0       56 2023-06-30 00:13:15.870498 problem_bank_helpers-0.2.0/data/vehicles.csv
+-rw-r--r--   0        0        0      716 2023-07-26 03:56:04.969547 problem_bank_helpers-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-07-26 03:57:08.453361 problem_bank_helpers-0.2.0/src/problem_bank_helpers/__init__.py
+-rw-r--r--   0        0        0       44 2023-06-29 23:59:26.052387 problem_bank_helpers-0.2.0/src/problem_bank_helpers/data/animals.csv
+-rw-r--r--   0        0        0       61 2023-06-29 23:59:26.052468 problem_bank_helpers-0.2.0/src/problem_bank_helpers/data/jumpers.csv
+-rw-r--r--   0        0        0       84 2023-06-29 23:59:26.052539 problem_bank_helpers-0.2.0/src/problem_bank_helpers/data/manual_vehicles.csv
+-rw-r--r--   0        0        0      248 2023-06-29 23:59:26.052616 problem_bank_helpers-0.2.0/src/problem_bank_helpers/data/metals.csv
+-rw-r--r--   0        0        0       75 2023-06-29 23:59:26.052689 problem_bank_helpers-0.2.0/src/problem_bank_helpers/data/names.csv
+-rw-r--r--   0        0        0       56 2023-06-29 23:59:26.052756 problem_bank_helpers-0.2.0/src/problem_bank_helpers/data/vehicles.csv
+-rw-r--r--   0        0        0    17971 2023-07-26 03:50:49.754889 problem_bank_helpers-0.2.0/src/problem_bank_helpers/problem_bank_helpers.py
+-rw-r--r--   0        0        0     2130 2023-07-26 04:01:39.772310 problem_bank_helpers-0.2.0/setup.py
+-rw-r--r--   0        0        0     1981 2023-07-26 04:01:39.772508 problem_bank_helpers-0.2.0/PKG-INFO
```

### Comparing `problem_bank_helpers-0.1.9/README.md` & `problem_bank_helpers-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `problem_bank_helpers-0.1.9/setup.py` & `problem_bank_helpers-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 package_dir = \
 {'': 'src'}
 
 packages = \
 ['problem_bank_helpers']
 
 package_data = \
-{'': ['*']}
+{'': ['*'], 'problem_bank_helpers': ['data/*']}
 
 install_requires = \
-['numpy>=1.20.3,<2.0.0', 'sigfig>=1.1.9,<2.0.0']
+['numpy>=1.20.3,<2.0.0', 'pandas>=2.0.0,<3.0.0', 'sigfig>=1.1.9,<2.0.0']
 
 setup_kwargs = {
     'name': 'problem-bank-helpers',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': 'Helpful utilities for the open problem bank.',
     'long_description': '# Problem Bank Helpers \n\n[![Python](https://img.shields.io/badge/python-3.9-blue)]()\n[![codecov](https://codecov.io/gh/open-resources/problem_bank_helpers/branch/main/graph/badge.svg)](https://codecov.io/gh/open-resources/problem_bank_helpers)\n[![Documentation Status](https://readthedocs.org/projects/problem_bank_helpers/badge/?version=latest)](https://problem_bank_helpers.readthedocs.io/en/latest/?badge=latest)\n\n\n## Installation\n\n```bash\n$ pip install -i https://test.pypi.org/simple/ problem_bank_helpers\n```\n\n## Features\n\n- TODO\n\n## Dependencies\n\n- TODO\n\n## Usage\n\n- TODO\n\n## Documentation\n\nThe official documentation is hosted on Read the Docs: https://problem_bank_helpers.readthedocs.io/en/latest/\n\n## Contributors\n\nWe welcome and recognize all contributions. You can see a list of current contributors in the [contributors tab](https://github.com/open-resources/problem_bank_helpers/graphs/contributors).\n\n### Credits\n\nThis package was created with Cookiecutter and the UBC-MDS/cookiecutter-ubc-mds project template, modified from the [pyOpenSci/cookiecutter-pyopensci](https://github.com/pyOpenSci/cookiecutter-pyopensci) project template and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).\n',
     'author': 'Firas Moosvi and Jake Bobowski',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/open-resources/problem_bank_helpers',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `problem_bank_helpers-0.1.9/PKG-INFO` & `problem_bank_helpers-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: problem-bank-helpers
-Version: 0.1.9
+Version: 0.2.0
 Summary: Helpful utilities for the open problem bank.
 Home-page: https://github.com/open-resources/problem_bank_helpers
 License: MIT
 Author: Firas Moosvi and Jake Bobowski
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: numpy (>=1.20.3,<2.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: sigfig (>=1.1.9,<2.0.0)
 Project-URL: Documentation, https://problem_bank_helpers.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/open-resources/problem_bank_helpers
 Description-Content-Type: text/markdown
 
 # Problem Bank Helpers
```

