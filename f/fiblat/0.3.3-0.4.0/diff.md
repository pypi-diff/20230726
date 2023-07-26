# Comparing `tmp/fiblat-0.3.3.tar.gz` & `tmp/fiblat-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiblat-0.3.3.tar", max compression
+gzip compressed data, was "fiblat-0.4.0.tar", max compression
```

## Comparing `fiblat-0.3.3.tar` & `fiblat-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rwxr-xr-x   0        0        0     1070 2019-12-15 22:36:29.090443 fiblat-0.3.3/LICENSE
--rw-r--r--   0        0        0      922 2022-04-11 04:00:28.361585 fiblat-0.3.3/README.md
--rwxr-xr-x   0        0        0       84 2020-01-21 03:06:44.838004 fiblat-0.3.3/fiblat/__init__.py
--rwxr-xr-x   0        0        0     1029 2022-04-08 04:55:51.541446 fiblat-0.3.3/fiblat/_cube_lattice.py
--rwxr-xr-x   0        0        0      985 2022-04-08 01:50:06.811446 fiblat-0.3.3/fiblat/_irrational.py
--rw-r--r--   0        0        0     2631 2022-04-11 03:59:03.161585 fiblat-0.3.3/fiblat/_sphere_lattice.py
--rw-r--r--   0        0        0      628 2022-10-25 15:51:53.547982 fiblat-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1671 2022-10-25 15:52:19.195386 fiblat-0.3.3/setup.py
--rw-r--r--   0        0        0     1652 2022-10-25 15:52:19.195586 fiblat-0.3.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2019-12-15 22:36:29.090443 fiblat-0.4.0/LICENSE
+-rw-r--r--   0        0        0      903 2023-07-26 13:42:05.248327 fiblat-0.4.0/README.md
+-rw-r--r--   0        0        0       84 2023-04-19 04:57:59.345473 fiblat-0.4.0/fiblat/__init__.py
+-rwxr-xr-x   0        0        0     1029 2022-04-08 04:55:51.541446 fiblat-0.4.0/fiblat/_cube_lattice.py
+-rwxr-xr-x   0        0        0      985 2022-04-08 01:50:06.811446 fiblat-0.4.0/fiblat/_irrational.py
+-rw-r--r--   0        0        0     2631 2022-04-11 03:59:03.161585 fiblat-0.4.0/fiblat/_sphere_lattice.py
+-rw-r--r--   0        0        0      597 2023-07-26 13:43:03.488328 fiblat-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1626 1970-01-01 00:00:00.000000 fiblat-0.4.0/PKG-INFO
```

### Comparing `fiblat-0.3.3/LICENSE` & `fiblat-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fiblat-0.3.3/README.md` & `fiblat-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 sphere = sphere_lattice(3, 100)
 ```
 
 Development
 -----------
 
 - setup: `poetry install`
-- tests: `poetry run pytest && poetry run pyre`
+- tests: `poetry run pytest`
```

### Comparing `fiblat-0.3.3/fiblat/_cube_lattice.py` & `fiblat-0.4.0/fiblat/_cube_lattice.py`

 * *Files identical despite different names*

### Comparing `fiblat-0.3.3/fiblat/_irrational.py` & `fiblat-0.4.0/fiblat/_irrational.py`

 * *Files identical despite different names*

### Comparing `fiblat-0.3.3/fiblat/_sphere_lattice.py` & `fiblat-0.4.0/fiblat/_sphere_lattice.py`

 * *Files identical despite different names*

### Comparing `fiblat-0.3.3/pyproject.toml` & `fiblat-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [tool.poetry]
 name = "fiblat"
-version = "0.3.3"
+version = "0.4.0"
 description = "A package for generating evenly distributed points on a sphere"
 repository = "https://github.com/erikbrinkman/fibonacci_lattice"
 authors = ["Erik Brinkman <erik.brinkman@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.pytest.ini_options]
 addopts = "--cov fiblat --cov-report term-missing"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-numba = "^0.56.3"
-numpy = "^1.23.4"
+python = "^3.9"
+numba = "^0.57"
+numpy = "^1.24"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
-pyre-check = "^0.9.16"
+pytest = "^7.4"
+pytest-cov = "^4.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fiblat-0.3.3/PKG-INFO` & `fiblat-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fiblat
-Version: 0.3.3
+Version: 0.4.0
 Summary: A package for generating evenly distributed points on a sphere
 Home-page: https://github.com/erikbrinkman/fibonacci_lattice
 License: MIT
 Author: Erik Brinkman
 Author-email: erik.brinkman@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: numba (>=0.56.3,<0.57.0)
-Requires-Dist: numpy (>=1.23.4,<2.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numba (>=0.57,<0.58)
+Requires-Dist: numpy (>=1.24,<2.0)
 Project-URL: Repository, https://github.com/erikbrinkman/fibonacci_lattice
 Description-Content-Type: text/markdown
 
 Fibonacci Lattice
 =================
 [![pypi](https://img.shields.io/pypi/v/fiblat)](https://pypi.org/project/fiblat/)
 [![build](https://github.com/erikbrinkman/fibonacci_lattice/actions/workflows/build.yml/badge.svg)](https://github.com/erikbrinkman/fibonacci_lattice/actions/workflows/build.yml)
@@ -43,9 +43,9 @@
 sphere = sphere_lattice(3, 100)
 ```
 
 Development
 -----------
 
 - setup: `poetry install`
-- tests: `poetry run pytest && poetry run pyre`
+- tests: `poetry run pytest`
```

