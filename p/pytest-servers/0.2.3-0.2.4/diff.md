# Comparing `tmp/pytest-servers-0.2.3.tar.gz` & `tmp/pytest-servers-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-servers-0.2.3.tar", last modified: Thu Jul 13 17:34:52 2023, max compression
+gzip compressed data, was "pytest-servers-0.2.4.tar", last modified: Wed Jul 26 14:00:16 2023, max compression
```

## Comparing `pytest-servers-0.2.3.tar` & `pytest-servers-0.2.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:34:52.958284 pytest-servers-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:34:52.954284 pytest-servers-0.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:34:52.954284 pytest-servers-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-13 17:34:52.958284 pytest-servers-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-13 17:34:52.958284 pytest-servers-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:34:52.954284 pytest-servers-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:34:52.958284 pytest-servers-0.2.3/src/pytest_servers/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/src/pytest_servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/src/pytest_servers/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/src/pytest_servers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/src/pytest_servers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/src/pytest_servers/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/src/pytest_servers/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/src/pytest_servers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/src/pytest_servers/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/src/pytest_servers/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/src/pytest_servers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:34:52.958284 pytest-servers-0.2.3/src/pytest_servers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-13 17:34:52.000000 pytest-servers-0.2.3/src/pytest_servers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-13 17:34:52.000000 pytest-servers-0.2.3/src/pytest_servers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:34:52.000000 pytest-servers-0.2.3/src/pytest_servers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-13 17:34:52.000000 pytest-servers-0.2.3/src/pytest_servers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 17:34:52.000000 pytest-servers-0.2.3/src/pytest_servers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-13 17:34:52.000000 pytest-servers-0.2.3/src/pytest_servers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 17:34:52.000000 pytest-servers-0.2.3/src/pytest_servers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 17:34:52.958284 pytest-servers-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/tests/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-13 17:34:25.000000 pytest-servers-0.2.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:00:16.334371 pytest-servers-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:00:16.330371 pytest-servers-0.2.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:00:16.330371 pytest-servers-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-26 14:00:16.334371 pytest-servers-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-26 14:00:16.338371 pytest-servers-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:00:16.330371 pytest-servers-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:00:16.334371 pytest-servers-0.2.4/src/pytest_servers/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/src/pytest_servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/src/pytest_servers/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/src/pytest_servers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/src/pytest_servers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/src/pytest_servers/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/src/pytest_servers/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/src/pytest_servers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/src/pytest_servers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/src/pytest_servers/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/src/pytest_servers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:00:16.334371 pytest-servers-0.2.4/src/pytest_servers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-26 14:00:16.000000 pytest-servers-0.2.4/src/pytest_servers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-26 14:00:16.000000 pytest-servers-0.2.4/src/pytest_servers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:00:16.000000 pytest-servers-0.2.4/src/pytest_servers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-26 14:00:16.000000 pytest-servers-0.2.4/src/pytest_servers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:00:16.000000 pytest-servers-0.2.4/src/pytest_servers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-26 14:00:16.000000 pytest-servers-0.2.4/src/pytest_servers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 14:00:16.000000 pytest-servers-0.2.4/src/pytest_servers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:00:16.334371 pytest-servers-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/tests/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-26 13:59:52.000000 pytest-servers-0.2.4/tests/test_utils.py
```

### Comparing `pytest-servers-0.2.3/.cruft.json` & `pytest-servers-0.2.4/.cruft.json`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/.github/dependabot.yml` & `pytest-servers-0.2.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/.github/workflows/release.yml` & `pytest-servers-0.2.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/.github/workflows/tests.yml` & `pytest-servers-0.2.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/.gitignore` & `pytest-servers-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/.pre-commit-config.yaml` & `pytest-servers-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/CODE_OF_CONDUCT.rst` & `pytest-servers-0.2.4/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/CONTRIBUTING.rst` & `pytest-servers-0.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/LICENSE` & `pytest-servers-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/PKG-INFO` & `pytest-servers-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-servers
-Version: 0.2.3
+Version: 0.2.4
 Summary: pytest servers
 Home-page: https://github.com/iterative/pytest-servers
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pytest-servers-0.2.3/README.rst` & `pytest-servers-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/noxfile.py` & `pytest-servers-0.2.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/pyproject.toml` & `pytest-servers-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/setup.cfg` & `pytest-servers-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/src/pytest_servers/azure.py` & `pytest-servers-0.2.4/src/pytest_servers/azure.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     with FileLock(azurite_lock):
         try:
             port = docker_client.api.port(container_name, AZURITE_PORT)[0]["HostPort"]
             container = None
         except NotFound:
             container = docker_client.containers.run(
-                "mcr.microsoft.com/azure-storage/azurite:3.24.0",  # renovate
+                "mcr.microsoft.com/azure-storage/azurite:3.25.0",  # renovate
                 command="azurite-blob --loose --blobHost 0.0.0.0",
                 name=container_name,
                 stdout=True,
                 stderr=True,
                 detach=True,
                 remove=True,
                 ports={f"{AZURITE_PORT}/tcp": None},  # assign a random port
```

### Comparing `pytest-servers-0.2.3/src/pytest_servers/factory.py` & `pytest-servers-0.2.4/src/pytest_servers/factory.py`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/src/pytest_servers/fixtures.py` & `pytest-servers-0.2.4/src/pytest_servers/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/src/pytest_servers/gcs.py` & `pytest-servers-0.2.4/src/pytest_servers/gcs.py`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/src/pytest_servers/s3.py` & `pytest-servers-0.2.4/src/pytest_servers/s3.py`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/src/pytest_servers/utils.py` & `pytest-servers-0.2.4/src/pytest_servers/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/src/pytest_servers.egg-info/PKG-INFO` & `pytest-servers-0.2.4/src/pytest_servers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-servers
-Version: 0.2.3
+Version: 0.2.4
 Summary: pytest servers
 Home-page: https://github.com/iterative/pytest-servers
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pytest-servers-0.2.3/src/pytest_servers.egg-info/SOURCES.txt` & `pytest-servers-0.2.4/src/pytest_servers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/src/pytest_servers.egg-info/requires.txt` & `pytest-servers-0.2.4/src/pytest_servers.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/tests/test_factory.py` & `pytest-servers-0.2.4/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.2.3/tests/test_utils.py` & `pytest-servers-0.2.4/tests/test_utils.py`

 * *Files identical despite different names*

