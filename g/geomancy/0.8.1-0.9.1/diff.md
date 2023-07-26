# Comparing `tmp/geomancy-0.8.1.tar.gz` & `tmp/geomancy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomancy-0.8.1.tar", last modified: Tue Jul 25 18:59:09 2023, max compression
+gzip compressed data, was "geomancy-0.9.1.tar", last modified: Wed Jul 26 14:44:17 2023, max compression
```

## Comparing `geomancy-0.8.1.tar` & `geomancy-0.9.1.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:09.007358 geomancy-0.8.1/
--rw-r--r--   0 jlorieau   (501) staff       (20)      256 2023-07-20 19:04:04.000000 geomancy-0.8.1/.editorconfig
--rw-r--r--   0 jlorieau   (501) staff       (20)     1780 2023-07-24 22:25:03.000000 geomancy-0.8.1/.gitignore
--rw-r--r--   0 jlorieau   (501) staff       (20)      233 2023-07-25 16:40:32.000000 geomancy-0.8.1/.readthedocs.yaml
--rw-r--r--   0 jlorieau   (501) staff       (20)    35142 2023-07-19 19:00:29.000000 geomancy-0.8.1/LICENSE.md
--rw-r--r--   0 jlorieau   (501) staff       (20)     4847 2023-07-25 18:59:09.006869 geomancy-0.8.1/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)     4431 2023-07-25 16:59:47.000000 geomancy-0.8.1/README.md
--rw-r--r--   0 jlorieau   (501) staff       (20)     1571 2023-07-25 18:54:25.000000 geomancy-0.8.1/Taskfile.yml
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.979115 geomancy-0.8.1/changelog/
--rw-r--r--   0 jlorieau   (501) staff       (20)      310 2023-07-25 18:53:41.000000 geomancy-0.8.1/changelog/changelog_template.jinja
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.980955 geomancy-0.8.1/docs/
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.982170 geomancy-0.8.1/docs/_static/
--rw-r--r--   0 jlorieau   (501) staff       (20)    49829 2023-07-25 15:23:09.000000 geomancy-0.8.1/docs/_static/geomancy_logo.png
--rw-r--r--   0 jlorieau   (501) staff       (20)     1820 2023-07-25 15:22:31.000000 geomancy-0.8.1/docs/_static/geomancy_logo.svg
--rw-r--r--   0 jlorieau   (501) staff       (20)      736 2023-07-25 18:54:35.000000 geomancy-0.8.1/docs/changelog.md
--rw-r--r--   0 jlorieau   (501) staff       (20)     2122 2023-07-25 15:30:06.000000 geomancy-0.8.1/docs/conf.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      458 2023-07-25 18:44:33.000000 geomancy-0.8.1/docs/index.md
--rw-r--r--   0 jlorieau   (501) staff       (20)      121 2023-07-25 15:07:00.000000 geomancy-0.8.1/docs/quickstart.md
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.982595 geomancy-0.8.1/docs/usage/
--rw-r--r--   0 jlorieau   (501) staff       (20)     6459 2023-07-25 17:03:06.000000 geomancy-0.8.1/docs/usage/index.md
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.984117 geomancy-0.8.1/examples/
--rw-r--r--   0 jlorieau   (501) staff       (20)     1485 2023-07-24 19:24:24.000000 geomancy-0.8.1/examples/geomancy.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)      512 2023-07-22 13:17:41.000000 geomancy-0.8.1/examples/pyproject.toml
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.985426 geomancy-0.8.1/geomancy/
--rw-r--r--   0 jlorieau   (501) staff       (20)       59 2023-07-23 20:49:04.000000 geomancy-0.8.1/geomancy/__description__.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)      485 2023-07-25 18:43:01.000000 geomancy-0.8.1/geomancy/__init__.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.994141 geomancy-0.8.1/geomancy/checks/
--rw-r--r--   0 jlorieau   (501) staff       (20)      345 2023-07-24 12:18:52.000000 geomancy-0.8.1/geomancy/checks/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)    11675 2023-07-24 19:29:23.000000 geomancy-0.8.1/geomancy/checks/base.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1717 2023-07-24 18:15:32.000000 geomancy-0.8.1/geomancy/checks/env.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2426 2023-07-24 15:55:52.000000 geomancy-0.8.1/geomancy/checks/exec.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1549 2023-07-23 16:57:23.000000 geomancy-0.8.1/geomancy/checks/path.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2912 2023-07-24 15:55:58.000000 geomancy-0.8.1/geomancy/checks/python.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     5888 2023-07-24 20:38:18.000000 geomancy-0.8.1/geomancy/checks/utils.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2336 2023-07-24 15:55:27.000000 geomancy-0.8.1/geomancy/checks/version.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.995667 geomancy-0.8.1/geomancy/cli/
--rw-r--r--   0 jlorieau   (501) staff       (20)       42 2023-07-23 11:20:13.000000 geomancy-0.8.1/geomancy/cli/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     9027 2023-07-23 16:16:44.000000 geomancy-0.8.1/geomancy/cli/term.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.996880 geomancy-0.8.1/geomancy/config/
--rw-r--r--   0 jlorieau   (501) staff       (20)      137 2023-07-22 15:14:01.000000 geomancy-0.8.1/geomancy/config/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     9726 2023-07-22 15:36:57.000000 geomancy-0.8.1/geomancy/config/config.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.998093 geomancy-0.8.1/geomancy/environment/
--rw-r--r--   0 jlorieau   (501) staff       (20)      164 2023-07-25 01:07:06.000000 geomancy-0.8.1/geomancy/environment/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     4140 2023-07-25 01:16:29.000000 geomancy-0.8.1/geomancy/environment/load_environment.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     6074 2023-07-25 01:48:52.000000 geomancy-0.8.1/geomancy/main.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.988000 geomancy-0.8.1/geomancy.egg-info/
--rw-r--r--   0 jlorieau   (501) staff       (20)     4847 2023-07-25 18:59:08.000000 geomancy-0.8.1/geomancy.egg-info/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)     1267 2023-07-25 18:59:08.000000 geomancy-0.8.1/geomancy.egg-info/SOURCES.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-07-25 18:59:08.000000 geomancy-0.8.1/geomancy.egg-info/dependency_links.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)       47 2023-07-25 18:59:08.000000 geomancy-0.8.1/geomancy.egg-info/entry_points.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)      124 2023-07-25 18:59:08.000000 geomancy-0.8.1/geomancy.egg-info/requires.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        9 2023-07-25 18:59:08.000000 geomancy-0.8.1/geomancy.egg-info/top_level.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)     2070 2023-07-25 17:48:20.000000 geomancy-0.8.1/pyproject.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-07-25 18:59:09.007465 geomancy-0.8.1/setup.cfg
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.999276 geomancy-0.8.1/tests/
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:09.002973 geomancy-0.8.1/tests/checks/
--rw-r--r--   0 jlorieau   (501) staff       (20)     2955 2023-07-24 19:21:58.000000 geomancy-0.8.1/tests/checks/test_base.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2665 2023-07-23 16:39:02.000000 geomancy-0.8.1/tests/checks/test_env.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1461 2023-07-24 15:35:23.000000 geomancy-0.8.1/tests/checks/test_exec.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2347 2023-07-23 10:43:50.000000 geomancy-0.8.1/tests/checks/test_path.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2442 2023-07-24 15:31:44.000000 geomancy-0.8.1/tests/checks/test_python.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      828 2023-07-22 11:59:17.000000 geomancy-0.8.1/tests/checks/test_utils.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:09.004571 geomancy-0.8.1/tests/config/
--rw-r--r--   0 jlorieau   (501) staff       (20)       73 2023-07-20 16:27:03.000000 geomancy-0.8.1/tests/config/config1.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)     6468 2023-07-22 15:36:00.000000 geomancy-0.8.1/tests/config/test_config.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      524 2023-07-25 04:11:09.000000 geomancy-0.8.1/tests/conftest.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:09.005229 geomancy-0.8.1/tests/data/
--rw-r--r--   0 jlorieau   (501) staff       (20)      159 2023-07-25 01:20:06.000000 geomancy-0.8.1/tests/data/test.env
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:09.005844 geomancy-0.8.1/tests/environment/
--rw-r--r--   0 jlorieau   (501) staff       (20)     3181 2023-07-25 04:09:51.000000 geomancy-0.8.1/tests/environment/test_load_environment.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2655 2023-07-25 04:08:28.000000 geomancy-0.8.1/tests/test_main.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.303730 geomancy-0.9.1/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      345 2023-07-26 14:41:25.000000 geomancy-0.9.1/.editorconfig
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1780 2023-07-24 22:25:03.000000 geomancy-0.9.1/.gitignore
+-rw-r--r--   0 jlorieau   (501) staff       (20)      233 2023-07-25 16:40:32.000000 geomancy-0.9.1/.readthedocs.yaml
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1023 2023-07-26 00:50:48.000000 geomancy-0.9.1/LICENSE
+-rw-r--r--   0 jlorieau   (501) staff       (20)     5792 2023-07-26 14:44:17.303147 geomancy-0.9.1/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)     4612 2023-07-26 14:41:25.000000 geomancy-0.9.1/README.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1711 2023-07-26 14:41:25.000000 geomancy-0.9.1/Taskfile.yaml
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.279383 geomancy-0.9.1/changelog/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      310 2023-07-25 18:53:41.000000 geomancy-0.9.1/changelog/changelog_template.jinja
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.281240 geomancy-0.9.1/docs/
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.282444 geomancy-0.9.1/docs/_static/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      466 2023-07-26 14:41:25.000000 geomancy-0.9.1/docs/_static/custom.css
+-rw-r--r--   0 jlorieau   (501) staff       (20)    49829 2023-07-25 15:23:09.000000 geomancy-0.9.1/docs/_static/geomancy_logo.png
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1858 2023-07-26 14:41:25.000000 geomancy-0.9.1/docs/_static/geomancy_logo.svg
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1281 2023-07-26 14:41:25.000000 geomancy-0.9.1/docs/changelog.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2120 2023-07-26 14:41:25.000000 geomancy-0.9.1/docs/conf.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      563 2023-07-26 14:41:25.000000 geomancy-0.9.1/docs/index.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)      121 2023-07-25 15:07:00.000000 geomancy-0.9.1/docs/quickstart.md
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.282744 geomancy-0.9.1/docs/usage/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     9995 2023-07-26 14:41:25.000000 geomancy-0.9.1/docs/usage/index.md
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.284199 geomancy-0.9.1/examples/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1485 2023-07-24 19:24:24.000000 geomancy-0.9.1/examples/geomancy.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1280 2023-07-26 14:41:25.000000 geomancy-0.9.1/examples/geomancy.yaml
+-rw-r--r--   0 jlorieau   (501) staff       (20)      272 2023-07-26 14:41:25.000000 geomancy-0.9.1/examples/geomancy_flat.yaml
+-rw-r--r--   0 jlorieau   (501) staff       (20)      512 2023-07-22 13:17:41.000000 geomancy-0.9.1/examples/pyproject.toml
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.285208 geomancy-0.9.1/geomancy/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       59 2023-07-23 20:49:04.000000 geomancy-0.9.1/geomancy/__description__.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)      485 2023-07-26 14:43:56.000000 geomancy-0.9.1/geomancy/__init__.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.291693 geomancy-0.9.1/geomancy/checks/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      345 2023-07-24 12:18:52.000000 geomancy-0.9.1/geomancy/checks/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)    11675 2023-07-24 19:29:23.000000 geomancy-0.9.1/geomancy/checks/base.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1717 2023-07-24 18:15:32.000000 geomancy-0.9.1/geomancy/checks/env.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2426 2023-07-24 15:55:52.000000 geomancy-0.9.1/geomancy/checks/exec.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1549 2023-07-23 16:57:23.000000 geomancy-0.9.1/geomancy/checks/path.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2912 2023-07-24 15:55:58.000000 geomancy-0.9.1/geomancy/checks/python.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     5888 2023-07-24 20:38:18.000000 geomancy-0.9.1/geomancy/checks/utils.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2336 2023-07-24 15:55:27.000000 geomancy-0.9.1/geomancy/checks/version.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.293198 geomancy-0.9.1/geomancy/cli/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       42 2023-07-23 11:20:13.000000 geomancy-0.9.1/geomancy/cli/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     9027 2023-07-23 16:16:44.000000 geomancy-0.9.1/geomancy/cli/term.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.294801 geomancy-0.9.1/geomancy/config/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      137 2023-07-22 15:14:01.000000 geomancy-0.9.1/geomancy/config/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     9901 2023-07-26 14:41:25.000000 geomancy-0.9.1/geomancy/config/config.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.296296 geomancy-0.9.1/geomancy/environment/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      164 2023-07-25 01:07:06.000000 geomancy-0.9.1/geomancy/environment/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     4140 2023-07-25 01:16:29.000000 geomancy-0.9.1/geomancy/environment/load_environment.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6683 2023-07-26 14:41:25.000000 geomancy-0.9.1/geomancy/main.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.287484 geomancy-0.9.1/geomancy.egg-info/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     5792 2023-07-26 14:44:17.000000 geomancy-0.9.1/geomancy.egg-info/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1340 2023-07-26 14:44:17.000000 geomancy-0.9.1/geomancy.egg-info/SOURCES.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-07-26 14:44:17.000000 geomancy-0.9.1/geomancy.egg-info/dependency_links.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)       47 2023-07-26 14:44:17.000000 geomancy-0.9.1/geomancy.egg-info/entry_points.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)      136 2023-07-26 14:44:17.000000 geomancy-0.9.1/geomancy.egg-info/requires.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        9 2023-07-26 14:44:17.000000 geomancy-0.9.1/geomancy.egg-info/top_level.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2793 2023-07-26 14:41:25.000000 geomancy-0.9.1/pyproject.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-07-26 14:44:17.303868 geomancy-0.9.1/setup.cfg
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.297353 geomancy-0.9.1/tests/
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.300348 geomancy-0.9.1/tests/checks/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2955 2023-07-24 19:21:58.000000 geomancy-0.9.1/tests/checks/test_base.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2665 2023-07-23 16:39:02.000000 geomancy-0.9.1/tests/checks/test_env.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1461 2023-07-24 15:35:23.000000 geomancy-0.9.1/tests/checks/test_exec.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2347 2023-07-23 10:43:50.000000 geomancy-0.9.1/tests/checks/test_path.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2442 2023-07-24 15:31:44.000000 geomancy-0.9.1/tests/checks/test_python.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      828 2023-07-22 11:59:17.000000 geomancy-0.9.1/tests/checks/test_utils.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.301264 geomancy-0.9.1/tests/config/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       73 2023-07-20 16:27:03.000000 geomancy-0.9.1/tests/config/config1.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6468 2023-07-22 15:36:00.000000 geomancy-0.9.1/tests/config/test_config.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      524 2023-07-25 04:11:09.000000 geomancy-0.9.1/tests/conftest.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.301708 geomancy-0.9.1/tests/data/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      159 2023-07-25 01:20:06.000000 geomancy-0.9.1/tests/data/test.env
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-26 14:44:17.302170 geomancy-0.9.1/tests/environment/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     3181 2023-07-25 04:09:51.000000 geomancy-0.9.1/tests/environment/test_load_environment.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2802 2023-07-26 14:41:25.000000 geomancy-0.9.1/tests/test_main.py
```

### Comparing `geomancy-0.8.1/.gitignore` & `geomancy-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/PKG-INFO` & `geomancy-0.9.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,130 +1,115 @@
-Metadata-Version: 2.1
-Name: geomancy
-Version: 0.8.1
-Summary: Geomancy validates deployment and development environments
-Author: Justin Lorieau
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE.md
-
-<!-- start intro -->
+<!-- start logo -->
 <img src="https://raw.githubusercontent.com/jlorieau/geomancy/main/docs/_static/geomancy_logo.svg" alt="geomancy logo" height="150px"/>
