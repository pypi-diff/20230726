# Comparing `tmp/tcod_ecs-3.5.0.tar.gz` & `tmp/tcod_ecs-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcod_ecs-3.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tcod_ecs-4.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tcod_ecs-3.5.0.tar` & `tcod_ecs-4.0.0.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0     1079 2023-07-23 10:27:37.759252 tcod_ecs-3.5.0/LICENSE
--rw-r--r--   0        0        0    10473 2023-07-23 10:27:37.759252 tcod_ecs-3.5.0/README.md
--rw-r--r--   0        0        0     3534 2023-07-23 10:27:37.759252 tcod_ecs-3.5.0/pyproject.toml
--rw-r--r--   0        0        0    44807 2023-07-23 10:27:37.759252 tcod_ecs-3.5.0/tcod/ecs/__init__.py
--rw-r--r--   0        0        0     1512 2023-07-23 10:27:37.759252 tcod_ecs-3.5.0/tcod/ecs/_converter.py
--rw-r--r--   0        0        0      160 2023-07-23 10:27:46.603264 tcod_ecs-3.5.0/tcod/ecs/_version.py
--rw-r--r--   0        0        0        0 2023-07-23 10:27:37.759252 tcod_ecs-3.5.0/tcod/ecs/py.typed
--rw-r--r--   0        0        0    11727 1970-01-01 00:00:00.000000 tcod_ecs-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-26 13:05:26.038310 tcod_ecs-4.0.0/LICENSE
+-rw-r--r--   0        0        0    10473 2023-07-26 13:05:26.038310 tcod_ecs-4.0.0/README.md
+-rw-r--r--   0        0        0     3527 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1394 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/tcod/ecs/__init__.py
+-rw-r--r--   0        0        0     1512 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/tcod/ecs/_converter.py
+-rw-r--r--   0        0        0      160 2023-07-26 13:05:35.514398 tcod_ecs-4.0.0/tcod/ecs/_version.py
+-rw-r--r--   0        0        0    28196 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/tcod/ecs/entity.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/tcod/ecs/py.typed
+-rw-r--r--   0        0        0    11466 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/tcod/ecs/query.py
+-rw-r--r--   0        0        0      914 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/tcod/ecs/typing.py
+-rw-r--r--   0        0        0    11638 2023-07-26 13:05:26.042310 tcod_ecs-4.0.0/tcod/ecs/world.py
+-rw-r--r--   0        0        0    11727 1970-01-01 00:00:00.000000 tcod_ecs-4.0.0/PKG-INFO
```

### Comparing `tcod_ecs-3.5.0/LICENSE` & `tcod_ecs-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcod_ecs-3.5.0/README.md` & `tcod_ecs-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tcod_ecs-3.5.0/pyproject.toml` & `tcod_ecs-4.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,16 @@
 [tool.isort] # https://pycqa.github.io/isort/docs/configuration/options.html
 py_version = "38"
 line_length = 120
 profile = "black"
 skip_gitignore = true
 
 [tool.mypy] # https://mypy.readthedocs.io/en/stable/config_file.html
-files = "**/*.py"
+files = "."
+exclude = ['^build/', '^\.']
 explicit_package_bases = true
 python_version = "3.10"            # Type check Python version with EllipsisType
 warn_unused_configs = true
 disallow_any_generics = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
@@ -94,15 +95,14 @@
     "B",   # flake8-bugbear
     "C4",  # flake8-comprehensions
     "DTZ", # flake8-datetimez
     "EM",  # flake8-errmsg
     "EXE", # flake8-executable
     "RET", # flake8-return
     "ICN", # flake8-import-conventions
-    "INP", # flake8-no-pep420
     "PIE", # flake8-pie
     "PT",  # flake8-pytest-style
     "SIM", # flake8-simplify
     "PTH", # flake8-use-pathlib
     "PL",  # Pylint
     "TRY", # tryceratops
     "RUF", # NumPy-specific rules
```

### Comparing `tcod_ecs-3.5.0/tcod/ecs/_converter.py` & `tcod_ecs-4.0.0/tcod/ecs/_converter.py`

 * *Files identical despite different names*

### Comparing `tcod_ecs-3.5.0/PKG-INFO` & `tcod_ecs-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcod-ecs
-Version: 3.5.0
+Version: 4.0.0
 Summary: A type-hinted Entity Component System based on Python dictionaries and sets.
 Author-email: Kyle Benesch <4b796c65+github@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

