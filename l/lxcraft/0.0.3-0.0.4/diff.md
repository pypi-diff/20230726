# Comparing `tmp/lxcraft-0.0.3.tar.gz` & `tmp/lxcraft-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxcraft-0.0.3.tar", last modified: Wed Jul 26 04:46:37 2023, max compression
+gzip compressed data, was "lxcraft-0.0.4.tar", last modified: Wed Jul 26 20:09:42 2023, max compression
```

## Comparing `lxcraft-0.0.3.tar` & `lxcraft-0.0.4.tar`

### file list

```diff
@@ -1,71 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.774244 lxcraft-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.766244 lxcraft-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.github/workflows/docker-test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.python-version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-26 04:46:27.000000 lxcraft-0.0.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-26 04:46:27.000000 lxcraft-0.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-26 04:46:27.000000 lxcraft-0.0.3/Justfile
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-26 04:46:27.000000 lxcraft-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-26 04:46:27.000000 lxcraft-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-26 04:46:37.774244 lxcraft-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-26 04:46:27.000000 lxcraft-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/develop/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-26 04:46:27.000000 lxcraft-0.0.3/develop/docker-bash
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 04:46:27.000000 lxcraft-0.0.3/develop/just-test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-26 04:46:27.000000 lxcraft-0.0.3/develop/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-26 04:46:27.000000 lxcraft-0.0.3/docs/resource.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/lxcraft/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/lxcraft/debian/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/debian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/debian/apt_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/debian/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/lxcraft/path/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/path/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/path/filecontent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/lxcraft/python/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/python/pip_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.774244 lxcraft-0.0.3/lxcraft/user/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-26 04:46:27.000000 lxcraft-0.0.3/lxcraft/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 04:46:37.000000 lxcraft-0.0.3/lxcraft/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.770244 lxcraft-0.0.3/lxcraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-26 04:46:37.000000 lxcraft-0.0.3/lxcraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-26 04:46:37.000000 lxcraft-0.0.3/lxcraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 04:46:37.000000 lxcraft-0.0.3/lxcraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-26 04:46:37.000000 lxcraft-0.0.3/lxcraft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-26 04:46:37.000000 lxcraft-0.0.3/lxcraft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-26 04:46:27.000000 lxcraft-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-26 04:46:27.000000 lxcraft-0.0.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 04:46:27.000000 lxcraft-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-26 04:46:37.774244 lxcraft-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-26 04:46:27.000000 lxcraft-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.774244 lxcraft-0.0.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:46:37.774244 lxcraft-0.0.3/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/templates/gunicorn_start
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/templates/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/templates/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/templates/wwwkindos.conf
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_apt_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_fastapi_uvicorn_gunicorn_supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_filecontent.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_pip_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_resourrce.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-26 04:46:27.000000 lxcraft-0.0.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.508579 lxcraft-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.500579 lxcraft-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.github/workflows/docker-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.python-version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-26 20:09:33.000000 lxcraft-0.0.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-26 20:09:33.000000 lxcraft-0.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-26 20:09:33.000000 lxcraft-0.0.4/Justfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-26 20:09:33.000000 lxcraft-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-26 20:09:33.000000 lxcraft-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-26 20:09:42.508579 lxcraft-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-26 20:09:33.000000 lxcraft-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-26 20:09:33.000000 lxcraft-0.0.4/develop/docker-bash
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 20:09:33.000000 lxcraft-0.0.4/develop/just-test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-26 20:09:33.000000 lxcraft-0.0.4/develop/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-26 20:09:33.000000 lxcraft-0.0.4/docs/debugging.md
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-26 20:09:33.000000 lxcraft-0.0.4/docs/resource.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/lxcraft/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/lxcraft/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/debian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/debian/apt_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/lxcraft/path/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/path/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/path/filecontent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/lxcraft/python/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/python/pip_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.508579 lxcraft-0.0.4/lxcraft/user/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-26 20:09:33.000000 lxcraft-0.0.4/lxcraft/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 20:09:42.000000 lxcraft-0.0.4/lxcraft/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.504579 lxcraft-0.0.4/lxcraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-26 20:09:42.000000 lxcraft-0.0.4/lxcraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-26 20:09:42.000000 lxcraft-0.0.4/lxcraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:09:42.000000 lxcraft-0.0.4/lxcraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-26 20:09:42.000000 lxcraft-0.0.4/lxcraft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-26 20:09:42.000000 lxcraft-0.0.4/lxcraft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-26 20:09:33.000000 lxcraft-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-26 20:09:33.000000 lxcraft-0.0.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:09:33.000000 lxcraft-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-26 20:09:33.000000 lxcraft-0.0.4/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-26 20:09:42.508579 lxcraft-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-26 20:09:33.000000 lxcraft-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.508579 lxcraft-0.0.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:09:42.508579 lxcraft-0.0.4/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/templates/gunicorn_start
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/templates/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/templates/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/templates/wwwkindos.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_apt_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_fastapi_uvicorn_gunicorn_supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_filecontent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_pip_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_resourrce.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-26 20:09:33.000000 lxcraft-0.0.4/tests/test_version.py
```

### Comparing `lxcraft-0.0.3/.cruft.json` & `lxcraft-0.0.4/.cruft.json`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.3/.github/workflows/release.yaml` & `lxcraft-0.0.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.3/.gitignore` & `lxcraft-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.3/.pre-commit-config.yaml` & `lxcraft-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.3/LICENSE` & `lxcraft-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.3/PKG-INFO` & `lxcraft-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxcraft
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple declarative configuration build tool for Linux systems
 Home-page: https://github.com/joaompinto/lxcraft
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lxcraft-0.0.3/README.md` & `lxcraft-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.3/develop/setup.sh` & `lxcraft-0.0.4/develop/setup.sh`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.3/docs/resource.md` & `lxcraft-0.0.4/docs/resource.md`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.3/lxcraft/debian/apt_package.py` & `lxcraft-0.0.4/lxcraft/debian/apt_package.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,13 +27,13 @@
     def is_consistent(self):
         # TODO: Add support for version checking
         return True
 
     @staticmethod
     def is_installed(package_name: str):
         command = (
-            f"dpkg-query --showformat {package_name}"
-            " '${Status}\n' --show passwd | grep -q '^install ok installed$'"
+            "dpkg-query --showformat '${Status}'"
+            f" --show {package_name} | grep -q '^install ok installed$'"
         )
         rc, _ = getstatusoutput(command)
-        lxcraft.debug("command", rc, command)
+        lxcraft.debug("command", command, f"# rc={rc}")
         return rc == 0
```

