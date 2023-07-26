# Comparing `tmp/swh.scrubber-2.0.1.tar.gz` & `tmp/swh.scrubber-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.scrubber-2.0.1.tar", last modified: Wed Jul 26 09:00:08 2023, max compression
+gzip compressed data, was "swh.scrubber-2.0.2.tar", last modified: Wed Jul 26 13:28:08 2023, max compression
```

## Comparing `swh.scrubber-2.0.1.tar` & `swh.scrubber-2.0.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 09:00:08.365483 swh.scrubber-2.0.1/
--rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)     1039 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      149 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     3822 2023-07-26 09:00:08.365483 swh.scrubber-2.0.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     2901 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/README.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 09:00:08.361483 swh.scrubber-2.0.1/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     2901 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 09:00:08.361483 swh.scrubber-2.0.1/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 09:00:08.361483 swh.scrubber-2.0.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)      156 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      246 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      413 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      222 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       75 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      261 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-07-26 09:00:08.365483 swh.scrubber-2.0.1/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2454 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 09:00:08.361483 swh.scrubber-2.0.1/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 09:00:08.365483 swh.scrubber-2.0.1/swh/scrubber/
--rw-r--r--   0 jenkins    (115) docker     (999)      727 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12162 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)    27791 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/db.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7601 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/fixer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2764 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/journal_checker.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3052 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/origin_locator.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/py.typed
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 09:00:08.365483 swh.scrubber-2.0.1/swh/scrubber/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)      201 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/sql/20-enums.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5735 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3081 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/sql/60-indexes.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 09:00:08.365483 swh.scrubber-2.0.1/swh/scrubber/sql/upgrades/
--rw-r--r--   0 jenkins    (115) docker     (999)      942 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/sql/upgrades/2.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2338 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/sql/upgrades/3.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      989 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/sql/upgrades/4.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1567 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/sql/upgrades/5.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2524 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/sql/upgrades/6.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    16136 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/storage_checker.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 09:00:08.365483 swh.scrubber-2.0.1/swh/scrubber/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1329 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/tests/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)    14835 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/tests/storage_checker_tests.py
--rw-r--r--   0 jenkins    (115) docker     (999)    15808 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8262 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/tests/test_db.py
--rw-r--r--   0 jenkins    (115) docker     (999)    11471 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/tests/test_fixer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1053 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/tests/test_init.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3913 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/tests/test_journal_kafka.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5408 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/tests/test_origin_locator.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1035 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/tests/test_storage_cassandra.py
--rw-r--r--   0 jenkins    (115) docker     (999)      780 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/tests/test_storage_postgresql.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1671 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/swh/scrubber/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 09:00:08.361483 swh.scrubber-2.0.1/swh.scrubber.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     3822 2023-07-26 09:00:08.000000 swh.scrubber-2.0.1/swh.scrubber.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1531 2023-07-26 09:00:08.000000 swh.scrubber-2.0.1/swh.scrubber.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-07-26 09:00:08.000000 swh.scrubber-2.0.1/swh.scrubber.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       50 2023-07-26 09:00:08.000000 swh.scrubber-2.0.1/swh.scrubber.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      219 2023-07-26 09:00:08.000000 swh.scrubber-2.0.1/swh.scrubber.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-07-26 09:00:08.000000 swh.scrubber-2.0.1/swh.scrubber.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1550 2023-07-26 09:00:02.000000 swh.scrubber-2.0.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 13:28:08.836970 swh.scrubber-2.0.2/
+-rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      134 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)     1039 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      149 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     3822 2023-07-26 13:28:08.836970 swh.scrubber-2.0.2/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     2901 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/README.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 13:28:08.832970 swh.scrubber-2.0.2/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     2901 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 13:28:08.832970 swh.scrubber-2.0.2/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 13:28:08.832970 swh.scrubber-2.0.2/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)      156 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      246 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      413 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      222 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       75 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      261 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-07-26 13:28:08.836970 swh.scrubber-2.0.2/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2454 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 13:28:08.832970 swh.scrubber-2.0.2/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 13:28:08.836970 swh.scrubber-2.0.2/swh/scrubber/
+-rw-r--r--   0 jenkins    (115) docker     (999)      727 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12167 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    27791 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/db.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7601 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/fixer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2764 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/journal_checker.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3052 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/origin_locator.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/py.typed
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 13:28:08.836970 swh.scrubber-2.0.2/swh/scrubber/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)      201 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/sql/20-enums.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5735 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3081 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/sql/60-indexes.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 13:28:08.836970 swh.scrubber-2.0.2/swh/scrubber/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) docker     (999)      942 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/sql/upgrades/2.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2338 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/sql/upgrades/3.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      989 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/sql/upgrades/4.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1567 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/sql/upgrades/5.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2524 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/sql/upgrades/6.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    16136 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/storage_checker.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 13:28:08.836970 swh.scrubber-2.0.2/swh/scrubber/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1329 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/tests/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    14835 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/tests/storage_checker_tests.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    16129 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8262 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/tests/test_db.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    11471 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/tests/test_fixer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1053 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3913 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/tests/test_journal_kafka.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5408 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/tests/test_origin_locator.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1035 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/tests/test_storage_cassandra.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      780 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/tests/test_storage_postgresql.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1671 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/swh/scrubber/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-26 13:28:08.832970 swh.scrubber-2.0.2/swh.scrubber.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3822 2023-07-26 13:28:08.000000 swh.scrubber-2.0.2/swh.scrubber.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1531 2023-07-26 13:28:08.000000 swh.scrubber-2.0.2/swh.scrubber.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-07-26 13:28:08.000000 swh.scrubber-2.0.2/swh.scrubber.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       50 2023-07-26 13:28:08.000000 swh.scrubber-2.0.2/swh.scrubber.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      219 2023-07-26 13:28:08.000000 swh.scrubber-2.0.2/swh.scrubber.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-07-26 13:28:08.000000 swh.scrubber-2.0.2/swh.scrubber.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1550 2023-07-26 13:28:01.000000 swh.scrubber-2.0.2/tox.ini
```

### Comparing `swh.scrubber-2.0.1/.pre-commit-config.yaml` & `swh.scrubber-2.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/CODE_OF_CONDUCT.md` & `swh.scrubber-2.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/LICENSE` & `swh.scrubber-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/PKG-INFO` & `swh.scrubber-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.scrubber
-Version: 2.0.1
+Version: 2.0.2
 Summary: Software Heritage Datastore Scrubber
 Home-page: https://forge.softwareheritage.org/diffusion/swh-scrubber
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-scrubber
```

### Comparing `swh.scrubber-2.0.1/README.rst` & `swh.scrubber-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/docs/README.rst` & `swh.scrubber-2.0.2/docs/README.rst`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/setup.py` & `swh.scrubber-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/__init__.py` & `swh.scrubber-2.0.2/swh/scrubber/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/cli.py` & `swh.scrubber-2.0.2/swh/scrubber/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022  The Software Heritage developers
+# Copyright (C) 2022-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import os
 from typing import Optional
 import warnings
@@ -311,15 +311,15 @@
 
     from .storage_checker import StorageChecker
 
     if name and config_id is None:
         config_id = db.config_get_by_name(name)
 
     if config_id is None:
-        raise click.ClickExceptino("A valid configuration name/id must be set")
+        raise click.ClickException("A valid configuration name/id must be set")
     checker = StorageChecker(
         db=ctx.obj["db"],
         storage=get_storage(**conf["storage"]),
         config_id=config_id,
         limit=limit,
     )
```

