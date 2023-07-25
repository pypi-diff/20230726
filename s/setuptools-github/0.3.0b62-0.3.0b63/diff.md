# Comparing `tmp/setuptools-github-0.3.0b62.tar.gz` & `tmp/setuptools-github-0.3.0b63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.0b62.tar", last modified: Tue Jul 25 22:10:47 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.0b63.tar", last modified: Tue Jul 25 22:13:35 2023, max compression
```

## Comparing `setuptools-github-0.3.0b62.tar` & `setuptools-github-0.3.0b63.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:10:47.235353 setuptools-github-0.3.0b62/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-25 22:10:47.235353 setuptools-github-0.3.0b62/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 22:10:47.235353 setuptools-github-0.3.0b62/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:10:47.231353 setuptools-github-0.3.0b62/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-25 22:10:47.000000 setuptools-github-0.3.0b62/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-25 22:10:47.000000 setuptools-github-0.3.0b62/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 22:10:47.000000 setuptools-github-0.3.0b62/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 22:10:47.000000 setuptools-github-0.3.0b62/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 22:10:47.000000 setuptools-github-0.3.0b62/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 22:10:47.000000 setuptools-github-0.3.0b62/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:10:47.231353 setuptools-github-0.3.0b62/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:10:47.235353 setuptools-github-0.3.0b62/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 22:10:47.000000 setuptools-github-0.3.0b62/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:10:47.235353 setuptools-github-0.3.0b62/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-25 22:10:14.000000 setuptools-github-0.3.0b62/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:13:35.592287 setuptools-github-0.3.0b63/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-25 22:13:35.592287 setuptools-github-0.3.0b63/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 22:13:35.592287 setuptools-github-0.3.0b63/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:13:35.588287 setuptools-github-0.3.0b63/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-25 22:13:35.000000 setuptools-github-0.3.0b63/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-25 22:13:35.000000 setuptools-github-0.3.0b63/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 22:13:35.000000 setuptools-github-0.3.0b63/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 22:13:35.000000 setuptools-github-0.3.0b63/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 22:13:35.000000 setuptools-github-0.3.0b63/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 22:13:35.000000 setuptools-github-0.3.0b63/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:13:35.588287 setuptools-github-0.3.0b63/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:13:35.592287 setuptools-github-0.3.0b63/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 22:13:35.000000 setuptools-github-0.3.0b63/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:13:35.592287 setuptools-github-0.3.0b63/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-25 22:12:56.000000 setuptools-github-0.3.0b63/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.0b62/LICENSE` & `setuptools-github-0.3.0b63/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b62/PKG-INFO` & `setuptools-github-0.3.0b63/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.0b62
+Version: 0.3.0b63
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setuptools-github-0.3.0b62/README.md` & `setuptools-github-0.3.0b63/README.md`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b62/setup.py` & `setuptools-github-0.3.0b63/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b62/setuptools_github.egg-info/PKG-INFO` & `setuptools-github-0.3.0b63/setuptools_github.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-github
-Version: 0.3.0b62
+Version: 0.3.0b63
 Summary: supports github releases
 Home-page: https://github.com/cav71/setuptools-github
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setuptools-github-0.3.0b62/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.0b63/setuptools_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b62/src/setuptools_github/checks.py` & `setuptools-github-0.3.0b63/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b62/src/setuptools_github/cli.py` & `setuptools-github-0.3.0b63/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b62/src/setuptools_github/scm.py` & `setuptools-github-0.3.0b63/src/setuptools_github/scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b62/src/setuptools_github/script.py` & `setuptools-github-0.3.0b63/src/setuptools_github/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         options.repo.commit(
             options.initfile, f"version bump {version} -> {new_version}"
         )
 
         print(
             tools.indent(
                 f"""
-        The release is almost completed.
+        The release is almost complete.
 
         To proceed:
             git push origin release/{version}
 
         To rever this script:
             git reset --hard HEAD~1
             git tag -d release/{version}
```

### Comparing `setuptools-github-0.3.0b62/src/setuptools_github/tools.py` & `setuptools-github-0.3.0b63/src/setuptools_github/tools.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b62/tests/conftest.py` & `setuptools-github-0.3.0b63/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b62/tests/test_checks.py` & `setuptools-github-0.3.0b63/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b62/tests/test_cli.py` & `setuptools-github-0.3.0b63/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b62/tests/test_conftest.py` & `setuptools-github-0.3.0b63/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b62/tests/test_scm.py` & `setuptools-github-0.3.0b63/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b62/tests/test_script.py` & `setuptools-github-0.3.0b63/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b62/tests/test_tools.py` & `setuptools-github-0.3.0b63/tests/test_tools.py`

 * *Files identical despite different names*