+<!-- end logo -->
 
+<!-- start badges -->
 [![pypi version](https://img.shields.io/pypi/v/geomancy.svg)](https://pypi.org/project/geomancy/)
 [![python versions](https://img.shields.io/pypi/pyversions/geomancy.svg)](https://pypi.org/project/geomancy/)
 [![Black formatting](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Documentation Status](https://readthedocs.org/projects/geomancy/badge/?version=latest)](https://geomancy.readthedocs.io/en/latest/?badge=latest)
-
+<!-- end badges -->
+<!-- start intro -->
 The ``geomancy`` tool makes it easy to check and validate environments, such
 as development, testing and production.
 
-Environment checks and tests are helpful for testing external dependencies,
-like LaTeX, remote dependencies, like AWS buckets or SSM parameters, or for
-checking environments that use the [12-factor](http://12factor.net/) principles.
+Environment checks and tests are helpful for testing the correct setting
+of environment variables, the installation and versions of installed
+executables, the state of external dependencies, like LaTeX packages, or cloud
+resources, or for checking environments that use the
+[12-factor](http://12factor.net/) principles.
 <!-- end intro -->
 
+## Quickstart
+<!-- start quickstart -->
+1. Create a ``.geomancy.yaml`` file with checks.
+
+    ```yaml
+    checks:
+      Environment:
+        desc: Check environment variables common to all development environments
+
+        Username:
+          desc: The current username
+          checkEnv: "{USER}"
+          regex: "[a-z_][a-z0-9_-]*[$]?"
+
+      Paths:
+        desc: Checks the existence of needed files and directories
+        subchecks: any  # at least one of the files must be present
+
+          Geomancy:
+            desc: Check for the 'geomancy.toml' file
+            checkPath: examples/geomancy.toml
+            type: file
+          Pyproject:
+            desc: Check for 'pyproject.toml' file
+            checkPath: examples/pyproject.toml
+            type: file
+
+      Executables:
+        desc: Check the availability of commands and their versions
+
+        Python:
+          desc: Python interpreter ver 3.11 or higher
+          checkExec: python3>=3.11
+    ```
+
+2. Use ``geo`` to run the checks.
+
+    ```shell
+    $ geo
+    =============================== .geomancy.toml ================================
+        checks (9 checks)
+    [✔]   Environment (1 checks)
+    [✔]     Check environment variable '{USER}'...passed
+    [✔]   Paths (2 checks)
+    [✔]     Check path 'examples/geomancy.toml'...passed
+    [✔]     Check path 'examples/pyproject.toml'...passed
+    [✔]   Executables (1 checks)
+    [✔]     Check executable 'python3>=3.11'...passed
+    ========================== PASSED.  8 checks in 0.01s =========================
+    ```
+
+    (By default, ``geomancy`` will search ``.geomancy.y[a]ml``, ``geomancy.y[a]ml``
+    ``.geomancy.toml``, ``geomancy.toml`` and ``pyproject.toml``.)
+<!-- end quickstart -->
+
 ## Features
 <!-- start features -->
 ``geomancy`` can:
 
 - __Environment variables__. Check environment variables are properly set and,
   optionally, check that they have valid values
   ([checkEnv](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkenv))
 - __Paths__. Check file and directory path existence
   ([checkPath](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpath))
 - __Executables__. Check executables are available and, optionally, have the
   minimum or correct versions
   ([checkExec](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkexec))
-- __Python Packages__. Check python packages are availabile and, optionally,
+- __Python Packages__. Check python packages are available and, optionally,
   have the minimum or correct versions
   ([checkPythonPkg](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpythonpkg))
 - __Group Checks__. Nested group checks with conditional (all or any) pass
   criteria ([groups of checks](https://geomancy.readthedocs.io/en/latest/usage/index.html#check-groups))
-- __Environment Substitution__. Subsitute parameter values from environment
+- __Environment Substitution__. Substitute parameter values from environment
   variables. ex: ``checkPath: {HOME}/.geomancy.toml``
+- __Multiple Formats__. Checks files can be in yaml (e.g. ``.geomancy.yaml``)
+  or in [toml](https://toml.io/en/) (e.g. ``.geomancy.toml`` or
+  ``pyproject.toml``)
 <!-- end features -->
 
-## Quickstart
-<!-- start quickstart -->
-Create a ``.geomancy.[toml](https://toml.io/en/)`` file with checks.
-
-```toml
-[checks.Environment]
-desc = "Check environment variables common to all development environments"
-
-    [checks.Environment.Username]
-    desc = "The current username"
-    checkEnv = "{USER}"
-    regex = "[a-z_][a-z0-9_-]*[$]?"
-
-[checks.Paths]
-desc = "Checks the existence of needed files and directories"
-subchecks = "any"  # at least one sub-check should pass
-
-    [checks.Paths.Geomancy]
-    desc = "Check for 'geomancy.toml' file"
-    checkPath = "examples/geomancy.toml"
-    type = "file"
-
-    [checks.Paths.Pyproject]
-    desc = "Check for 'pyproject.toml' file"
-    checkPath = "examples/pyproject.toml"
-    type = "file"
-
-[checks.Executables]
-desc = "Check the availability of commands and their versions"
-
-    [checks.Executables.Python]
-    desc = "Python interpreter"
-    checkExec = "python3>=3.11"
-
-[checks.PythonPackages]
-desc = "Check the presence and, optional, the version of python packages"
-
-    [checks.PythonPackages.geomancy]
-    desc = "Geomancy python package"
-    checkPythonPkg = "geomancy>=0.1"
-```
-
-By default, ``geomancy`` will search ``.geomancy.toml``, ``geomancy.toml`` and
-``pyproject.toml``.
-
-Use ``geo`` to run the checks
-
-```shell
-$ geo
-=============================== .geomancy.toml ================================
-    checks (9 checks)
-[✔]   Environment (1 checks)
-[✔]     Check environment variable '{USER}'...passed
-[✔]   Paths (2 checks)
-[✔]     Check path 'examples/geomancy.toml'...passed
-[✔]     Check path 'examples/pyproject.toml'...passed
-[✔]   Executables (1 checks)
-[✔]     Check executable 'python3>=3.11'...passed
-[✔]   PythonPackages (1 checks)
-[✔]     Check python package 'geomancy>=0.1'...passed
-======================= PASSED. 10 checks in 0.01s =======================
-```
-<!-- end quickstart -->
-
 ## Documentation
 
 For full documentation please see https://geomancy.readthedocs.io/en/latest.
 
 
 ## Bugs or Requests
 Please use the [GitHub issue tracker](https://github.com/jlorieau/geomancy/issues)
 to submit bugs or request features.
 
 ## License
 
 Copyright Justin Lorieau and others, 2023.
 
-Distributed under the terms of the [GPLv3 license](LICENSE.md).
+Distributed under the terms of the [MIT license](LICENSE).
 geomancy is free and open source software.
```

### Comparing `geomancy-0.8.1/README.md` & `geomancy-0.9.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,116 +1,144 @@
-<!-- start intro -->
+Metadata-Version: 2.1
+Name: geomancy
+Version: 0.9.1
+Summary: Geomancy validates deployment and development environments
+Author: Justin Lorieau
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Bug Tracking
+Classifier: Topic :: Software Development :: Debuggers
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Acceptance
+Classifier: Topic :: System :: Monitoring
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Utilities
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
+
+<!-- start logo -->
 <img src="https://raw.githubusercontent.com/jlorieau/geomancy/main/docs/_static/geomancy_logo.svg" alt="geomancy logo" height="150px"/>
+<!-- end logo -->
 
+<!-- start badges -->
 [![pypi version](https://img.shields.io/pypi/v/geomancy.svg)](https://pypi.org/project/geomancy/)
 [![python versions](https://img.shields.io/pypi/pyversions/geomancy.svg)](https://pypi.org/project/geomancy/)
 [![Black formatting](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Documentation Status](https://readthedocs.org/projects/geomancy/badge/?version=latest)](https://geomancy.readthedocs.io/en/latest/?badge=latest)
-
+<!-- end badges -->
+<!-- start intro -->
 The ``geomancy`` tool makes it easy to check and validate environments, such
 as development, testing and production.
 
-Environment checks and tests are helpful for testing external dependencies,
-like LaTeX, remote dependencies, like AWS buckets or SSM parameters, or for
-checking environments that use the [12-factor](http://12factor.net/) principles.
+Environment checks and tests are helpful for testing the correct setting
+of environment variables, the installation and versions of installed
+executables, the state of external dependencies, like LaTeX packages, or cloud
+resources, or for checking environments that use the
+[12-factor](http://12factor.net/) principles.
 <!-- end intro -->
 
+## Quickstart
+<!-- start quickstart -->
+1. Create a ``.geomancy.yaml`` file with checks.
+
+    ```yaml
+    checks:
+      Environment:
+        desc: Check environment variables common to all development environments
+
+        Username:
+          desc: The current username
+          checkEnv: "{USER}"
+          regex: "[a-z_][a-z0-9_-]*[$]?"
+
+      Paths:
+        desc: Checks the existence of needed files and directories
+        subchecks: any  # at least one of the files must be present
+
+          Geomancy:
+            desc: Check for the 'geomancy.toml' file
+            checkPath: examples/geomancy.toml
+            type: file
+          Pyproject:
+            desc: Check for 'pyproject.toml' file
+            checkPath: examples/pyproject.toml
+            type: file
+
+      Executables:
+        desc: Check the availability of commands and their versions
+
+        Python:
+          desc: Python interpreter ver 3.11 or higher
+          checkExec: python3>=3.11
+    ```
+
+2. Use ``geo`` to run the checks.
+
+    ```shell
+    $ geo
+    =============================== .geomancy.toml ================================
+        checks (9 checks)
+    [✔]   Environment (1 checks)
+    [✔]     Check environment variable '{USER}'...passed
+    [✔]   Paths (2 checks)
+    [✔]     Check path 'examples/geomancy.toml'...passed
+    [✔]     Check path 'examples/pyproject.toml'...passed
+    [✔]   Executables (1 checks)
+    [✔]     Check executable 'python3>=3.11'...passed
+    ========================== PASSED.  8 checks in 0.01s =========================
+    ```
+
+    (By default, ``geomancy`` will search ``.geomancy.y[a]ml``, ``geomancy.y[a]ml``
+    ``.geomancy.toml``, ``geomancy.toml`` and ``pyproject.toml``.)
+<!-- end quickstart -->
+
 ## Features
 <!-- start features -->
 ``geomancy`` can:
 
 - __Environment variables__. Check environment variables are properly set and,
   optionally, check that they have valid values
   ([checkEnv](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkenv))
 - __Paths__. Check file and directory path existence
   ([checkPath](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpath))
 - __Executables__. Check executables are available and, optionally, have the
   minimum or correct versions
   ([checkExec](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkexec))
-- __Python Packages__. Check python packages are availabile and, optionally,
+- __Python Packages__. Check python packages are available and, optionally,
   have the minimum or correct versions
   ([checkPythonPkg](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpythonpkg))
 - __Group Checks__. Nested group checks with conditional (all or any) pass
   criteria ([groups of checks](https://geomancy.readthedocs.io/en/latest/usage/index.html#check-groups))
-- __Environment Substitution__. Subsitute parameter values from environment
+- __Environment Substitution__. Substitute parameter values from environment
   variables. ex: ``checkPath: {HOME}/.geomancy.toml``
+- __Multiple Formats__. Checks files can be in yaml (e.g. ``.geomancy.yaml``)
+  or in [toml](https://toml.io/en/) (e.g. ``.geomancy.toml`` or
+  ``pyproject.toml``)
 <!-- end features -->
 
-## Quickstart
-<!-- start quickstart -->
-Create a ``.geomancy.[toml](https://toml.io/en/)`` file with checks.
-
-```toml
-[checks.Environment]
-desc = "Check environment variables common to all development environments"
-
-    [checks.Environment.Username]
-    desc = "The current username"
-    checkEnv = "{USER}"
-    regex = "[a-z_][a-z0-9_-]*[$]?"
-
-[checks.Paths]
-desc = "Checks the existence of needed files and directories"
-subchecks = "any"  # at least one sub-check should pass
-
-    [checks.Paths.Geomancy]
-    desc = "Check for 'geomancy.toml' file"
-    checkPath = "examples/geomancy.toml"
-    type = "file"
-
-    [checks.Paths.Pyproject]
-    desc = "Check for 'pyproject.toml' file"
-    checkPath = "examples/pyproject.toml"
-    type = "file"
-
-[checks.Executables]
-desc = "Check the availability of commands and their versions"
-
-    [checks.Executables.Python]
-    desc = "Python interpreter"
-    checkExec = "python3>=3.11"
-
-[checks.PythonPackages]
-desc = "Check the presence and, optional, the version of python packages"
-
-    [checks.PythonPackages.geomancy]
-    desc = "Geomancy python package"
-    checkPythonPkg = "geomancy>=0.1"
-```
-
-By default, ``geomancy`` will search ``.geomancy.toml``, ``geomancy.toml`` and
-``pyproject.toml``.
-
-Use ``geo`` to run the checks
-
-```shell
-$ geo
-=============================== .geomancy.toml ================================
-    checks (9 checks)
-[✔]   Environment (1 checks)
-[✔]     Check environment variable '{USER}'...passed
-[✔]   Paths (2 checks)
-[✔]     Check path 'examples/geomancy.toml'...passed
-[✔]     Check path 'examples/pyproject.toml'...passed
-[✔]   Executables (1 checks)
-[✔]     Check executable 'python3>=3.11'...passed
-[✔]   PythonPackages (1 checks)
-[✔]     Check python package 'geomancy>=0.1'...passed
-======================= PASSED. 10 checks in 0.01s =======================
-```
-<!-- end quickstart -->
-
 ## Documentation
 
 For full documentation please see https://geomancy.readthedocs.io/en/latest.
 
 
 ## Bugs or Requests
 Please use the [GitHub issue tracker](https://github.com/jlorieau/geomancy/issues)
 to submit bugs or request features.
 
 ## License
 
 Copyright Justin Lorieau and others, 2023.
 
-Distributed under the terms of the [GPLv3 license](LICENSE.md).
+Distributed under the terms of the [MIT license](LICENSE).
 geomancy is free and open source software.
```

### Comparing `geomancy-0.8.1/Taskfile.yml` & `geomancy-0.9.1/Taskfile.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # https://taskfile.dev/
 version: '3'
 
 vars:
     PROJECT_NAME: geomancy
-    SPHINX_BUILD: sphinx-build
+    SPHINX_BUILD: .venv/bin/sphinx-build  # run from within virtualenv
     SPHINX_OPTS: ""
     SPHINX_SOURCE_DIR: .
     SPHINX_BUILD_DIR: _build
 
 tasks:
 
   create-env:
@@ -37,27 +37,31 @@
       - python -m build
       - twine upload dist/*
 
   docs:help:
       desc: Print the docs building help message
       dir: docs
       cmds:
-          - "{{.SPHINX_BUILD}} -M help {{.SPHINX_SOURCE_DIR}} {{.SPHINX_BUILD_DIR}} {{.SPHINX_OPTS}}"
+          - "../{{.SPHINX_BUILD}} -M help {{.SPHINX_SOURCE_DIR}} {{.SPHINX_BUILD_DIR}} {{.SPHINX_OPTS}}"
 
   docs:build:
       desc: Build the docs
       dir: docs
       cmds:
-          - "{{.SPHINX_BUILD}} -M html {{.SPHINX_SOURCE_DIR}} {{.SPHINX_BUILD_DIR}} {{.SPHINX_OPTS}}"
+          - "../{{.SPHINX_BUILD}} -M html {{.SPHINX_SOURCE_DIR}} {{.SPHINX_BUILD_DIR}} -E -a {{.SPHINX_OPTS}}"
+      sources:
+          - "**/*.md"
+          - "**/*.rst"
+          - "_static/**"
 
   docs:clean:
       desc: Clean the docs build directories
       dir: docs
       cmds:
-          - "{{.SPHINX_BUILD}} -M clean {{.SPHINX_SOURCE_DIR}} {{.SPHINX_BUILD_DIR}} {{.SPHINX_OPTS}}"
+          - "../{{.SPHINX_BUILD}} -M clean {{.SPHINX_SOURCE_DIR}} {{.SPHINX_BUILD_DIR}} {{.SPHINX_OPTS}}"
 
   towncrier:cmds:
       desc: A refresher of towncrier commands
       silent: true
       cmds:
           - echo "towncrier create -c {msg} {issue}.{type}.md"
           - echo "towncrier build [--draft] --name {{.PROJECT_NAME}}"
```

### Comparing `geomancy-0.8.1/docs/_static/geomancy_logo.png` & `geomancy-0.9.1/docs/_static/geomancy_logo.png`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/docs/_static/geomancy_logo.svg` & `geomancy-0.9.1/docs/_static/geomancy_logo.svg`

 * *Files 7% similar despite different names*

```diff
@@ -49,66 +49,69 @@
 00000300: 683a 322e 3532 3432 3b73 7472 6f6b 652d  h:2.5242;stroke-
 00000310: 6d69 7465 726c 696d 6974 3a31 303b 7d0a  miterlimit:10;}.
 00000320: 092e 7374 377b 6669 6c6c 3a23 4339 4339  ..st7{fill:#C9C9
 00000330: 4339 3b73 7472 6f6b 653a 2338 4338 4338  C9;stroke:#8C8C8
 00000340: 433b 7374 726f 6b65 2d77 6964 7468 3a32  C;stroke-width:2
 00000350: 2e35 3234 323b 7374 726f 6b65 2d6d 6974  .5242;stroke-mit
 00000360: 6572 6c69 6d69 743a 3130 3b7d 0a09 2e73  erlimit:10;}...s
-00000370: 7438 7b66 696c 6c3a 6e6f 6e65 3b73 7472  t8{fill:none;str
-00000380: 6f6b 653a 2346 4646 4646 463b 7374 726f  oke:#FFFFFF;stro
-00000390: 6b65 2d77 6964 7468 3a37 3b73 7472 6f6b  ke-width:7;strok
-000003a0: 652d 6d69 7465 726c 696d 6974 3a31 303b  e-miterlimit:10;
-000003b0: 7d0a 092e 7374 397b 666f 6e74 2d66 616d  }...st9{font-fam
-000003c0: 696c 793a 2748 656c 7665 7469 6361 4e65  ily:'HelveticaNe
-000003d0: 7565 273b 7d0a 092e 7374 3130 7b66 6f6e  ue';}...st10{fon
-000003e0: 742d 7369 7a65 3a34 3870 783b 7d0a 092e  t-size:48px;}...
-000003f0: 7374 3131 7b66 696c 6c3a 2334 3534 3534  st11{fill:#45454
-00000400: 353b 7d0a 3c2f 7374 796c 653e 0a3c 6720  5;}.</style>.<g 
-00000410: 636c 6173 733d 2273 7430 223e 0a09 3c63  class="st0">..<c
-00000420: 6972 636c 6520 636c 6173 733d 2273 7431  ircle class="st1
-00000430: 2220 6378 3d22 3833 2e39 2220 6379 3d22  " cx="83.9" cy="
-00000440: 3636 2e38 2220 723d 2234 352e 3322 2f3e  66.8" r="45.3"/>
-00000450: 0a09 3c63 6972 636c 6520 636c 6173 733d  ..<circle class=
-00000460: 2273 7432 2220 6378 3d22 3833 2e39 2220  "st2" cx="83.9" 
-00000470: 6379 3d22 3232 2e33 2220 723d 2231 372e  cy="22.3" r="17.
-00000480: 3722 2f3e 0a09 3c63 6972 636c 6520 636c  7"/>..<circle cl
-00000490: 6173 733d 2273 7433 2220 6378 3d22 3833  ass="st3" cx="83
-000004a0: 2e37 2220 6379 3d22 3232 2e33 2220 723d  .7" cy="22.3" r=
-000004b0: 2231 332e 3922 2f3e 0a09 3c63 6972 636c  "13.9"/>..<circl
-000004c0: 6520 636c 6173 733d 2273 7432 2220 6378  e class="st2" cx
-000004d0: 3d22 3132 362e 3222 2063 793d 2235 332e  ="126.2" cy="53.
-000004e0: 3522 2072 3d22 3137 2e37 222f 3e0a 093c  5" r="17.7"/>..<
-000004f0: 6369 7263 6c65 2063 6c61 7373 3d22 7374  circle class="st
-00000500: 3422 2063 783d 2231 3236 2e31 2220 6379  4" cx="126.1" cy
-00000510: 3d22 3533 2e35 2220 723d 2231 332e 3922  ="53.5" r="13.9"
-00000520: 2f3e 0a09 3c63 6972 636c 6520 636c 6173  />..<circle clas
-00000530: 733d 2273 7432 2220 6378 3d22 3431 2e36  s="st2" cx="41.6
-00000540: 2220 6379 3d22 3533 2e35 2220 723d 2231  " cy="53.5" r="1
-00000550: 372e 3722 2f3e 0a09 3c63 6972 636c 6520  7.7"/>..<circle 
-00000560: 636c 6173 733d 2273 7435 2220 6378 3d22  class="st5" cx="
-00000570: 3431 2e36 2220 6379 3d22 3533 2e35 2220  41.6" cy="53.5" 
-00000580: 723d 2231 332e 3922 2f3e 0a09 3c63 6972  r="13.9"/>..<cir
-00000590: 636c 6520 636c 6173 733d 2273 7432 2220  cle class="st2" 
-000005a0: 6378 3d22 3130 392e 3722 2063 793d 2231  cx="109.7" cy="1
-000005b0: 3032 2e37 2220 723d 2231 372e 3722 2f3e  02.7" r="17.7"/>
-000005c0: 0a09 3c63 6972 636c 6520 636c 6173 733d  ..<circle class=
-000005d0: 2273 7436 2220 6378 3d22 3130 392e 3722  "st6" cx="109.7"
-000005e0: 2063 793d 2231 3032 2e37 2220 723d 2231   cy="102.7" r="1
-000005f0: 332e 3922 2f3e 0a09 3c63 6972 636c 6520  3.9"/>..<circle 
-00000600: 636c 6173 733d 2273 7432 2220 6378 3d22  class="st2" cx="
-00000610: 3537 2e36 2220 6379 3d22 3130 322e 3722  57.6" cy="102.7"
-00000620: 2072 3d22 3137 2e37 222f 3e0a 093c 6369   r="17.7"/>..<ci
-00000630: 7263 6c65 2063 6c61 7373 3d22 7374 3722  rcle class="st7"
-00000640: 2063 783d 2235 372e 3622 2063 793d 2231   cx="57.6" cy="1
-00000650: 3032 2e37 2220 723d 2231 332e 3922 2f3e  02.7" r="13.9"/>
-00000660: 0a3c 2f67 3e0a 3c74 6578 7420 7472 616e  .</g>.<text tran
-00000670: 7366 6f72 6d3d 226d 6174 7269 7828 3120  sform="matrix(1 
-00000680: 3020 3020 3120 3636 2e32 3131 3320 3835  0 0 1 66.2113 85
-00000690: 2e30 3136 3629 2220 636c 6173 733d 2273  .0166)" class="s
-000006a0: 7438 2073 7439 2073 7431 3022 3e47 656f  t8 st9 st10">Geo
-000006b0: 6d61 6e63 793c 2f74 6578 743e 0a3c 7465  mancy</text>.<te
-000006c0: 7874 2074 7261 6e73 666f 726d 3d22 6d61  xt transform="ma
-000006d0: 7472 6978 2831 2030 2030 2031 2036 362e  trix(1 0 0 1 66.
-000006e0: 3231 3135 2038 352e 3031 3635 2922 2063  2115 85.0165)" c
-000006f0: 6c61 7373 3d22 7374 3131 2073 7439 2073  lass="st11 st9 s
-00000700: 7431 3022 3e47 656f 6d61 6e63 793c 2f74  t10">Geomancy</t
-00000710: 6578 743e 0a3c 2f73 7667 3e0a            ext>.</svg>.
+00000370: 7438 7b6f 7061 6369 7479 3a30 2e38 3b66  t8{opacity:0.8;f
+00000380: 696c 6c3a 6e6f 6e65 3b73 7472 6f6b 653a  ill:none;stroke:
+00000390: 2346 4646 4646 463b 7374 726f 6b65 2d77  #FFFFFF;stroke-w
+000003a0: 6964 7468 3a35 3b73 7472 6f6b 652d 6d69  idth:5;stroke-mi
+000003b0: 7465 726c 696d 6974 3a31 303b 656e 6162  terlimit:10;enab
+000003c0: 6c65 2d62 6163 6b67 726f 756e 643a 6e65  le-background:ne
+000003d0: 7720 2020 203b 7d0a 092e 7374 397b 666f  w    ;}...st9{fo
+000003e0: 6e74 2d66 616d 696c 793a 2748 656c 7665  nt-family:'Helve
+000003f0: 7469 6361 4e65 7565 273b 7d0a 092e 7374  ticaNeue';}...st
+00000400: 3130 7b66 6f6e 742d 7369 7a65 3a34 3870  10{font-size:48p
+00000410: 783b 7d0a 092e 7374 3131 7b66 696c 6c3a  x;}...st11{fill:
+00000420: 2334 3534 3534 353b 7d0a 3c2f 7374 796c  #454545;}.</styl
+00000430: 653e 0a3c 6720 636c 6173 733d 2273 7430  e>.<g class="st0
+00000440: 223e 0a09 3c63 6972 636c 6520 636c 6173  ">..<circle clas
+00000450: 733d 2273 7431 2220 6378 3d22 3833 2e39  s="st1" cx="83.9
+00000460: 2220 6379 3d22 3636 2e38 2220 723d 2234  " cy="66.8" r="4
+00000470: 352e 3322 2f3e 0a09 3c63 6972 636c 6520  5.3"/>..<circle 
+00000480: 636c 6173 733d 2273 7432 2220 6378 3d22  class="st2" cx="
+00000490: 3833 2e39 2220 6379 3d22 3232 2e33 2220  83.9" cy="22.3" 
+000004a0: 723d 2231 372e 3722 2f3e 0a09 3c63 6972  r="17.7"/>..<cir
+000004b0: 636c 6520 636c 6173 733d 2273 7433 2220  cle class="st3" 
+000004c0: 6378 3d22 3833 2e37 2220 6379 3d22 3232  cx="83.7" cy="22
+000004d0: 2e33 2220 723d 2231 332e 3922 2f3e 0a09  .3" r="13.9"/>..
+000004e0: 3c63 6972 636c 6520 636c 6173 733d 2273  <circle class="s
+000004f0: 7432 2220 6378 3d22 3132 362e 3222 2063  t2" cx="126.2" c
+00000500: 793d 2235 332e 3522 2072 3d22 3137 2e37  y="53.5" r="17.7
+00000510: 222f 3e0a 093c 6369 7263 6c65 2063 6c61  "/>..<circle cla
+00000520: 7373 3d22 7374 3422 2063 783d 2231 3236  ss="st4" cx="126
+00000530: 2e31 2220 6379 3d22 3533 2e35 2220 723d  .1" cy="53.5" r=
+00000540: 2231 332e 3922 2f3e 0a09 3c63 6972 636c  "13.9"/>..<circl
+00000550: 6520 636c 6173 733d 2273 7432 2220 6378  e class="st2" cx
+00000560: 3d22 3431 2e36 2220 6379 3d22 3533 2e35  ="41.6" cy="53.5
+00000570: 2220 723d 2231 372e 3722 2f3e 0a09 3c63  " r="17.7"/>..<c
+00000580: 6972 636c 6520 636c 6173 733d 2273 7435  ircle class="st5
+00000590: 2220 6378 3d22 3431 2e36 2220 6379 3d22  " cx="41.6" cy="
+000005a0: 3533 2e35 2220 723d 2231 332e 3922 2f3e  53.5" r="13.9"/>
+000005b0: 0a09 3c63 6972 636c 6520 636c 6173 733d  ..<circle class=
+000005c0: 2273 7432 2220 6378 3d22 3130 392e 3722  "st2" cx="109.7"
+000005d0: 2063 793d 2231 3032 2e37 2220 723d 2231   cy="102.7" r="1
+000005e0: 372e 3722 2f3e 0a09 3c63 6972 636c 6520  7.7"/>..<circle 
+000005f0: 636c 6173 733d 2273 7436 2220 6378 3d22  class="st6" cx="
+00000600: 3130 392e 3722 2063 793d 2231 3032 2e37  109.7" cy="102.7
+00000610: 2220 723d 2231 332e 3922 2f3e 0a09 3c63  " r="13.9"/>..<c
+00000620: 6972 636c 6520 636c 6173 733d 2273 7432  ircle class="st2
+00000630: 2220 6378 3d22 3537 2e36 2220 6379 3d22  " cx="57.6" cy="
+00000640: 3130 322e 3722 2072 3d22 3137 2e37 222f  102.7" r="17.7"/
+00000650: 3e0a 093c 6369 7263 6c65 2063 6c61 7373  >..<circle class
+00000660: 3d22 7374 3722 2063 783d 2235 372e 3622  ="st7" cx="57.6"
+00000670: 2063 793d 2231 3032 2e37 2220 723d 2231   cy="102.7" r="1
+00000680: 332e 3922 2f3e 0a3c 2f67 3e0a 3c74 6578  3.9"/>.</g>.<tex
+00000690: 7420 7472 616e 7366 6f72 6d3d 226d 6174  t transform="mat
+000006a0: 7269 7828 3120 3020 3020 3120 3636 2e32  rix(1 0 0 1 66.2
+000006b0: 3131 3320 3835 2e30 3136 3629 2220 636c  113 85.0166)" cl
+000006c0: 6173 733d 2273 7438 2073 7439 2073 7431  ass="st8 st9 st1
+000006d0: 3022 3e47 656f 6d61 6e63 793c 2f74 6578  0">Geomancy</tex
+000006e0: 743e 0a3c 7465 7874 2074 7261 6e73 666f  t>.<text transfo
+000006f0: 726d 3d22 6d61 7472 6978 2831 2030 2030  rm="matrix(1 0 0
+00000700: 2031 2036 362e 3231 3135 2038 352e 3031   1 66.2115 85.01
+00000710: 3635 2922 2063 6c61 7373 3d22 7374 3131  65)" class="st11
+00000720: 2073 7439 2073 7431 3022 3e47 656f 6d61   st9 st10">Geoma
+00000730: 6e63 793c 2f74 6578 743e 0a3c 2f73 7667  ncy</text>.</svg
+00000740: 3e0a                                     >.
```

### Comparing `geomancy-0.8.1/docs/conf.py` & `geomancy-0.9.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,8 +52,8 @@
 html_theme = "sphinx_book_theme"
 html_logo = "_static/geomancy_logo.svg"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
-# html_css_files = ["custom.css"]
+html_css_files = ["custom.css"]
```

### Comparing `geomancy-0.8.1/docs/usage/index.md` & `geomancy-0.9.1/docs/usage/index.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,288 +1,396 @@
 # Usage
 
 ## Format
 
-The checks file is formatted in [TOML](https://toml.io/en/), and it contains a
-listing of checks and, optionally, configuration options for ``geomancy``.
+The checks file is formatted in [YAML](https://yaml.org) or [TOML](https://toml.io/en/),
+and it contains a listing of checks and, optionally, configuration options
+for ``geomancy``.
 
 ### Filenames
 
 The checks file may be a dedicated file for ``geomancy``, such as a
-``.geomancy.toml`` file or a ``geomancy.toml`` file in the project root
+``.geomancy.yaml`` or ``.geomancy.toml`` file in the project root
 directory, or it may be incorporated as part of a ``pyproject.toml`` file
 under the ``[tool.geomancy]`` section.
 
 ::::{tab-set}
-
-:::{tab-item} .geomancy.toml
+:::{tab-item} geomancy.yaml
+```yaml
+checks:
+  Username:
+    desc: The current username
+    checkEnv: "{USER}"
+    regex: "[a-z_][a-z0-9_-]*[$]?"
+```
+:::
+:::{tab-item} geomancy.toml
 ```toml
 [checks.Username]
 desc = "The current username"
 checkEnv = "{USER}"
 regex = "[a-z_][a-z0-9_-]*[$]?"
 ```
 :::
-
 :::{tab-item} pyproject.toml
 ```toml
 [tool.geomancy.checks.Username]
 desc = "The current username"
 checkEnv = "{USER}"
 regex = "[a-z_][a-z0-9_-]*[$]?"
 ```
 :::
-
 ::::
 
 ### Nesting and Listing Checks
 
 Checks can be grouped into sections of related checks, and the pass condition
 for child checks can be customized.
 
 ::::{tab-set}
+:::{tab-item} geomancy.yaml
+By default, all child checks must pass for the parent check to pass.
+In this example, the parent check, ``ChecksFile``, may pass if any of the
+3 child checks pass--either ``GeomancyToml``, ``PyprojectToml`` or
+``GeomancyYaml``. This condition is specified by ``subchecks = any`` option.
 
-:::{tab-item} .geomancy.toml
+```yaml
+checksFile:
+  desc: Checks that at least on of the files exists
+  subchecks: any
+
+  GeomancyToml:
+    desc: Check for 'geomancy.toml' file
+    checkPath: examples/geomancy.toml
+    type: file
+  PyprojectToml:
+    desc: Check for 'pyproject.toml' file
+    checkPath: examples/pyproject.toml
+    type: file
+  GeomancyYaml:
+    desc: Check for 'geomancy.yaml' file
+    checkPath: examples/geomancy.yaml
+    type: file
+```
+:::
+:::{tab-item} geomancy.toml
 By default, all child checks must pass for the parent check to pass.
 In this example, the parent check, ``ChecksFile``, may pass if any of the
-3 child checks pass--either ``Geomancy``, ``Pyproject`` or ``missing``. This
-condition is specified by ``subchecks = "any"`` option.
+3 child checks pass--either ``GeomancyToml``, ``PyprojectToml`` or
+``GeomancyYaml``. This condition is specified by ``subchecks = "any"`` option.
 
 ```toml
 [checks.ChecksFile]
 desc = "Checks that at least one checks file exists"
 subchecks = "any"
 
-    [checks.ChecksFile.Geomancy]
-    desc = "Check for 'geomancy.toml' file"
-    checkPath = "examples/geomancy.toml"
-    type = "file"
-
-    [checks.ChecksFile.Pyproject]
-    desc = "Check for 'pyproject.toml' file"
-    checkPath = "examples/pyproject.toml"
-    type = "file"
-
-    [checks.ChecksFile.missing]
-    desc = "Check a missing file"
-    checkPath = ".missing__.txt"
-    type = "file"
+[checks.ChecksFile.GeomancyToml]
+desc = "Check for 'geomancy.toml' file"
+checkPath = "examples/geomancy.toml"
+type = "file"
+
+[checks.ChecksFile.PyprojectToml]
+desc = "Check for 'pyproject.toml' file"
+checkPath = "examples/pyproject.toml"
+type = "file"
+
+[checks.ChecksFile.GeomancyYaml]
+desc = "Check for 'geomancy.yaml' file"
+checkPath = "examples/geomancy.yaml"
+type = "file"
 ```
 :::
+:::{tab-item} pyproject.toml
+By default, all child checks must pass for the parent check to pass.
+In this example, the parent check, ``ChecksFile``, may pass if any of the
+3 child checks pass--either ``GeomancyToml``, ``PyprojectToml`` or
+``GeomancyYaml``. This condition is specified by ``subchecks = "any"`` option.
+
+```toml
+[tool.geomancy.checks.ChecksFile]
+desc = "Checks that at least one checks file exists"
+subchecks = "any"
+
+[tool.geomancy.checks.ChecksFile.GeomancyToml]
+desc = "Check for 'geomancy.toml' file"
+checkPath = "examples/geomancy.toml"
+type = "file"
+
+[tool.geomancy.checks.ChecksFile.PyprojectToml]
+desc = "Check for 'pyproject.toml' file"
+checkPath = "examples/pyproject.toml"
+type = "file"
+
+[tool.geomancy.checks.ChecksFile.GeomancyYaml]
+desc = "Check for 'geomancy.yaml' file"
+checkPath = "examples/geomancy.yaml"
+type = "file"
+```
 
+:::
 ::::
 
 ### Configuration
+
 Checks files may optionally include configuration settings for ``geomancy``.
-These are specifid under the ``[config]`` section or the
-``[tool.geomancy.config]`` section for ``pyproject.toml`` files.
 
 ::::{tab-set}
-
-:::{tab-item} .geomancy.toml
+:::{tab-item} geomancy.yaml
+Configuration settings are specified the ``config`` section.
+```yaml
+config:
+  CHECKBASE:
+    ENV_SUBSTITUTE_DEFAULT: true
+```
+:::
+:::{tab-item} geomancy.toml
+Configuration settings are specified the ``[config]`` section.
 ```toml
 [config]
-  [config.CHECKBASE]
-  ENV_SUBSTITUTE_DEFAULT=true
+[config.CHECKBASE]
+ENV_SUBSTITUTE_DEFAULT = true
 ```
 :::
-
 :::{tab-item} pyproject.toml
+Configuration settings are specified in the ``[tool.geomancy.config]`` section.
 ```toml
 [tool.geomancy.config]
-  [tool.geomancy.config.CHECKBASE]
-  ENV_SUBSTITUTE_DEFAULT=true
+[tool.geomancy.config.CHECKBASE]
+ENV_SUBSTITUTE_DEFAULT = true
 ```
 :::
 ::::
 
 :::{tip}
 All configuration options and their defaults can be listed in
 [TOML](https://toml.io/en/) format using the ``geo --config`` command.
 :::
 
-
-
 ## Checks
 
 The following describes the various checks and their options.
 
 ### checkEnv
 
 Check the existence and, optionally, the value of an environment variable.
 
 :checkEnv: Environment variable to check, wrapped in curly braces for
-    substitution. <br>
-    __aliases__: ``checkEnv``, ``CheckEnv``
+substitution. <br>
+__aliases__: ``checkEnv``, ``CheckEnv``
 :desc: _(Optional)_ The description for the check
 :regex: _(Optional)_ A regular expression to check against the environment
-    variable value
+variable value
 
 ::::{tab-set}
-
-:::{tab-item} Example 1
+:::{tab-item} Example 1 (yaml)
+The ``checkEnv`` check in YAML format.
+```yaml
+checks:
+  Environment:
+    Username:
+      desc: The current username
+      checkEnv: "{USER}"
+      regex: "[a-z_][a-z0-9_-]*[$]?"
+```
+:::
+:::{tab-item} Example 2 (toml)
+The ``checkEnv`` check in TOML format.
 ```toml
 [checks.Environment.Username]
 desc = "The current username"
 checkEnv = "{USER}"
 regex = "[a-z_][a-z0-9_-]*[$]?"
 ```
 :::
-
-:::{tab-item} Example 2 (abbreviated)
+:::{tab-item} Example 3 (toml)
+The ``checkEnv`` check in abbreviated TOML format.
 ```toml
 [checks.Environment]
-Username = {checkEnv = "{USER}", regex="[a-z_][a-z0-9_-]*[$]?"}
+Username = { checkEnv = "{USER}", regex = "[a-z_][a-z0-9_-]*[$]?" }
 ```
 :::
-
 ::::
 
-
 ### checkExec
 
 Check the existence and, optionally, the version of available executables or
 commands.
 
 :checkExec: Executable to check. Additionally, an optional version check
-    can be added with a test operator. <br>
-    __aliases__: ``checkExec``, ``CheckExec``
+can be added with a test operator. <br>
+__aliases__: ``checkExec``, ``CheckExec``
 :desc: _(Optional)_ The description for the check
 
 ::::{tab-set}
-
-:::{tab-item} Example 1
-```toml
-[checks.Executables.Ls]
-desc = "List files"
-checkExec = "ls"
+:::{tab-item} Example 1 (yaml)
+The ``checkExec`` check in YAML format.
+```yaml
+checks:
+  Ls:
+    desc: List files
+    checkExec: "ls"
+```
+:::
+:::{tab-item} Example 2 (yaml)
+The ``checkExec`` check with version checking in YAML format.
+```yaml
+checks:
+  Python:
+    desc: Python interpreter (version 3.11 or higher)
+    checkExec: "python3>=3.11"
 ```
 :::
-
-:::{tab-item} Example 2 (with version)
+:::{tab-item} Example 3 (toml)
+The ``checkExec`` check with version checking in TOML format.
 ```toml
 [checks.Executables.Python]
 desc = "Python interpreter (version 3.11 or higher)"
 checkExec = "python3>=3.11"
 ```
 :::
-
-:::{tab-item} Example 3 (abbreviated)
+:::{tab-item} Example 4 (toml)
+The ``checkExec`` check with version checking in abbreviated TOML format.
 ```toml
 [checks.Executables]
-Python = {checkExec = "python3>=3.11"}
+Python = { checkExec = "python3>=3.11" }
 ```
 :::
-
 ::::
 
-
 ### checkPath
 
 Check the existence and, optionally, the type of a path.
 
 :checkPath: Path to check, which may include environment variables wrapped
-    in curly braces for substitution. <br>
-    __aliases__: ``checkPath``, ``CheckPath``
+in curly braces for substitution. <br>
+__aliases__: ``checkPath``, ``CheckPath``
 :desc: _(Optional)_ The description for the check
 :type: _(Optional)_ Additionally check whether the path corresponds to a
-    valid ``'file'`` or ``'dir'``.
+valid ``'file'`` or ``'dir'``.
 
 ::::{tab-set}
-
-:::{tab-item} Example 1
+:::{tab-item} Example 1 (yaml)
+The ``checkPath`` check in YAML format.
+```yaml
+checks:
+  Pyproject:
+    desc: A project's pyprojectfile
+    checkPath: ./pyproject.toml
+    type: file
+```
+:::
+:::{tab-item} Example 2 (toml)
+The ``checkPath`` check in TOML format.
 ```toml
 [checks.Environment.Pyproject]
 desc = "A project's pyprojectfile"
 checkPath = "./pyproject.toml"
-path_type = "file"
+type = "file"
 ```
 :::
-
-:::{tab-item} Example 2 (abbreviated)
+:::{tab-item} Example 3 (toml)
+The ``checkPath`` check in abbreviated TOML format.
 ```toml
 [checks.Environment]
-Pyproject = {checkPath = "./pyproject.toml", path_type = "file"}
+Pyproject = { checkPath = "./pyproject.toml", type = "file" }
 ```
 :::
-
 ::::
 
 ### checkPythonPkg
 
 Checks whether the python package is installed and, optionally, check its
 version.
 
 :checkPythonPkg: Python package to check. Additionally, an optional version
-    check can be added with a test operator. <br>
-    __aliases__: ``checkPythonPkg``, ``CheckPythonPkg``,
-    ``checkPythonPackage``, ``CheckPythonPackage``
+check can be added with a test operator. <br>
+__aliases__: ``checkPythonPkg``, ``CheckPythonPkg``,
+``checkPythonPackage``, ``CheckPythonPackage``
 :desc: _(Optional)_ The description for the check
 
 ::::{tab-set}
-
-:::{tab-item} Example 1
+:::{tab-item} Example 1 (yaml)
+The ``checkPythonPkg`` check in YAML format.
+```yaml
+checks:
+  PythonPackages:
+    geomancy:
+      desc: Geomancy python package
+      checkPythonPkg: "geomancy>=0.1"
+```
+:::
+:::{tab-item} Example 2 (toml)
+The ``checkPythonPkg`` check in TOML format.
 ```toml
 [checks.PythonPackages.geomancy]
 desc = "Geomancy python package"
 checkPythonPkg = "geomancy>=0.1"
 ```
 :::
-
-:::{tab-item} Example 2 (abbreviated)
+:::{tab-item} Example 3 (toml)
+The ``checkPythonPkg`` check in abbreviated TOML format.
 ```toml
 [checks.PythonPackages]
-geomancy = {checkPythonPkg = "geomancy>=0.1"}
+geomancy = { checkPythonPkg = "geomancy>=0.1" }
 ```
 :::
-
 ::::
 
-
 ### Check Groups
 
 Check groups are sections which contain one or more child checks.
 
 :desc: _(Optional)_ The description for the check section
 :subchecks: _(Optional)_ Either ``'all'`` to require that all sub-checks
-    pass or ``'any'`` to require that only one sub-check passes.<br>
-    Default: ``'all'``<br>
-    __aliases__: ``condition``
+pass or ``'any'`` to require that only one sub-check passes.<br>
+Default: ``'all'``<br>
+__aliases__: ``condition``
 
 ::::{tab-set}
-
-:::{tab-item} Example 1
+:::{tab-item} Example 1 (yaml)
+The following is a check group ``ChecksFile`` with 2 checks, ``Geomancy`` and
+``Pyproject``.
+```yaml
+checksFiles:
+  desc: Checks that at least one checks file exists
+
+  Geomancy:
+    desc: Check for the 'geomancy.toml' file
+    checkPath: examples/geomancy.toml
+    type: file
+  Pyproject:
+    desc: Check for 'pyproject.toml' file
+    checkPath: examples/pyproject.toml
+    type: file
+```
+:::
+:::{tab-item} Example 2 (toml)
 The following is a check group ``ChecksFile`` with 2 checks, ``Geomancy`` and
 ``Pyproject``.
-
 ```toml
 [checks.ChecksFile]
 desc = "Checks that at least one checks file exists"
 subchecks = "any"
 
-    [checks.ChecksFile.Geomancy]
-    desc = "Check for 'geomancy.toml' file"
-    checkPath = "examples/geomancy.toml"
-    type = "file"
-
-    [checks.ChecksFile.Pyproject]
-    desc = "Check for 'pyproject.toml' file"
-    checkPath = "examples/pyproject.toml"
-    type = "file"
+[checks.ChecksFile.Geomancy]
+desc = "Check for 'geomancy.toml' file"
+checkPath = "examples/geomancy.toml"
+type = "file"
+
+[checks.ChecksFile.Pyproject]
+desc = "Check for 'pyproject.toml' file"
+checkPath = "examples/pyproject.toml"
+type = "file"
 ```
 :::
-
-:::{tab-item} Example 2 (abbreviated)
+:::{tab-item} Example 3 (toml)
 The following is a check group ``ChecksFile`` with 2 checks, ``Geomancy`` and
 ``Pyproject``, in abbreviated format.
-
 ```toml
 [checks.ChecksFile]
 subchecks = "any"
 
-Geomancy = {checkPath = "examples/geomancy.toml", type = "file"}
-Pyproject = {checkPath = "examples/pyproject.toml", type = "file"}
+Geomancy = { checkPath = "examples/geomancy.toml", type = "file" }
+Pyproject = { checkPath = "examples/pyproject.toml", type = "file" }
 ```
-
 :::
-
 ::::
```

### Comparing `geomancy-0.8.1/examples/geomancy.toml` & `geomancy-0.9.1/examples/geomancy.toml`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/examples/pyproject.toml` & `geomancy-0.9.1/examples/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/geomancy/checks/base.py` & `geomancy-0.9.1/geomancy/checks/base.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/geomancy/checks/env.py` & `geomancy-0.9.1/geomancy/checks/env.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/geomancy/checks/exec.py` & `geomancy-0.9.1/geomancy/checks/exec.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/geomancy/checks/path.py` & `geomancy-0.9.1/geomancy/checks/path.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/geomancy/checks/python.py` & `geomancy-0.9.1/geomancy/checks/python.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/geomancy/checks/utils.py` & `geomancy-0.9.1/geomancy/checks/utils.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/geomancy/checks/version.py` & `geomancy-0.9.1/geomancy/checks/version.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/geomancy/cli/term.py` & `geomancy-0.9.1/geomancy/cli/term.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/geomancy/config/config.py` & `geomancy-0.9.1/geomancy/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """An instance-wide configuration"""
 import typing as t
 from threading import Lock
 from pathlib import Path
 from collections.abc import Mapping
 import re
 import tomllib
+import logging
 
 __all__ = ("ConfigException", "Config", "Parameter")
 
+logger = logging.getLogger(__name__)
+
 
 class ConfigException(Exception):
     """An exception raised in validating or modifying the config"""
 
 
 class ConfigMeta(type):
     """A metaclass to set up the creation of Config objects and singleton"""
@@ -129,14 +132,15 @@
             elif isinstance(current_value, Config) and len(current_value.__dict__) > 0:
                 # In this case, the update value 'v' is a simple parameter but the
                 # current_value is a sub-config with items in it. This is not allowed.
                 raise ConfigException(
                     f"Cannot replace config section '{k}' with a parameter '{v}'"
                 )
             else:
+                logger.debug(f"Config.update(): set {k}={v}")
                 setattr(self, k, v)
 
     @classmethod
     def load(cls, d: dict, root=True) -> "Config":
         """Load config with values from a dict.
 
         Parameters
@@ -162,14 +166,15 @@
 
             if isinstance(v, dict):
                 # Create a sub Config and load the sub dict
                 sub_config = Config.load(v, root=False)
                 setattr(config, k, sub_config)
             else:
                 # Otherwise just store the value
+                logger.debug(f"Config.load(): set {k}={v}")
                 setattr(config, k, v)
 
         return config
 
     @classmethod
     def toml_loads(cls, s: str) -> "Config":
         """Load config from a string formatted in TOML format.
```

### Comparing `geomancy-0.8.1/geomancy/environment/load_environment.py` & `geomancy-0.9.1/geomancy/environment/load_environment.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/geomancy/main.py` & `geomancy-0.9.1/geomancy/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,33 +6,52 @@
 """
 import typing as t
 import argparse
 import logging
 from pathlib import Path
 import tomllib
 
+import yaml
+
 from . import get_version
 from .config import Config
 from .checks import CheckBase
 from .environment import load_env
 
 __description__ = (Path(__file__).parent / "__description__.txt").read_text().strip()
 
 logger = logging.getLogger(__name__)  # Create a default logger
 config = Config()  # Set up config defaults for the CLI
 
 # Set current version
 config.VERSION = get_version()
 
 # Default paths for checks files
-config.CLI.CHECKS_PATHS = ["pyproject.toml", ".geomancy.toml", "geomancy.toml"]
+config.CLI.CHECKS_PATHS = [
+    "pyproject.toml",
+    ".geomancy.toml",
+    "geomancy.toml",
+    "geomancy.yaml",
+    "geomancy.yml",
+    ".geomancy.yaml",
+    ".geomancy.yml",
+]
+
+# Default file extensions for TOML files
+config.CLI.TOML_EXTS = [".toml"]
+
+# Default file extensions for YAML files
+config.CLI.YAML_EXTS = [".yml", ".yaml"]
 
 # Default paths for settings
 config.CLI.SETTINGS_PATHS = ["{HOME}/.geomancerrc"]
 
+# Default names for config sections in checks files
+config.CLI.CONFIG_NAMES = ["config", "Config"]
+
 
 def filepath(string: str, required: bool = True) -> t.Union["Path", None]:
     """Given a path string, verifies that the path is an existing file and
     converts it to a path.
 
     Parameters
     ----------
@@ -95,15 +114,15 @@
     return parser
 
 
 def setup_logging(debug: bool = False):
     """Set up the default logging"""
     logging.basicConfig(
         level=logging.DEBUG if debug else None,
-        format="%(name)s:%(levelname)s: %(message)s",
+        format="%(levelname)s:%(name)s: %(message)s",
     )
 
 
 def action_check(args: argparse.Namespace) -> t.Union[bool, None]:
     """Handle execution of the 'check' sub-command
 
     Parameters
@@ -132,29 +151,35 @@
         logger.error(f"Could not find a checks file")
         return None
 
     # Convert the checks_files into root checks
     checks = []
     for checks_file in checks_files:
         # Parse the file by filetype
-        if checks_file.suffix in (".toml",):
+        if checks_file.suffix in config.CLI.TOML_EXTS:
             with open(checks_file, "rb") as f:
                 d = tomllib.load(f)
+
+        elif checks_file.suffix in config.CLI.YAML_EXTS:
+            with open(checks_file, "r") as f:
+                d = yaml.load(f, Loader=yaml.SafeLoader)
+
         else:
             continue
 
         # pyproject.toml files have their items placed under the [tool.geomancy]
         # section
         if checks_file.name == "pyproject.toml":
             d = d.get("tool", dict()).get("geomancy", dict())
 
         # Load config section, if available
-        config_section = d.pop("config", None)
-        if isinstance(config_section, dict):
-            config.update(config_section)
+        for config_name in config.CLI.CONFIG_NAMES:
+            config_section = d.pop(config_name, None)
+            if isinstance(config_section, dict):
+                config.update(config_section)
 
         # Load the rest into a root CheckBase
         check = CheckBase.load(d, name=str(checks_file))
         if check is not None:
             checks.append(check)
 
     # Create a root check, if there are a lot of checks
```

### Comparing `geomancy-0.8.1/geomancy.egg-info/PKG-INFO` & `geomancy-0.9.1/geomancy.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,130 +1,144 @@
 Metadata-Version: 2.1
 Name: geomancy
-Version: 0.8.1
+Version: 0.9.1
 Summary: Geomancy validates deployment and development environments
 Author: Justin Lorieau
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Bug Tracking
+Classifier: Topic :: Software Development :: Debuggers
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: Acceptance
+Classifier: Topic :: System :: Monitoring
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Utilities
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
-License-File: LICENSE.md
+License-File: LICENSE
 
-<!-- start intro -->
+<!-- start logo -->
 <img src="https://raw.githubusercontent.com/jlorieau/geomancy/main/docs/_static/geomancy_logo.svg" alt="geomancy logo" height="150px"/>
+<!-- end logo -->
 
+<!-- start badges -->
 [![pypi version](https://img.shields.io/pypi/v/geomancy.svg)](https://pypi.org/project/geomancy/)
 [![python versions](https://img.shields.io/pypi/pyversions/geomancy.svg)](https://pypi.org/project/geomancy/)
 [![Black formatting](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Documentation Status](https://readthedocs.org/projects/geomancy/badge/?version=latest)](https://geomancy.readthedocs.io/en/latest/?badge=latest)
-
+<!-- end badges -->
+<!-- start intro -->
 The ``geomancy`` tool makes it easy to check and validate environments, such
 as development, testing and production.
 
-Environment checks and tests are helpful for testing external dependencies,
-like LaTeX, remote dependencies, like AWS buckets or SSM parameters, or for
-checking environments that use the [12-factor](http://12factor.net/) principles.
+Environment checks and tests are helpful for testing the correct setting
+of environment variables, the installation and versions of installed
+executables, the state of external dependencies, like LaTeX packages, or cloud
+resources, or for checking environments that use the
+[12-factor](http://12factor.net/) principles.
 <!-- end intro -->
 
+## Quickstart
+<!-- start quickstart -->
+1. Create a ``.geomancy.yaml`` file with checks.
+
+    ```yaml
+    checks:
+      Environment:
+        desc: Check environment variables common to all development environments
+
+        Username:
+          desc: The current username
+          checkEnv: "{USER}"
+          regex: "[a-z_][a-z0-9_-]*[$]?"
+
+      Paths:
+        desc: Checks the existence of needed files and directories
+        subchecks: any  # at least one of the files must be present
+
+          Geomancy:
+            desc: Check for the 'geomancy.toml' file
+            checkPath: examples/geomancy.toml
+            type: file
+          Pyproject:
+            desc: Check for 'pyproject.toml' file
+            checkPath: examples/pyproject.toml
+            type: file
+
+      Executables:
+        desc: Check the availability of commands and their versions
+
+        Python:
+          desc: Python interpreter ver 3.11 or higher
+          checkExec: python3>=3.11
+    ```
+
+2. Use ``geo`` to run the checks.
+
+    ```shell
+    $ geo
+    =============================== .geomancy.toml ================================
+        checks (9 checks)
+    [✔]   Environment (1 checks)
+    [✔]     Check environment variable '{USER}'...passed
+    [✔]   Paths (2 checks)
+    [✔]     Check path 'examples/geomancy.toml'...passed
+    [✔]     Check path 'examples/pyproject.toml'...passed
+    [✔]   Executables (1 checks)
+    [✔]     Check executable 'python3>=3.11'...passed
+    ========================== PASSED.  8 checks in 0.01s =========================
+    ```
+
+    (By default, ``geomancy`` will search ``.geomancy.y[a]ml``, ``geomancy.y[a]ml``
+    ``.geomancy.toml``, ``geomancy.toml`` and ``pyproject.toml``.)
+<!-- end quickstart -->
+
 ## Features
 <!-- start features -->
 ``geomancy`` can:
 
 - __Environment variables__. Check environment variables are properly set and,
   optionally, check that they have valid values
   ([checkEnv](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkenv))
 - __Paths__. Check file and directory path existence
   ([checkPath](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpath))
 - __Executables__. Check executables are available and, optionally, have the
   minimum or correct versions
   ([checkExec](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkexec))
-- __Python Packages__. Check python packages are availabile and, optionally,
+- __Python Packages__. Check python packages are available and, optionally,
   have the minimum or correct versions
   ([checkPythonPkg](https://geomancy.readthedocs.io/en/latest/usage/index.html#checkpythonpkg))
 - __Group Checks__. Nested group checks with conditional (all or any) pass
   criteria ([groups of checks](https://geomancy.readthedocs.io/en/latest/usage/index.html#check-groups))
-- __Environment Substitution__. Subsitute parameter values from environment
+- __Environment Substitution__. Substitute parameter values from environment
   variables. ex: ``checkPath: {HOME}/.geomancy.toml``
+- __Multiple Formats__. Checks files can be in yaml (e.g. ``.geomancy.yaml``)
+  or in [toml](https://toml.io/en/) (e.g. ``.geomancy.toml`` or
+  ``pyproject.toml``)
 <!-- end features -->
 
-## Quickstart
-<!-- start quickstart -->
-Create a ``.geomancy.[toml](https://toml.io/en/)`` file with checks.
-
-```toml
-[checks.Environment]
-desc = "Check environment variables common to all development environments"
-
-    [checks.Environment.Username]
-    desc = "The current username"
-    checkEnv = "{USER}"
-    regex = "[a-z_][a-z0-9_-]*[$]?"
-
-[checks.Paths]
-desc = "Checks the existence of needed files and directories"
-subchecks = "any"  # at least one sub-check should pass
-
-    [checks.Paths.Geomancy]
-    desc = "Check for 'geomancy.toml' file"
-    checkPath = "examples/geomancy.toml"
-    type = "file"
-
-    [checks.Paths.Pyproject]
-    desc = "Check for 'pyproject.toml' file"
-    checkPath = "examples/pyproject.toml"
-    type = "file"
-
-[checks.Executables]
-desc = "Check the availability of commands and their versions"
-
-    [checks.Executables.Python]
-    desc = "Python interpreter"
-    checkExec = "python3>=3.11"
-
-[checks.PythonPackages]
-desc = "Check the presence and, optional, the version of python packages"
-
-    [checks.PythonPackages.geomancy]
-    desc = "Geomancy python package"
-    checkPythonPkg = "geomancy>=0.1"
-```
-
-By default, ``geomancy`` will search ``.geomancy.toml``, ``geomancy.toml`` and
-``pyproject.toml``.
-
-Use ``geo`` to run the checks
-
-```shell
-$ geo
-=============================== .geomancy.toml ================================
-    checks (9 checks)
-[✔]   Environment (1 checks)
-[✔]     Check environment variable '{USER}'...passed
-[✔]   Paths (2 checks)
-[✔]     Check path 'examples/geomancy.toml'...passed
-[✔]     Check path 'examples/pyproject.toml'...passed
-[✔]   Executables (1 checks)
-[✔]     Check executable 'python3>=3.11'...passed
-[✔]   PythonPackages (1 checks)
-[✔]     Check python package 'geomancy>=0.1'...passed
-======================= PASSED. 10 checks in 0.01s =======================
-```
-<!-- end quickstart -->
-
 ## Documentation
 
 For full documentation please see https://geomancy.readthedocs.io/en/latest.
 
 
 ## Bugs or Requests
 Please use the [GitHub issue tracker](https://github.com/jlorieau/geomancy/issues)
 to submit bugs or request features.
 
 ## License
 
 Copyright Justin Lorieau and others, 2023.
 
-Distributed under the terms of the [GPLv3 license](LICENSE.md).
+Distributed under the terms of the [MIT license](LICENSE).
 geomancy is free and open source software.
```

### Comparing `geomancy-0.8.1/geomancy.egg-info/SOURCES.txt` & `geomancy-0.9.1/geomancy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 .editorconfig
 .gitignore
 .readthedocs.yaml
-LICENSE.md
+LICENSE
 README.md
-Taskfile.yml
+Taskfile.yaml
 pyproject.toml
 changelog/changelog_template.jinja
 docs/changelog.md
 docs/conf.py
 docs/index.md
 docs/quickstart.md
+docs/_static/custom.css
 docs/_static/geomancy_logo.png
 docs/_static/geomancy_logo.svg
 docs/usage/index.md
 examples/geomancy.toml
+examples/geomancy.yaml
+examples/geomancy_flat.yaml
 examples/pyproject.toml
 geomancy/__description__.txt
 geomancy/__init__.py
 geomancy/main.py
 geomancy.egg-info/PKG-INFO
 geomancy.egg-info/SOURCES.txt
 geomancy.egg-info/dependency_links.txt
```

### Comparing `geomancy-0.8.1/pyproject.toml` & `geomancy-0.9.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -6,19 +6,35 @@
 name = "geomancy"
 authors = [
     {name = "Justin Lorieau"},
 ]
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
+    "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
-    "Development Status :: 4 - Beta"
+    "Environment :: Console",
+    "Environment :: Web Environment",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Information Technology",
+    "License :: OSI Approved :: MIT License",
+    "Topic :: Software Development :: Bug Tracking",
+    "Topic :: Software Development :: Debuggers",
+    "Topic :: Software Development :: Documentation",
+    "Topic :: Software Development :: Quality Assurance",
+    "Topic :: Software Development :: Testing",
+    "Topic :: Software Development :: Testing :: Acceptance",
+    "Topic :: System :: Monitoring",
+    "Topic :: System :: Systems Administration",
+    "Topic :: Utilities",
+    "Development Status :: 4 - Beta",
     ]
 dynamic = ["version", "description"]
+dependencies = ["pyyaml>=6.0"]
 
 [tool.setuptools]
 packages = ["geomancy"]
 
 [tool.setuptools.dynamic]
 version = {attr = "geomancy.__version__"}
 description = {file = "geomancy/__description__.txt"}
@@ -76,15 +92,15 @@
 
     [[tool.towncrier.type]]
     directory = "bugfix"
     name = "Bug Fixes"
     showcontent = true
 
     [[tool.towncrier.type]]
-    directory = "docs"
+    directory = "doc"
     name = "Improved Documentation"
     showcontent = true
 
     [[tool.towncrier.type]]
     directory = "trivial"
     name = "Trivial/Internal Changes"
     showcontent = true
```

### Comparing `geomancy-0.8.1/tests/checks/test_base.py` & `geomancy-0.9.1/tests/checks/test_base.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/tests/checks/test_env.py` & `geomancy-0.9.1/tests/checks/test_env.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/tests/checks/test_exec.py` & `geomancy-0.9.1/tests/checks/test_exec.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/tests/checks/test_path.py` & `geomancy-0.9.1/tests/checks/test_path.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/tests/checks/test_python.py` & `geomancy-0.9.1/tests/checks/test_python.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/tests/checks/test_utils.py` & `geomancy-0.9.1/tests/checks/test_utils.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/tests/config/test_config.py` & `geomancy-0.9.1/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/tests/conftest.py` & `geomancy-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/tests/environment/test_load_environment.py` & `geomancy-0.9.1/tests/environment/test_load_environment.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.8.1/tests/test_main.py` & `geomancy-0.9.1/tests/test_main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Test the main CLI entrypoint"""
 import typing as t
 from pathlib import Path
+from itertools import chain
 import os
 
 import pytest
 
 from geomancy.main import main_cli
 from geomancy.config import Config
 
@@ -78,14 +79,18 @@
 
         # The variables are loaded in the current process
         for name, value in variables.items():
             assert os.environ[name] == value
 
 
 @pytest.mark.parametrize(
-    "options", (Path("examples") / "geomancy.toml", Path("examples") / "pyproject.toml")
+    "options",
+    chain(*tuple(Path("examples").glob(f"*.{ext}") for ext in ("toml", "yaml"))),
 )
 def test_cli_check(run, options):
-    """Test the default checks"""
+    """Test all the checks files in the examples directory"""
     captured = run(str(options))
-    # Check environment variables
-    assert "Check environment variable" in captured.out
+
+    # Check, for example, that environment variables were checked
+    assert any(
+        msg in captured.out for msg in ("Check environment variable", "Check path")
+    )
```

