# Comparing `tmp/lxcraft-0.0.2.tar.gz` & `tmp/lxcraft-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxcraft-0.0.2.tar", last modified: Sun Jul 23 19:55:56 2023, max compression
+gzip compressed data, was "lxcraft-0.0.3.tar", last modified: Wed Jul 26 04:46:37 2023, max compression
```

## Comparing `lxcraft-0.0.2.tar` & `lxcraft-0.0.3.tar`

### file list

```diff
@@ -1,62 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:55:56.863034 lxcraft-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-23 19:55:47.000000 lxcraft-0.0.2/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:55:56.855034 lxcraft-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:55:56.859034 lxcraft-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-23 19:55:47.000000 lxcraft-0.0.2/.github/workflows/docker-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-23 19:55:47.000000 lxcraft-0.0.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-23 19:55:47.000000 lxcraft-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-23 19:55:47.000000 lxcraft-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-23 19:55:47.000000 lxcraft-0.0.2/.python-version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:55:56.859034 lxcraft-0.0.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-23 19:55:47.000000 lxcraft-0.0.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-23 19:55:47.000000 lxcraft-0.0.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-23 19:55:47.000000 lxcraft-0.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-23 19:55:47.000000 lxcraft-0.0.2/Justfile
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-23 19:55:47.000000 lxcraft-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-23 19:55:47.000000 lxcraft-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-23 19:55:56.863034 lxcraft-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-23 19:55:47.000000 lxcraft-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:55:56.859034 lxcraft-0.0.2/develop/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-23 19:55:47.000000 lxcraft-0.0.2/develop/docker-bash
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-23 19:55:47.000000 lxcraft-0.0.2/develop/just-test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-23 19:55:47.000000 lxcraft-0.0.2/develop/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:55:56.859034 lxcraft-0.0.2/lxcraft/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-23 19:55:47.000000 lxcraft-0.0.2/lxcraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-23 19:55:47.000000 lxcraft-0.0.2/lxcraft/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-23 19:55:47.000000 lxcraft-0.0.2/lxcraft/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:55:56.863034 lxcraft-0.0.2/lxcraft/debian/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-23 19:55:47.000000 lxcraft-0.0.2/lxcraft/debian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-23 19:55:47.000000 lxcraft-0.0.2/lxcraft/debian/package.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-23 19:55:47.000000 lxcraft-0.0.2/lxcraft/debian/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:55:56.863034 lxcraft-0.0.2/lxcraft/path/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-23 19:55:47.000000 lxcraft-0.0.2/lxcraft/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-23 19:55:47.000000 lxcraft-0.0.2/lxcraft/path/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-23 19:55:47.000000 lxcraft-0.0.2/lxcraft/path/filecontent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-23 19:55:47.000000 lxcraft-0.0.2/lxcraft/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:55:56.863034 lxcraft-0.0.2/lxcraft/python/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-23 19:55:47.000000 lxcraft-0.0.2/lxcraft/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-23 19:55:47.000000 lxcraft-0.0.2/lxcraft/python/pip_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-23 19:55:47.000000 lxcraft-0.0.2/lxcraft/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-23 19:55:56.000000 lxcraft-0.0.2/lxcraft/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:55:56.859034 lxcraft-0.0.2/lxcraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-23 19:55:56.000000 lxcraft-0.0.2/lxcraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-23 19:55:56.000000 lxcraft-0.0.2/lxcraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 19:55:56.000000 lxcraft-0.0.2/lxcraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-23 19:55:56.000000 lxcraft-0.0.2/lxcraft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-23 19:55:56.000000 lxcraft-0.0.2/lxcraft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-23 19:55:47.000000 lxcraft-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-23 19:55:47.000000 lxcraft-0.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 19:55:47.000000 lxcraft-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-23 19:55:56.863034 lxcraft-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-23 19:55:47.000000 lxcraft-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:55:56.863034 lxcraft-0.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 19:55:56.863034 lxcraft-0.0.2/tests/template/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-23 19:55:47.000000 lxcraft-0.0.2/tests/template/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-23 19:55:47.000000 lxcraft-0.0.2/tests/template/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-23 19:55:47.000000 lxcraft-0.0.2/tests/template/wwwkindos.conf
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-23 19:55:47.000000 lxcraft-0.0.2/tests/test_debian_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-23 19:55:47.000000 lxcraft-0.0.2/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-23 19:55:47.000000 lxcraft-0.0.2/tests/test_fastapi_uvicorn_gunicorn_supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-23 19:55:47.000000 lxcraft-0.0.2/tests/test_file_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-23 19:55:47.000000 lxcraft-0.0.2/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-23 19:55:47.000000 lxcraft-0.0.2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.774244 lxcraft-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.766244 lxcraft-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.github/workflows/docker-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.python-version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-26 04:46:27.000000 lxcraft-0.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-26 04:46:27.000000 lxcraft-0.0.3/Justfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-26 04:46:27.000000 lxcraft-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-26 04:46:27.000000 lxcraft-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-26 04:46:37.774244 lxcraft-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-26 04:46:27.000000 lxcraft-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-26 04:46:27.000000 lxcraft-0.0.3/develop/docker-bash
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 04:46:27.000000 lxcraft-0.0.3/develop/just-test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-26 04:46:27.000000 lxcraft-0.0.3/develop/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-26 04:46:27.000000 lxcraft-0.0.3/docs/resource.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/lxcraft/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/lxcraft/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/debian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/debian/apt_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/debian/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/lxcraft/path/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/path/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/path/filecontent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/lxcraft/python/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/python/pip_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.774244 lxcraft-0.0.3/lxcraft/user/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 04:46:37.000000 lxcraft-0.0.3/lxcraft/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/lxcraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-26 04:46:37.000000 lxcraft-0.0.3/lxcraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-26 04:46:37.000000 lxcraft-0.0.3/lxcraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 04:46:37.000000 lxcraft-0.0.3/lxcraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-26 04:46:37.000000 lxcraft-0.0.3/lxcraft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-26 04:46:37.000000 lxcraft-0.0.3/lxcraft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-26 04:46:27.000000 lxcraft-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-26 04:46:27.000000 lxcraft-0.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 04:46:27.000000 lxcraft-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-26 04:46:37.774244 lxcraft-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-26 04:46:27.000000 lxcraft-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.774244 lxcraft-0.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.774244 lxcraft-0.0.3/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/templates/gunicorn_start
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/templates/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/templates/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/templates/wwwkindos.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_apt_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_fastapi_uvicorn_gunicorn_supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_filecontent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_pip_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_resourrce.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_version.py
```

### Comparing `lxcraft-0.0.2/.cruft.json` & `lxcraft-0.0.3/.cruft.json`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.2/.github/workflows/release.yaml` & `lxcraft-0.0.3/.github/workflows/release.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,16 @@
       - 'v*' # Push events to matching v*, i.e. v1.0, v2.1.3
 
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to TestPyPI and PyPI
     runs-on: ubuntu-latest
     permissions:
-      id-token: write
+      id-token: write # Need to publish to PyPI
+      contents: write # Needed to create a release
     steps:
       - name: Checkout code
         uses: actions/checkout@v3
 
       - name: Set up Python 3.10
         uses: actions/setup-python@v4
         with:
```

