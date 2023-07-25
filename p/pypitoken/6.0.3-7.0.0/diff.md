# Comparing `tmp/pypitoken-6.0.3.tar.gz` & `tmp/pypitoken-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypitoken-6.0.3.tar", max compression
+gzip compressed data, was "pypitoken-7.0.0.tar", max compression
```

## Comparing `pypitoken-6.0.3.tar` & `pypitoken-7.0.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1072 2023-01-29 21:37:06.896021 pypitoken-6.0.3/LICENSE.rst
--rw-r--r--   0        0        0     4201 2023-01-29 21:37:06.896021 pypitoken-6.0.3/README.rst
--rw-r--r--   0        0        0      872 2023-01-29 21:37:06.896021 pypitoken-6.0.3/pypitoken/__init__.py
--rw-r--r--   0        0        0     1194 2023-01-29 21:37:06.896021 pypitoken-6.0.3/pypitoken/exceptions.py
--rw-r--r--   0        0        0    21094 2023-01-29 21:37:06.896021 pypitoken-6.0.3/pypitoken/restrictions.py
--rw-r--r--   0        0        0    13836 2023-01-29 21:37:06.896021 pypitoken-6.0.3/pypitoken/token.py
--rw-r--r--   0        0        0     1067 2023-01-29 21:37:47.792289 pypitoken-6.0.3/pyproject.toml
--rw-r--r--   0        0        0     5010 1970-01-01 00:00:00.000000 pypitoken-6.0.3/setup.py
--rw-r--r--   0        0        0     5202 1970-01-01 00:00:00.000000 pypitoken-6.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-25 22:19:51.812716 pypitoken-7.0.0/LICENSE.rst
+-rw-r--r--   0        0        0     4201 2023-07-25 22:19:51.812716 pypitoken-7.0.0/README.rst
+-rw-r--r--   0        0        0      872 2023-07-25 22:19:51.812716 pypitoken-7.0.0/pypitoken/__init__.py
+-rw-r--r--   0        0        0     1194 2023-07-25 22:19:51.812716 pypitoken-7.0.0/pypitoken/exceptions.py
+-rw-r--r--   0        0        0    21094 2023-07-25 22:19:51.812716 pypitoken-7.0.0/pypitoken/restrictions.py
+-rw-r--r--   0        0        0    13836 2023-07-25 22:19:51.812716 pypitoken-7.0.0/pypitoken/token.py
+-rw-r--r--   0        0        0     1099 2023-07-25 22:20:06.084939 pypitoken-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 pypitoken-7.0.0/PKG-INFO
```

### Comparing `pypitoken-6.0.3/LICENSE.rst` & `pypitoken-7.0.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pypitoken-6.0.3/README.rst` & `pypitoken-7.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     :alt: MIT License
 
 .. image:: https://img.shields.io/badge/Contributor%20Covenant-v1.4%20adopted-ff69b4.svg
     :target: https://github.com/ewjoachim/pypitoken/blob/main/CODE_OF_CONDUCT.md
     :alt: Contributor Covenant
 
 
-PyPIToken is an open-source Python 3.7+ library for generating and manipulating
+PyPIToken is an open-source Python 3.8+ library for generating and manipulating
 PyPI tokens.
 
 PyPI tokens are very powerful, as that they are based on Macaroons_. They allow
 the bearer to add additional restrictions to an existing token. For example, given
 a PyPI token that can upload releases for any project of its owner, you can generate
 a token that will only allow some projects, or even a single one.
```

### Comparing `pypitoken-6.0.3/pypitoken/__init__.py` & `pypitoken-7.0.0/pypitoken/__init__.py`

 * *Files identical despite different names*

### Comparing `pypitoken-6.0.3/pypitoken/exceptions.py` & `pypitoken-7.0.0/pypitoken/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypitoken-6.0.3/pypitoken/restrictions.py` & `pypitoken-7.0.0/pypitoken/restrictions.py`

 * *Files identical despite different names*

### Comparing `pypitoken-6.0.3/pypitoken/token.py` & `pypitoken-7.0.0/pypitoken/token.py`

 * *Files identical despite different names*

### Comparing `pypitoken-6.0.3/pyproject.toml` & `pypitoken-7.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "pypitoken"
-version = "6.0.3"
+version = "7.0.0"
 description = "Manipulate PyPI API tokens"
 license = "MIT"
 authors = ["Joachim Jablon <ewjoachim@gmail.com>"]
 classifiers = [
     "Topic :: Security",
     "Topic :: System :: Archiving :: Packaging"
 ]
 readme = "README.rst"
 homepage = "https://pypitoken.readthedocs.io/en/latest/"
 repository = "https://github.com/ewjoachim/pypitoken"
 documentation = "https://pypitoken.readthedocs.io/en/latest/"
 keywords = ["pypi", "api", "token", "security", "packaging"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 pymacaroons = "^0.13.0"
 jsonschema = "*"
 typing-extensions = "*"
 
 [tool.poetry.group.releasec.dependencies]
 dunamai = "*"
 
@@ -32,14 +32,14 @@
 [tool.poetry.group.tests.dependencies]
 pytest = "*"
 pytest-cov = "*"
 pytest-mock = "*"
 
 [tool.poetry.group.lint.dependencies]
 black = "*"
-isort = "*"
+isort = { version = "*", python = ">=3.8" }
 flake8 = "*"
 mypy = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pypitoken-6.0.3/PKG-INFO` & `pypitoken-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pypitoken
-Version: 6.0.3
+Version: 7.0.0
 Summary: Manipulate PyPI API tokens
 Home-page: https://pypitoken.readthedocs.io/en/latest/
 License: MIT
 Keywords: pypi,api,token,security,packaging
 Author: Joachim Jablon
 Author-email: ewjoachim@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Archiving :: Packaging
 Requires-Dist: jsonschema
@@ -56,15 +55,15 @@
     :alt: MIT License
 
 .. image:: https://img.shields.io/badge/Contributor%20Covenant-v1.4%20adopted-ff69b4.svg
     :target: https://github.com/ewjoachim/pypitoken/blob/main/CODE_OF_CONDUCT.md
     :alt: Contributor Covenant
 
 
-PyPIToken is an open-source Python 3.7+ library for generating and manipulating
+PyPIToken is an open-source Python 3.8+ library for generating and manipulating
 PyPI tokens.
 
 PyPI tokens are very powerful, as that they are based on Macaroons_. They allow
 the bearer to add additional restrictions to an existing token. For example, given
 a PyPI token that can upload releases for any project of its owner, you can generate
 a token that will only allow some projects, or even a single one.
```

