# Comparing `tmp/pymssgl-2.2.8.dev28.tar.gz` & `tmp/pymssgl-2.2.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymssgl-2.2.8.dev28.tar", last modified: Wed Jul 26 14:19:14 2023, max compression
+gzip compressed data, was "pymssgl-2.2.9.dev0.tar", last modified: Wed Jul 26 14:36:56 2023, max compression
```

## Comparing `pymssgl-2.2.8.dev28.tar` & `pymssgl-2.2.9.dev0.tar`

### file list

```diff
@@ -1,112 +1,111 @@
-drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:19:14.675855 pymssgl-2.2.8.dev28/
--rw-r--r--   0 teserak    (501) staff       (20)       40 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/.dockerignore
-drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:19:14.658580 pymssgl-2.2.8.dev28/.github/
-drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:19:14.658756 pymssgl-2.2.8.dev28/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 teserak    (501) staff       (20)      724 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 teserak    (501) staff       (20)      238 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/.github/dependabot.yml
-drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:19:14.659330 pymssgl-2.2.8.dev28/.github/workflows/
--rw-r--r--   0 teserak    (501) staff       (20)     3213 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/.github/workflows/test_linux.yml
--rw-r--r--   0 teserak    (501) staff       (20)     2507 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/.github/workflows/test_macos.yml
--rw-r--r--   0 teserak    (501) staff       (20)     2317 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/.github/workflows/test_windows.yml
--rw-r--r--   0 teserak    (501) staff       (20)      224 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/.gitignore
--rw-r--r--   0 teserak    (501) staff       (20)      223 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/.pypirc
--rw-r--r--   0 teserak    (501) staff       (20)      505 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/.readthedocs.yaml
--rw-r--r--   0 teserak    (501) staff       (20)    38518 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/ChangeLog.old
--rw-r--r--   0 teserak    (501) staff       (20)    17337 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/ChangeLog.rst
--rw-r--r--   0 teserak    (501) staff       (20)      964 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/Dockerfile
--rw-r--r--   0 teserak    (501) staff       (20)    26436 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/LICENSE
--rw-r--r--   0 teserak    (501) staff       (20)       52 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/MANIFEST.in
--rw-r--r--   0 teserak    (501) staff       (20)     4548 2023-07-26 14:19:14.675954 pymssgl-2.2.8.dev28/PKG-INFO
--rw-r--r--   0 teserak    (501) staff       (20)     2448 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/README.rst
--rw-r--r--   0 teserak    (501) staff       (20)     8473 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/appveyor.yml
-drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:19:14.661281 pymssgl-2.2.8.dev28/dev/
--rw-r--r--   0 teserak    (501) staff       (20)       55 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/__init__.py
-drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:19:14.662476 pymssgl-2.2.8.dev28/dev/appveyor/
--rw-r--r--   0 teserak    (501) staff       (20)     2270 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/appveyor/install-win-iconv.ps1
--rw-r--r--   0 teserak    (501) staff       (20)     7195 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/appveyor/install.ps1
--rw-r--r--   0 teserak    (501) staff       (20)      223 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/appveyor/pypirc
--rw-r--r--   0 teserak    (501) staff       (20)     4130 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/appveyor/run_with_env.cmd
--rw-r--r--   0 teserak    (501) staff       (20)     1362 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/appveyor/sql-server-activate-tcp-fixed-port.ps1
--rw-r--r--   0 teserak    (501) staff       (20)      658 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/appveyor/tests.cfg
--rw-r--r--   0 teserak    (501) staff       (20)     8222 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/build.py
--rwxr-xr-x   0 teserak    (501) staff       (20)     1128 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/build_freetds.sh
--rwxr-xr-x   0 teserak    (501) staff       (20)     3409 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/build_manylinux_wheels.sh
--rw-r--r--   0 teserak    (501) staff       (20)     2533 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/ccompiler.py
--rw-r--r--   0 teserak    (501) staff       (20)       53 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/dev-requirements.pip
--rwxr-xr-x   0 teserak    (501) staff       (20)     2033 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/hudson.sh
--rwxr-xr-x   0 teserak    (501) staff       (20)      920 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/memmonitor.py
--rwxr-xr-x   0 teserak    (501) staff       (20)      464 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/memtest.py
--rwxr-xr-x   0 teserak    (501) staff       (20)       73 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/memtest.sh
--rw-r--r--   0 teserak    (501) staff       (20)      171 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/requirements-dev.txt
--rwxr-xr-x   0 teserak    (501) staff       (20)     1305 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/dev/test_manylinux_wheels.sh
--rw-r--r--   0 teserak    (501) staff       (20)      811 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docker-compose.yml
-drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:19:14.666414 pymssgl-2.2.8.dev28/docs/
--rw-r--r--   0 teserak    (501) staff       (20)     6766 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/Makefile
--rw-r--r--   0 teserak    (501) staff       (20)     4952 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/_mssql_examples.rst
--rw-r--r--   0 teserak    (501) staff       (20)     1010 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/azure.rst
--rw-r--r--   0 teserak    (501) staff       (20)     6130 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/building_and_developing.rst
--rw-r--r--   0 teserak    (501) staff       (20)      160 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/changelog.rst
--rw-r--r--   0 teserak    (501) staff       (20)     9287 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/conf.py
--rw-r--r--   0 teserak    (501) staff       (20)     1726 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/docker.rst
--rw-r--r--   0 teserak    (501) staff       (20)    10196 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/faq.rst
--rw-r--r--   0 teserak    (501) staff       (20)     6000 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/freetds.rst
--rw-r--r--   0 teserak    (501) staff       (20)     2213 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/freetds_and_dates.rst
--rw-r--r--   0 teserak    (501) staff       (20)     1738 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/history.rst
-drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:19:14.666970 pymssgl-2.2.8.dev28/docs/images/
--rw-r--r--   0 teserak    (501) staff       (20)    15267 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/images/pymssql-stack.graphml
--rw-r--r--   0 teserak    (501) staff       (20)    25535 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/images/pymssql-stack.png
--rw-r--r--   0 teserak    (501) staff       (20)     2133 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/index.rst
--rw-r--r--   0 teserak    (501) staff       (20)     4106 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/intro.rst
--rw-r--r--   0 teserak    (501) staff       (20)     6703 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/make.bat
--rw-r--r--   0 teserak    (501) staff       (20)     5513 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/migrate_1_x_to_2_x.rst
--rw-r--r--   0 teserak    (501) staff       (20)     8572 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/pymssql_examples.rst
-drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:19:14.667656 pymssgl-2.2.8.dev28/docs/ref/
--rw-r--r--   0 teserak    (501) staff       (20)    18085 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/ref/_mssql.rst
--rw-r--r--   0 teserak    (501) staff       (20)    18441 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/ref/pymssql.rst
--rw-r--r--   0 teserak    (501) staff       (20)     3943 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/release_notes.rst
--rw-r--r--   0 teserak    (501) staff       (20)       93 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/requirements.txt
--rw-r--r--   0 teserak    (501) staff       (20)       59 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/docs/todo.rst
--rw-r--r--   0 teserak    (501) staff       (20)      292 2023-07-26 14:01:33.000000 pymssgl-2.2.8.dev28/pyproject.toml
--rw-r--r--   0 teserak    (501) staff       (20)      447 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/pytest.ini
--rw-r--r--   0 teserak    (501) staff       (20)      149 2023-07-26 14:19:14.676213 pymssgl-2.2.8.dev28/setup.cfg
--rw-r--r--   0 teserak    (501) staff       (20)    11908 2023-07-26 14:19:07.000000 pymssgl-2.2.8.dev28/setup.py
-drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:19:14.653952 pymssgl-2.2.8.dev28/src/
-drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:19:14.668570 pymssgl-2.2.8.dev28/src/pymssgl.egg-info/
--rw-r--r--   0 teserak    (501) staff       (20)     4548 2023-07-26 14:19:14.000000 pymssgl-2.2.8.dev28/src/pymssgl.egg-info/PKG-INFO
--rw-r--r--   0 teserak    (501) staff       (20)     2161 2023-07-26 14:19:14.000000 pymssgl-2.2.8.dev28/src/pymssgl.egg-info/SOURCES.txt
--rw-r--r--   0 teserak    (501) staff       (20)        1 2023-07-26 14:19:14.000000 pymssgl-2.2.8.dev28/src/pymssgl.egg-info/dependency_links.txt
--rw-r--r--   0 teserak    (501) staff       (20)        1 2023-07-26 14:19:14.000000 pymssgl-2.2.8.dev28/src/pymssgl.egg-info/not-zip-safe
--rw-r--r--   0 teserak    (501) staff       (20)        8 2023-07-26 14:19:14.000000 pymssgl-2.2.8.dev28/src/pymssgl.egg-info/top_level.txt
-drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:19:14.670762 pymssgl-2.2.8.dev28/src/pymssql/
--rw-r--r--   0 teserak    (501) staff       (20)      131 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/src/pymssql/__init__.py
--rw-r--r--   0 teserak    (501) staff       (20)     2082 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/src/pymssql/_mssql.pxd
--rw-r--r--   0 teserak    (501) staff       (20)    75831 2023-07-26 14:02:31.000000 pymssgl-2.2.8.dev28/src/pymssql/_mssql.pyx
--rw-r--r--   0 teserak    (501) staff       (20)    23380 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/src/pymssql/_pymssql.pyx
--rw-r--r--   0 teserak    (501) staff       (20)    25773 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/src/pymssql/sqlfront.pxd
--rw-r--r--   0 teserak    (501) staff       (20)       37 2023-07-26 14:19:14.000000 pymssgl-2.2.8.dev28/src/pymssql/version.h
-drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:19:14.675678 pymssgl-2.2.8.dev28/tests/
--rw-r--r--   0 teserak    (501) staff       (20)       32 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/__init__.py
--rw-r--r--   0 teserak    (501) staff       (20)     3342 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/conftest.py
--rw-r--r--   0 teserak    (501) staff       (20)    16087 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/helpers.py
--rwxr-xr-x   0 teserak    (501) staff       (20)     1913 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/run_sqlalchemy_tests.py
--rw-r--r--   0 teserak    (501) staff       (20)     5367 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_bulk_copy.py
--rw-r--r--   0 teserak    (501) staff       (20)     3936 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_config.py
--rw-r--r--   0 teserak    (501) staff       (20)     1294 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_connection_as_dict.py
--rw-r--r--   0 teserak    (501) staff       (20)      631 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_connection_timeout.py
--rw-r--r--   0 teserak    (501) staff       (20)     5939 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_connections.py
--rw-r--r--   0 teserak    (501) staff       (20)     1340 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_context_managers.py
--rw-r--r--   0 teserak    (501) staff       (20)     8007 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_datetime.py
--rw-r--r--   0 teserak    (501) staff       (20)     1052 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_debug_queries.py
--rw-r--r--   0 teserak    (501) staff       (20)     2481 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_err_handle.py
--rw-r--r--   0 teserak    (501) staff       (20)     4469 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_green.py
--rw-r--r--   0 teserak    (501) staff       (20)     1059 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_memory.py
--rw-r--r--   0 teserak    (501) staff       (20)     7321 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_pymssql.py
--rw-r--r--   0 teserak    (501) staff       (20)     3772 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_queries.py
--rw-r--r--   0 teserak    (501) staff       (20)    23311 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_sprocs.py
--rw-r--r--   0 teserak    (501) staff       (20)     1879 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_sqlalchemy.py
--rw-r--r--   0 teserak    (501) staff       (20)     3260 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_threaded.py
--rw-r--r--   0 teserak    (501) staff       (20)     9101 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_types.py
--rw-r--r--   0 teserak    (501) staff       (20)      756 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_unicode.py
--rw-r--r--   0 teserak    (501) staff       (20)     5215 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_user_msghandler.py
--rw-r--r--   0 teserak    (501) staff       (20)     6119 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/test_utils.py
--rw-r--r--   0 teserak    (501) staff       (20)      679 2023-07-26 14:00:44.000000 pymssgl-2.2.8.dev28/tests/tests.cfg.tpl
+drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:36:56.166913 pymssgl-2.2.9.dev0/
+-rw-r--r--   0 teserak    (501) staff       (20)       40 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/.dockerignore
+drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:36:56.145812 pymssgl-2.2.9.dev0/.github/
+drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:36:56.151008 pymssgl-2.2.9.dev0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 teserak    (501) staff       (20)      724 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/.github/ISSUE_TEMPLATE/bug_report.md
+drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:36:56.151694 pymssgl-2.2.9.dev0/.github/workflows/
+-rw-r--r--   0 teserak    (501) staff       (20)     3120 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/.github/workflows/test_linux.yml
+-rw-r--r--   0 teserak    (501) staff       (20)     2491 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/.github/workflows/test_macos.yml
+-rw-r--r--   0 teserak    (501) staff       (20)     2301 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/.github/workflows/test_windows.yml
+-rw-r--r--   0 teserak    (501) staff       (20)      224 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/.gitignore
+-rw-r--r--   0 teserak    (501) staff       (20)      223 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/.pypirc
+-rw-r--r--   0 teserak    (501) staff       (20)      505 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/.readthedocs.yaml
+-rw-r--r--   0 teserak    (501) staff       (20)    38518 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/ChangeLog.old
+-rw-r--r--   0 teserak    (501) staff       (20)    16762 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/ChangeLog.rst
+-rw-r--r--   0 teserak    (501) staff       (20)      964 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/Dockerfile
+-rw-r--r--   0 teserak    (501) staff       (20)    26436 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/LICENSE
+-rw-r--r--   0 teserak    (501) staff       (20)       52 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/MANIFEST.in
+-rw-r--r--   0 teserak    (501) staff       (20)     4197 2023-07-26 14:36:56.167019 pymssgl-2.2.9.dev0/PKG-INFO
+-rw-r--r--   0 teserak    (501) staff       (20)     2448 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/README.rst
+-rw-r--r--   0 teserak    (501) staff       (20)     8473 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/appveyor.yml
+drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:36:56.153974 pymssgl-2.2.9.dev0/dev/
+-rw-r--r--   0 teserak    (501) staff       (20)       55 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/__init__.py
+drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:36:56.155083 pymssgl-2.2.9.dev0/dev/appveyor/
+-rw-r--r--   0 teserak    (501) staff       (20)     2270 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/appveyor/install-win-iconv.ps1
+-rw-r--r--   0 teserak    (501) staff       (20)     7195 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/appveyor/install.ps1
+-rw-r--r--   0 teserak    (501) staff       (20)      223 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/appveyor/pypirc
+-rw-r--r--   0 teserak    (501) staff       (20)     4130 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/appveyor/run_with_env.cmd
+-rw-r--r--   0 teserak    (501) staff       (20)     1362 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/appveyor/sql-server-activate-tcp-fixed-port.ps1
+-rw-r--r--   0 teserak    (501) staff       (20)      658 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/appveyor/tests.cfg
+-rw-r--r--   0 teserak    (501) staff       (20)     8222 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/build.py
+-rwxr-xr-x   0 teserak    (501) staff       (20)     1128 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/build_freetds.sh
+-rwxr-xr-x   0 teserak    (501) staff       (20)     3033 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/dev/build_manylinux_wheels.sh
+-rw-r--r--   0 teserak    (501) staff       (20)     2533 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/ccompiler.py
+-rw-r--r--   0 teserak    (501) staff       (20)       53 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/dev-requirements.pip
+-rwxr-xr-x   0 teserak    (501) staff       (20)     2033 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/hudson.sh
+-rwxr-xr-x   0 teserak    (501) staff       (20)      920 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/memmonitor.py
+-rwxr-xr-x   0 teserak    (501) staff       (20)      464 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/memtest.py
+-rwxr-xr-x   0 teserak    (501) staff       (20)       73 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/memtest.sh
+-rw-r--r--   0 teserak    (501) staff       (20)       95 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/dev/requirements-dev.txt
+-rwxr-xr-x   0 teserak    (501) staff       (20)     1305 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/dev/test_manylinux_wheels.sh
+-rw-r--r--   0 teserak    (501) staff       (20)      811 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docker-compose.yml
+drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:36:56.158821 pymssgl-2.2.9.dev0/docs/
+-rw-r--r--   0 teserak    (501) staff       (20)     6766 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/Makefile
+-rw-r--r--   0 teserak    (501) staff       (20)     4952 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/_mssql_examples.rst
+-rw-r--r--   0 teserak    (501) staff       (20)     1010 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/azure.rst
+-rw-r--r--   0 teserak    (501) staff       (20)     5831 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/docs/building_and_developing.rst
+-rw-r--r--   0 teserak    (501) staff       (20)      160 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/changelog.rst
+-rw-r--r--   0 teserak    (501) staff       (20)     9287 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/conf.py
+-rw-r--r--   0 teserak    (501) staff       (20)     1726 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/docs/docker.rst
+-rw-r--r--   0 teserak    (501) staff       (20)    10194 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/docs/faq.rst
+-rw-r--r--   0 teserak    (501) staff       (20)     6000 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/freetds.rst
+-rw-r--r--   0 teserak    (501) staff       (20)     2213 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/freetds_and_dates.rst
+-rw-r--r--   0 teserak    (501) staff       (20)     1738 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/history.rst
+drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:36:56.159264 pymssgl-2.2.9.dev0/docs/images/
+-rw-r--r--   0 teserak    (501) staff       (20)    15267 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/images/pymssql-stack.graphml
+-rw-r--r--   0 teserak    (501) staff       (20)    25535 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/images/pymssql-stack.png
+-rw-r--r--   0 teserak    (501) staff       (20)     2133 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/index.rst
+-rw-r--r--   0 teserak    (501) staff       (20)     4106 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/intro.rst
+-rw-r--r--   0 teserak    (501) staff       (20)     6703 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/make.bat
+-rw-r--r--   0 teserak    (501) staff       (20)     5513 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/migrate_1_x_to_2_x.rst
+-rw-r--r--   0 teserak    (501) staff       (20)     8452 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/docs/pymssql_examples.rst
+drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:36:56.160144 pymssgl-2.2.9.dev0/docs/ref/
+-rw-r--r--   0 teserak    (501) staff       (20)    17465 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/docs/ref/_mssql.rst
+-rw-r--r--   0 teserak    (501) staff       (20)    17748 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/docs/ref/pymssql.rst
+-rw-r--r--   0 teserak    (501) staff       (20)     3943 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/release_notes.rst
+-rw-r--r--   0 teserak    (501) staff       (20)       77 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/docs/requirements.txt
+-rw-r--r--   0 teserak    (501) staff       (20)       59 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/docs/todo.rst
+-rw-r--r--   0 teserak    (501) staff       (20)      139 2023-07-26 14:36:48.000000 pymssgl-2.2.9.dev0/pyproject.toml
+-rw-r--r--   0 teserak    (501) staff       (20)      447 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/pytest.ini
+-rw-r--r--   0 teserak    (501) staff       (20)       91 2023-07-26 14:36:56.167287 pymssgl-2.2.9.dev0/setup.cfg
+-rw-r--r--   0 teserak    (501) staff       (20)    11458 2023-07-26 14:35:19.000000 pymssgl-2.2.9.dev0/setup.py
+drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:36:56.146666 pymssgl-2.2.9.dev0/src/
+drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:36:56.161301 pymssgl-2.2.9.dev0/src/pymssgl.egg-info/
+-rw-r--r--   0 teserak    (501) staff       (20)     4197 2023-07-26 14:36:56.000000 pymssgl-2.2.9.dev0/src/pymssgl.egg-info/PKG-INFO
+-rw-r--r--   0 teserak    (501) staff       (20)     2123 2023-07-26 14:36:56.000000 pymssgl-2.2.9.dev0/src/pymssgl.egg-info/SOURCES.txt
+-rw-r--r--   0 teserak    (501) staff       (20)        1 2023-07-26 14:36:56.000000 pymssgl-2.2.9.dev0/src/pymssgl.egg-info/dependency_links.txt
+-rw-r--r--   0 teserak    (501) staff       (20)        1 2023-07-26 14:19:14.000000 pymssgl-2.2.9.dev0/src/pymssgl.egg-info/not-zip-safe
+-rw-r--r--   0 teserak    (501) staff       (20)        8 2023-07-26 14:36:56.000000 pymssgl-2.2.9.dev0/src/pymssgl.egg-info/top_level.txt
+drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:36:56.163450 pymssgl-2.2.9.dev0/src/pymssql/
+-rw-r--r--   0 teserak    (501) staff       (20)      101 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/src/pymssql/__init__.py
+-rw-r--r--   0 teserak    (501) staff       (20)     2082 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/src/pymssql/_mssql.pxd
+-rw-r--r--   0 teserak    (501) staff       (20)    74940 2023-07-26 14:33:05.000000 pymssgl-2.2.9.dev0/src/pymssql/_mssql.pyx
+-rw-r--r--   0 teserak    (501) staff       (20)    23171 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/src/pymssql/_pymssql.pyx
+-rw-r--r--   0 teserak    (501) staff       (20)    25047 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/src/pymssql/sqlfront.pxd
+-rw-r--r--   0 teserak    (501) staff       (20)       36 2023-07-26 14:36:53.000000 pymssgl-2.2.9.dev0/src/pymssql/version.h
+drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 14:36:56.166662 pymssgl-2.2.9.dev0/tests/
+-rw-r--r--   0 teserak    (501) staff       (20)       32 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/tests/__init__.py
+-rw-r--r--   0 teserak    (501) staff       (20)     2534 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/conftest.py
+-rw-r--r--   0 teserak    (501) staff       (20)    14782 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/helpers.py
+-rwxr-xr-x   0 teserak    (501) staff       (20)     1913 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/tests/run_sqlalchemy_tests.py
+-rw-r--r--   0 teserak    (501) staff       (20)     5363 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_bulk_copy.py
+-rw-r--r--   0 teserak    (501) staff       (20)     3799 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_config.py
+-rw-r--r--   0 teserak    (501) staff       (20)     1292 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_connection_as_dict.py
+-rw-r--r--   0 teserak    (501) staff       (20)      578 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_connection_timeout.py
+-rw-r--r--   0 teserak    (501) staff       (20)     5965 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_connections.py
+-rw-r--r--   0 teserak    (501) staff       (20)     1336 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_context_managers.py
+-rw-r--r--   0 teserak    (501) staff       (20)     1048 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_debug_queries.py
+-rw-r--r--   0 teserak    (501) staff       (20)     2497 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_err_handle.py
+-rw-r--r--   0 teserak    (501) staff       (20)     4372 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_green.py
+-rw-r--r--   0 teserak    (501) staff       (20)     1041 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_memory.py
+-rw-r--r--   0 teserak    (501) staff       (20)     7329 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_pymssql.py
+-rw-r--r--   0 teserak    (501) staff       (20)     3768 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_queries.py
+-rw-r--r--   0 teserak    (501) staff       (20)    20989 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_sprocs.py
+-rw-r--r--   0 teserak    (501) staff       (20)     1904 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_sqlalchemy.py
+-rw-r--r--   0 teserak    (501) staff       (20)     3222 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_threaded.py
+-rw-r--r--   0 teserak    (501) staff       (20)    12180 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_types.py
+-rw-r--r--   0 teserak    (501) staff       (20)      861 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_unicode.py
+-rw-r--r--   0 teserak    (501) staff       (20)     5211 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_user_msghandler.py
+-rw-r--r--   0 teserak    (501) staff       (20)     6133 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tests/test_utils.py
+-rw-r--r--   0 teserak    (501) staff       (20)      679 2023-07-26 14:00:44.000000 pymssgl-2.2.9.dev0/tests/tests.cfg.tpl
+-rw-r--r--   0 teserak    (501) staff       (20)      617 2023-07-26 14:32:58.000000 pymssgl-2.2.9.dev0/tox.ini
```

### Comparing `pymssgl-2.2.8.dev28/.github/ISSUE_TEMPLATE/bug_report.md` & `pymssgl-2.2.9.dev0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/.github/workflows/test_linux.yml` & `pymssgl-2.2.9.dev0/.github/workflows/test_linux.yml`

 * *Files 4% similar despite different names*

```diff
@@ -20,46 +20,45 @@
 jobs:
 
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ['3.6', '3.7', '3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.7', '3.8', '3.9', '3.10']
         os: [ubuntu-18.04]
 
     services:
       SQLServer:
         image: mcr.microsoft.com/mssql/server:2017-latest
         env:
           ACCEPT_EULA: Y
           SA_PASSWORD: sqlServerPassw0rd
         ports:
           - 1433:1433
 
     steps:
 
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v2
       with:
         fetch-depth: 0
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: build & install
       run: |