### Comparing `lxcraft-0.0.2/.gitignore` & `lxcraft-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.2/.pre-commit-config.yaml` & `lxcraft-0.0.3/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -41,10 +41,10 @@
     - id: ruff
 
 -   repo: local
     hooks:
     -   id: run-just
         name: Run tests using just
         entry:
-            just test
+            just all
         language: system
         pass_filenames: false
```

### Comparing `lxcraft-0.0.2/LICENSE` & `lxcraft-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.2/PKG-INFO` & `lxcraft-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1
-Name: lxcraft
-Version: 0.0.2
-Summary: Create the skeleton for a python package/project
-Home-page: https://github.com/joaompinto/lxcraft
-Author: João Pinto
-Author-email: lamego.pinto@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# LXCraft
 
-# Pythonic Configuration Manager for Linux Systems
+A Declarative Configuration Build Tool for Linux Systems
 
 [![PyPi](https://img.shields.io/pypi/v/lxcraft.svg?style=flat-square)](https://pypi.python.org/pypi/lxcraft)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
+A simple declarative configuration build tool for Linux systems.
+
+- 🐍 Pure Python declarative code
+    - No need to learn a new DSL/programming language
+    - Leverage IDE features like inline documentation, code completion, linting, etc.
+- 📏 Ephemeral target system
+    - No need to worry about maintaing the system state
+- Simpler than Chef, Puppet, Ansible, Terraform, SaltStack, etc. due to the above
+
 
 ## How to use
 ```python
 from lxcraft import Plan
-from lxcraft.debian import APTPackages
+from lxcraft.debian import AptPackages
 
-Plan("ensure nginx is installed", [
-    APTPackages(["nginx"])
-]).run()
+Plan([
+    AptPackages(["nginx"])
+]).execute()
 ```
 
 ## How to develop
 
 In order to develop you must use Linux or WSL with docker.
 
 ```sh
```

### Comparing `lxcraft-0.0.2/lxcraft/debian/package.py` & `lxcraft-0.0.3/lxcraft/debian/apt_package.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,39 @@
-import os
 from dataclasses import dataclass
-from functools import partial
 from subprocess import getstatusoutput
 
+import lxcraft
+
 
 @dataclass
-class APTPackages:
+class AptPackages(lxcraft.Resource):
     """List of packages that must be installed"""
 
     package_list: list[str]
 
-    def get_actions(self):
-        package_list = []
+    def create(self):
+        package_list = " ".join(self.package_list)
+        lxcraft.system(f"apt install -y {package_list}")
+
+    def destroy(self):
+        package_list = " ".join(self.package_list)
+        lxcraft.system(f"apt remove -y {package_list}")
+
+    def is_created(self):
         for package in self.package_list:
-            if self.is_installed(package):
-                continue
-            package_list.append(package)
-        if not package_list:
-            return
-        return [partial(self.package_action, " ".join(package_list))]
-
-    def package_action(self, package_list: str):
-        rc = os.system(f"apt install -y {package_list}")
-        if rc != 0:
-            raise Exception(f"Command terminated with non zero exit code {rc}")
+            if not self.is_installed(package):
+                return False
+        return True
+
+    def is_consistent(self):
+        # TODO: Add support for version checking
+        return True
 
     @staticmethod
     def is_installed(package_name: str):
-        rc, _ = getstatusoutput(f"dpkg -s {package_name}")
+        command = (
+            f"dpkg-query --showformat {package_name}"
+            " '${Status}\n' --show passwd | grep -q '^install ok installed$'"
+        )
+        rc, _ = getstatusoutput(command)
+        lxcraft.debug("command", rc, command)
         return rc == 0
```

### Comparing `lxcraft-0.0.2/lxcraft/path/filecontent.py` & `lxcraft-0.0.3/lxcraft/path/filecontent.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,87 @@
 import grp
 import os
 import pwd
 from dataclasses import dataclass, field
 from pathlib import Path
 
-from lxcraft.base import BaseAction, action_engine
+import lxcraft
 
 
 @dataclass
-class FileContent(BaseAction):
+class FileContent(lxcraft.Resource):
     """Create file with content"""
 
     target_path: str
-    source_path: str
+    source_path: str = ""
     owner_user: str = ""
     owner_group: str = ""
     mode: int = 0o644
     replace: dict = field(default_factory=dict)
+    templates_directory = "templates"
 
-    def get_source_text(self):
-        replaced_text = Path(self.source_path).read_text()
+    @staticmethod
+    def set_templates_directory(directory: str):
+        FileContent.templates_directory = directory
+
+    def create(self):
+        Path(self.target_path).write_text(self.get_template_text())
+        if self.owner_user != "" or self.owner_group != "":
+            self.chown()
+        if self.mode:
+            self.chmod()
+
+    def destroy(self):
+        Path(self.target_path).unlink()
+
+    def is_created(self):
+        return Path(self.target_path).exists()
+
+    def is_consistent(self):
+        return (
+            self.is_created()
+            and self.get_template_text() == Path(self.target_path).read_text()
+            and self.mode_matches()
+            and self.owner_matches()
+        )
+
+    def get_template_text(self):
+        if self.source_path:
+            source_path = Path(self.source_path)
+        else:
+            filename = Path(self.target_path).name
+            source_path = Path(self.templates_directory) / filename
+        if source_path.exists():
+            source_text = source_path.read_text()
+        else:
+            raise FileNotFoundError(f"Source file {source_path} not found")
+
+        replaced_text = source_text
         for key, value in self.replace.items():
             replaced_text = replaced_text.replace(key, value)
         return replaced_text
 
-    def content_differs(self):
-        try:
-            target_text = Path(self.target_path).read_text()
-        except FileNotFoundError:
-            return True
-        return self.get_source_text() != target_text
-
-    def owner_differs(self):
-        if not self.owner_user and not self.owner_group:
-            return False
-
-        try:
-            current_uid = Path(self.target_path).stat().st_uid
-            current_gid = Path(self.target_path).stat().st_gid
-        except FileNotFoundError:  # The target file is not yet on the system
-            return True
+    def owner_matches(self):
+        current_uid = Path(self.target_path).stat().st_uid
+        current_gid = Path(self.target_path).stat().st_gid
         if self.owner_user and pwd.getpwnam(self.owner_user).pw_uid != current_uid:
-            return True
+            return False
         if self.owner_group and grp.getgrnam(self.owner_group).gr_gid != current_gid:
-            return True
-
-    def mode_differs(self):
-        try:
-            return self.mode != Path(self.target_path).stat().st_mode & 0o777
-        except FileNotFoundError:
-            return True
-
-    def get_actions(self):
-        return action_engine(
-            {
-                self.content_differs: self.create,
-                self.owner_differs: self.chown,
-                self.mode_differs: self.chmod,
-            }
-        )
+            return False
+        return True
 
-    def create(self):
-        Path(self.target_path).write_text(self.get_source_text())
+    def mode_matches(self):
+        return self.mode == Path(self.target_path).stat().st_mode & 0o777
 
     def chown(self):
-        os.chown(
-            self.target_path,
-            pwd.getpwnam(self.owner_user).pw_uid,
-            grp.getgrnam(self.owner_group).gr_gid,
-        )
+        if self.owner_user == "":
+            uid = os.getuid()
+        else:
+            uid = pwd.getpwnam(self.owner_user).pw_uid
+        if self.owner_group == "":
+            gid = os.getgid()
+        else:
+            gid = grp.getgrnam(self.owner_group).gr_gid
+        os.chown(self.target_path, uid, gid)
 
     def chmod(self):
         os.chmod(self.target_path, self.mode)
```

### Comparing `lxcraft-0.0.2/lxcraft.egg-info/SOURCES.txt` & `lxcraft-0.0.3/lxcraft.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,35 +15,42 @@
 .github/workflows/docker-test.yaml
 .github/workflows/release.yaml
 .vscode/launch.json
 .vscode/settings.json
 develop/docker-bash
 develop/just-test.sh
 develop/setup.sh
+docs/resource.md
 lxcraft/__init__.py
-lxcraft/__main__.py
-lxcraft/base.py
+lxcraft/debug.py
 lxcraft/plan.py
-lxcraft/user.py
+lxcraft/resource.py
+lxcraft/system.py
 lxcraft/version.py
 lxcraft.egg-info/PKG-INFO
 lxcraft.egg-info/SOURCES.txt
 lxcraft.egg-info/dependency_links.txt
 lxcraft.egg-info/entry_points.txt
 lxcraft.egg-info/top_level.txt
 lxcraft/debian/__init__.py
-lxcraft/debian/package.py
+lxcraft/debian/apt_package.py
 lxcraft/debian/service.py
 lxcraft/path/__init__.py
 lxcraft/path/directory.py
 lxcraft/path/filecontent.py
 lxcraft/python/__init__.py
-lxcraft/python/pip_packages.py
-tests/test_debian_package.py
+lxcraft/python/pip_package.py
+lxcraft/user/__init__.py
+lxcraft/user/user.py
+tests/test_apt_package.py
 tests/test_directory.py
 tests/test_fastapi_uvicorn_gunicorn_supervisor.py
-tests/test_file_content.py
+tests/test_filecontent.py
+tests/test_pip_package.py
+tests/test_plan.py
+tests/test_resourrce.py
 tests/test_user.py
 tests/test_version.py
-tests/template/main.py
-tests/template/test.txt
-tests/template/wwwkindos.conf
+tests/templates/gunicorn_start
+tests/templates/main.py
+tests/templates/test.txt
+tests/templates/wwwkindos.conf
```

### Comparing `lxcraft-0.0.2/setup.py` & `lxcraft-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.2/tests/test_fastapi_uvicorn_gunicorn_supervisor.py` & `lxcraft-0.0.3/tests/test_fastapi_uvicorn_gunicorn_supervisor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,42 @@
 #!/usr/bin/env python3
-from lxcraft import Plan, User
-from lxcraft.debian import APTPackages
+import os
+
+from lxcraft import Plan
+from lxcraft.debian import AptPackages
 from lxcraft.path import Directory, FileContent
 from lxcraft.python import PipPackages
+from lxcraft.user import User
 
 USERNAME = "wwwkindos"
 
 
+def custom_file(
+    filename: str, user: str = USERNAME, group: str = USERNAME, mode: int = 0o644
+):
+    return FileContent(
+        filename,
+        owner_user=user,
+        owner_group=group,
+        replace={"{USER}": USERNAME},
+        mode=mode,
+    )
+
+
+def supervisorctl_reload():
+    os.system("supervisorctl reread && supervisorctl update")
+
+
 def test_fastapi_uvicorn_gunicorn_supervisor():
     plan_components = [
         PipPackages(["fastapi", "uvicorn", "gunicorn"]),
-        APTPackages(["supervisor"]),
+        AptPackages(["supervisor"]),
         User(USERNAME),
         Directory(f"/run/user/{USERNAME}"),
-        FileContent(
-            f"/home/{USERNAME}/main.py",
-            "tests/template/main.py",
-            owner_user=USERNAME,
-            owner_group=USERNAME,
-        ),
-        FileContent(
-            f"/etc/supervisor/conf.d/{USERNAME}.conf",
-            f"tests/template/{USERNAME}.conf",
-            replace={"{USER}": USERNAME},
-        ),
+        custom_file(f"/home/{USERNAME}/main.py"),
+        custom_file(f"/home/{USERNAME}/gunicorn_start", mode=0o755),
+        custom_file(
+            f"/etc/supervisor/conf.d/{USERNAME}.conf", "root", "root"
+        ).on_change(supervisorctl_reload),
     ]
-    Plan("my-plan", plan_components).run()
+    with Plan(plan_components) as plan:
+        plan.execute()
```