### Comparing `swh.scrubber-2.0.1/swh/scrubber/db.py` & `swh.scrubber-2.0.2/swh/scrubber/db.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/fixer.py` & `swh.scrubber-2.0.2/swh/scrubber/fixer.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/journal_checker.py` & `swh.scrubber-2.0.2/swh/scrubber/journal_checker.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/origin_locator.py` & `swh.scrubber-2.0.2/swh/scrubber/origin_locator.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/sql/30-schema.sql` & `swh.scrubber-2.0.2/swh/scrubber/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/sql/60-indexes.sql` & `swh.scrubber-2.0.2/swh/scrubber/sql/60-indexes.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/sql/upgrades/2.sql` & `swh.scrubber-2.0.2/swh/scrubber/sql/upgrades/2.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/sql/upgrades/3.sql` & `swh.scrubber-2.0.2/swh/scrubber/sql/upgrades/3.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/sql/upgrades/4.sql` & `swh.scrubber-2.0.2/swh/scrubber/sql/upgrades/4.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/sql/upgrades/5.sql` & `swh.scrubber-2.0.2/swh/scrubber/sql/upgrades/5.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/sql/upgrades/6.sql` & `swh.scrubber-2.0.2/swh/scrubber/sql/upgrades/6.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/storage_checker.py` & `swh.scrubber-2.0.2/swh/scrubber/storage_checker.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/tests/conftest.py` & `swh.scrubber-2.0.2/swh/scrubber/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/tests/storage_checker_tests.py` & `swh.scrubber-2.0.2/swh/scrubber/tests/storage_checker_tests.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/tests/test_cli.py` & `swh.scrubber-2.0.2/swh/scrubber/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,21 @@
     result = invoke(
         scrubber_db, ["check", "storage", "--config-id", "1"], storage=swh_storage
     )
     assert result.exit_code == 0, result.output
     assert result.output == ""
 
 