### Comparing `lxcraft-0.0.3/lxcraft/path/filecontent.py` & `lxcraft-0.0.4/lxcraft/path/filecontent.py`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.3/lxcraft/plan.py` & `lxcraft-0.0.4/lxcraft/plan.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,65 @@
 import sys
 from dataclasses import dataclass, field
 from typing import Callable
 
-from lxcraft.debug import debug
+import lxcraft
 
 from .resource import Resource
 
 
 @dataclass
 class Plan:
-    resources: Resource | list[Resource] = field(
+    resources: list[Resource] = field(
         default_factory=list[Resource]
     )  # List of plan resources
 
     # Check if all the resources are based on Resource to avoid type errors
     def __post_init__(self):
-        if not isinstance(self.resources, list):
-            self.resources = [self.resources]
         assert self.resources, "Plan must have at least one resource"
-        for resource in self.resources:
-            assert isinstance(
-                resource, Resource
-            ), f"{resource} is not based on Resource"
+        # for resource in self.resources:
+        #     assert isinstance(
+        #         resource, Resource
+        #     ), f"{resource} is not based on Resource"
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         for resource in self.resources:
-            debug("destroy", "__exit__ Destroying", resource)
-            resource.destroy()
-
-    def find_missing(self):
-        for resource in self.resources:
-            if not resource.is_created():
-                debug("missing", resource)
-                yield resource
-
-    def find_inconsistent(self):
-        for resource in self.resources:
-            if not resource.is_consistent():
-                yield resource
+            lxcraft.debug("destroy", "__exit__ Destroying", resource)
+            resource.destroy()  # type: ignore[attr-defined]
 
     def try_and_point(self, action: Callable):
-        debug("action", "Trying to execute", action)
+        lxcraft.debug("action", "Trying to execute", action)
         try:
             action()
         except Exception as e:
             print(
                 "EXCEPTION related to ",
-                action.__self__.source_repr(),
+                action.__self__.source_repr(),  # type: ignore[attr-defined]
                 file=sys.stderr,
             )
             raise e
 
     def execute(self):
         """Execute all the actions required to create the resources
         and bring them to a consistent state"""
-        for resource in self.find_missing():
-            self.try_and_point(resource.create)
+        for resource in self.resources:
+            if not resource.is_created():  # type: ignore[attr-defined]
+                lxcraft.debug("action", "Creating missing", resource)
+                self.try_and_point(resource.create)  # type: ignore[attr-defined]
+                on_change_callback = getattr(resource, "on_change_callback", None)
+                if on_change_callback:
+                    lxcraft.debug("action", "on_change", resource, on_change_callback)
+                    on_change_callback()
+            if not resource.is_consistent():  # type: ignore[attr-defined]
+                self.try_and_point(resource.destroy)  # type: ignore[attr-defined]
+                self.try_and_point(resource.create)  # type: ignore[attr-defined]
 
-        for resource in self.find_inconsistent():
-            debug("action", "recreate inconsistent", resource)
-            self.try_and_point(resource.destroy)
-            self.try_and_point(resource.create)
+    def destroy(self):
+        """Destroy all the resources"""
+        for resource in self.resources:
+            lxcraft.debug("destroy", "Destroying all resources")
+            for resource in self.resources:
+                if resource.is_created():  # type: ignore[attr-defined]
+                    self.try_and_point(resource.destroy)  # type: ignore[attr-defined]
```

### Comparing `lxcraft-0.0.3/lxcraft/python/pip_package.py` & `lxcraft-0.0.4/lxcraft/python/pip_package.py`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.3/lxcraft/user/user.py` & `lxcraft-0.0.4/lxcraft/user/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import grp
 import pwd
 from dataclasses import dataclass, field
 
 import lxcraft
 
 
 @dataclass
@@ -37,18 +38,21 @@
             return False
         if self.home is not None and self.home != user_data.pw_dir:
             return False
         if self.uid is not None and self.uid != user_data.pw_uid:
             return False
         if self.gid is not None and self.gid != user_data.pw_gid:
             return False
-        if self.groups is not None and self.groups != user_data.pw_gid:
+        if self.groups is not None and self.groups != self.current_user_groups():
             return False
         return True
 
+    def current_user_groups(self):
+        return [g.gr_name for g in grp.getgrall() if self.username in g.gr_mem]
+
     def create_user(self):
         cmd = f"useradd {self.username}"
         if self.gecos is not None:
             cmd += f" -c {self.gecos}"
         if self.password is not None:
             cmd += f" -p {self.password}"
         if self.shell is not None:
```

### Comparing `lxcraft-0.0.3/lxcraft.egg-info/PKG-INFO` & `lxcraft-0.0.4/lxcraft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxcraft
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple declarative configuration build tool for Linux systems
 Home-page: https://github.com/joaompinto/lxcraft
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lxcraft-0.0.3/lxcraft.egg-info/SOURCES.txt` & `lxcraft-0.0.4/lxcraft.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,46 +6,48 @@
 Justfile
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
+ruff.toml
 setup.cfg
 setup.py
 .github/workflows/docker-test.yaml
 .github/workflows/release.yaml
 .vscode/launch.json
 .vscode/settings.json
 develop/docker-bash
 develop/just-test.sh
 develop/setup.sh
+docs/debugging.md
 docs/resource.md
 lxcraft/__init__.py
 lxcraft/debug.py
 lxcraft/plan.py
 lxcraft/resource.py
 lxcraft/system.py
 lxcraft/version.py
 lxcraft.egg-info/PKG-INFO
 lxcraft.egg-info/SOURCES.txt
 lxcraft.egg-info/dependency_links.txt
 lxcraft.egg-info/entry_points.txt
 lxcraft.egg-info/top_level.txt
 lxcraft/debian/__init__.py
 lxcraft/debian/apt_package.py
-lxcraft/debian/service.py
 lxcraft/path/__init__.py
 lxcraft/path/directory.py
 lxcraft/path/filecontent.py
 lxcraft/python/__init__.py
 lxcraft/python/pip_package.py
 lxcraft/user/__init__.py
 lxcraft/user/user.py
 tests/test_apt_package.py
+tests/test_debug.py
 tests/test_directory.py
 tests/test_fastapi_uvicorn_gunicorn_supervisor.py
 tests/test_filecontent.py
 tests/test_pip_package.py
 tests/test_plan.py
 tests/test_resourrce.py
 tests/test_user.py
```

### Comparing `lxcraft-0.0.3/setup.py` & `lxcraft-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `lxcraft-0.0.3/tests/test_fastapi_uvicorn_gunicorn_supervisor.py` & `lxcraft-0.0.4/tests/test_fastapi_uvicorn_gunicorn_supervisor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 #!/usr/bin/env python3
 import os
 
 from lxcraft import Plan
 from lxcraft.debian import AptPackages
 from lxcraft.path import Directory, FileContent
-from lxcraft.python import PipPackages
 from lxcraft.user import User
 
 USERNAME = "wwwkindos"
 
 
 def custom_file(
     filename: str, user: str = USERNAME, group: str = USERNAME, mode: int = 0o644
 ):
     return FileContent(
         filename,
         owner_user=user,
         owner_group=group,
-        replace={"{USER}": USERNAME},
+        replace={"{USERNAME}": USERNAME},
         mode=mode,
     )
 
 
-def supervisorctl_reload():
-    os.system("supervisorctl reread && supervisorctl update")
-
-
 def test_fastapi_uvicorn_gunicorn_supervisor():
+    def supervisorctl_reload():
+        os.system("supervisorctl reread && supervisorctl update")
+
     plan_components = [
-        PipPackages(["fastapi", "uvicorn", "gunicorn"]),
-        AptPackages(["supervisor"]),
+        AptPackages(["systemctl", "supervisor"]),
+        AptPackages(["python3-fastapi", "uvicorn", "gunicorn"]),
         User(USERNAME),
         Directory(f"/run/user/{USERNAME}"),
+        Directory(f"/var/log/{USERNAME}/"),
         custom_file(f"/home/{USERNAME}/main.py"),
         custom_file(f"/home/{USERNAME}/gunicorn_start", mode=0o755),
         custom_file(
             f"/etc/supervisor/conf.d/{USERNAME}.conf", "root", "root"
         ).on_change(supervisorctl_reload),
     ]
     with Plan(plan_components) as plan:
```

### Comparing `lxcraft-0.0.3/tests/test_filecontent.py` & `lxcraft-0.0.4/tests/test_filecontent.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,51 +7,51 @@
 
 FileContent.set_templates_directory("tests/templates")
 SOURCE_PATH = "tests/templates/test.txt"
 TARGET_PATH = "/tmp/test.txt"
 
 
 def test_filecontent_create():
-    with Plan(FileContent(TARGET_PATH)) as plan:
+    with Plan([FileContent(TARGET_PATH)]) as plan:
         plan.execute()
         target_text = Path(TARGET_PATH).read_text()
         assert "this is a {word} test\n" == target_text
 
-    with Plan(FileContent(TARGET_PATH, SOURCE_PATH)) as plan:
+    with Plan([FileContent(TARGET_PATH, SOURCE_PATH)]) as plan:
         plan.execute()
         target_text = Path(TARGET_PATH).read_text()
         assert "this is a {word} test\n" == target_text
 
     with pytest.raises(FileNotFoundError):
-        with Plan(FileContent(TARGET_PATH, "missing_file")) as plan:
+        with Plan([FileContent(TARGET_PATH, "missing_file")]) as plan:
             plan.execute()
 
 
 def test_filecontent_create_replace():
-    with Plan(FileContent(TARGET_PATH, replace={"{word}": "bananas"})) as plan:
+    with Plan([FileContent(TARGET_PATH, replace={"{word}": "bananas"})]) as plan:
         plan.execute()
         target_text = Path(TARGET_PATH).read_text()
         assert "bananas" in target_text
 
 
 def test_filecontent_chmod():
-    with Plan(FileContent(TARGET_PATH, mode=0o600)) as plan:
+    with Plan([FileContent(TARGET_PATH, mode=0o600)]) as plan:
         plan.execute()
         assert oct(Path(TARGET_PATH).stat().st_mode & 0o777) == "0o600"
 
 
 def test_filencontnet_chown():
     # Adjust owner on creation
-    with Plan(FileContent(TARGET_PATH, owner_user="daemon")) as plan:
+    with Plan([FileContent(TARGET_PATH, owner_user="daemon")]) as plan:
         plan.execute()
         assert Path(TARGET_PATH).stat().st_uid == 1
 
     # Adjust owner after creation
-    Plan(FileContent(TARGET_PATH)).execute()
-    with Plan(FileContent(TARGET_PATH, owner_user="daemon")) as plan:
+    Plan([FileContent(TARGET_PATH)]).execute()
+    with Plan([FileContent(TARGET_PATH, owner_user="daemon")]) as plan:
         plan.execute()
         assert Path(TARGET_PATH).stat().st_uid == 1
 
-    Plan(FileContent(TARGET_PATH)).execute()
-    with Plan(FileContent(TARGET_PATH, owner_group="bin")) as plan:
+    Plan([FileContent(TARGET_PATH)]).execute()
+    with Plan([FileContent(TARGET_PATH, owner_group="bin")]) as plan:
         plan.execute()
         assert Path(TARGET_PATH).stat().st_gid == 2
```

### Comparing `lxcraft-0.0.3/tests/test_plan.py` & `lxcraft-0.0.4/tests/test_plan.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,18 +36,23 @@
         return self.was_created
 
     def is_consistent(self):
         return True
 
 
 def test_plan():
-    with pytest.raises(Exception, match=r"is not based on Resource"):
-        lxcraft.Plan("text")
+    # with pytest.raises(Exception, match=r"is not based on Resource"):
+    #     lxcraft.Plan("text")
 
     # Test the context manager
-    with lxcraft.Plan(MyTestresource()) as plan:
+    with lxcraft.Plan([MyTestresource()]) as plan:
         plan.execute()
+        plan.destroy()
 
-    lxcraft.Plan(MyTestresourceWithActions()).execute()
+    with lxcraft.Plan([MyTestresourceWithActions()]) as plan:
+        plan.execute()
+        plan.destroy()
+
+    lxcraft.Plan([MyTestresourceWithActions()]).execute()
 
     with pytest.raises(Exception, match=r"TestresourceWithActionsException"):
-        lxcraft.Plan(MyTestresourceWithActions(raise_exeception=True)).execute()
+        lxcraft.Plan([MyTestresourceWithActions(raise_exeception=True)]).execute()
```

### Comparing `lxcraft-0.0.3/tests/test_resourrce.py` & `lxcraft-0.0.4/tests/test_resourrce.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     def is_created(self):
         return not self.pending_action
 
     def is_consistent(self):
         return True
 
 
-def test_plan_resource():
-    resource = MyTestresourceWithAction()
-    with lxcraft.Plan(resource) as plan:
-        assert resource.source_repr()
+def test_resource():
+    def change_callback():
+        pass
 
+    resource = MyTestresourceWithAction().on_change(change_callback)
+    assert resource.source_repr()
+    with lxcraft.Plan([resource]) as plan:
         plan.execute()
         plan.execute()
```