-        sudo apt-get update
-        sudo apt-get install libssl-dev libkrb5-dev
+        sudo apt-get install libssl-dev
         python -m pip install --upgrade pip
         pip install -r dev/requirements-dev.txt
         python dev/build.py \
             --ws-dir=./freetds \
             --dist-dir=./dist \
-            --freetds-version="1.3.13" \
+            --freetds-version="1.3.9" \
             --with-openssl=yes \
             --enable-krb5 \
             --sdist \
             --static-freetds
         pip install pymssql --no-index -f dist
         python -c "import pymssql; print(pymssql.version_info())"
 
@@ -82,31 +81,31 @@
     strategy:
       matrix:
         arch: [i686, x86_64]
         manylinux: [manylinux1, manylinux2010, manylinux2014, manylinux_2_24]
 
     steps:
 
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v2
       with:
         fetch-depth: 0
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v2
 
     - name: Build and test wheels
       env:
         DOCKER_IMAGE: quay.io/pypa/${{ matrix.manylinux }}_${{ matrix.arch }}
       run: |
         docker pull $DOCKER_IMAGE
-        docker run --rm --net="host" -w=/io -v `pwd`:/io -e MANYLINUX=${{ matrix.manylinux }} $DOCKER_IMAGE /io/dev/build_manylinux_wheels.sh
+        docker run --rm --net="host" -w=/io -v `pwd`:/io $DOCKER_IMAGE /io/dev/build_manylinux_wheels.sh
         ls -la dist
 
     - name: Archive wheels and sdist
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v2
       with:
         name: pymssql-${{ runner.os }}-${{ matrix.manylinux }}_${{ matrix.arch }}-${{ github.sha }}
         path: dist
 
     - name: Publish wheels and sdist
       if: github.repository_owner == 'pymssql' && startsWith(github.ref, 'refs/tags/v')
       run: |
```

### Comparing `pymssgl-2.2.8.dev28/.github/workflows/test_macos.yml` & `pymssgl-2.2.9.dev0/.github/workflows/test_macos.yml`

 * *Files 2% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-            python-version: ['3.6', '3.7', '3.8', '3.9', '3.10', '3.11']
+            python-version: ['3.7', '3.8', '3.9', '3.10']
             os: [macos-latest]
 
     steps:
 
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v2
       with:
         fetch-depth: 0
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v2
       with:
             python-version: ${{ matrix.python-version }}
 
     - name: build wheel and sdist
       env:
             LDFLAGS: -L/usr/local/opt/openssl@1.1/lib
             CPPFLAGS: -I/usr/local/opt/openssl@1.1/include
@@ -48,30 +48,30 @@
             pip install delocate
             python setup.py sdist
             brew install openssl@1.1
             brew install libiconv
             python dev/build.py \
                 --ws-dir=./freetds \
                 --dist-dir=./dist \
-                --freetds-version="1.3.13" \
+                --freetds-version="1.3.9" \
                 --with-openssl=yes \
                 --sdist \
                 --static-freetds
             delocate-listdeps --all dist/*.whl
             delocate-wheel -v dist/*.whl
             delocate-listdeps --all dist/*.whl
             pip install pymssql --no-index -f dist
             python -c "import pymssql; print(pymssql.version_info())"
 
     - name: Test with pytest
       run: |
         pytest -sv
 
     - name: Archive wheels and sdist
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v2
       with:
         name: pymssql-${{ runner.os }}-${{ github.sha }}
         path: dist
 
     - name: Publish wheels
       if: github.repository_owner == 'pymssql' && startsWith(github.ref, 'refs/tags/v')
       run: |
```

### Comparing `pymssgl-2.2.8.dev28/.github/workflows/test_windows.yml` & `pymssgl-2.2.9.dev0/.github/workflows/test_windows.yml`

 * *Files 6% similar despite different names*

```diff
@@ -21,26 +21,26 @@
   build:
 
     runs-on: ${{ matrix.os }}
 
     strategy:
       fail-fast: false
       matrix:
-            python-version: ['3.6', '3.7', '3.8', '3.9', '3.10', '3.11']
+            python-version: ['3.7', '3.8', '3.9', '3.10']
             os: [windows-latest]
             python-architecture: [x86, x64]
 
     steps:
 
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v2
       with:
         fetch-depth: 0
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v2
       with:
             python-version: ${{ matrix.python-version }}
             architecture: ${{ matrix.python-architecture}}
 
     - name: Install OpenSSL x86
       if: matrix.python-architecture == 'x86'
       run: choco install openssl --forcex86
@@ -50,24 +50,24 @@
       run: choco install openssl
 
     - name: Install & build dependencies
       run: |
         choco install gperf
         python -m pip install --upgrade pip
         pip install -r dev/requirements-dev.txt
-        python dev/build.py --ws-dir=freetds --dist-dir=dist --sdist --freetds-version="1.3.13"
+        python dev/build.py --ws-dir=freetds --dist-dir=dist --sdist --freetds-version="1.3.9"
         pip install pymssql --no-index -f dist
         python -c "import pymssql; print(pymssql.version_info())"
 
     - name: Test with pytest
       run: |
         pytest -sv
 
     - name: Archive wheels and sdist
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v2
       with:
         name: pymssql-${{ runner.os }}-${{ matrix.python-architecture }}-${{ github.sha }}
         path: dist
 
     - name: Publish wheels
       if: github.repository_owner == 'pymssql' && startsWith(github.ref, 'refs/tags/v')
       run: |
```

### Comparing `pymssgl-2.2.8.dev28/ChangeLog.old` & `pymssgl-2.2.9.dev0/ChangeLog.old`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/ChangeLog.rst` & `pymssgl-2.2.9.dev0/ChangeLog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,11 @@
 Recent Changes
 ==============
 
