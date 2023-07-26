# Comparing `tmp/preset-cli-0.2.4.tar.gz` & `tmp/preset-cli-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preset-cli-0.2.4.tar", last modified: Thu Jul 20 16:14:06 2023, max compression
+gzip compressed data, was "preset-cli-0.2.5.tar", last modified: Wed Jul 26 21:25:08 2023, max compression
```

## Comparing `preset-cli-0.2.4.tar` & `preset-cli-0.2.5.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.496666 preset-cli-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.468665 preset-cli-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.484666 preset-cli-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.github/workflows/python-package-daily.yml
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-20 16:13:55.000000 preset-cli-0.2.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-07-20 16:13:55.000000 preset-cli-0.2.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-07-20 16:13:55.000000 preset-cli-0.2.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 16:13:55.000000 preset-cli-0.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-20 16:13:55.000000 preset-cli-0.2.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-07-20 16:14:06.496666 preset-cli-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24105 2023-07-20 16:13:55.000000 preset-cli-0.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-20 16:13:55.000000 preset-cli-0.2.4/dev-requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-20 16:13:55.000000 preset-cli-0.2.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.484666 preset-cli-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.484666 preset-cli-0.2.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.484666 preset-cli-0.2.4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   271378 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/images/export_dashboards.png
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.468665 preset-cli-0.2.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/examples/exports/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/examples/exports/charts/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-20 16:13:55.000000 preset-cli-0.2.4/examples/exports/charts/Total_count_134.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/examples/exports/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-20 16:13:55.000000 preset-cli-0.2.4/examples/exports/dashboards/White_label_test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/examples/exports/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-20 16:13:55.000000 preset-cli-0.2.4/examples/exports/databases/Google_Sheets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.468665 preset-cli-0.2.4/examples/exports/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/examples/exports/datasets/Google_Sheets/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-20 16:13:55.000000 preset-cli-0.2.4/examples/exports/datasets/Google_Sheets/country_cnt.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/examples/exports/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-20 16:13:55.000000 preset-cli-0.2.4/examples/exports/functions/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-20 16:13:55.000000 preset-cli-0.2.4/examples/exports/metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-20 16:13:55.000000 preset-cli-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 16:13:55.000000 preset-cli-0.2.4/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-20 16:13:55.000000 preset-cli-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-20 16:14:06.496666 preset-cli-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-20 16:13:55.000000 preset-cli-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.472666 preset-cli-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/src/preset_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/src/preset_cli/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/src/preset_cli/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/api/clients/dbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/api/clients/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)    37259 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/api/clients/superset.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/api/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/src/preset_cli/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/auth/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/auth/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/auth/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/auth/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/auth/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/src/preset_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/src/preset_cli/cli/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/exposures.py
--rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/native/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/src/preset_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-07-20 16:14:06.000000 preset-cli-0.2.4/src/preset_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-20 16:14:06.000000 preset-cli-0.2.4/src/preset_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:14:06.000000 preset-cli-0.2.4/src/preset_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-20 16:14:06.000000 preset-cli-0.2.4/src/preset_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:14:06.000000 preset-cli-0.2.4/src/preset_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-20 16:14:06.000000 preset-cli-0.2.4/src/preset_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 16:14:06.000000 preset-cli-0.2.4/src/preset_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/tests/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53266 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/api/clients/dbt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/api/clients/preset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    95330 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/api/clients/superset_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.496666 preset-cli-0.2.4/tests/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/auth/jwt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/auth/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/auth/main_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/auth/password_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/auth/preset_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.496666 preset-cli-0.2.4/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52383 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.496666 preset-cli-0.2.4/tests/cli/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/export_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/import_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/main_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sql_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.496666 preset-cli-0.2.4/tests/cli/superset/sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.496666 preset-cli-0.2.4/tests/cli/superset/sync/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/databases_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34788 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28144 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/exposures_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/metrics_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.496666 preset-cli-0.2.4/tests/cli/superset/sync/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26997 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/native/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.651804 preset-cli-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-26 21:24:56.000000 preset-cli-0.2.5/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-26 21:24:56.000000 preset-cli-0.2.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.631803 preset-cli-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.639803 preset-cli-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-26 21:24:56.000000 preset-cli-0.2.5/.github/workflows/python-package-daily.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-26 21:24:56.000000 preset-cli-0.2.5/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-26 21:24:56.000000 preset-cli-0.2.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-26 21:24:56.000000 preset-cli-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 21:24:56.000000 preset-cli-0.2.5/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-26 21:24:56.000000 preset-cli-0.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-26 21:24:56.000000 preset-cli-0.2.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-26 21:24:56.000000 preset-cli-0.2.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-26 21:24:56.000000 preset-cli-0.2.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-07-26 21:24:56.000000 preset-cli-0.2.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-07-26 21:24:56.000000 preset-cli-0.2.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-26 21:24:56.000000 preset-cli-0.2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-26 21:24:56.000000 preset-cli-0.2.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-07-26 21:25:08.651804 preset-cli-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24105 2023-07-26 21:24:56.000000 preset-cli-0.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 21:24:56.000000 preset-cli-0.2.5/dev-requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-26 21:24:56.000000 preset-cli-0.2.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.639803 preset-cli-0.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-26 21:24:56.000000 preset-cli-0.2.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.639803 preset-cli-0.2.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 21:24:56.000000 preset-cli-0.2.5/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 21:24:56.000000 preset-cli-0.2.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 21:24:56.000000 preset-cli-0.2.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-26 21:24:56.000000 preset-cli-0.2.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 21:24:56.000000 preset-cli-0.2.5/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.639803 preset-cli-0.2.5/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   271378 2023-07-26 21:24:56.000000 preset-cli-0.2.5/docs/images/export_dashboards.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-26 21:24:56.000000 preset-cli-0.2.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-26 21:24:56.000000 preset-cli-0.2.5/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-26 21:24:56.000000 preset-cli-0.2.5/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-26 21:24:56.000000 preset-cli-0.2.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.635803 preset-cli-0.2.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.639803 preset-cli-0.2.5/examples/exports/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.639803 preset-cli-0.2.5/examples/exports/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-26 21:24:56.000000 preset-cli-0.2.5/examples/exports/charts/Total_count_134.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.639803 preset-cli-0.2.5/examples/exports/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-26 21:24:56.000000 preset-cli-0.2.5/examples/exports/dashboards/White_label_test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.639803 preset-cli-0.2.5/examples/exports/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-26 21:24:56.000000 preset-cli-0.2.5/examples/exports/databases/Google_Sheets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.635803 preset-cli-0.2.5/examples/exports/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.639803 preset-cli-0.2.5/examples/exports/datasets/Google_Sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-26 21:24:56.000000 preset-cli-0.2.5/examples/exports/datasets/Google_Sheets/country_cnt.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.639803 preset-cli-0.2.5/examples/exports/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-26 21:24:56.000000 preset-cli-0.2.5/examples/exports/functions/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-26 21:24:56.000000 preset-cli-0.2.5/examples/exports/metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-26 21:24:56.000000 preset-cli-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 21:24:56.000000 preset-cli-0.2.5/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-26 21:24:56.000000 preset-cli-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-26 21:25:08.651804 preset-cli-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-26 21:24:56.000000 preset-cli-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.635803 preset-cli-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.639803 preset-cli-0.2.5/src/preset_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.643803 preset-cli-0.2.5/src/preset_cli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.643803 preset-cli-0.2.5/src/preset_cli/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21072 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/api/clients/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/api/clients/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37259 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/api/clients/superset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/api/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.643803 preset-cli-0.2.5/src/preset_cli/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/auth/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/auth/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/auth/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/auth/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/auth/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.643803 preset-cli-0.2.5/src/preset_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.643803 preset-cli-0.2.5/src/preset_cli/cli/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.643803 preset-cli-0.2.5/src/preset_cli/cli/superset/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.647803 preset-cli-0.2.5/src/preset_cli/cli/superset/sync/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/sync/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/sync/dbt/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/sync/dbt/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/sync/dbt/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/sync/dbt/exposures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/sync/dbt/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/sync/dbt/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/sync/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.647803 preset-cli-0.2.5/src/preset_cli/cli/superset/sync/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/sync/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/cli/superset/sync/native/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-26 21:24:56.000000 preset-cli-0.2.5/src/preset_cli/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.643803 preset-cli-0.2.5/src/preset_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-07-26 21:25:08.000000 preset-cli-0.2.5/src/preset_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-26 21:25:08.000000 preset-cli-0.2.5/src/preset_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:25:08.000000 preset-cli-0.2.5/src/preset_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-26 21:25:08.000000 preset-cli-0.2.5/src/preset_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:25:08.000000 preset-cli-0.2.5/src/preset_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-26 21:25:08.000000 preset-cli-0.2.5/src/preset_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 21:25:08.000000 preset-cli-0.2.5/src/preset_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.647803 preset-cli-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.647803 preset-cli-0.2.5/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.647803 preset-cli-0.2.5/tests/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53266 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/api/clients/dbt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/api/clients/preset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95330 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/api/clients/superset_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.647803 preset-cli-0.2.5/tests/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/auth/jwt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/auth/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/auth/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/auth/password_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/auth/preset_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.647803 preset-cli-0.2.5/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52383 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.647803 preset-cli-0.2.5/tests/cli/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/export_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/import_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/sql_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.647803 preset-cli-0.2.5/tests/cli/superset/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.651804 preset-cli-0.2.5/tests/cli/superset/sync/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/sync/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/sync/dbt/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/sync/dbt/databases_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34788 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/sync/dbt/datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28144 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/sync/dbt/exposures_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/sync/dbt/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/sync/dbt/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/sync/dbt/metrics_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:25:08.651804 preset-cli-0.2.5/tests/cli/superset/sync/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/sync/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26997 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/cli/superset/sync/native/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tests/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-26 21:24:56.000000 preset-cli-0.2.5/tox.ini
```

### Comparing `preset-cli-0.2.4/.coveragerc` & `preset-cli-0.2.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/.github/workflows/python-package-daily.yml` & `preset-cli-0.2.5/.github/workflows/python-package-daily.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/.github/workflows/python-package.yml` & `preset-cli-0.2.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/.github/workflows/python-publish.yml` & `preset-cli-0.2.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/.gitignore` & `preset-cli-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/.pre-commit-config.yaml` & `preset-cli-0.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/CHANGELOG.rst` & `preset-cli-0.2.5/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/CONTRIBUTING.rst` & `preset-cli-0.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/Makefile` & `preset-cli-0.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/PKG-INFO` & `preset-cli-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preset-cli
-Version: 0.2.4
+Version: 0.2.5
 Summary: A CLI to interact with Preset (https://preset.io/) workspaces.
 Home-page: https://github.com/preset-io/backend-sdk
 Author: Beto Dealmeida
 Author-email: beto@preset.io
 License: Other/Proprietary License
 Project-URL: Documentation, https://github.com/preset-io/backend-sdk/blob/master/README.rst
 Platform: any
```

### Comparing `preset-cli-0.2.4/README.rst` & `preset-cli-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/dev-requirements.txt` & `preset-cli-0.2.5/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/docs/Makefile` & `preset-cli-0.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/docs/conf.py` & `preset-cli-0.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/docs/images/export_dashboards.png` & `preset-cli-0.2.5/docs/images/export_dashboards.png`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/docs/index.rst` & `preset-cli-0.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/examples/exports/charts/Total_count_134.yaml` & `preset-cli-0.2.5/examples/exports/charts/Total_count_134.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/examples/exports/dashboards/White_label_test.yaml` & `preset-cli-0.2.5/examples/exports/dashboards/White_label_test.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/examples/exports/datasets/Google_Sheets/country_cnt.yaml` & `preset-cli-0.2.5/examples/exports/datasets/Google_Sheets/country_cnt.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/requirements.txt` & `preset-cli-0.2.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/setup.cfg` & `preset-cli-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/setup.py` & `preset-cli-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/api/clients/dbt.py` & `preset-cli-0.2.5/src/preset_cli/api/clients/dbt.py`

 * *Files 4% similar despite different names*

```diff
@@ -313,15 +313,15 @@
 
 
 class ConnectionSchema(PostelSchema):
     """
     Schema for connection information.
     """
 
-    id = fields.Integer()
+    id = fields.Integer(allow_none=True)
     account_id = fields.Integer()
     project_id = fields.Integer()
     name = fields.String()
     type = PostelEnumField(ConnectionType)
     state = fields.Integer()
     created_by_id = fields.Integer(allow_none=True)
     created_by_service_token_id = fields.Integer(allow_none=True)
@@ -354,62 +354,65 @@
 
 
 class RepositorySchema(PostelSchema):
     """
     Schema for a repository.
     """
 
-    id = fields.Integer()
+    id = fields.Integer(allow_none=True)
     account_id = fields.Integer()
-    remote_url = fields.String()
+    remote_url = fields.String(allow_none=True)
     remote_backend = fields.String(allow_none=True)
     git_clone_strategy = PostelEnumField(GitCloneStrategy)
-    deploy_key_id = fields.Integer()
+    deploy_key_id = fields.Integer(allow_none=True)
     github_installation_id = fields.Integer(allow_none=True)
     state = fields.Integer()
     created_at = fields.DateTime()
     updated_at = fields.DateTime()
 
     # not present in the spec
     full_name = fields.String(allow_none=True)
     repository_credentials_id = fields.Integer(allow_none=True)
     gitlab = fields.String(allow_none=True)
     name = fields.String()
     pull_request_url_template = fields.String(allow_none=True)
     git_provider_id = fields.Integer(allow_none=True)
     git_provider = fields.String(allow_none=True)
-    project_id = fields.Integer()
+    project_id = fields.Integer(allow_none=True)
     deploy_key = fields.Nested(DeployKeySchema)
     github_repo = fields.String(allow_none=True)
 
 
 class ProjectSchema(PostelSchema):
     """
     Schema for a dbt project.
     """
 
-    id = fields.Integer()
+    id = fields.Integer(allow_none=True)
     account_id = fields.Integer()
-    connection = fields.Nested(ConnectionSchema)
-    connection_id = fields.Integer()
+    connection = fields.Nested(ConnectionSchema, allow_none=True)
+    connection_id = fields.Integer(allow_none=True)
     dbt_project_subdirectory = fields.String(allow_none=True)
     name = fields.String()
-    repository = fields.Nested(RepositorySchema)
-    repository_id = fields.Integer()
+    repository = fields.Nested(RepositorySchema, allow_none=True)
+    repository_id = fields.Integer(allow_none=True)
     state = fields.Integer()
-    created_at = fields.DateTime()
-    updated_at = fields.DateTime()
+    created_at = fields.DateTime(allow_none=True)
+    updated_at = fields.DateTime(allow_none=True)
 
     # not present in the spec
-    group_permissions = fields.List(fields.Nested(GroupPermissionSchema))
+    group_permissions = fields.List(
+        fields.Nested(GroupPermissionSchema),
+        allow_none=True,
+    )
     docs_job = fields.Nested("JobSchema", allow_none=True)
     docs_job_id = fields.Integer(allow_none=True)
     freshness_job_id = fields.Integer(allow_none=True)
     freshness_job = fields.Nested("JobSchema", allow_none=True)
-    skipped_setup = fields.Boolean()
+    skipped_setup = fields.Boolean(allow_none=True)
 
 
 class TriggerSchema(PostelSchema):
     """
     Schema for a job trigger.
     """
 
@@ -521,15 +524,15 @@
     schedule = fields.Nested(ScheduleSchema)
 
     # not present in the spec
     lifecycle_webhooks_url = fields.String(allow_none=True)
     cron_humanized = fields.String()
     created_at = fields.DateTime()
     next_run = fields.DateTime(allow_none=True)
-    lifecycle_webhooks = fields.Boolean()
+    lifecycle_webhooks = fields.Boolean(allow_none=True)
     next_run_humanized = fields.String(allow_none=True)
     deferring_job_definition_id = fields.Integer(allow_none=True)
     deactivated = fields.Boolean()
     is_deferrable = fields.Boolean()
     updated_at = fields.DateTime()
     execution = fields.Nested(ExecutionSchema)
     run_failure_count = fields.Integer()
```

### Comparing `preset-cli-0.2.4/src/preset_cli/api/clients/preset.py` & `preset-cli-0.2.5/src/preset_cli/api/clients/preset.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/api/clients/superset.py` & `preset-cli-0.2.5/src/preset_cli/api/clients/superset.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/auth/jwt.py` & `preset-cli-0.2.5/src/preset_cli/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/auth/lib.py` & `preset-cli-0.2.5/src/preset_cli/auth/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/auth/main.py` & `preset-cli-0.2.5/src/preset_cli/auth/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/auth/password.py` & `preset-cli-0.2.5/src/preset_cli/auth/password.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/auth/preset.py` & `preset-cli-0.2.5/src/preset_cli/auth/preset.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/cli/main.py` & `preset-cli-0.2.5/src/preset_cli/cli/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/cli/superset/export.py` & `preset-cli-0.2.5/src/preset_cli/cli/superset/export.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/cli/superset/import_.py` & `preset-cli-0.2.5/src/preset_cli/cli/superset/import_.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/cli/superset/main.py` & `preset-cli-0.2.5/src/preset_cli/cli/superset/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/cli/superset/sql.py` & `preset-cli-0.2.5/src/preset_cli/cli/superset/sql.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/command.py` & `preset-cli-0.2.5/src/preset_cli/cli/superset/sync/dbt/command.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/databases.py` & `preset-cli-0.2.5/src/preset_cli/cli/superset/sync/dbt/databases.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/datasets.py` & `preset-cli-0.2.5/src/preset_cli/cli/superset/sync/dbt/datasets.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/exposures.py` & `preset-cli-0.2.5/src/preset_cli/cli/superset/sync/dbt/exposures.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/lib.py` & `preset-cli-0.2.5/src/preset_cli/cli/superset/sync/dbt/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/metrics.py` & `preset-cli-0.2.5/src/preset_cli/cli/superset/sync/dbt/metrics.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/cli/superset/sync/native/command.py` & `preset-cli-0.2.5/src/preset_cli/cli/superset/sync/native/command.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/exceptions.py` & `preset-cli-0.2.5/src/preset_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli/lib.py` & `preset-cli-0.2.5/src/preset_cli/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli.egg-info/PKG-INFO` & `preset-cli-0.2.5/src/preset_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preset-cli
-Version: 0.2.4
+Version: 0.2.5
 Summary: A CLI to interact with Preset (https://preset.io/) workspaces.
 Home-page: https://github.com/preset-io/backend-sdk
 Author: Beto Dealmeida
 Author-email: beto@preset.io
 License: Other/Proprietary License
 Project-URL: Documentation, https://github.com/preset-io/backend-sdk/blob/master/README.rst
 Platform: any
```

### Comparing `preset-cli-0.2.4/src/preset_cli.egg-info/SOURCES.txt` & `preset-cli-0.2.5/src/preset_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/src/preset_cli.egg-info/requires.txt` & `preset-cli-0.2.5/src/preset_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/api/clients/dbt_test.py` & `preset-cli-0.2.5/tests/api/clients/dbt_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/api/clients/preset_test.py` & `preset-cli-0.2.5/tests/api/clients/preset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/api/clients/superset_test.py` & `preset-cli-0.2.5/tests/api/clients/superset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/auth/jwt_test.py` & `preset-cli-0.2.5/tests/auth/jwt_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/auth/lib_test.py` & `preset-cli-0.2.5/tests/auth/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/auth/main_test.py` & `preset-cli-0.2.5/tests/auth/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/auth/password_test.py` & `preset-cli-0.2.5/tests/auth/password_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/auth/preset_test.py` & `preset-cli-0.2.5/tests/auth/preset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/cli/main_test.py` & `preset-cli-0.2.5/tests/cli/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/cli/superset/export_test.py` & `preset-cli-0.2.5/tests/cli/superset/export_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/cli/superset/import_test.py` & `preset-cli-0.2.5/tests/cli/superset/import_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/cli/superset/main_test.py` & `preset-cli-0.2.5/tests/cli/superset/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/cli/superset/sql_test.py` & `preset-cli-0.2.5/tests/cli/superset/sql_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/cli/superset/sync/dbt/command_test.py` & `preset-cli-0.2.5/tests/cli/superset/sync/dbt/command_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/cli/superset/sync/dbt/databases_test.py` & `preset-cli-0.2.5/tests/cli/superset/sync/dbt/databases_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/cli/superset/sync/dbt/datasets_test.py` & `preset-cli-0.2.5/tests/cli/superset/sync/dbt/datasets_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/cli/superset/sync/dbt/exposures_test.py` & `preset-cli-0.2.5/tests/cli/superset/sync/dbt/exposures_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/cli/superset/sync/dbt/lib_test.py` & `preset-cli-0.2.5/tests/cli/superset/sync/dbt/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/cli/superset/sync/dbt/manifest.json` & `preset-cli-0.2.5/tests/cli/superset/sync/dbt/manifest.json`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/cli/superset/sync/dbt/metrics_test.py` & `preset-cli-0.2.5/tests/cli/superset/sync/dbt/metrics_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/cli/superset/sync/native/command_test.py` & `preset-cli-0.2.5/tests/cli/superset/sync/native/command_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tests/lib_test.py` & `preset-cli-0.2.5/tests/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.4/tox.ini` & `preset-cli-0.2.5/tox.ini`

 * *Files identical despite different names*