+def test_check_storage_ko(mocker, scrubber_db, swh_storage):
+    # using the config id instead of the config name
+    result = invoke(scrubber_db, ["check", "storage"], storage=swh_storage)
+    assert result.exit_code == 1, result.output
+    assert result.output == "Error: A valid configuration name/id must be set\n"
+
+
 def test_check_list(mocker, scrubber_db, swh_storage):
     mocker.patch("swh.scrubber.get_scrubber_db", return_value=scrubber_db)
     result = invoke(scrubber_db, ["check", "list"], storage=swh_storage)
     assert result.exit_code == 0, result.output
     assert result.output == ""
     with swh_storage.db() as db:
         dsn = db.conn.dsn
```

### Comparing `swh.scrubber-2.0.1/swh/scrubber/tests/test_db.py` & `swh.scrubber-2.0.2/swh/scrubber/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/tests/test_fixer.py` & `swh.scrubber-2.0.2/swh/scrubber/tests/test_fixer.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/tests/test_init.py` & `swh.scrubber-2.0.2/swh/scrubber/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/tests/test_journal_kafka.py` & `swh.scrubber-2.0.2/swh/scrubber/tests/test_journal_kafka.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/tests/test_origin_locator.py` & `swh.scrubber-2.0.2/swh/scrubber/tests/test_origin_locator.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/tests/test_storage_cassandra.py` & `swh.scrubber-2.0.2/swh/scrubber/tests/test_storage_cassandra.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/tests/test_storage_postgresql.py` & `swh.scrubber-2.0.2/swh/scrubber/tests/test_storage_postgresql.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh/scrubber/utils.py` & `swh.scrubber-2.0.2/swh/scrubber/utils.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/swh.scrubber.egg-info/PKG-INFO` & `swh.scrubber-2.0.2/swh.scrubber.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.scrubber
-Version: 2.0.1
+Version: 2.0.2
 Summary: Software Heritage Datastore Scrubber
 Home-page: https://forge.softwareheritage.org/diffusion/swh-scrubber
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-scrubber
```

### Comparing `swh.scrubber-2.0.1/swh.scrubber.egg-info/SOURCES.txt` & `swh.scrubber-2.0.2/swh.scrubber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.scrubber-2.0.1/tox.ini` & `swh.scrubber-2.0.2/tox.ini`

 * *Files identical despite different names*

