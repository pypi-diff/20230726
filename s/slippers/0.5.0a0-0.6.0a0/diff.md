# Comparing `tmp/slippers-0.5.0a0.tar.gz` & `tmp/slippers-0.6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slippers-0.5.0a0.tar", max compression
+gzip compressed data, was "slippers-0.6.0a0.tar", max compression
```

## Comparing `slippers-0.5.0a0.tar` & `slippers-0.6.0a0.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0     1072 2022-10-30 12:11:15.688739 slippers-0.5.0a0/LICENSE
--rw-r--r--   0        0        0     2059 2022-10-30 12:11:15.688739 slippers-0.5.0a0/README.md
--rw-r--r--   0        0        0     1065 2022-10-30 12:11:15.696740 slippers-0.5.0a0/pyproject.toml
--rw-r--r--   0        0        0       52 2022-10-30 12:11:15.696740 slippers-0.5.0a0/slippers/__init__.py
--rw-r--r--   0        0        0     1861 2022-10-30 12:11:15.700740 slippers-0.5.0a0/slippers/apps.py
--rw-r--r--   0        0        0     5801 2022-10-30 12:11:15.700740 slippers-0.5.0a0/slippers/template.py
--rw-r--r--   0        0        0        0 2022-10-30 12:11:15.700740 slippers-0.5.0a0/slippers/templatetags/__init__.py
--rw-r--r--   0        0        0     6031 2022-10-30 12:11:15.700740 slippers-0.5.0a0/slippers/templatetags/slippers.py
--rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 slippers-0.5.0a0/setup.py
--rw-r--r--   0        0        0     3269 1970-01-01 00:00:00.000000 slippers-0.5.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-12-29 13:18:15.967791 slippers-0.6.0a0/LICENSE
+-rw-r--r--   0        0        0     2059 2022-12-29 13:18:15.967791 slippers-0.6.0a0/README.md
+-rw-r--r--   0        0        0     1208 2022-12-29 13:18:15.979791 slippers-0.6.0a0/pyproject.toml
+-rw-r--r--   0        0        0       52 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/__init__.py
+-rw-r--r--   0        0        0     1861 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/apps.py
+-rw-r--r--   0        0        0      807 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/conf.py
+-rw-r--r--   0        0        0     6215 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/props.py
+-rw-r--r--   0        0        0     7367 2022-12-29 13:19:16.988254 slippers-0.6.0a0/slippers/static/slippers/main.css
+-rw-r--r--   0        0        0   145904 2022-12-29 13:19:16.988254 slippers-0.6.0a0/slippers/static/slippers/main.js
+-rw-r--r--   0        0        0     5801 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/template.py
+-rw-r--r--   0        0        0      179 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/templates/slippers/errors.html
+-rw-r--r--   0        0        0        0 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/templatetags/__init__.py
+-rw-r--r--   0        0        0     9037 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/templatetags/slippers.py
+-rw-r--r--   0        0        0     3175 1970-01-01 00:00:00.000000 slippers-0.6.0a0/setup.py
+-rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 slippers-0.6.0a0/PKG-INFO
```

### Comparing `slippers-0.5.0a0/LICENSE` & `slippers-0.6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `slippers-0.5.0a0/README.md` & `slippers-0.6.0a0/README.md`

 * *Files identical despite different names*