-Version 2.2.7 - 2022-11-15  - Mikhail Terekhov
-==============================================
-
-General
--------
-
-- Build wheels for Python-3.6 (fix 787).
-
-Version 2.2.6 - 2022-11-12  - Mikhail Terekhov
-==============================================
-
-General
--------
-
-- Build wheels for Python-3.11.
-- Use FreeTDS-1.3.13 for official wheels on PyPi.
-- Fix build on Alpine Linux (fix #762).
-- Fill in result description in cursor.callproc (fix #772).
-- Add explicit link to krb5 (fix #776), thanks to James Coder.
-- Some small doc fixes, thanks to guillaumep and Logan Elandt.
-
-Version 2.2.5 - 2022-04-12  - Mikhail Terekhov
+Version 2.2.4 - 2022-04-12  - Mikhail Terekhov
 ==============================================
 
 General
 -------
 
 - Added bytes and bytearray to support bulk_copy types, thanks to steve-strickland (#756).
 - Use FreeTDS-1.3.9 for official wheels on PyPi.
```

### Comparing `pymssgl-2.2.8.dev28/Dockerfile` & `pymssgl-2.2.9.dev0/Dockerfile`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/LICENSE` & `pymssgl-2.2.9.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/PKG-INFO` & `pymssgl-2.2.9.dev0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: pymssgl
-Version: 2.2.8.dev28
+Version: 2.2.9.dev0
 Summary: DB-API interface to Microsoft SQL Server for Python. (new Cython-based version)
 Author: Damien Churchill
 Author-email: damoxc@gmail.com
-Maintainer: Mikhail Terekhov
-Maintainer-email: termim@gmail.com
+Maintainer: pymssql development team
+Maintainer-email: pymssql@googlegroups.com
 License: LGPL
 Project-URL: Documentation, http://pymssql.readthedocs.io
 Project-URL: Source, https://github.com/pymssql/pymssql
 Project-URL: Changelog, https://github.com/pymssql/pymssql/blob/master/ChangeLog.rst
 Keywords: mssql,SQL Server,database,DB-API
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
@@ -107,27 +105,16 @@
 
     conn.close()
 
 
 Recent Changes
 ==============
 
-Version 2.2.7 - 2022-11-15  - Mikhail Terekhov
+Version 2.2.4 - 2022-04-12  - Mikhail Terekhov
 ==============================================
 
 General
 -------
 
-- Build wheels for Python-3.6 (fix 787).
-
-Version 2.2.6 - 2022-11-12  - Mikhail Terekhov
-==============================================
-
-General
--------
-
-- Build wheels for Python-3.11.
-- Use FreeTDS-1.3.13 for official wheels on PyPi.
-- Fix build on Alpine Linux (fix #762).
-- Fill in result description in cursor.callproc (fix #772).
-- Add explicit link to krb5 (fix #776), thanks to James Coder.
-- Some small doc fixes, thanks to guillaumep and Logan Elandt.
+- Added bytes and bytearray to support bulk_copy types, thanks to steve-strickland (#756).
+- Use FreeTDS-1.3.9 for official wheels on PyPi.
+- Enable krb5 in Linux wheels, this time for real (#754).
```

### Comparing `pymssgl-2.2.8.dev28/README.rst` & `pymssgl-2.2.9.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/appveyor.yml` & `pymssgl-2.2.9.dev0/appveyor.yml`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/dev/appveyor/install-win-iconv.ps1` & `pymssgl-2.2.9.dev0/dev/appveyor/install-win-iconv.ps1`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/dev/appveyor/install.ps1` & `pymssgl-2.2.9.dev0/dev/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/dev/appveyor/run_with_env.cmd` & `pymssgl-2.2.9.dev0/dev/appveyor/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/dev/appveyor/sql-server-activate-tcp-fixed-port.ps1` & `pymssgl-2.2.9.dev0/dev/appveyor/sql-server-activate-tcp-fixed-port.ps1`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/dev/appveyor/tests.cfg` & `pymssgl-2.2.9.dev0/dev/appveyor/tests.cfg`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/dev/build.py` & `pymssgl-2.2.9.dev0/dev/build.py`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/dev/build_freetds.sh` & `pymssgl-2.2.9.dev0/dev/build_freetds.sh`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/dev/build_manylinux_wheels.sh` & `pymssgl-2.2.9.dev0/dev/build_manylinux_wheels.sh`

 * *Files 16% similar despite different names*

```diff
@@ -27,38 +27,33 @@
 # These docker commands will run, build the wheel, attempt to install and then finally upload
 # docker run --name manylinux_x86_x64 --rm -w=/io -v `pwd`:/io quay.io/pypa/manylinux1_x86_64 /io/dev/build_wheels.sh
 # docker run --name manylinux_i686 --rm -w=/io -v `pwd`:/io quay.io/pypa/manylinux1_i686 /io/dev/build_wheels.sh
 #
 # https://www.gnu.org/software/bash/manual/html_node/The-Set-Builtin.html
 set -e -x
 
-if ! git status ; then
-  git config --global --add safe.directory "$(pwd)"
-fi
-git status
-
 if which yum; then
-    yum install -y openssl-devel krb5-devel
+    yum install -y openssl-devel
 else
     apt-get update
     apt-get install -y libssl1.1
-    apt-get install -y libssl-dev libkrb5-dev
+    apt-get install -y libssl-dev
 fi
 
 /opt/python/cp38-cp38/bin/python dev/build.py \
     --ws-dir=./freetds \
     --dist-dir=. \
     --prefix=/usr/local \
-    --freetds-version="1.3.13" \
+    --freetds-version="1.3.9" \
     --with-openssl=yes \
     --enable-krb5 \
     --static-freetds
 
 # Install Python dependencies and compile wheels
-PYTHONS="cp36-cp36m cp37-cp37m cp38-cp38 cp39-cp39 cp310-cp310 cp311-cp311"
+PYTHONS="cp36-cp36m cp37-cp37m cp38-cp38 cp39-cp39 cp310-cp310"
 for i in $PYTHONS; do
     PYBIN="/opt/python/$i/bin"
     if  [ -d ${PYBIN} ] ; then
         "${PYBIN}/pip" install --upgrade pip setuptools Cython wheel
         "${PYBIN}/pip" wheel . -w .
     fi
 done
@@ -72,24 +67,19 @@
     fi
 done
 
 # Create .tar.gz dist.
 /opt/python/cp38-cp38/bin/python setup.py sdist
 
 # Install the wheels that were built. Need to be able to connect to mssql and to run the pytest suite after install
-# psutil 5.9.2 had a bug preventing it from being imported on some platforms.
-# https://github.com/giampaolo/psutil/issues/2138
 for i in $PYTHONS; do
     PYBIN="/opt/python/$i/bin"
     if  [ -d ${PYBIN} ] ; then
         "${PYBIN}/pip" install pymssql --no-index -f dist
-        "${PYBIN}/pip" install 'psutil<5.9.2' pytest pytest-timeout pytest-subtests
-        if [ "$MANYLINUX" != "manylinux1" ] ;  then
-            "${PYBIN}/pip" install SQLAlchemy
-        fi
+        "${PYBIN}/pip" install psutil pytest pytest-timeout SQLAlchemy
         "${PYBIN}/pytest" -s .
         "${PYBIN}/python" -c "import pymssql; print(pymssql.version_info());"
     fi
 done
 
 # Remove wheel and egg directory for next container build (i686 vs x86_x64)
 rm -rf .eggs/ pymssql.egg-info/
```

### Comparing `pymssgl-2.2.8.dev28/dev/ccompiler.py` & `pymssgl-2.2.9.dev0/dev/ccompiler.py`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/dev/hudson.sh` & `pymssgl-2.2.9.dev0/dev/hudson.sh`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/dev/memmonitor.py` & `pymssgl-2.2.9.dev0/dev/memmonitor.py`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/dev/test_manylinux_wheels.sh` & `pymssgl-2.2.9.dev0/dev/test_manylinux_wheels.sh`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/docker-compose.yml` & `pymssgl-2.2.9.dev0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/docs/Makefile` & `pymssgl-2.2.9.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/docs/_mssql_examples.rst` & `pymssgl-2.2.9.dev0/docs/_mssql_examples.rst`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/docs/azure.rst` & `pymssgl-2.2.9.dev0/docs/azure.rst`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/docs/building_and_developing.rst` & `pymssgl-2.2.9.dev0/docs/building_and_developing.rst`

 * *Files 4% similar despite different names*

```diff
@@ -70,23 +70,14 @@
 
 .. note::
     If Windows computer is not readily available then
     `virtual machine <https://developer.microsoft.com/en-us/windows/downloads/virtual-machines/>`_
     from Microsoft could be used.
 
 
-Linux
-_____
-
-For example on Alpine Linux the following command will install all necessary
-packages for building pymssql::
-
-    apk add git gcc musl-dev krb5-dev openssl-dev freetds-dev
-
-
 Building ``pymssql`` wheel
 __________________________
 
 It is recommended to use python virtual environment for building ``pymssql``::
 
     python3 -m venv <path_to_pve>
 
@@ -195,21 +186,13 @@
 
   py.test --pymssql-section=AllTestsWillRun
 
 to avoid slow tests::
 
   py.test -m "not slow"
 
-or::
-
-  py.test --skip-slow
-
-to skip tests that require MSSQL server::
-
-  py.test --skip-mssql-server-required
-
 to select specific tests to run::
 
   py.test tests/test_types.py
   py.test tests/test_types.py tests/test_sprocs.py
   py.test tests/test_types.py::TestTypes
   py.test tests/test_types.py::TestTypes::test_image
```

### Comparing `pymssgl-2.2.8.dev28/docs/conf.py` & `pymssgl-2.2.9.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/docs/docker.rst` & `pymssgl-2.2.9.dev0/docs/docker.rst`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Docker
 ======
 
 (Experimental)
 
 There is a pymssql Docker image on the Docker Registry at:
 
-https://registry.hub.docker.com/r/pymssql/pymssql/
+https://registry.hub.docker.com/u/pymssql/pymssql/
 
 The image bundles:
 
 * Ubuntu 14.04 LTS (trusty)
 * Python 2.7.6
 * pymssql 2.1.2.dev
 * FreeTDS 0.91
```

### Comparing `pymssgl-2.2.8.dev28/docs/faq.rst` & `pymssgl-2.2.9.dev0/docs/faq.rst`

 * *Files 0% similar despite different names*

```diff
@@ -227,8 +227,8 @@
 More troubleshooting
 ====================
 
 If the above hasn't covered the problem you can send a message describing it to
 the pymssql mailing list. You can also consult FreeTDS troubleshooting `page for
 issues related to the TDS protocol`_.
 
-.. _page for issues related to the TDS protocol: https://www.freetds.org/userguide/troubleshooting.html
+.. _page for issues related to the TDS protocol: http://www.freetds.org/userguide/troubleshooting.htm
```

### Comparing `pymssgl-2.2.8.dev28/docs/freetds.rst` & `pymssgl-2.2.9.dev0/docs/freetds.rst`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/docs/freetds_and_dates.rst` & `pymssgl-2.2.9.dev0/docs/freetds_and_dates.rst`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/docs/history.rst` & `pymssgl-2.2.9.dev0/docs/history.rst`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/docs/images/pymssql-stack.graphml` & `pymssgl-2.2.9.dev0/docs/images/pymssql-stack.graphml`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/docs/images/pymssql-stack.png` & `pymssgl-2.2.9.dev0/docs/images/pymssql-stack.png`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/docs/index.rst` & `pymssgl-2.2.9.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/docs/intro.rst` & `pymssgl-2.2.9.dev0/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/docs/make.bat` & `pymssgl-2.2.9.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/docs/migrate_1_x_to_2_x.rst` & `pymssgl-2.2.9.dev0/docs/migrate_1_x_to_2_x.rst`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/docs/pymssql_examples.rst` & `pymssgl-2.2.9.dev0/docs/pymssql_examples.rst`

 * *Files 1% similar despite different names*

```diff
@@ -197,16 +197,14 @@
             CREATE PROCEDURE FindPerson
                 @name VARCHAR(100)
             AS BEGIN
                 SELECT * FROM persons WHERE name = @name
             END
             """)
             cursor.callproc('FindPerson', ('Jane Doe',))
-            # you must call commit() to persist your data if you don't set autocommit to True
-            conn.commit()
             for row in cursor:
                 print("ID=%d, Name=%s" % (row['id'], row['name']))
 
 Using pymssql with cooperative multi-tasking systems
 ====================================================
 
 .. versionadded:: 2.1.0
```

### Comparing `pymssgl-2.2.8.dev28/docs/ref/_mssql.rst` & `pymssgl-2.2.9.dev0/docs/ref/_mssql.rst`

 * *Files 4% similar despite different names*

```diff
@@ -75,39 +75,24 @@
                        * ``'SQLHOST'`` -- Default instance at default port (Windows only)
                        * ``'SQLHOST'`` -- Specific instance at specific port set up in freetds.conf (Linux/\*nix only)
                        * ``'SQLHOST,1433'`` -- Specified TCP port at specified host
                        * ``'SQLHOST:1433'`` -- The same as above
                        * ``'SQLHOST,5000'`` -- If you have set up an instance to listen on port 5000
                        * ``'SQLHOST:5000'`` -- The same as above
 
-    :param str encryption: Specify if encryption is desired. Supported for
-                        Microsoft servers. Possible values are:
-
-                           * ``'off'`` -- disables encryption
-                           * ``'request'`` -- means use if available
-                           * ``'require'`` -- means create and allow encrypted connections only
-                        Default: ``'request'`` for tds version > 7.1, otherwise ``'off'``
-
-                        .. versionadded:: 2.2.8
-
     :param str user: Database user to connect as
 
     :param str password: User's password
 
     :param str charset: Character set name to set for the connection.
 
     :param str database: The database you want to initially to connect to; by
                          default, *SQL Server* selects the database which is set as
                          the default for the specific user
 
-    :param bool read_only: Tell server we only intent to do read-only queries.
-                        This is supported from MSSQL 2012.
-
-                        .. versionadded:: 2.2.8
-
     :param str appname: Set the application name to use for the connection
 
     :param str port: the TCP port to use to connect to the server
 
     :param str tds_version: TDS protocol version to ask for. Default value: ``None``
 
     :param conn_properties: SQL queries to send to the server upon connection
@@ -235,14 +220,17 @@
    .. versionadded:: 2.2.0
 
    The TDS version used by this connection in tuple form which is more easily
    handled (parse, compare) programmatically. Can be one of ``(4, 2)``,
    ``(5, 0)``, ``(7, 0)``, ``(7, 1)``, ``(7, 2)``, ``(7, 3)`` or ``None`` if no
    TDS version could be detected.
 
+   .. versionchanged:: 2.1.3
+      ``7.3`` was added as a possible value.
+
 ``MSSQLConnection`` object methods
 ----------------------------------
 
 .. method:: MSSQLConnection.cancel()
 
    Cancel all pending results from the last SQL operation. It can be called more
    than one time in a row. No exception is raised in this case.
```

### Comparing `pymssgl-2.2.8.dev28/docs/ref/pymssql.rst` & `pymssgl-2.2.9.dev0/docs/ref/pymssql.rst`

 * *Files 1% similar despite different names*

```diff
@@ -72,29 +72,14 @@
                      * ``'SQLHOST'`` -- specific instance at specific port set up in freetds.conf (Linux/\*nix only)
                      * ``'SQLHOST,1433'`` -- specified TCP port at specified host
                      * ``'SQLHOST:1433'`` -- the same as above
                      * ``'SQLHOST,5000'`` -- if you have set up an instance to listen on port 5000
                      * ``'SQLHOST:5000'`` -- the same as above
 
                      ``'.'`` (the local host) is assumed if host is not provided.
-
-   :param str encryption: Specify if encryption is desired. Supported for
-                        Microsoft servers. Possible values are:
-
-                           * ``'off'`` -- disables encryption
-                           * ``'request'`` -- means use if available
-                           * ``'require'`` -- means create and allow encrypted connections only
-                        Default: ``'request'`` for tds version > 7.1, otherwise ``'off'``
-
-                        .. versionadded:: 2.2.8
-
-   :param bool read_only: Tell server we only intent to do read-only queries.
-                        This is supported from MSSQL 2012.
-
-                        .. versionadded:: 2.2.8
    :keyword str appname: Set the application name to use for the connection
    :keyword str port: the TCP port to use to connect to the server
    :keyword conn_properties: SQL queries to send to the server upon connection
                              establishment. Can be a string or another kind of
                              iterable of strings.  Default value: See
                              :class:`_mssql.connect() <_mssql.MSSQLConnection>`
    :keyword bool autocommit: Whether to use default autocommiting mode or not
```

### Comparing `pymssgl-2.2.8.dev28/docs/release_notes.rst` & `pymssgl-2.2.9.dev0/docs/release_notes.rst`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/setup.py` & `pymssgl-2.2.9.dev0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     elif val.upper() in ('0', 'NO', 'FALSE'):
        return False
     else:
        raise Exception(f"Unsupported environment value {env_name}={val}")
 
 LINK_FREETDS_STATICALLY = check_env('LINK_FREETDS_STATICALLY', 'YES')
 LINK_OPENSSL = check_env('LINK_OPENSSL', 'YES')
-LINK_KRB5 = check_env('LINK_KRB5', 'YES')
 
 # 32 bit or 64 bit system?
 BITNESS = struct.calcsize("P") * 8
 WINDOWS = platform.system() == 'Windows'
 
 include_dirs = []
 library_dirs = []
@@ -96,25 +95,26 @@
 print("setup.py: platform.system() =>", platform.system())
 print("setup.py: platform.architecture() =>", platform.architecture())
 if not WINDOWS:
     print("setup.py: platform.libc_ver() =>", platform.libc_ver())
 print("setup.py: include_dirs =>", include_dirs)
 print("setup.py: library_dirs =>", library_dirs)
 
-if not WINDOWS and platform.libc_ver()[0] == 'glibc':
+if not WINDOWS:
     # check for clock_gettime, link with librt for glibc<2.17
     from dev import ccompiler
     compiler = ccompiler.new_compiler()
     if not compiler.has_function('clock_gettime(0,NULL)', includes=['time.h']):
         if compiler.has_function('clock_gettime(0,NULL)', includes=['time.h'], libraries=['rt']):
             libraries.append('rt')
         else:
             print("setup.py: could not locate 'clock_gettime' function required by FreeTDS.")
             sys.exit(1)
 
+
 class build_ext(_build_ext):
     """
     Subclass the Cython build_ext command so it:
     * Can handle different C compilers on Windows
     * Links in the libraries we collected
     """
 
@@ -166,16 +166,14 @@
                 if LINK_OPENSSL:
                     if BITNESS == 32:
                         e.library_dirs.append("c:/Program Files (x86)/OpenSSL-Win32/lib")
                     else:
                         e.library_dirs.append("c:/Program Files/OpenSSL-Win64/lib")
 
         else:
-            if LINK_KRB5:
-                libraries.extend([ 'gssapi_krb5', 'krb5'] )
             if LINK_OPENSSL and LINK_FREETDS_STATICALLY:
                 libraries.extend([ 'ssl', 'crypto' ])
 
             for e in self.extensions:
                 e.libraries.extend(libraries)
 
         _build_ext.build_extensions(self)
@@ -264,46 +262,42 @@
         ),
     ]
     for e in ext_modules:
         e.cython_directives = {'language_level': sys.version_info[0]}
     return ext_modules
 
 
-def mk_long_description(numrev=1):
+def mk_long_description():
 
     readme = (Path('__file__').parent / 'README.rst').read_text()
     chlog = Path('__file__').parent / 'ChangeLog.rst'
     lines = []
     with chlog.open('r') as f:
         count = 0
         l = f.readline()
         while l:
             if l.startswith('Version 2'):
                 count += 1
-            if count > numrev:
+            if count > 1:
                 break
             lines.append(l)
             l = f.readline()
     return readme + "\n\n" + ''.join(lines).strip()
 
 
 setup(
     name  = 'pymssgl',
-    use_scm_version = {
-        "write_to": "src/pymssql/version.h",
-        "write_to_template": '#define PYMSSQL_VERSION "{version}"',
-        "local_scheme": "no-local-version",
-    },
+    version = "2.2.9.dev0",
     description = 'DB-API interface to Microsoft SQL Server for Python. (new Cython-based version)',
-    long_description = mk_long_description(2),
+    long_description = mk_long_description(),
     long_description_content_type = 'text/x-rst',
     author = 'Damien Churchill',
     author_email = 'damoxc@gmail.com',
-    maintainer = 'Mikhail Terekhov',
-    maintainer_email = 'termim@gmail.com',
+    maintainer = 'pymssql development team',
+    maintainer_email = 'pymssql@googlegroups.com',
     license = 'LGPL',
     platforms = 'any',
     keywords = ['mssql', 'SQL Server', 'database', 'DB-API'],
     project_urls={
         "Documentation": "http://pymssql.readthedocs.io",
         "Source": "https://github.com/pymssql/pymssql",
         "Changelog": "https://github.com/pymssql/pymssql/blob/master/ChangeLog.rst",
@@ -318,24 +312,22 @@
       "Intended Audience :: Developers",
       "License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)",
       "Programming Language :: Python",
       "Programming Language :: Python :: 3.6",
       "Programming Language :: Python :: 3.7",
       "Programming Language :: Python :: 3.8",
       "Programming Language :: Python :: 3.9",
-      "Programming Language :: Python :: 3.10",
-      "Programming Language :: Python :: 3.11",
       "Programming Language :: Python :: Implementation :: CPython",
       "Topic :: Database",
       "Topic :: Database :: Database Engines/Servers",
       "Topic :: Software Development :: Libraries :: Python Modules",
       "Operating System :: Microsoft :: Windows",
       "Operating System :: POSIX",
       "Operating System :: Unix",
     ],
     zip_safe = False,
-    setup_requires=['setuptools_scm[toml]>=5.0,<8.0', 'Cython>=0.29.22'],
-    tests_require=['psutil<5.9.5', 'pytest', 'pytest-timeout'],
+    setup_requires=['setuptools_scm', 'Cython'],
+    tests_require=['psutil', 'pytest', 'pytest-timeout'],
     ext_modules = ext_modules(),
     packages = [ 'pymssql'],
     package_dir = {'': 'src'},
 )
```

### Comparing `pymssgl-2.2.8.dev28/src/pymssgl.egg-info/PKG-INFO` & `pymssgl-2.2.9.dev0/src/pymssgl.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: pymssgl
-Version: 2.2.8.dev28
+Version: 2.2.9.dev0
 Summary: DB-API interface to Microsoft SQL Server for Python. (new Cython-based version)
 Author: Damien Churchill
 Author-email: damoxc@gmail.com
-Maintainer: Mikhail Terekhov
-Maintainer-email: termim@gmail.com
+Maintainer: pymssql development team
+Maintainer-email: pymssql@googlegroups.com
 License: LGPL
 Project-URL: Documentation, http://pymssql.readthedocs.io
 Project-URL: Source, https://github.com/pymssql/pymssql
 Project-URL: Changelog, https://github.com/pymssql/pymssql/blob/master/ChangeLog.rst
 Keywords: mssql,SQL Server,database,DB-API
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
@@ -107,27 +105,16 @@
 
     conn.close()
 
 
 Recent Changes
 ==============
 
-Version 2.2.7 - 2022-11-15  - Mikhail Terekhov
+Version 2.2.4 - 2022-04-12  - Mikhail Terekhov
 ==============================================
 
 General
 -------
 
-- Build wheels for Python-3.6 (fix 787).
-
-Version 2.2.6 - 2022-11-12  - Mikhail Terekhov
-==============================================
-
-General
--------
-
-- Build wheels for Python-3.11.
-- Use FreeTDS-1.3.13 for official wheels on PyPi.
-- Fix build on Alpine Linux (fix #762).
-- Fill in result description in cursor.callproc (fix #772).
-- Add explicit link to krb5 (fix #776), thanks to James Coder.
-- Some small doc fixes, thanks to guillaumep and Logan Elandt.
+- Added bytes and bytearray to support bulk_copy types, thanks to steve-strickland (#756).
+- Use FreeTDS-1.3.9 for official wheels on PyPi.
+- Enable krb5 in Linux wheels, this time for real (#754).
```

### Comparing `pymssgl-2.2.8.dev28/src/pymssgl.egg-info/SOURCES.txt` & `pymssgl-2.2.9.dev0/src/pymssgl.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 README.rst
 appveyor.yml
 docker-compose.yml
 pyproject.toml
 pytest.ini
 setup.cfg
 setup.py
-.github/dependabot.yml
+tox.ini
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/workflows/test_linux.yml
 .github/workflows/test_macos.yml
 .github/workflows/test_windows.yml
 dev/__init__.py
 dev/build.py
 dev/build_freetds.sh
@@ -77,15 +77,14 @@
 tests/run_sqlalchemy_tests.py
 tests/test_bulk_copy.py
 tests/test_config.py
 tests/test_connection_as_dict.py
 tests/test_connection_timeout.py
 tests/test_connections.py
 tests/test_context_managers.py
-tests/test_datetime.py
 tests/test_debug_queries.py
 tests/test_err_handle.py
 tests/test_green.py
 tests/test_memory.py
 tests/test_pymssql.py
 tests/test_queries.py
 tests/test_sprocs.py
```

### Comparing `pymssgl-2.2.8.dev28/src/pymssql/_mssql.pxd` & `pymssgl-2.2.9.dev0/src/pymssql/_mssql.pxd`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/src/pymssql/_mssql.pyx` & `pymssgl-2.2.9.dev0/src/pymssql/_mssql.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,14 @@
 import socket
 import decimal
 import binascii
 import datetime
 import re
 import uuid
 
-class datetime2(datetime.datetime): pass
-
 from .sqlfront cimport *
 
 from libc.stdio cimport fprintf, snprintf, stderr, FILE
 from libc.string cimport strlen, strncpy, memcpy, memset
 
 from cpython cimport bool
 from cpython.mem cimport PyMem_Malloc, PyMem_Free
@@ -137,25 +135,14 @@
 SQLVARCHAR = SYBVARCHAR
 SQLUUID = 36
 
 SQLDATE = 40
 SQLTIME = 41
 SQLDATETIME2 = 42
 
-####################
-## TDS_ENCRYPTION_LEVEL ##
-####################
-
-cdef dict TDS_ENCRYPTION_LEVEL = {
-    'default': 0,  # TDS_ENCRYPTION_DEFAULT,
-    'off':     1,  # TDS_ENCRYPTION_OFF,
-    'request': 2,  # TDS_ENCRYPTION_REQUEST,
-    'require': 3   # TDS_ENCRYPTION_REQUIRE
-}
-
 ###################
 ## Type mappings ##
 ###################
 
 cdef dict DBTYPES = {
     'bool': SQLBITN,
     'str': SQLVARCHAR,
@@ -606,74 +593,81 @@
         self.last_msg_srv[0] = <char>0
         self.last_msg_proc = <char *>PyMem_Malloc(PYMSSQL_MSGSIZE)
         self.last_msg_proc[0] = <char>0
         self.column_names = None
         self.column_types = None
 
     def __init__(self, server="localhost", user=None, password=None,
-                        charset='UTF-8', database='', appname=None, port='1433',
-                        tds_version=None, encryption=None, read_only=False,
-                        conn_properties=None):
+            charset='UTF-8', database='', appname=None, port='1433', tds_version=None, conn_properties=None):
         log("_mssql.MSSQLConnection.__init__()")
 
         cdef LOGINREC *login
         cdef RETCODE rtc
+        cdef char *_charset
 
         # support MS methods of connecting locally
         instance = ""
         if "\\" in server:
             server, instance = server.split("\\")
 
         if server in (".", "(local)"):
             server = "localhost"
 
         server = server + "\\" + instance if instance else server
 
-        # add the port to the server string if it doesn't have one already and
-        # if we are not using an instance
-        if ':' not in server and not instance:
-            server = '%s:%s' % (server, port)
-
-        cdef bytes server_bytes = server.encode('utf-8')
-        cdef char *server_cstr = server_bytes
-
         login = dblogin()
         if login == NULL:
             raise MSSQLDriverException("dblogin() failed")
 
         appname = appname or "pymssql=%s" % __full_version__
-        cdef bytes appname_bytes = appname.encode('utf-8')
-        cdef char *appname_cstr = appname_bytes
-        DBSETLAPP(login, appname_cstr)
 
+        # For Python 3, we need to convert unicode to byte strings
         cdef bytes user_bytes
         cdef char *user_cstr = NULL
         if user is not None:
             user_bytes = user.encode('utf-8')
             user_cstr = user_bytes
-            DBSETLUSER(login, user_cstr)
-
         cdef bytes password_bytes
         cdef char *password_cstr = NULL
         if password is not None:
             password_bytes = password.encode('utf-8')
             password_cstr = password_bytes
-            DBSETLPWD(login, password_cstr)
+        cdef bytes appname_bytes = appname.encode('utf-8')
+        cdef char *appname_cstr = appname_bytes
 
+        if user is not None:
+            DBSETLUSER(login, user_cstr)
+        if password is not None:
+            DBSETLPWD(login, password_cstr)
+        DBSETLAPP(login, appname_cstr)
         if tds_version is not None:
             DBSETLVERSION(login, _tds_ver_str_to_constant(tds_version))
 
-        if encryption is not None:
-            if encryption in TDS_ENCRYPTION_LEVEL:
-                DBSETLENCRYPT(login, TDS_ENCRYPTION_LEVEL[encryption])
-            else:
-                raise ValueError(f"'encryption' option should be {TDS_ENCRYPTION_LEVEL.keys())} or None.")
+        # add the port to the server string if it doesn't have one already and
+        # if we are not using an instance
+        if ':' not in server and not instance:
+            server = '%s:%s' % (server, port)
+
+        # override the HOST to be the portion without the server, otherwise
+        # FreeTDS chokes when server still has the port definition.
+        # BUT, a patch on the mailing list fixes the need for this.  I am
+        # leaving it here just to remind us how to fix the problem if the bug
+        # doesn't get fixed for a while.  But if it does get fixed, this code
+        # can be deleted.
+        # patch: http://lists.ibiblio.org/pipermail/freetds/2011q2/026997.html
+        #if ':' in server:
+        #    os.environ['TDSHOST'] = server.split(':', 1)[0]
+        #else:
+        #    os.environ['TDSHOST'] = server
+
+        # Add ourselves to the global connection list
+        connection_object_list.append(self)
 
         cdef bytes charset_bytes
-        cdef char *_charset
+
         # Set the character set name
         if charset:
             charset_bytes = charset.encode('utf-8')
             _charset = charset_bytes
             strncpy(self._charset, _charset, PYMSSQL_CHARSETBUFSIZE)
             DBSETLCHARSET(login, self._charset)
 
@@ -682,35 +676,31 @@
         cdef char *dbname_cstr
         # Put the DB name in the login LOGINREC because it helps with connections to Azure
         if database:
             dbname_bytes = database.encode('utf-8')
             dbname_cstr = dbname_bytes
             DBSETLDBNAME(login, dbname_cstr)
 
-        if read_only:
-            DBSETLREADONLY(login, 1)
-
-        # Add ourselves to the global connection list
-        connection_object_list.append(self)
-
         # Set the login timeout
         # XXX: Currently this will set it application wide :-(
         dbsetlogintime(login_timeout)
 
+        cdef bytes server_bytes = server.encode('utf-8')
+        cdef char *server_cstr = server_bytes
+
         # Connect to the server
         with nogil:
             self.dbproc = dbopen(login, server_cstr)
 
         # Frees the login record, can be called immediately after dbopen.
         dbloginfree(login)
 
         if self.dbproc == NULL:
             log("_mssql.MSSQLConnection.__init__() -> dbopen() returned NULL")
-            if self in connection_object_list:
-                connection_object_list.remove(self)
+            connection_object_list.remove(self)
             maybe_raise_MSSQLDatabaseException(None)
             raise MSSQLDriverException("Connection to the database failed for an unknown reason.")
 
         self._connected = 1
 
         if conn_properties is None:
             conn_properties = \
@@ -728,15 +718,15 @@
             conn_properties = ' '.join(conn_properties)
         cdef bytes conn_props_bytes
         cdef char *conn_props_cstr
         if conn_properties:
             log("_mssql.MSSQLConnection.__init__() -> dbcmd() setting connection values")
             # Set connection properties, some reasonable values are used by
             # default but they can be customized
-            conn_props_bytes = conn_properties.encode('utf-8')
+            conn_props_bytes = conn_properties.encode(charset)
             conn_props_cstr = conn_props_bytes
             dbcmd(self.dbproc, conn_props_bytes)
 
             rtc = db_sqlexec(self.dbproc)
             if (rtc == FAIL):
                 raise MSSQLDriverException("Could not set connection properties")
 
@@ -829,15 +819,15 @@
 
     cdef object convert_db_value(self, BYTE *data, int dbtype, int length):
         log("_mssql.MSSQLConnection.convert_db_value()")
         cdef char buf[NUMERIC_BUF_SZ] # buffer in which we store text rep of bug nums
         cdef int converted_length
         cdef long prevPrecision
         cdef BYTE precision
-        cdef DBDATEREC2 di
+        cdef DBDATEREC di
         cdef DBDATETIME dt
         cdef DBCOL dbcol
 
         IF PYMSSQL_DEBUG == 1:
             sys.stderr.write("convert_db_value: dbtype = %d; length = %d\n" % (dbtype, length))
 
         if dbtype == SQLBIT:
@@ -873,31 +863,37 @@
                 <BYTE *>buf, NUMERIC_BUF_SZ)
 
             with decimal.localcontext() as ctx:
                 # Python 3 doesn't like decimal.localcontext() with prec == 0
                 ctx.prec = precision if precision > 0 else 1
                 return decimal.Decimal(_remove_locale(buf, converted_length).decode(self._charset))
 
-        elif dbtype == SQLDATETIME2:
-            dbanydatecrack(self.dbproc, &di, dbtype, data)
-            return datetime2(di.year, di.month, di.day,
-                di.hour, di.minute, di.second, di.nanosecond // 1000)
-
-        elif dbtype in (SQLDATETIM4, SQLDATETIME):
-            dbanydatecrack(self.dbproc, &di, dbtype, data)
+        elif dbtype in (SQLDATETIM4, SQLDATETIME2):
+            dbconvert(self.dbproc, dbtype, data, -1, SQLDATETIME,
+                <BYTE *>&dt, -1)
+            dbdatecrack(self.dbproc, &di, <DBDATETIME *><BYTE *>&dt)
             return datetime.datetime(di.year, di.month, di.day,
-                di.hour, di.minute, di.second, di.nanosecond // 1000)
+                di.hour, di.minute, di.second, di.millisecond * 1000)
 
         elif dbtype == SQLDATE:
-            dbanydatecrack(self.dbproc, &di, dbtype, data)
+            dbconvert(self.dbproc, dbtype, data, -1, SQLDATETIME,
+                <BYTE *>&dt, -1)
+            dbdatecrack(self.dbproc, &di, <DBDATETIME *><BYTE *>&dt)
             return datetime.date(di.year, di.month, di.day)
 
         elif dbtype == SQLTIME:
-            dbanydatecrack(self.dbproc, &di, dbtype, data)
-            return datetime.time(di.hour, di.minute, di.second, di.nanosecond // 1000)
+            dbconvert(self.dbproc, dbtype, data, -1, SQLDATETIME,
+                <BYTE *>&dt, -1)
+            dbdatecrack(self.dbproc, &di, <DBDATETIME *><BYTE *>&dt)
+            return datetime.time(di.hour, di.minute, di.second, di.millisecond * 1000)
+
+        elif dbtype == SQLDATETIME:
+            dbdatecrack(self.dbproc, &di, <DBDATETIME *>data)
+            return datetime.datetime(di.year, di.month, di.day,
+                di.hour, di.minute, di.second, di.millisecond * 1000)
 
         elif dbtype in (SQLVARCHAR, SQLCHAR, SQLTEXT):
             if strlen(self._charset):
                 return (<char *>data)[:length].decode(self._charset)
             else:
                 return (<char *>data)[:length]
 
@@ -966,41 +962,20 @@
 
         if dbtype[0] == SQLFLT8:
             dblValue = <double *>PyMem_Malloc(sizeof(double))
             dblValue[0] = <double>value
             dbValue[0] = <BYTE *><DBFLT8 *>dblValue
             return 0
 
-        if dbtype[0] == SQLDATE:
-            if not isinstance(value, datetime.date):
-                raise TypeError('value can only be a datetime.date')
-            value = value.strftime('%4Y-%m-%d').encode(self.charset)
-            dbtype[0] = SQLCHAR
-
-        if dbtype[0] == SQLDATETIME2:
+        if dbtype[0] in (SQLDATETIM4, SQLDATETIME):
             if type(value) not in (datetime.date, datetime.datetime):
                 raise TypeError('value can only be a date or datetime')
-            value = value.strftime('%04Y-%m-%d %H:%M:%S.%f').encode(self.charset)
-            dbtype[0] = SQLCHAR
-
-        if dbtype[0] == SQLTIME:
-            if not isinstance(value, datetime.time):
-                raise TypeError(f'value can only be a datetime.time, got {type(value)}')
-            value = value.strftime('%H:%M:%S.%f')
-            value = value.encode(self.charset)
-            dbtype[0] = SQLCHAR
 
-        if dbtype[0] in (SQLDATETIM4, SQLDATETIME, SQLDATETIME2):
-            if type(value) not in (datetime.date, datetime.datetime):
-                raise TypeError('value can only be a date or datetime')
-            microseconds=0
-            if type(value) in (datetime.datetime,):
-                microseconds=value.microsecond // 1000
-            value = value.strftime('%4Y-%m-%d %H:%M:%S.') + \
-                "%03d" % (microseconds)
+            value = value.strftime('%Y-%m-%d %H:%M:%S.') + \
+                "%03d" % (value.microsecond // 1000)
             value = value.encode(self.charset)
             dbtype[0] = SQLCHAR
 
         if dbtype[0] in (SQLNUMERIC, SQLDECIMAL):
             # There seems to be no harm in setting precision higher than
             # necessary
             decimal_type_info.precision = 33
@@ -1071,15 +1046,15 @@
             binValue = <BYTE *>PyMem_Malloc(16)
             memcpy(binValue, <char *>value.bytes_le, 16)
             length[0] = 16
             dbValue[0] = <BYTE *>binValue
             return 0
 
         # No conversion was possible so raise an error
-        raise MSSQLDriverException(f'Unable to convert value dbtype={dbtype[0]}')
+        raise MSSQLDriverException('Unable to convert value')
 
     cpdef execute_non_query(self, query_string, params=None):
         """
         execute_non_query(query_string, params=None)
 
         This method sends a query to the MS SQL Server to which this object
         instance is connected. After completion, its results (if any) are
@@ -1916,25 +1891,25 @@
     cdef size_t l = strlen(s)
     return _remove_locale(s, l)
 
 cdef int _tds_ver_str_to_constant(verstr) except -1:
     """
         http://www.freetds.org/userguide/choosingtdsprotocol.htm
     """
-    if verstr == '4.2':
+    if verstr == u'4.2':
         return DBVERSION_42
-    if verstr == '7.0':
+    if verstr == u'7.0':
         return DBVERSION_70
-    if verstr in ('7.1', '8.0'):
+    if verstr in (u'7.1', u'8.0'):
         return DBVERSION_71
-    if verstr == '7.2':
+    if verstr == u'7.2':
         return DBVERSION_72
-    if verstr == '7.3':
+    if verstr == u'7.3':
         return DBVERSION_73
-    if verstr == '8.0':
+    if verstr == u'8.0':
         return DBVERSION_71
     raise MSSQLException('unrecognized tds version: %s' % verstr)
 
 #######################
 ## Quoting Functions ##
 #######################
 cdef _quote_simple_value(value, charset='utf8'):
@@ -1975,29 +1950,24 @@
             return b'0x' + binascii.hexlify(value)
 
         # will still be string type if there was a null byte in it or if the
         # decoding failed.  In this case, just send it as hex.
         if isinstance(value, str):
             return '0x' + value.encode('hex')
 
-    if isinstance(value, datetime2):
-        return  value.strftime("'%04Y-%m-%d %H:%M:%S.%f'")
-
     if isinstance(value, datetime.datetime):
-        return value.strftime("'%04Y-%m-%d %H:%M:%S.") + \
-                "%03d'" % (value.microsecond // 1000)
+        return "'%04d-%02d-%02d %02d:%02d:%02d.%03d'" % (
+            value.year, value.month, value.day,
+            value.hour, value.minute, value.second,
+            value.microsecond / 1000)
 
     if isinstance(value, datetime.date):
         return "'%04d-%02d-%02d'" % (
         value.year, value.month, value.day)
 
-    if isinstance(value, datetime.time):
-        return value.strftime("'%H:%M:%S.") + \
-                "%06d'" % (value.microsecond)
-
     return None
 
 cdef _quote_or_flatten(data, charset='utf8'):
     result = _quote_simple_value(data, charset)
 
     if result is not None:
         return result
@@ -2042,15 +2012,15 @@
 _re_name_param = re.compile(br'(%\(([^\)]+)\)(?:[sd]))')
 cdef _substitute_params(toformat, params, charset):
     if params is None:
         return toformat
 
     if not issubclass(type(params),
             (bool, int, long, float, unicode, str, bytes, bytearray, dict, tuple,
-             datetime.datetime, datetime.date, datetime.time, dict, decimal.Decimal, uuid.UUID)):
+             datetime.datetime, datetime.date, dict, decimal.Decimal, uuid.UUID)):
         raise ValueError("'params' arg (%r) can be only a tuple or a dictionary." % type(params))
 
     if charset:
         quoted = _quote_data(params, charset)
     else:
         quoted = _quote_data(params)
 
@@ -2111,15 +2081,14 @@
             # do the string substitution
             match_start = match.start(1) + offset
             match_end = match.end(1) + offset
             toformat = toformat[:match_start] + ensure_bytes(param_val) + toformat[match_end:]
             #print(param_val, param_val_len, offset_adjust, match_start, match_end)
             # adjust the offset for the next usage
             offset += offset_adjust
-
     return toformat
 
 # We'll add these methods to the module to allow for unit testing of the
 # underlying C methods.
 def quote_simple_value(value):
     return _quote_simple_value(value)
```

### Comparing `pymssgl-2.2.8.dev28/src/pymssql/_pymssql.pyx` & `pymssgl-2.2.9.dev0/src/pymssql/_pymssql.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -434,15 +434,14 @@
                 param_output = False
 
             db_type = _mssql.py2db_type(param_type, param_value)
 
             proc.bind(param_value, db_type, output=param_output)
         try:
             self._returnvalue = proc.execute()
-            self.description = self._source._conn.get_header()
         except _mssql.MSSQLDatabaseException, e:
             raise DatabaseError, e.args[0]
         return tuple([proc.parameters[p] for p in proc.parameters])
 
     def close(self):
         """
         Closes the cursor. The cursor is unusable from this point.
@@ -588,16 +587,15 @@
         """
         This method does nothing, as permitted by DB-API specification.
         """
         pass
 
 def connect(server='.', user=None, password=None, database='', timeout=0,
         login_timeout=60, charset='UTF-8', as_dict=False,
-        host='', appname=None, port='1433', encryption=None, read_only=False,
-        conn_properties=None, autocommit=False, tds_version=None):
+        host='', appname=None, port='1433', conn_properties=None, autocommit=False, tds_version=None):
     """
     Constructor for creating a connection to the database. Returns a
     Connection object.
 
     :param server: database host
     :type server: string
     :param user: database user to connect as. Default value: None.
@@ -641,19 +639,17 @@
     except ValueError:
         timeout = 0
 
     if host:
         server = host
 
     try:
-        conn = _mssql.connect(server=server, encryption=encryption,
-                              user=user, password=password,
+        conn = _mssql.connect(server=server, user=user, password=password,
                               charset=charset, database=database,
                               appname=appname, port=port, tds_version=tds_version,
-                              read_only=read_only,
                               conn_properties=conn_properties)
 
     except _mssql.MSSQLDatabaseException, e:
         raise OperationalError(e.args[0])
 
     except _mssql.MSSQLDriverException, e:
         raise InterfaceError(e.args[0])
```

### Comparing `pymssgl-2.2.8.dev28/src/pymssql/sqlfront.pxd` & `pymssgl-2.2.9.dev0/src/pymssql/sqlfront.pxd`

 * *Files 5% similar despite different names*

```diff
@@ -69,28 +69,14 @@
         DBINT weekday
         DBINT hour
         DBINT minute
         DBINT second
         DBINT millisecond
         DBINT tzone
 
-    ctypedef struct            DBDATEREC2:
-        DBINT year
-        DBINT quarter
-        DBINT month
-        DBINT day
-        DBINT dayofyear
-        DBINT week
-        DBINT weekday
-        DBINT hour
-        DBINT minute
-        DBINT second
-        DBINT nanosecond
-        DBINT tzone
-
     ctypedef struct DBNUMERIC:
         BYTE precision
         BYTE scale
         BYTE array[33]
 
     ctypedef DBNUMERIC DBDECIMAL
 
@@ -313,31 +299,26 @@
     #     column    Nth column in computeid, starting from 1.
     #
     #   Returns:
     #     pointer to the data, or NULL if data is NULL, or if column is
     #     out of range
     BYTE * dbdata(DBPROCESS *, int) nogil
 
-    # Break any kind of date or time value into useful pieces.
+    # Break a DBDATETIME value into useful pieces.
     #
     #   Parameters:
-    #     dbproc     contains all information needed by db-lib to manage
-    #                     communications with the server.
-    #     di             output: structure to contain the exploded parts of
-    #                     datetime.
-    #     type         input: type of date/time value returned by dbcoltype().
+    #     dbproc    contains all information needed by db-lib to manage
+    #               communications with the server.
+    #     di        output: structure to contain the exploded parts of
+    #                       datetime.
     #     datetime  input: DBDATETIME to be converted.
     #
     #   Return values:
     #     SUCCEED always
-    #
-    # remarks
-    #           The members of \a di have different names, depending on whether \c --with-msdblib was configured.
-    #           This is an extension to dbdatecrack(), see it for more information.
-    RETCODE dbanydatecrack(DBPROCESS * , DBDATEREC2 * , int , const void *)
+    RETCODE dbdatecrack(DBPROCESS *, DBDATEREC *, DBDATETIME *)
 
     # Get size of current row's data in a regular result column.
     #
     #   Parameters:
     #     dbproc    contains all information needed by db-lib to manage
     #               communications with the server.
     #     column    Nth column in computeid, starting from 1.
@@ -761,11 +742,9 @@
     RETCODE DBSETLAPP(LOGINREC *x, char *y)
     RETCODE DBSETLHOST(LOGINREC *x, char *y)
     RETCODE DBSETLPWD(LOGINREC *x, char *y)
     RETCODE DBSETLUSER(LOGINREC *x, char *y)
     RETCODE DBSETLCHARSET(LOGINREC *x, char *y)
     RETCODE DBSETLVERSION(LOGINREC *login, BYTE version)
     RETCODE DBSETLDBNAME(LOGINREC *x, char *y)
-    RETCODE DBSETLENCRYPT(LOGINREC *login, int x)
-    RETCODE DBSETLREADONLY(LOGINREC *login, int x)
 
 ctypedef int LINE_T
```

### Comparing `pymssgl-2.2.8.dev28/tests/conftest.py` & `pymssgl-2.2.9.dev0/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,49 @@
 # -*- coding: utf-8 -*-
 """
 Pytest configuration.
 """
 
+from os.path import dirname
+import sys
+
+# When using tox, it can accidentally pick up a {pymssql,_mssql}.so file in the
+# root directory and then get ImportError because of incompatibility in Python
+# versions. By removing the root directory from the sys.path, it forces tox to
+# import the library from correct place in the tox virtualenv.
+if '.tox' in sys.executable:
+    root_dir = dirname(dirname(__file__))
+    sys.path.remove(root_dir)
+
 import decimal
 import os
 from configparser import ConfigParser
 
 import pytest
 
 import tests.helpers as th
 from .helpers import cfgpath, clear_db, get_app_lock, release_app_lock
 
-
-@pytest.fixture(scope="module")
-def mssql_conn():
-    return th.mssqlconn()
-
 _parser = ConfigParser({
     'server': 'localhost',
     'username': 'sa',
     'password': 'sqlServerPassw0rd',
     'database': 'tempdb',
     'port': '1433',
     'ipaddress': '127.0.0.1',
     'instance': '',
 })
 
-optional_markers = {
-    "slow": {"help": "Skip long tests",
-             "marker-descr": "Mark tests that run longer than ~3 seconds",
-             "skip-reason": "Test runs too long."},
-    "mssql_server_required": {"help": "Skip tests that require MSSQL server",
-             "marker-descr": "Mark tests that require MSSQL server",
-             "skip-reason": "Test only runs if MSSQL server is available."},
-    # add further markers here
-}
-
 def pytest_addoption(parser):
     parser.addoption(
         "--pymssql-section",
         type=str,
         default=os.environ.get('PYMSSQL_TEST_CONFIG', 'DEFAULT'),
         help="The name of the section to use from tests.cfg"
     )
-    for marker, info in optional_markers.items():
-        parser.addoption("--skip-{}".format(marker.replace('_','-')), action="store_true",
-                         default=False, help=info['help'])
 
 def pytest_configure(config):
     _parser.read(cfgpath)
     section = config.getoption('--pymssql-section')
 
     if not _parser.has_section(section) and section != 'DEFAULT':
         raise ValueError('the tests.cfg file does not have section: %s' % section)
@@ -59,35 +52,23 @@
     th.config.user = os.getenv('PYMSSQL_TEST_USERNAME') or _parser.get(section, 'username')
     th.config.password = os.getenv('PYMSSQL_TEST_PASSWORD') or _parser.get(section, 'password')
     th.config.database = os.getenv('PYMSSQL_TEST_DATABASE') or _parser.get(section, 'database')
     th.config.port = os.getenv('PYMSSQL_TEST_PORT') or _parser.get(section, 'port')
     th.config.ipaddress = os.getenv('PYMSSQL_TEST_IPADDRESS') or _parser.get(section, 'ipaddress')
     th.config.instance = os.getenv('PYMSSQL_TEST_INSTANCE') or _parser.get(section, 'instance')
     th.config.orig_decimal_prec = decimal.getcontext().prec
-
-    for marker, info in optional_markers.items():
-        config.addinivalue_line("markers",
-                                "{}: {}".format(marker, info['marker-descr']))
+    th.mark_slow = pytest.mark.slow
+    th.skip_test = pytest.skip
 
     if get_app_lock():
         clear_db()
 
 def pytest_unconfigure(config):
     release_app_lock()
 
 
 def pytest_collection_modifyitems(config, items):
-
-    marker = "mssql_server_required"
-    info = optional_markers[marker]
-    if th.global_mssqlconn is None or config.getoption("--skip-{}".format(marker.replace('_','-'))):
-        skip = pytest.mark.skip(reason=info['skip-reason'])
-        for item in items:
-            if marker in item.keywords:
-                item.add_marker(skip)
-    marker = "slow"
-    info = optional_markers[marker]
-    if th.global_mssqlconn is None or config.getoption("--skip-{}".format(marker)):
-        skip = pytest.mark.skip(reason=info['skip-reason'])
+    if th.global_mssqlconn is None:
+        skip = pytest.mark.skip(reason="Need test server to run")
         for item in items:
-            if marker in item.keywords:
+            if "mssql_server_required" in item.keywords:
                 item.add_marker(skip)
```

### Comparing `pymssgl-2.2.8.dev28/tests/helpers.py` & `pymssgl-2.2.9.dev0/tests/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 """
 
 import logging
 from os import path
 import time
 
 import pytest
-from pymssql import _mssql
-import pymssql
-
 
 def eq_(a, b):
-    assert a == b, f"'{a}' != '{b}'"
+    assert a == b
 
 def skip_test(reason='No reason given to skip_test'):
     pytest.skip(reason)
 
 def mark_slow(f):
     return f
 
 mssql_server_required = pytest.mark.mssql_server_required
 
+from pymssql import _mssql
+import pymssql
 
 
 class Config(object):
     def __str__(self):
         return f"server={self.server}, port={self.port}, database={self.database}, " \
                f"user={self.user}, password={self.password}"
 
 config = Config()
 
 cdir = path.dirname(__file__)
+tmpdir = path.join(cdir, 'tmp')
 cfgpath = path.join(cdir, 'tests.cfg')
 global_mssqlconn = None
 
 def mssqlconn(conn_properties=None):
     return _mssql.connect(
         server=config.server,
         user=config.user,
@@ -318,15 +318,15 @@
 
         eq_(cur.rowcount, 5)
 
     def test_as_dict(self):
         # test for http://code.google.com/p/pymssql/issues/detail?id=92
         cur = self.conn.cursor(as_dict=True)
         cur.execute("SELECT 'foo' AS first_name, 'bar' AS last_name")
-        eq_(cur.fetchall(), [{'first_name': 'foo', 'last_name': 'bar'}])
+        eq_(cur.fetchall(), [{'first_name': u'foo', 'last_name': u'bar'}])
 
     def test_as_dict_no_column_name(self):
         cur = self.conn.cursor(as_dict=True)
         try:
             # SQL Server >= 2008:
             #
             #   SELECT MAX(x), MIN(x) AS [MIN(x)]
@@ -414,16 +414,15 @@
     }
     delete_sql = []
     for type, drop_sql in mapping.items():
         sql = 'select name, object_name( parent_object_id ) as parent_name '\
             'from sys.objects where type in (\'%s\')' % '", "'.join(type)
         conn.execute_query(sql)
         for row in conn:
-            if row['name'][0] not in ('#','@'):
-                delete_sql.append(drop_sql % dict(row))
+            delete_sql.append(drop_sql % dict(row))
     for sql in delete_sql:
         conn.execute_non_query(sql)
 
 
 class StoredProc(object):
     def __init__(self, name, args, body, mssql=None):
         self.name = name
@@ -502,46 +501,7 @@
     elif ver_code == 10:
         major_version = 2008
     elif ver_code == 9:
         major_version = 2005
     else:
         major_version = 2000
     return major_version
-
-
-
-@mssql_server_required
-class TestCaseWithTable:
-
-    table_name = "dbo.test1"
-    ddl_create = f"CREATE TABLE {table_name} (test DATETIME2)"
-
-    @classmethod
-    def setup_class(cls):
-        cls.conn = mssqlconn()
-        cls.create_table()
-
-    @classmethod
-    def create_table(cls):
-        cls.ddl_drop = f"IF OBJECT_ID('{cls.table_name}') IS NOT NULL DROP TABLE {cls.table_name}"
-        cls.conn.execute_non_query(cls.ddl_drop)
-        cls.conn.execute_non_query(cls.ddl_create)
-
-    @classmethod
-    def teardown_class(cls):
-        cls.conn.execute_non_query(cls.ddl_drop)
-
-    def setup_method(self, method):
-        self.conn.execute_non_query(f"DELETE FROM {self.table_name}")
-
-    def insert_and_select(self, cname, value, params_as_dict=False):
-        if params_as_dict:
-            inssql = f'insert into {self.table_name} ({cname}) values (%(value)s)'
-            self.conn.execute_non_query(inssql, dict(value=value))
-        else:
-            inssql = f'insert into {self.table_name} ({cname}) values (%s)'
-            self.conn.execute_non_query(inssql, value)
-        self.conn.execute_query(f'select {cname} from {self.table_name}')
-        rows = tuple(self.conn)
-        eq_(len(rows), 1)
-        cval = rows[0][cname]
-        return cval
```

### Comparing `pymssgl-2.2.8.dev28/tests/run_sqlalchemy_tests.py` & `pymssgl-2.2.9.dev0/tests/run_sqlalchemy_tests.py`

 * *Files identical despite different names*

### Comparing `pymssgl-2.2.8.dev28/tests/test_bulk_copy.py` & `pymssgl-2.2.9.dev0/tests/test_bulk_copy.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 """
 Test bulk copy.
 """
 
 import unittest
 import datetime
 
-import pytest
-
 from pymssql import _mssql
-from tests.helpers import drop_table, pymssqlconn
+from tests.helpers import drop_table, pymssqlconn, mssql_server_required
 
 
 tablename = "pymssql"
 simple_table = "CREATE TABLE %s (a1 INT, a2 INT, a3 INT)" % tablename
 complex_table = """
     CREATE TABLE %s (
         pk_id int IDENTITY (1, 1) NOT NULL,
@@ -24,15 +22,15 @@
         col_bit bit,
         col_varchar varchar(50),
         col_varbinary varbinary(50)
     )
 """ % tablename
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestTypes(unittest.TestCase):
     def setUp(self):
         self.conn = pymssqlconn()
         drop_table(self.conn._conn, tablename)
 
     def tearDown(self):
         self.conn.close()
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_config.py` & `pymssgl-2.2.9.dev0/tests/test_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 # -*- coding: utf-8 -*-
 """
 Test connection config.
 """
 
 from __future__ import with_statement
-from os import path, environ
-import tempfile
-
-import pytest
+from os import path, makedirs, environ
+import shutil
 
 from pymssql import _mssql
 
-@pytest.mark.mssql_server_required
+from .helpers import tmpdir, skip_test, mssql_server_required
+config_dump_path = path.join(tmpdir, 'freetds-config-dump.txt')
+
+def setup_module():
+    if not path.isdir(tmpdir):
+        makedirs(tmpdir)
+
+@mssql_server_required
 class TestConfig(object):
     def connect(self, **kwargs):
-        with tempfile.TemporaryDirectory() as tmpdir:
-            config_dump_path = path.join(tmpdir, 'freetds-config-dump.txt')
-            environ['TDSDUMPCONFIG'] = config_dump_path
-            try:
-                _mssql.connect(**kwargs)
-                assert False
-            except _mssql.MSSQLDriverException as e:
-                # we get this when the name of the server is not valid
-                if 'Connection to the database failed' not in str(e):
-                    raise
-            except _mssql.MSSQLDatabaseException as e:
-                # we get this when the name or IP can be obtained but the connection
-                # can not be made
-                if e.args[0][0] != 20009:
-                    raise
-            with open(config_dump_path, 'r') as fh:
-                return fh.read()
+        environ['TDSDUMPCONFIG'] = config_dump_path
+        try:
+            _mssql.connect(**kwargs)
+            assert False
+        except _mssql.MSSQLDriverException as e:
+            # we get this when the name of the server is not valid
+            if 'Connection to the database failed' not in str(e):
+                raise
+        except _mssql.MSSQLDatabaseException as e:
+            # we get this when the name or IP can be obtained but the connection
+            # can not be made
+            if e.args[0][0] != 20009:
+                raise
+        with open(config_dump_path, 'r') as fh:
+            return fh.read()
 
-    @pytest.mark.slow
     def test_config_values(self):
         config_dump = self.connect(
             server='dontnameyourserverthis',
             user = 'bob',
             database = 'tempdb',
             tds_version='7.1'
             )
@@ -45,57 +47,52 @@
         # test default port
         assert 'port = 1433' in config_dump
         # not sure why 7.1 version is used instead of 8.0 which is the
         # default
         assert 'major_version = 7' in config_dump
         assert 'minor_version = 1' in config_dump
 
-    @pytest.mark.slow
     def test_tds_protocol_version_42(self):
         config_dump = self.connect(
             server='dontnameyourserverthis',
             tds_version='4.2'
             )
         assert 'major_version = 4' in config_dump
         assert 'minor_version = 2' in config_dump
 
-    @pytest.mark.slow
     def test_tds_protocol_version_70(self):
         config_dump = self.connect(
             server='dontnameyourserverthis',
             tds_version='7.0'
             )
         assert 'major_version = 7' in config_dump
         assert 'minor_version = 0' in config_dump
 
-    @pytest.mark.slow
     def test_tds_protocol_version_71(self):
         config_dump = self.connect(
             server='dontnameyourserverthis',
             tds_version='7.1'
             )
         assert 'major_version = 7' in config_dump
         assert 'minor_version = 1' in config_dump
 
-    @pytest.mark.slow
     def test_tds_protocol_version_80(self):
         # follow-up: turns out 8.0 was erroneous.  MS named the new protocol
         # 7.1 instead of 8.0, so FreeTDS will accept 8.0 but shows as 7.1.
         # got that from the FreeTDS mailling list.  New FreeTDS docs,built from
         # source, have a page that describes the protocol and that page lists
         # versions 7.0, 7.1, and 7.2 among others.
 
         config_dump = self.connect(
             server='dontnameyourserverthis',
             tds_version='8.0'
             )
         assert 'major_version = 7' in config_dump
         assert 'minor_version = 1' in config_dump
 
-    @pytest.mark.slow
     def test_tds_protocol_version_72(self):
         config_dump = self.connect(
             server='dontnameyourserverthis',
             tds_version='7.2'
             )
         assert 'major_version = 7' in config_dump
         assert 'minor_version = 2' in config_dump
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_connection_as_dict.py` & `pymssgl-2.2.9.dev0/tests/test_connection_as_dict.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 # -*- coding: utf-8 -*-
 """
 Test connection with as_dict=True.
 """
 
 import unittest
 
-import pytest
-
 import pymssql
 
-from .helpers import config
+from .helpers import config, mssql_server_required
 
 def pymssqlconn(**kwargs):
     return pymssql.connect(
             server=config.server,
             user=config.user,
             password=config.password,
             database=config.database,
             port=config.port,
             **kwargs
         )
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestConnectionAsDict(unittest.TestCase):
 
     def setUp(self):
         self.conn = pymssqlconn(as_dict=True)
 
     def test_fetchall_with_connection_as_dict(self):
         # This test is for http://code.google.com/p/pymssql/issues/detail?id=18
         cursor = self.conn.cursor()
         cursor.execute("SELECT 'foo' AS first_name, 'bar' AS last_name")
         data = cursor.fetchall()
-        self.assertEqual(data, [{'first_name': 'foo', 'last_name': 'bar'}])
+        self.assertEqual(data, [{'first_name': u'foo', 'last_name': u'bar'}])
 
     def test_no_results_with_connection_as_dict(self):
         # Make sure that checking for columns without names doesn't break
         # statements that don't return results
 
         cursor = self.conn.cursor()
         cursor.execute("""
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_connection_timeout.py` & `pymssgl-2.2.9.dev0/tests/test_connection_timeout.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import time
 import pytest
 import pymssql
 
 
-@pytest.mark.slow
-@pytest.mark.mssql_server_required
 @pytest.mark.timeout(120)
 @pytest.mark.xfail(strict=False)
 @pytest.mark.parametrize('to', [2])
 def test_remote_connect_timeout(to):
 
     t = time.time()
     try:
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_connections.py` & `pymssgl-2.2.9.dev0/tests/test_connections.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,41 +3,44 @@
 Test connection to database.
 """
 
 from __future__ import with_statement
 from os import path, makedirs, environ
 import re
 import unittest
-import tempfile
-
 import pytest
 
 from pymssql import _mssql
 
-from .helpers import config, mssqlconn
+from .helpers import config, skip_test, mssqlconn, mssql_server_required
 server = config.server
 username = config.user
 password = config.password
 database = config.database
 port = config.port
 ipaddress = config.ipaddress
 instance = config.instance
 
+cdir = path.dirname(__file__)
+tmpdir = path.join(cdir, 'tmp')
+config_dump_path = path.join(tmpdir, 'freetds-config-dump.txt')
+dump_path = path.join(tmpdir, 'freetds-dump.txt')
+
+def setup_module():
+    if not path.isdir(tmpdir):
+        makedirs(tmpdir)
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestCons(unittest.TestCase):
     def connect(self, **kwargs):
-        with tempfile.TemporaryDirectory() as tmpdir:
-            config_dump_path = path.join(tmpdir, 'freetds-config-dump.txt')
-            dump_path = path.join(tmpdir, 'freetds-dump.txt')
-            environ['TDSDUMPCONFIG'] = config_dump_path
-            environ['TDSDUMP'] = dump_path
-            _mssql.connect(**kwargs)
-            with open(config_dump_path, 'r') as fh:
-                return fh.read()
+        environ['TDSDUMPCONFIG'] = config_dump_path
+        environ['TDSDUMP'] = dump_path
+        _mssql.connect(**kwargs)
+        with open(config_dump_path, 'r') as fh:
+            return fh.read()
 
     def test_connection_by_dns_name(self):
         cdump = self.connect(server=server, port=port, user=username, password=password)
         dump_server_name = re.search('server_name = (\\S+)', cdump).groups()[0]
         self.assertIn(server, dump_server_name)
         dump_server_host_name = re.search('server_host_name = (\\S+)', cdump).groups()[0]
         self.assertEqual(dump_server_host_name, server)
@@ -71,15 +74,15 @@
         dump_server_host_name = re.search('server_host_name = (\\S+)', cdump).groups()[0]
         self.assertEqual(dump_server_host_name, server)
         dump_port = re.search('port = (\\S+)', cdump).groups()[0]
         self.assertIn(port, dump_port)
 
     def test_instance(self):
         if not instance:
-            pytest.skip()
+            skip_test()
         server_join = r'%s\%s' % (server, instance)
         cdump = self.connect(server=server_join, user=username, password=password)
         dump_server_name = re.search('server_name = (\\S+)', cdump).groups()[0]
         self.assertIn(server, dump_server_name)
         dump_server_host_name = re.search('server_host_name = (\\S+)', cdump).groups()[0]
         self.assertEqual(dump_server_host_name, server)
         dump_port = re.search('port = (\\S+)', cdump).groups()[0]
@@ -118,15 +121,14 @@
             server=server,
             user=username,
             password=password
         )
         conn.close()
 
 
-@pytest.mark.slow
 class TestFailedConnection(unittest.TestCase):
 
     @pytest.mark.xfail(strict=False, reason="Could timeout, or fail with different error messages")
     @pytest.mark.timeout(600)
     def test_repeated_failed_connections(self):
         # This is a test for https://github.com/pymssql/pymssql/issues/145
         # (Repeated failed connections result in error string getting longer
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_context_managers.py` & `pymssgl-2.2.9.dev0/tests/test_context_managers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # -*- coding: utf-8 -*-
 """
 Test context managers -- i.e.: the `with` statement
 """
 
 import unittest
 
-import pytest
-
 from pymssql import InterfaceError
-from .helpers import pymssqlconn, mssqlconn
+from .helpers import pymssqlconn, mssqlconn, mssql_server_required
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestContextManagers(unittest.TestCase):
     def test_pymssql_Connection_with(self):
         with pymssqlconn() as conn:
             cursor = conn.cursor()
             cursor.execute("SELECT @@version AS version")
             self.assertIsNotNone(conn._conn)
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_debug_queries.py` & `pymssgl-2.2.9.dev0/tests/test_debug_queries.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 """
 
 from contextlib import contextmanager
 from io import StringIO
 import sys
 import unittest
 
-import pytest
-
-from .helpers import mssqlconn
+from .helpers import mssqlconn, mssql_server_required
 
 
 @contextmanager
 def redirect_stderr():
     sys.stderr = StringIO()
     yield sys.stderr
     sys.stderr = sys.__stderr__
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestMSSQLConnectionWithDebugQueries(unittest.TestCase):
 
     def setUp(self):
         self.conn = mssqlconn()
         self.conn.debug_queries = True
 
     def test_MSSQLConnection_with_debug_queries(self):
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_err_handle.py` & `pymssgl-2.2.9.dev0/tests/test_err_handle.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 """
 Test error handling.
 """
 
 from datetime import datetime
 import unittest
 
-import pytest
-
 from pymssql import _mssql
+from .helpers import mssql_server_required
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class ErrHandleTests(unittest.TestCase):
 
     def test01DBError(self):
         connection = None
         severity = 8
         dberr = 101
         oserr = 0
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_green.py` & `pymssgl-2.2.9.dev0/tests/test_green.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 # -*- coding: utf-8 -*-
 """
 Some async tests with gevent.
 """
 
 import datetime
-import unittest
-
 import pytest
+import unittest
 
 import pymssql
-from .helpers import mssqlconn, pymssqlconn
+from .helpers import mssqlconn, pymssqlconn, mark_slow, mssql_server_required
 
 gevent = pytest.importorskip("gevent")
-try:
-    import gevent.socket
-except ImportError:
-    pytest.skip('gevent is not available', allow_module_level=True)
+import gevent.socket
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class GreenletTests(unittest.TestCase):
 
     def greenlet_run_pymssql_execute(self, num):
         with pymssqlconn() as conn:
             cur = conn.cursor()
             cur.execute("""
             WAITFOR DELAY '00:00:05'  -- sleep for 5 seconds
@@ -76,29 +72,29 @@
 
         gevent.joinall(greenlets)
 
         dt2 = datetime.datetime.now()
 
         return dt2 - dt1
 
-    @pytest.mark.slow
+    @mark_slow
     def test_gevent_socket_pymssql_execute_wait_read_concurrency(self):
         def wait_callback(read_fileno):
             gevent.socket.wait_read(read_fileno)
 
         pymssql.set_wait_callback(wait_callback)
 
         elapsed_time = self._run_all_greenlets(
             self.greenlet_run_pymssql_execute)
 
         self.assertTrue(
             elapsed_time < datetime.timedelta(seconds=20),
             'elapsed_time < 20 seconds')
 
-    @pytest.mark.slow
+    @mark_slow
     def test_gevent_socket_pymssql_callproc_wait_read_concurrency(self):
         def wait_callback(read_fileno):
             gevent.socket.wait_read(read_fileno)
 
         pymssql.set_wait_callback(wait_callback)
 
         with pymssqlconn() as conn:
@@ -118,15 +114,15 @@
         elapsed_time = self._run_all_greenlets(
             self.greenlet_run_pymssql_callproc)
 
         self.assertTrue(
             elapsed_time < datetime.timedelta(seconds=20),
             'elapsed_time < 20 seconds')
 
-    @pytest.mark.slow
+    @mark_slow
     def test_gevent_socket_mssql_execute_wait_read_concurrency(self):
         def wait_callback(read_fileno):
             gevent.socket.wait_read(read_fileno)
 
         pymssql.set_wait_callback(wait_callback)
 
         elapsed_time = self._run_all_greenlets(
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_memory.py` & `pymssgl-2.2.9.dev0/tests/test_memory.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import gc
 import sys
 import psutil
 import pymssql
 import pytest
 
 
-@pytest.mark.slow
 @pytest.mark.xfail(reason="Memory test is not stable")
 def test_memory_leak_on_unsuccessful_connect():
     """
     This test checks python process memory usage and not just unsuccessful
     connect path. Many other factors (i.e. garbage collection) affect memory
     usage pattern. So this is an indirect test which is somewhat flaky and
     because of that is marked 'xfail'.
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_pymssql.py` & `pymssgl-2.2.9.dev0/tests/test_pymssql.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 
 import unittest
 
 import pytest
 
 import pymssql as pym
 
-from .helpers import pymssqlconn, PyTableBase, CursorBase, eq_, config
+from .helpers import (pymssqlconn, PyTableBase, CursorBase, eq_, config,
+                      skip_test, mssql_server_required)
 
 class TestDBAPI2(object):
     def test_version(self):
         assert pym.__version__
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestTransaction(unittest.TestCase, PyTableBase):
     tname = 'users'
     cols = (
         'name varchar(50)',
     )
 
     def setUp(self):
@@ -88,24 +89,24 @@
             # encountered an error, so we want to rollback
             self.conn.rollback()
         # rollback should have resulted in user's insert getting rolled back
         # too
         eq_(self.row_count(), 0)
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestCursor(CursorBase):
     dbmod = pym
 
     @classmethod
     def newconn(cls):
         cls.conn = pymssqlconn()
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestBasicConnection(unittest.TestCase):
 
     def connect(self, conn_props=None):
         return pym.connect(
             server=config.server,
             user=config.user,
             password=config.password,
@@ -140,15 +141,15 @@
             server=config.server,
             user=config.user,
             password=config.password
         )
         conn.close()
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestAutocommit(unittest.TestCase, PyTableBase):
     tname = 'test'
     cols = (
         'name varchar(50)',
     )
 
     insert_query = 'INSERT INTO {tname} VALUES (%s)'.format(tname=tname)
@@ -168,15 +169,15 @@
         """
         cur = pymssqlconn(autocommit=True).cursor()
         try:
             cur.execute("CREATE DATABASE {0}".format(self.test_db_name))
         except pym.OperationalError as e:
             expected_msg = "CREATE DATABASE permission denied in database 'master'"
             if expected_msg in str(e.args[1]):
-                pytest.skip('We have no CREATE DATABASE permission on test database')
+                skip_test('We have no CREATE DATABASE permission on test database')
             else:
                 pytest.fail()
         else:
             cur.execute("DROP DATABASE {0}".format(self.test_db_name))
 
     def test_db_creation_without_autocommit(self):
         """
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_queries.py` & `pymssgl-2.2.9.dev0/tests/test_queries.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 """
 Test queries.
 """
 
 from datetime import datetime
 import unittest
 
-import pytest
-
 from pymssql import _mssql
 
-from .helpers import mssqlconn, drop_table
+from .helpers import mssqlconn, drop_table, mssql_server_required
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class QueryTests(unittest.TestCase):
 
     @classmethod
     def setup_class(cls):
         cls.mssql = mssqlconn()
         cls.createTestTable()
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_sprocs.py` & `pymssgl-2.2.9.dev0/tests/test_sprocs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,28 @@
 # -*- coding: utf-8 -*-
 """
 Test stored procedure usage.
 """
 
-from contextlib import contextmanager
 import decimal
 import datetime
 import os
+import sys
 import unittest
 
 import pymssql
 from pymssql import _mssql
 
 import pytest
 
-from .helpers import mssqlconn, pymssqlconn
-
-
-@contextmanager
-def stored_proc(mssqlcon, dbtype):
-
-    dbtype = dbtype.lower()
-    identifier = dbtype
-    if dbtype == 'decimal':
-        identifier = 'decimal(6, 5)'
-    elif dbtype == 'numeric':
-        identifier = 'numeric(6, 5)'
-    elif dbtype == 'time':
-        identifier = 'time(7)'
-
-    name = f"pymssqlTest_{dbtype}"
-
-    cmd = f"""
-        CREATE PROCEDURE [dbo].[{name}]
-            @inp {identifier},
-            @out {identifier} output
-        AS
-        BEGIN
-            SET @out = @inp;
-            RETURN 0;
-        END
-    """
-    mssqlcon.execute_non_query(cmd)
-
-    try:
-        yield name
-    finally:
-        # Code to release resource, e.g.:
-        mssqlcon.execute_non_query(f'DROP PROCEDURE [dbo].[{name}]')
-
+from .helpers import mssqlconn, pymssqlconn, eq_, skip_test, get_sql_server_version, mssql_server_required
 
 FIXED_TYPES = (
     'BigInt',
     'Bit',
-    'Date',
     'DateTime',
     'Decimal',
     'Int',
     'Money',
     'Numeric',
     'SmallInt',
     'TinyInt',
@@ -69,15 +34,15 @@
 VARIABLE_TYPES = (
     ('Char', 4),
     ('VarChar', 4),
     ('VarBinary', 4),
     ('Text', None)  # Leave this one in the last position in case it fails (see https://code.google.com/p/pymssql/issues/detail?id=113#c2)
 )
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestFixedTypeConversion(unittest.TestCase):
 
     def setUp(self):
         self.mssql = mssqlconn()
         self.pymssql = pymssqlconn()
 
         for name in FIXED_TYPES:
@@ -114,145 +79,151 @@
 
     def testBigInt(self):
         input = 123456789
         proc = self.mssql.init_procedure('pymssqlTestBigInt')
         proc.bind(input, _mssql.SQLINT8, '@ibigint')
         proc.bind(None, _mssql.SQLINT8, '@obigint', output=True)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@obigint'])
+        eq_(input, proc.parameters['@obigint'])
 
     def testBigIntPymssql(self):
         """Same as testBigInt above but from pymssql. Uses pymssql.output class."""
+
+        if sys.version_info >= (3, ):
+            py_type = int
+        else:
+            py_type = long
+
         in_val = 123456789
         cursor = self.pymssql.cursor()
-        retval = cursor.callproc('pymssqlTestBigInt', [in_val, pymssql.output(int)])
-        self.assertEqual(in_val, retval[1])
+        retval = cursor.callproc('pymssqlTestBigInt', [in_val, pymssql.output(py_type)])
+        eq_(in_val, retval[1])
 
         in_val = 2147483647
-        retval = cursor.callproc('pymssqlTestBigInt', [in_val, pymssql.output(int)])
-        self.assertEqual(in_val, retval[1])
+        retval = cursor.callproc('pymssqlTestBigInt', [in_val, pymssql.output(py_type)])
+        eq_(in_val, retval[1])
 
     def testBit(self):
         input = True
         proc = self.mssql.init_procedure('pymssqlTestBit')
         proc.bind(input, _mssql.SQLBITN, '@ibit')
         proc.bind(False, _mssql.SQLBITN, '@obit', output=True)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@obit'])
+        eq_(input, proc.parameters['@obit'])
 
     def testDateTime(self):
         input = datetime.datetime(2009, 8, 27, 15, 28, 38)
         proc = self.mssql.init_procedure('pymssqlTestDateTime')
         proc.bind(input, _mssql.SQLDATETIME, '@idatetime')
         proc.bind(None, _mssql.SQLDATETIME, '@odatetime', output=True)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@odatetime'])
+        eq_(input, proc.parameters['@odatetime'])
 
     def testDecimal(self):
         input = decimal.Decimal('5.12345')
         output = decimal.Decimal('0.00000')
         proc = self.mssql.init_procedure('pymssqlTestDecimal')
         proc.bind(input, _mssql.SQLDECIMAL, '@idecimal')
         proc.bind(output, _mssql.SQLDECIMAL, '@odecimal', output=True, max_length=6)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@odecimal'])
-        self.assertEqual(str(input), str(proc.parameters['@odecimal']))
+        eq_(input, proc.parameters['@odecimal'])
+        eq_(str(input), str(proc.parameters['@odecimal']))
 
     def testDecimal2(self):
         input = decimal.Decimal('6.23456')
         output = decimal.Decimal('0.00000')
         proc = self.mssql.init_procedure('pymssqlTestDecimal')
         proc.bind(input, _mssql.SQLDECIMAL, '@idecimal')
         proc.bind(output, _mssql.SQLDECIMAL, '@odecimal', output=True, max_length=6)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@odecimal'])
-        self.assertEqual(str(input), str(proc.parameters['@odecimal']))
+        eq_(input, proc.parameters['@odecimal'])
+        eq_(str(input), str(proc.parameters['@odecimal']))
 
     def testDecimal3(self):
         output = decimal.Decimal('0.00000')
         proc = self.mssql.init_procedure('pymssqlTestDecimal')
         input = decimal.Decimal('6.23400')
         proc.bind(input, _mssql.SQLDECIMAL, '@idecimal')
         proc.bind(output, _mssql.SQLDECIMAL, '@odecimal', output=True, max_length=6)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@odecimal'])
-        self.assertEqual(str(input), str(proc.parameters['@odecimal']))
+        eq_(input, proc.parameters['@odecimal'])
+        eq_(str(input), str(proc.parameters['@odecimal']))
 
     def testDecimal4(self):
         output = decimal.Decimal('1.0000000')
         proc = self.mssql.init_procedure('pymssqlTestDecimal')
         input = decimal.Decimal('6.2340000')
         proc.bind(input, _mssql.SQLDECIMAL, '@idecimal')
         proc.bind(output, _mssql.SQLDECIMAL, '@odecimal', output=True, max_length=15)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@odecimal'])
-        self.assertEqual(str(input), str(proc.parameters['@odecimal']))
+        eq_(input, proc.parameters['@odecimal'])
+        eq_(str(input), str(proc.parameters['@odecimal']))
 
     def testDecimal5(self):
         output = decimal.Decimal('1.000000000')
         proc = self.mssql.init_procedure('pymssqlTestDecimal')
         input = decimal.Decimal('6.234000000')
         proc.bind(input, _mssql.SQLDECIMAL, '@idecimal')
         proc.bind(output, _mssql.SQLDECIMAL, '@odecimal', output=True, max_length=15)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@odecimal'])
-        self.assertEqual(str(input), str(proc.parameters['@odecimal']))
+        eq_(input, proc.parameters['@odecimal'])
+        eq_(str(input), str(proc.parameters['@odecimal']))
 
     def testInt(self):
         input = 10056
         proc = self.mssql.init_procedure('pymssqlTestInt')
         proc.bind(input, _mssql.SQLINT4, '@iint')
         proc.bind(None, _mssql.SQLINT4, '@oint', output=True)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@oint'])
+        eq_(input, proc.parameters['@oint'])
 
     def testMoney(self):
         input = decimal.Decimal('5.12')
         proc = self.mssql.init_procedure('pymssqlTestMoney')
         proc.bind(input, _mssql.SQLMONEY, '@imoney')
         proc.bind(None, _mssql.SQLMONEY, '@omoney', output=True)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@omoney'])
+        eq_(input, proc.parameters['@omoney'])
 
     def testNumeric(self):
         input = decimal.Decimal('5.12345')
         output = decimal.Decimal('0.00000')
         proc = self.mssql.init_procedure('pymssqlTestNumeric')
         proc.bind(input, _mssql.SQLNUMERIC, '@inumeric')
         proc.bind(output, _mssql.SQLNUMERIC, '@onumeric', output=True)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@onumeric'])
-        self.assertEqual(str(input), str(proc.parameters['@onumeric']))
+        eq_(input, proc.parameters['@onumeric'])
+        eq_(str(input), str(proc.parameters['@onumeric']))
 
     def testSmallInt(self):
         input = 10056
         proc = self.mssql.init_procedure('pymssqlTestSmallInt')
         proc.bind(input, _mssql.SQLINT2, '@ismallint')
         proc.bind(None, _mssql.SQLINT2, '@osmallint', output=True)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@osmallint'])
+        eq_(input, proc.parameters['@osmallint'])
 
     def testTinyInt(self):
         input = 101
         proc = self.mssql.init_procedure('pymssqlTestTinyInt')
         proc.bind(input, _mssql.SQLINT1, '@itinyint')
         proc.bind(None, _mssql.SQLINT1, '@otinyint', output=True)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@otinyint'])
+        eq_(input, proc.parameters['@otinyint'])
 
     def testUuid(self):
         if os.environ.get('FREETDS_VERSION') != '0.91':
-            pytest.skip("UNIQUEIDENTIFIER as a SP param doesn't work with FreeTDS >= 0.95")
+            pytest.xfail("UNIQUEIDENTIFIER as a SP param doesn't work with FreeTDS >= 0.95")
         import uuid
         input = uuid.uuid4()
         proc = self.mssql.init_procedure('pymssqlTestUniqueIdentifier')
         proc.bind(input, _mssql.SQLUUID, '@iuniqueidentifier')
         proc.bind(None, _mssql.SQLUUID, '@ouniqueidentifier', output=True)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@ouniqueidentifier'])
+        eq_(input, proc.parameters['@ouniqueidentifier'])
 
     def testReal(self):
         input = 3.14
         proc = self.mssql.init_procedure('pymssqlTestReal')
         proc.bind(input, _mssql.SQLREAL, '@ireal')
         proc.bind(None, _mssql.SQLREAL, '@oreal', output=True)
         proc.execute()
@@ -263,86 +234,15 @@
         proc = self.mssql.init_procedure('pymssqlTestFloat')
         proc.bind(input, _mssql.SQLFLT8, '@ifloat')
         proc.bind(None, _mssql.SQLFLT8, '@ofloat', output=True)
         proc.execute()
         assert abs(input - proc.parameters['@ofloat']) < 0.00001
 
 
-@pytest.mark.mssql_server_required
-class TestDataTimeConversion:
-
-    def test_date(self, mssql_conn, subtests):
-        with stored_proc(mssql_conn, 'date') as proc_name:
-            for input in (
-                datetime.date(1, 1, 1), # min supported
-                datetime.date(90, 8, 27), # GH #454
-                datetime.date(906, 8, 27), # GH #454
-                datetime.date(2009, 8, 27),
-                datetime.date(9999, 12, 31), # max supported
-                ):
-                with subtests.test(date=input):
-                    proc = mssql_conn.init_procedure(proc_name)
-                    proc.bind(input, _mssql.SQLDATE, '@inp')
-                    proc.bind(None, _mssql.SQLDATE, '@out', output=True)
-                    res = proc.execute()
-                    assert res == 0
-                    assert input == proc.parameters['@out']
-
-    def test_time(self, mssql_conn, subtests):
-        with stored_proc(mssql_conn, 'time') as proc_name:
-            for input in (
-                datetime.time(0, 0, 0), # min supported
-                datetime.time(23, 59, 59, 0),
-                datetime.time(23, 59, 59, 999999), # max supported
-                ):
-                with subtests.test(time=input):
-                    proc = mssql_conn.init_procedure(proc_name)
-                    proc.bind(input, _mssql.SQLTIME, '@inp')
-                    proc.bind(None, _mssql.SQLTIME, '@out', output=True)
-                    res = proc.execute()
-                    assert res == 0
-                    assert input == proc.parameters['@out']
-
-    def test_datetime(self, mssql_conn, subtests):
-        with stored_proc(mssql_conn, 'datetime') as proc_name:
-            for input in (
-                datetime.datetime(1753, 1, 1), # min supported
-                datetime.datetime(2009, 8, 27),
-                datetime.datetime(2009, 8, 27, 23, 59, 59, 997000),
-                datetime.datetime(9999, 12, 31, 23, 59, 59, 997000), # max supported
-                ):
-                with subtests.test(datetime=input):
-                    proc = mssql_conn.init_procedure(proc_name)
-                    proc.bind(input, _mssql.SQLDATETIME, '@inp')
-                    proc.bind(None, _mssql.SQLDATETIME, '@out', output=True)
-                    res = proc.execute()
-                    assert res == 0
-                    assert input == proc.parameters['@out']
-
-    def test_datetime2(self, mssql_conn, subtests):
-        with stored_proc(mssql_conn, 'datetime2') as proc_name:
-            for input in (
-                datetime.datetime(1, 1, 1), # min supported
-                datetime.datetime(90, 8, 27),
-                datetime.datetime(906, 8, 27),
-                datetime.datetime(2009, 8, 27),
-                datetime.datetime(2009, 8, 27, 23, 59, 59, 999999),
-                datetime.datetime(9999, 12, 31, 23, 59, 59, 999999), # max supported
-                ):
-                with subtests.test(datetime=input):
-                    proc = mssql_conn.init_procedure(proc_name)
-                    proc.bind(input, _mssql.SQLDATETIME2, '@inp')
-                    proc.bind(None, _mssql.SQLDATETIME2, '@out', output=True)
-                    res = proc.execute()
-                    assert res == 0
-                    assert input == proc.parameters['@out']
-
-
-
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestCallProcFancy(unittest.TestCase):
     # "Fancy" because we test some exotic cases like passing None or Unicode
     # strings to a called procedure
 
     def setUp(self):
         self.pymssql = pymssqlconn()
         cursor = self.pymssql.cursor()
@@ -352,16 +252,16 @@
         	@some_arg NVARCHAR(64)
         AS
         BEGIN
         	SELECT @some_arg + N'!',
                    N'%(str1)s ' + @some_arg + N' %(str2)s'
         END
         """ % {
-            'str1': 'Здравствуй',
-            'str2': 'Мир',
+            'str1': u'\u0417\u0434\u0440\u0430\u0432\u0441\u0442\u0432\u0443\u0439',
+            'str2': u'\u041c\u0438\u0440',
         }
         sql = sql.encode('utf-8')
 
         cursor.execute(sql)
 
     def tearDown(self):
         cursor = self.pymssql.cursor()
@@ -370,95 +270,120 @@
 
     def testCallProcWithNone(self):
         cursor = self.pymssql.cursor()
         cursor.callproc(
             'someProcWithOneParam',
             (None,))
 
-        a, b = cursor.fetchone()
-        self.assertEqual(a, None)
-        self.assertEqual(b, None)
+        # For some reason, fetchone doesn't work
+        # It raises "OperationalError: Statement not executed or executed statement has no resultset"
+        # a, b = cursor.fetchone()
+
+        for a, b in cursor:
+            eq_(a, None)
+            eq_(b, None)
 
     def testCallProcWithAsciiString(self):
         cursor = self.pymssql.cursor()
         cursor.callproc(
             'someProcWithOneParam',
             ('hello',))
 
-        a, b = cursor.fetchone()
-        self.assertEqual(a, 'hello!')
-        self.assertEqual(b, 'Здравствуй hello Мир')
+        # For some reason, fetchone doesn't work
+        # It raises "OperationalError: Statement not executed or executed statement has no resultset"
+        # a, b = cursor.fetchone()
+
+        for a, b in cursor:
+            eq_(a, 'hello!')
+            eq_(b, u'\u0417\u0434\u0440\u0430\u0432\u0441\u0442\u0432\u0443\u0439 hello \u041c\u0438\u0440')
 
     def testCallProcWithUnicodeStringWithNoFunnyCharacters(self):
         cursor = self.pymssql.cursor()
         cursor.callproc(
             'someProcWithOneParam',
-            ('hello',))
+            (u'hello',))
 
-        a, b = cursor.fetchone()
-        self.assertEqual(a, 'hello!')
-        self.assertEqual(b, 'Здравствуй hello Мир')
+        # For some reason, fetchone doesn't work
+        # It raises "OperationalError: Statement not executed or executed statement has no resultset"
+        # a, b = cursor.fetchone()
+
+        for a, b in cursor:
+            eq_(a, u'hello!')
+            eq_(b, u'\u0417\u0434\u0440\u0430\u0432\u0441\u0442\u0432\u0443\u0439 hello \u041c\u0438\u0440')
 
     # This is failing for me - the Unicode params somehow gets rendered to a
     # blank string. I am not sure if this is another bug or a user error on my
     # part...?
     #
     def testCallProcWithUnicodeStringWithRussianCharacters(self):
         cursor = self.pymssql.cursor()
         cursor.callproc(
             'someProcWithOneParam',
-            ('Здравствуй',))  # Russian string
+            (u'\u0417\u0434\u0440\u0430\u0432\u0441\u0442\u0432\u0443\u0439',))  # Russian string
 
-        a, b = cursor.fetchone()
-        self.assertEqual(a, 'Здравствуй!')
-        self.assertEqual(b, 'Здравствуй Здравствуй Мир')
+        # For some reason, fetchone doesn't work
+        # It raises "OperationalError: Statement not executed or executed statement has no resultset"
+        # a, b = cursor.fetchone()
+
+        # This test fails with FreeTDS 0.91 (and probably older versions)
+        # because they don't seem to encode the Unicode string properly.
+        # See http://code.google.com/p/pymssql/issues/detail?id=109
+        skip_test()
+
+        for a, b in cursor:
+            eq_(a, u'\u0417\u0434\u0440\u0430\u0432\u0441\u0442\u0432\u0443\u0439!')
+            eq_(b, u'\u0417\u0434\u0440\u0430\u0432\u0441\u0442\u0432\u0443\u0439 \u0417\u0434\u0440\u0430\u0432\u0441\u0442\u0432\u0443\u0439 \u041c\u0438\u0440')
 
     def testExecuteWithNone(self):
         cursor = self.pymssql.cursor()
         cursor.execute(
-            'someProcWithOneParam %s',
+            u'someProcWithOneParam %s',
             (None,))
 
         a, b = cursor.fetchone()
-        self.assertEqual(a, None)
-        self.assertEqual(b, None)
+
+        eq_(a, None)
+        eq_(b, None)
 
     def testExecuteWithAsciiString(self):
         cursor = self.pymssql.cursor()
         cursor.execute(
-            'someProcWithOneParam %s',
+            u'someProcWithOneParam %s',
             ('hello',))
 
         a, b = cursor.fetchone()
-        self.assertEqual(a, 'hello!')
-        self.assertEqual(b, 'Здравствуй hello Мир')
+
+        eq_(a, 'hello!')
+        eq_(b, u'\u0417\u0434\u0440\u0430\u0432\u0441\u0442\u0432\u0443\u0439 hello \u041c\u0438\u0440')
 
     def testExecuteWithUnicodeStringWithNoFunnyCharacters(self):
         cursor = self.pymssql.cursor()
         cursor.execute(
-            'someProcWithOneParam %s',
-            ('hello',))
+            u'someProcWithOneParam %s',
+            (u'hello',))
 
         a, b = cursor.fetchone()
-        self.assertEqual(a, 'hello!')
-        self.assertEqual(b, 'Здравствуй hello Мир')
+
+        eq_(a, u'hello!')
+        eq_(b, u'\u0417\u0434\u0440\u0430\u0432\u0441\u0442\u0432\u0443\u0439 hello \u041c\u0438\u0440')
 
     def testExecuteWithUnicodeWithRussianCharacters(self):
         cursor = self.pymssql.cursor()
         cursor.execute(
-            'someProcWithOneParam %s',
-            ('Здравствуй',))  # Russian string
+            u'someProcWithOneParam %s',
+            (u'\u0417\u0434\u0440\u0430\u0432\u0441\u0442\u0432\u0443\u0439',))  # Russian string
 
         a, b = cursor.fetchone()
-        self.assertEqual(a, 'Здравствуй!')
-        self.assertEqual(b, 'Здравствуй Здравствуй Мир')
+
+        eq_(a, u'\u0417\u0434\u0440\u0430\u0432\u0441\u0442\u0432\u0443\u0439!')
+        eq_(b, u'\u0417\u0434\u0440\u0430\u0432\u0441\u0442\u0432\u0443\u0439 \u0417\u0434\u0440\u0430\u0432\u0441\u0442\u0432\u0443\u0439 \u041c\u0438\u0440')
 
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestStringTypeConversion(unittest.TestCase):
 
     def setUp(self):
         self.mssql = mssqlconn()
 
         for name, size in VARIABLE_TYPES:
             dbtype = name.lower()
@@ -490,49 +415,57 @@
 
     def testChar(self):
         input = 'test'
         proc = self.mssql.init_procedure('pymssqlTestChar')
         proc.bind(input, _mssql.SQLCHAR, '@ichar')
         proc.bind(None, _mssql.SQLCHAR, '@ochar', output=True, max_length=4)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@ochar'])
+        eq_(input, proc.parameters['@ochar'])
 
     def testText(self):
         input = 'test'
         proc = self.mssql.init_procedure('pymssqlTestText')
         proc.bind(input, _mssql.SQLTEXT, '@itext')
         proc.bind(None, _mssql.SQLVARCHAR, '@otext', output=True)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@otext'])
+        eq_(input, proc.parameters['@otext'])
 
     def testVarChar(self):
         input = 'test'
         proc = self.mssql.init_procedure('pymssqlTestVarChar')
         proc.bind(input, _mssql.SQLVARCHAR, '@ivarchar')
         proc.bind(None, _mssql.SQLVARCHAR, '@ovarchar', output=True)
         proc.execute()
-        self.assertEqual(input, proc.parameters['@ovarchar'])
+        eq_(input, proc.parameters['@ovarchar'])
 
     def testVarBinary(self):
         def check_conversion(input, output_type):
             proc = self.mssql.init_procedure('pymssqlTestVarBinary')
             proc.bind(input, _mssql.SQLVARBINARY, '@ivarbinary')
             proc.bind(None, _mssql.SQLVARBINARY, '@ovarbinary', output=True)
             proc.execute()
-            self.assertEqual(input, proc.parameters['@ovarbinary'])
-            self.assertEqual(output_type, type(proc.parameters['@ovarbinary']))
+            eq_(input, proc.parameters['@ovarbinary'])
+            eq_(output_type, type(proc.parameters['@ovarbinary']))
 
-        check_conversion(bytes(b'\xDE\xAD\xBE\xEF'), bytes)
-        check_conversion(bytearray(b'\xDE\xAD\xBE\xEF'), bytes)
-        with pytest.raises(TypeError) as exc_info:
-            check_conversion('FOO', bytes)
-            assert 'value can only be bytes or bytearray' == str(exc_info.value)
+        if sys.version_info[0] == 3:
+            check_conversion(bytes(b'\xDE\xAD\xBE\xEF'), bytes)
+            check_conversion(bytearray(b'\xDE\xAD\xBE\xEF'), bytes)
+            with pytest.raises(TypeError) as exc_info:
+                check_conversion('FOO', bytes)
+                assert 'value can only be bytes or bytearray' == str(exc_info.value)
+        else:
+            check_conversion(b'\xDE\xAD\xBE\xEF', str)
+            check_conversion(bytes(b'\xDE\xAD\xBE\xEF'), str)
+            check_conversion(bytearray(b'\xDE\xAD\xBE\xEF'), str)
+            with pytest.raises(TypeError) as exc_info:
+                check_conversion(unicode('Foo'), str)
+                assert 'value can only be str or bytearray' == str(exc_info.value)
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestFloatTypeConversion(unittest.TestCase):
     def setUp(self):
         self.mssql = mssqlconn()
         self.pymssql = pymssqlconn()
         cursor = self.pymssql.cursor()
 
         self.mssql.execute_non_query("""
@@ -577,15 +510,15 @@
             'pymssqlFloatTest',
             (5.44451787074e+39,))
 
         # TODO: Use the solution we implement once #134 gets fixed
         a = next(cursor)
         assert abs(a[0] - 5.44451787074e+39) < 0.000001
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestErrorInSP(unittest.TestCase):
 
     def setUp(self):
         self.pymssql = pymssqlconn()
         cursor = self.pymssql.cursor()
 
         sql = u"""
@@ -620,15 +553,15 @@
         # Must be a DatabaseError exception
         try:
             cursor.callproc('SPThatRaisesAnError')
         except Exception as e:
             self.assertTrue(isinstance(e,  pymssql.DatabaseError))
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestSPWithQueryResult(unittest.TestCase):
 
     SP_NAME = 'SPWithAQuery'
 
     def setUp(self):
         self.mssql = mssqlconn()
         self.pymssql = pymssqlconn()
@@ -649,18 +582,22 @@
 
     def testPymssql(self):
         cursor = self.pymssql.cursor()
         cursor.callproc(
             self.SP_NAME,
             ('hello',))
 
-        a, b = cursor.fetchone()
-        self.assertEqual(a, 'hello!')
-        self.assertEqual(b, 'hello!!')
+        # For some reason, fetchone doesn't work
+        # It raises "OperationalError: Statement not executed or executed statement has no resultset"
+        #a, b = cursor.fetchone()
+
+        for a, b in cursor:
+            eq_(a, 'hello!')
+            eq_(b, 'hello!!')
 
     def test_mssql(self):
         proc = self.mssql.init_procedure(self.SP_NAME)
         proc.bind('hello', _mssql.SQLVARCHAR)
         proc.execute()
 
         for row_dict in self.mssql:
-            self.assertEqual(row_dict, {0: 'hello!', 1: 'hello!!'})
+            eq_(row_dict, {0: 'hello!', 1: 'hello!!'})
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_sqlalchemy.py` & `pymssgl-2.2.9.dev0/tests/test_sqlalchemy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf-8 -*-
 """
 Basic SQLAlchemy tests.
 """
 
 import unittest
 
-import pytest
-
-from .helpers import config, eq_
+from .helpers import config, eq_, skip_test, mssql_server_required
 
 try:
     import sqlalchemy as sa
 except ImportError:
-    pytest.skip('SQLAlchemy is not available', allow_module_level=True)
-from sqlalchemy.orm import sessionmaker, declarative_base
+    skip_test('SQLAlchemy is not available')
+from sqlalchemy.orm import sessionmaker
+from sqlalchemy.ext.declarative import declarative_base
 
 engine = sa.create_engine(
         'mssql+pymssql://%s:%s@%s:%s/%s' % (
             config.user,
             config.password,
             config.server,
             config.port,
@@ -39,15 +38,15 @@
     data = sa.Column(sa.PickleType)
 
 #saotbl = SAObj.__table__
 #
 #saotbl.drop(engine, checkfirst=True)
 #saotbl.create(engine)
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestSA(unittest.TestCase):
 
     def setUp(self):
         self.sess = Session()
         self.saotbl = SAObj.__table__
         self.saotbl.drop(engine, checkfirst=True)
         self.saotbl.create(engine)
@@ -66,10 +65,10 @@
         assert s.id
         assert self.sess.query(SAObj).count() == 1
 
     def test_pickle_type(self):
         s = SAObj(name='foobar', data=['one'])
         self.sess.add(s)
         self.sess.commit()
-        res = self.sess.execute(sa.select(self.saotbl.c.data))
+        res = self.sess.execute(sa.select([self.saotbl.c.data]))
         row = res.fetchone()
-        eq_(row[0], ['one'])
+        eq_(row['data'], ['one'])
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_threaded.py` & `pymssgl-2.2.9.dev0/tests/test_threaded.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 """
 
 import sys
 import threading
 import time
 import unittest
 
-import pytest
-
 from pymssql._mssql import MSSQLDatabaseException
 
-from .helpers import mssqlconn, StoredProc
+from .helpers import mssqlconn, StoredProc, mark_slow, mssql_server_required
 
 
 error_sproc = StoredProc(
     "pymssqlErrorThreadTest",
     args=(),
     body="SELECT unknown_column FROM unknown_table")
 
@@ -34,35 +32,35 @@
                     num = mssql.execute_scalar('SELECT %d', (i,))
                     assert num == i
                     self.results.append(num)
         except Exception as exc:
             self.exc = exc
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class _TestingErrorThread(_TestingThread):
     def run(self):
         try:
             with mssqlconn() as mssql:
                 mssql.execute_query('SELECT unknown_column')
         except Exception as exc:
             self.exc = exc
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class _SprocTestingErrorThread(_TestingThread):
     def run(self):
         try:
             with mssqlconn() as mssql:
                 error_sproc.execute(mssql=mssql)
         except Exception as exc:
             self.exc = exc
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class ThreadedTests(unittest.TestCase):
     def run_threads(self, num, thread_class):
         threads = [thread_class() for _ in range(num)]
         for thread in threads:
             thread.start()
 
         results = []
@@ -81,33 +79,33 @@
             time.sleep(5)
 
         sys.stdout.write(" ")
         sys.stdout.flush()
 
         return results, exceptions
 
-    @pytest.mark.slow
+    @mark_slow
     def testThreadedUse(self):
         results, exceptions = self.run_threads(
             num=50,
             thread_class=_TestingThread)
         self.assertEqual(len(exceptions), 0)
         for result in results:
             self.assertEqual(result, list(range(0, 1000)))
 
-    @pytest.mark.slow
+    @mark_slow
     def testErrorThreadedUse(self):
         results, exceptions = self.run_threads(
             num=2,
             thread_class=_TestingErrorThread)
         self.assertEqual(len(exceptions), 2)
         for exc in exceptions:
             self.assertEqual(type(exc), MSSQLDatabaseException)
 
-    @pytest.mark.slow
+    @mark_slow
     def testErrorSprocThreadedUse(self):
         with error_sproc.create():
             results, exceptions = self.run_threads(
                 num=5,
                 thread_class=_SprocTestingErrorThread)
         self.assertEqual(len(exceptions), 5)
         for exc in exceptions:
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_user_msghandler.py` & `pymssgl-2.2.9.dev0/tests/test_user_msghandler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Test user message hanler.
 """
 
 import unittest
 
-import pytest
-
-from .helpers import config, mssqlconn
+from .helpers import config, mssqlconn, mssql_server_required
 
 msgs = []
 
 
 def user_msg_handler1(msgstate, severity, srvname, procname, line, msgtext):
     global msgs
     procname = procname.decode('ascii')
@@ -30,15 +28,15 @@
     msgs.append(entry)
 
 
 def wrong_signature_msg_handler():
     pass
 
 
-@pytest.mark.mssql_server_required
+@mssql_server_required
 class TestUserMsgHandler(unittest.TestCase):
 
     def test_basic_functionality(self):
         cnx = mssqlconn()
         try:
             cnx.set_msghandler(user_msg_handler1)
             msgs_before = len(msgs)
```

### Comparing `pymssgl-2.2.8.dev28/tests/test_utils.py` & `pymssgl-2.2.9.dev0/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,38 +17,38 @@
     res = substitute_params(
         'SELECT * FROM empl WHERE name = %s',
         b'John Doe')
     eq_(res, b"SELECT * FROM empl WHERE name = 'John Doe'")
 
     res = substitute_params(
         'SELECT * FROM empl WHERE name = %s',
-        'John Doe')
+        u'John Doe')
     eq_(res, b"SELECT * FROM empl WHERE name = N'John Doe'")
 
 
 def test_param_quote():
     res = substitute_params(
         'SELECT * FROM empl WHERE name = %s',
         b"John's Doe")
     eq_(res, b"SELECT * FROM empl WHERE name = 'John''s Doe'")
 
     res = substitute_params(
         'SELECT * FROM empl WHERE name = %s',
-        "John's Doe")
+        u"John's Doe")
     eq_(res, b"SELECT * FROM empl WHERE name = N'John''s Doe'")
 
 
 def test_unicode_params():
     res = substitute_params(
-        'SELECT * FROM \u0394 WHERE name = %s',
-        '\u03A8'
+        u'SELECT * FROM \u0394 WHERE name = %s',
+        u'\u03A8'
     )
     eq_(res, b"SELECT * FROM \xce\x94 WHERE name = N'\xce\xa8'")
 
-    res = substitute_params(u"testing ascii (\u0105\u010D\u0119) 1=%d 'one'=%s", (1, 'str'))
+    res = substitute_params(u"testing ascii (\u0105\u010D\u0119) 1=%d 'one'=%s", (1, u'str'))
     eq_(res, b"testing ascii (\xc4\x85\xc4\x8d\xc4\x99) 1=1 'one'=N'str'")
 
 
 def test_single_param_with_d():
     res = substitute_params(
         'SELECT * FROM employees WHERE id = %d',
         13)
@@ -77,62 +77,62 @@
     res = substitute_params(
         'SELECT * FROM empl WHERE id IN %s',
         ((b'foo', b'bar'),))
     eq_(res, b"SELECT * FROM empl WHERE id IN ('foo','bar')")
 
     res = substitute_params(
         'SELECT * FROM empl WHERE id IN %s',
-        (('foo', 'bar'),))
+        ((u'foo', u'bar'),))
     eq_(res, b"SELECT * FROM empl WHERE id IN (N'foo',N'bar')")
 
     # single item
     res = substitute_params(
         'SELECT * FROM empl WHERE id IN %s',
         ((b'foo',),))
     eq_(res, b"SELECT * FROM empl WHERE id IN ('foo')")
 
     res = substitute_params(
         'SELECT * FROM empl WHERE id IN %s',
-        (('foo',),))
+        ((u'foo',),))
     eq_(res, b"SELECT * FROM empl WHERE id IN (N'foo')")
 
 
 def test_percent_in_param():
     res = substitute_params(
         'SELECT * FROM empl WHERE name LIKE %s',
         b'J%')
     eq_(res, b"SELECT * FROM empl WHERE name LIKE 'J%'")
 
     res = substitute_params(
         'SELECT * FROM empl WHERE name LIKE %s',
-        'J%')
+        u'J%')
     eq_(res, b"SELECT * FROM empl WHERE name LIKE N'J%'")
 
 
 def test_single_dict_params():
     res = substitute_params(
         'SELECT * FROM cust WHERE salesrep = %(name)s',
         {'name': b'John Doe'})
     eq_(res, b"SELECT * FROM cust WHERE salesrep = 'John Doe'")
 
     res = substitute_params(
         'SELECT * FROM cust WHERE salesrep = %(name)s',
-        {'name': 'John Doe'})
+        {'name': u'John Doe'})
     eq_(res, b"SELECT * FROM cust WHERE salesrep = N'John Doe'")
 
 
 def test_weird_key_names_dict_params():
     res = substitute_params(
         'SELECT * FROM cust WHERE salesrep = %(n %s ##ame)s',
         {'n %s ##ame': b'John Doe'})
     eq_(res, b"SELECT * FROM cust WHERE salesrep = 'John Doe'")
 
     res = substitute_params(
         'SELECT * FROM cust WHERE salesrep = %(n %s ##ame)s',
-        {'n %s ##ame': 'John Doe'})
+        {'n %s ##ame': u'John Doe'})
     eq_(res, b"SELECT * FROM cust WHERE salesrep = N'John Doe'")
 
 
 def test_multi_dict_params():
     res = substitute_params(
         'SELECT * FROM empl '
         'WHERE (name = %(name)s AND city = %(city)s) '
@@ -142,15 +142,15 @@
              b"WHERE (name = 'John Doe' AND city = 'Nowhere') "
              b"OR supervisor = 'John Doe'")
 
     res = substitute_params(
         'SELECT * FROM empl '
         'WHERE (name = %(name)s AND city = %(city)s) '
         'OR supervisor = %(name)s',
-        {'name': 'John Doe', 'city': 'Nowhere'})
+        {'name': u'John Doe', 'city': u'Nowhere'})
     eq_(res, b"SELECT * FROM empl "
              b"WHERE (name = N'John Doe' AND city = N'Nowhere') "
              b"OR supervisor = N'John Doe'")
 
 
 def test_single_and_tuple():
     res = substitute_params(
@@ -159,15 +159,15 @@
         (b'John Doe', (1, 2, 3)))
     eq_(res, b"SELECT * FROM cust "
              b"WHERE salesrep = 'John Doe' AND id IN (1,2,3)")
 
     res = substitute_params(
         'SELECT * FROM cust '
         'WHERE salesrep = %s AND id IN %s',
-        ('John Doe', (1, 2, 3)))
+        (u'John Doe', (1, 2, 3)))
     eq_(res, b"SELECT * FROM cust "
              b"WHERE salesrep = N'John Doe' AND id IN (1,2,3)")
 
 
 def test_bare_percent_position():
     res = substitute_params('select 5 % %s', 3)
     eq_(res, b"select 5 % 3")
```

### Comparing `pymssgl-2.2.8.dev28/tests/tests.cfg.tpl` & `pymssgl-2.2.9.dev0/tests/tests.cfg.tpl`

 * *Files identical despite different names*