### Comparing `slippers-0.5.0a0/pyproject.toml` & `slippers-0.6.0a0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slippers"
-version = "0.5.0-alpha.0"
+version = "0.6.0a0"
 description = "Build reusable components in Django without writing a single line of Python."
 authors = ["Mitchel Cabuloy <mixxorz@gmail.com>"]
 keywords = ["django", "components"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/mixxorz/slippers"
 repository = "https://github.com/mixxorz/slippers"
@@ -17,20 +17,25 @@
     "Framework :: Django :: 2.2",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
 ]
 include = [
     "LICENSE",
+    "slippers/static/slippers/main.js",
+    "slippers/static/slippers/main.css",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.0"
 Django = ">=3.2, <4.2"
 PyYAML = ">=5.4.0, <7.0.0"
+typeguard = "^2.13.3"
+rich = "^12.6.0"
+typing-extensions = "^4.4.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 isort = "^5.9.2"
 flake8 = "^3.9.2"
 ipdb = "^0.13.9"
 tox = "^3.23.1"
```

### Comparing `slippers-0.5.0a0/slippers/apps.py` & `slippers-0.6.0a0/slippers/apps.py`

 * *Files identical despite different names*

### Comparing `slippers-0.5.0a0/slippers/template.py` & `slippers-0.6.0a0/slippers/template.py`

 * *Files identical despite different names*

### Comparing `slippers-0.5.0a0/setup.py` & `slippers-0.6.0a0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['slippers', 'slippers.templatetags']
 
 package_data = \
-{'': ['*']}
+{'': ['*'],
+ 'slippers': ['static/slippers/main.css',
+              'static/slippers/main.css',
+              'static/slippers/main.js',
+              'static/slippers/main.js',
+              'templates/slippers/*']}
 
 install_requires = \
-['Django>=3.2,<4.2', 'PyYAML>=5.4.0,<7.0.0']
+['Django>=3.2,<4.2',
+ 'PyYAML>=5.4.0,<7.0.0',
+ 'rich>=12.6.0,<13.0.0',
+ 'typeguard>=2.13.3,<3.0.0',
+ 'typing-extensions>=4.4.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'slippers',
-    'version': '0.5.0a0',
+    'version': '0.6.0a0',
     'description': 'Build reusable components in Django without writing a single line of Python.',
     'long_description': '[![Slippers](https://mitchel.me/slippers/img/slippers.svg)](https://github.com/mixxorz/slippers)\n\n---\n\n[![PyPI version](https://badge.fury.io/py/slippers.svg)](https://badge.fury.io/py/slippers)\n[![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/slippers.svg)](https://pypi.python.org/pypi/slippers/)\n[![PyPI Supported Django Versions](https://img.shields.io/pypi/djversions/slippers.svg)](https://docs.djangoproject.com/en/dev/releases/)\n[![GitHub Actions (Code quality and tests)](https://github.com/mixxorz/slippers/workflows/Code%20quality%20and%20tests/badge.svg)](https://github.com/mixxorz/slippers)\n\nBuild reusable components in Django without writing a single line of Python.\n\n```django\n{% #quote %}\n  {% quote_photo src="/project-hail-mary.jpg" %}\n\n  {% #quote_text %}\n    “I penetrated the outer cell membrane with a nanosyringe."\n    "You poked it with a stick?"\n    "No!" I said. "Well. Yes. But it was a scientific poke\n    with a very scientific stick.”\n  {% /quote_text %}\n\n  {% #quote_attribution %}\n    Andy Weir, Project Hail Mary\n  {% /quote_attribution %}\n{% /quote %}\n```\n\n## What is Slippers?\n\nThe Django Template Language is awesome. It\'s fast, rich in features, and overall pretty great to work with.\n\nSlippers aims to augment DTL, adding just enough functionality to make building interfaces just that bit more _comfortable_.\n\nIt includes additional template tags and filters, but its headline feature is **reusable components**.\n\n```django\n{% #button variant="primary" %}See how it works{% /button %}\n```\n\n[See how it works](https://mitchel.me/slippers/docs/getting-started/)\n\n## Installation\n\n```\npip install slippers\n```\n\nAdd it to your `INSTALLED_APPS`:\n\n```python\nINSTALLED_APPS = [\n    ...\n    \'slippers\',\n    ...\n]\n```\n\n## Documentation\n\nFull documentation can be found on the [Slippers documentation site](https://mitchel.me/slippers/).\n\n## Contributors\n\n[![Contributors](https://contrib.rocks/image?repo=mixxorz/slippers)](https://github.com/mixxorz/slippers/graphs/contributors)\n\n## License\n\nMIT\n',
     'author': 'Mitchel Cabuloy',
     'author_email': 'mixxorz@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mixxorz/slippers',
```

### Comparing `slippers-0.5.0a0/PKG-INFO` & `slippers-0.6.0a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slippers
-Version: 0.5.0a0
+Version: 0.6.0a0
 Summary: Build reusable components in Django without writing a single line of Python.
 Home-page: https://github.com/mixxorz/slippers
 License: MIT
 Keywords: django,components
 Author: Mitchel Cabuloy
 Author-email: mixxorz@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -22,14 +22,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=3.2,<4.2)
 Requires-Dist: PyYAML (>=5.4.0,<7.0.0)
+Requires-Dist: rich (>=12.6.0,<13.0.0)
+Requires-Dist: typeguard (>=2.13.3,<3.0.0)
+Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Repository, https://github.com/mixxorz/slippers
 Description-Content-Type: text/markdown
 
 [![Slippers](https://mitchel.me/slippers/img/slippers.svg)](https://github.com/mixxorz/slippers)
 
 ---
```

