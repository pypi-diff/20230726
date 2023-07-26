# Comparing `tmp/invenio-config-tuw-2023.2.4.tar.gz` & `tmp/invenio-config-tuw-2023.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-config-tuw-2023.2.4.tar", last modified: Fri May 26 12:35:41 2023, max compression
+gzip compressed data, was "invenio-config-tuw-2023.2.5.tar", last modified: Wed Jul 26 20:36:33 2023, max compression
```

## Comparing `invenio-config-tuw-2023.2.4.tar` & `invenio-config-tuw-2023.2.5.tar`

### file list

```diff
@@ -1,62 +1,67 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.839966 invenio-config-tuw-2023.2.4/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/.dockerignore
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      628 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/.editorconfig
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/.git-blame-ignore-revs
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.823966 invenio-config-tuw-2023.2.4/.tx/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1056 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/.tx/config
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      332 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/AUTHORS.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2505 2023-05-26 12:35:34.000000 invenio-config-tuw-2023.2.4/CHANGES.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3392 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/CONTRIBUTING.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      139 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/INSTALL.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/LICENSE
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1033 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/MANIFEST.in
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5442 2023-05-26 12:35:41.839966 invenio-config-tuw-2023.2.4/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1960 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.4/README.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      536 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/babel.ini
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.827966 invenio-config-tuw-2023.2.4/docs/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7457 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/Makefile
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      278 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/api.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/authors.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/changes.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10226 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/docs/conf.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      290 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/configuration.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      239 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/contributing.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      817 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/index.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/installation.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/license.rst
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7005 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/make.bat
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/requirements.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/docs/usage.rst
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.831966 invenio-config-tuw-2023.2.4/invenio_config_tuw/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      408 2023-05-26 12:35:34.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/__init__.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.835966 invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      540 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1006 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8845 2023-05-17 17:46:20.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/handlers.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2540 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/utils.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7792 2023-05-26 10:08:47.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/config.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2623 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/ext.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1337 2023-05-26 12:35:34.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/formatters.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3937 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/forms.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.835966 invenio-config-tuw-2023.2.4/invenio_config_tuw/permissions/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      780 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/permissions/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3170 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/permissions/generators.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11136 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/permissions/policies.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3862 2022-10-28 12:08:23.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/startup.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2739 2023-04-24 16:22:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw/utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.831966 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5442 2023-05-26 12:35:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1270 2023-05-26 12:35:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-05-26 12:35:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      421 2023-05-26 12:35:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-05-26 12:35:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/not-zip-safe
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2023-05-26 12:35:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       19 2023-05-26 12:35:41.000000 invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      492 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/requirements-devel.txt
--rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      411 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/run-tests.sh
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2767 2023-05-26 12:35:41.839966 invenio-config-tuw-2023.2.4/setup.cfg
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      339 2023-01-13 11:22:36.000000 invenio-config-tuw-2023.2.4/setup.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-05-26 12:35:41.839966 invenio-config-tuw-2023.2.4/tests/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/tests/conftest.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      789 2021-12-20 12:08:49.000000 invenio-config-tuw-2023.2.4/tests/test_invenio_config_tuw.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-26 20:36:33.297960 invenio-config-tuw-2023.2.5/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      124 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/.dockerignore
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      628 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.5/.editorconfig
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        0 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.5/.git-blame-ignore-revs
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-26 20:36:33.281960 invenio-config-tuw-2023.2.5/.tx/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1056 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/.tx/config
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      332 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.2.5/AUTHORS.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2603 2023-07-26 20:23:54.000000 invenio-config-tuw-2023.2.5/CHANGES.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3392 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.2.5/CONTRIBUTING.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      139 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/INSTALL.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1072 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/LICENSE
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1033 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.5/MANIFEST.in
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5540 2023-07-26 20:36:33.297960 invenio-config-tuw-2023.2.5/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1960 2022-08-09 11:57:39.000000 invenio-config-tuw-2023.2.5/README.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      536 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/babel.ini
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-26 20:36:33.285960 invenio-config-tuw-2023.2.5/docs/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7457 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/docs/Makefile
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      278 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/docs/api.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/docs/authors.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/docs/changes.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    10226 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.5/docs/conf.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      290 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/docs/configuration.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      239 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/docs/contributing.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      817 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/docs/index.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      234 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/docs/installation.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/docs/license.rst
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7005 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/docs/make.bat
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       17 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/docs/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/docs/usage.rst
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-26 20:36:33.289960 invenio-config-tuw-2023.2.5/invenio_config_tuw/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      408 2023-07-26 20:23:54.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/__init__.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-26 20:36:33.293960 invenio-config-tuw-2023.2.5/invenio_config_tuw/auth/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      540 2021-07-15 09:46:09.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/auth/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1006 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/auth/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     8845 2023-07-26 20:21:45.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/auth/handlers.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2540 2021-10-04 14:54:28.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/auth/utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     7800 2023-07-26 20:21:45.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/config.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2623 2022-11-24 12:57:07.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/ext.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1337 2023-05-26 12:34:11.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/formatters.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3905 2023-07-26 20:21:45.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/forms.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-26 20:36:33.293960 invenio-config-tuw-2023.2.5/invenio_config_tuw/permissions/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      780 2022-07-18 13:04:23.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/permissions/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3170 2022-10-11 13:14:29.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/permissions/generators.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11136 2023-04-27 15:56:14.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/permissions/policies.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3862 2022-10-28 12:03:49.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/startup.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     4599 2023-07-26 20:31:27.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/tasks.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-26 20:36:33.297960 invenio-config-tuw-2023.2.5/invenio_config_tuw/tiss/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      409 2023-07-26 14:21:51.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/tiss/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2404 2023-07-26 14:21:51.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/tiss/models.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1794 2023-07-26 14:21:51.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/tiss/utils.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2739 2023-04-24 16:03:59.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw/utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-26 20:36:33.293960 invenio-config-tuw-2023.2.5/invenio_config_tuw.egg-info/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     5540 2023-07-26 20:36:33.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     1401 2023-07-26 20:36:33.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-07-26 20:36:33.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      421 2023-07-26 20:36:33.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2023-07-26 20:36:33.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw.egg-info/not-zip-safe
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      254 2023-07-26 20:36:33.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       19 2023-07-26 20:36:33.000000 invenio-config-tuw-2023.2.5/invenio_config_tuw.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      104 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.5/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      492 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/requirements-devel.txt
+-rwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)      411 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.5/run-tests.sh
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     2767 2023-07-26 20:36:33.297960 invenio-config-tuw-2023.2.5/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      339 2022-11-23 16:27:25.000000 invenio-config-tuw-2023.2.5/setup.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2023-07-26 20:36:33.297960 invenio-config-tuw-2023.2.5/tests/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      990 2023-04-27 15:56:14.000000 invenio-config-tuw-2023.2.5/tests/conftest.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      789 2021-07-02 11:25:37.000000 invenio-config-tuw-2023.2.5/tests/test_invenio_config_tuw.py
```

### Comparing `invenio-config-tuw-2023.2.4/.editorconfig` & `invenio-config-tuw-2023.2.5/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/.tx/config` & `invenio-config-tuw-2023.2.5/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/CHANGES.rst` & `invenio-config-tuw-2023.2.5/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,23 @@
     Invenio Config TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.2 (released 2023-04-24, updated 2023-05-26)
+Version 2023.2 (released 2023-04-24, updated 2023-07-26)
+
 
 - v11 compat: Update permission policies and disable archive download
 - Set affiliation (hard-coded) to TU Wien in `user.profile`
 - Set a default template for the `description` metadata field
 - Add a null check for the current_user in the logging formatter
 - Prevent the logging formatter from blowing up outside of a request context
+- Add utilities and a celery task for updating the `names` vocabulary with information from TISS
 
 
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
```

### Comparing `invenio-config-tuw-2023.2.4/CONTRIBUTING.rst` & `invenio-config-tuw-2023.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/LICENSE` & `invenio-config-tuw-2023.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/MANIFEST.in` & `invenio-config-tuw-2023.2.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/PKG-INFO` & `invenio-config-tuw-2023.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tuw
-Version: 2023.2.4
+Version: 2023.2.5
 Summary: "Invenio module containing some customizations and configuration for TU Wien."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-config-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio tu wien configuration
 Platform: any
@@ -94,21 +94,23 @@
     Invenio Config TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.2 (released 2023-04-24, updated 2023-05-26)
+Version 2023.2 (released 2023-04-24, updated 2023-07-26)
+
 
 - v11 compat: Update permission policies and disable archive download
 - Set affiliation (hard-coded) to TU Wien in `user.profile`
 - Set a default template for the `description` metadata field
 - Add a null check for the current_user in the logging formatter
 - Prevent the logging formatter from blowing up outside of a request context
+- Add utilities and a celery task for updating the `names` vocabulary with information from TISS
 
 
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
```

### Comparing `invenio-config-tuw-2023.2.4/README.rst` & `invenio-config-tuw-2023.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/babel.ini` & `invenio-config-tuw-2023.2.5/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/docs/Makefile` & `invenio-config-tuw-2023.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/docs/conf.py` & `invenio-config-tuw-2023.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/docs/index.rst` & `invenio-config-tuw-2023.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/docs/make.bat` & `invenio-config-tuw-2023.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/__init__.py` & `invenio-config-tuw-2023.2.5/invenio_config_tuw/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/config.py` & `invenio-config-tuw-2023.2.5/invenio_config_tuw/auth/config.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/handlers.py` & `invenio-config-tuw-2023.2.5/invenio_config_tuw/auth/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,16 +210,16 @@
                 user.username = create_username_from_info(user_info)
 
             # update the full name if it has changed
             old_profile = user.user_profile or {}
             if new_full_name and new_full_name != user.user_profile["full_name"]:
                 user.user_profile = {"full_name": new_full_name, **old_profile}
 
-        # Hard code the affiliation to TU Wien, since we are currently not accepting any externals.
-        # It is set on every login.
+        # Hard code the affiliation to TU Wien, since we are currently
+        # not accepting any externals. It is set on every login.
         user.user_profile = {**user.user_profile, "affiliations": "TU Wien"}
 
         # Link account
         # ------------
         # Need to store token in database instead of only the session when
         # called first time.
         token = response_token_setter(remote, resp)
```

### Comparing `invenio-config-tuw-2023.2.4/invenio_config_tuw/auth/utils.py` & `invenio-config-tuw-2023.2.5/invenio_config_tuw/auth/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/invenio_config_tuw/config.py` & `invenio-config-tuw-2023.2.5/invenio_config_tuw/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         }
     ],
     "publisher": "TU Wien",
     "resource_type": {
         "id": "dataset",
     },
     "version": "1.0.0",
-    "description": "<h2>A primer on your dataset's description (to be edited)</h2><p>The influence of proper documentation on the reusability for research data should not be underestimated!<br>In order to help others understand how to interpret and reuse your data, we provide you with a few questions to help you structure your dataset's description (though please don't feel obligated to stick to them):</p><h3>Context and methodology</h3><ul><li>What is the research domain or project in which this dataset was created?</li><li>Which purpose does this dataset serve?</li><li>How was this dataset created?</li></ul><h3>Technical details</h3><ul><li>What is the structure of this dataset? Do the folders and files follow a certain naming convention?</li><li>Is any specific software required to open and work with this dataset?</li><li>Are there any additional resources available regarding the dataset, e.g. documentation, source code, etc.?</li></ul><h3>Further details</h3><ul><li>Is there anything else that other people may need to know when they want to reuse the dataset?</li></ul>",
+    "description": "<h2>A primer on your dataset's description (to be edited)</h2><p>The influence of proper documentation on the reusability for research data should not be underestimated!<br>In order to help others understand how to interpret and reuse your data, we provide you with a few questions to help you structure your dataset's description (though please don't feel obligated to stick to them):</p><h3>Context and methodology</h3><ul><li>What is the research domain or project in which this dataset was created?</li><li>Which purpose does this dataset serve?</li><li>How was this dataset created?</li></ul><h3>Technical details</h3><ul><li>What is the structure of this dataset? Do the folders and files follow a certain naming convention?</li><li>Is any specific software required to open and work with this dataset?</li><li>Are there any additional resources available regarding the dataset, e.g. documentation, source code, etc.?</li></ul><h3>Further details</h3><ul><li>Is there anything else that other people may need to know when they want to reuse the dataset?</li></ul>",  # noqa
 }
 
 RDM_CITATION_STYLES = [
     ("apa", _("APA")),
     ("bibtex", _("BibTeX")),
     ("ieee", _("IEEE")),
 ]
```

### Comparing `invenio-config-tuw-2023.2.4/invenio_config_tuw/ext.py` & `invenio-config-tuw-2023.2.5/invenio_config_tuw/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/invenio_config_tuw/formatters.py` & `invenio-config-tuw-2023.2.5/invenio_config_tuw/formatters.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/invenio_config_tuw/forms.py` & `invenio-config-tuw-2023.2.5/invenio_config_tuw/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020-2022 TU Wien.
+# Copyright (C) 2020-2023 TU Wien.
 #
 # Invenio-Config-TUW is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 from datetime import datetime
 
-from flask import current_app, url_for
-from flask_babelex import gettext as _
+from flask import current_app
 from markupsafe import Markup
 from werkzeug.local import LocalProxy
 from wtforms import BooleanField, Form, HiddenField, validators
 from wtforms.fields.core import FormField
 
 _security = LocalProxy(lambda: current_app.extensions["security"])
 
@@ -42,16 +41,17 @@
     Note: Invenio-OAuthClient 2.0 tweaked the workings of the registration a bit;
     now the precedence mask is applied to values from the user's input in the form,
     the result of which is then fed back to the form (for validation, I assume),
     which in turn is fetched again and used to populate the user account.
     This means that we have to actually hold information in the forms and can't
     just set every field to ``None``.
     """
-    # the url must contain the special characters rather than encoded values: Markup escapes them
-    terms_of_use_url = "https://www.tuwien.at/index.php?eID=dms&s=4&path=Directives and Regulations of the Rectorate/Research_Data_Terms_of_Use.pdf"
+    # the url must contain the special characters rather than encoded values:
+    # `Markup` escapes them
+    terms_of_use_url = "https://www.tuwien.at/index.php?eID=dms&s=4&path=Directives and Regulations of the Rectorate/Research_Data_Terms_of_Use.pdf"  # noqa
     message = Markup(
         f"Accept the <a href='{terms_of_use_url}' target='_blank'>Terms and Conditions</a>"  # noqa
     )
 
     class UserProfileForm(Form):
         """Form for the user profile."""
```

### Comparing `invenio-config-tuw-2023.2.4/invenio_config_tuw/permissions/__init__.py` & `invenio-config-tuw-2023.2.5/invenio_config_tuw/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/invenio_config_tuw/permissions/generators.py` & `invenio-config-tuw-2023.2.5/invenio_config_tuw/permissions/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/invenio_config_tuw/permissions/policies.py` & `invenio-config-tuw-2023.2.5/invenio_config_tuw/permissions/policies.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/invenio_config_tuw/startup.py` & `invenio-config-tuw-2023.2.5/invenio_config_tuw/startup.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/invenio_config_tuw/utils.py` & `invenio-config-tuw-2023.2.5/invenio_config_tuw/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/PKG-INFO` & `invenio-config-tuw-2023.2.5/invenio_config_tuw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-config-tuw
-Version: 2023.2.4
+Version: 2023.2.5
 Summary: "Invenio module containing some customizations and configuration for TU Wien."
 Home-page: https://gitlab.tuwien.ac.at/fairdata/invenio-config-tuw
 Author: TU Wien
 Author-email: tudata@tuwien.ac.at
 License: MIT
 Keywords: invenio tu wien configuration
 Platform: any
@@ -94,21 +94,23 @@
     Invenio Config TUW is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
-Version 2023.2 (released 2023-04-24, updated 2023-05-26)
+Version 2023.2 (released 2023-04-24, updated 2023-07-26)
+
 
 - v11 compat: Update permission policies and disable archive download
 - Set affiliation (hard-coded) to TU Wien in `user.profile`
 - Set a default template for the `description` metadata field
 - Add a null check for the current_user in the logging formatter
 - Prevent the logging formatter from blowing up outside of a request context
+- Add utilities and a celery task for updating the `names` vocabulary with information from TISS
 
 
 Version 2023.1 (released 2023-01-13)
 
 - Update definition of the default creator for new uploads
```

### Comparing `invenio-config-tuw-2023.2.4/invenio_config_tuw.egg-info/SOURCES.txt` & `invenio-config-tuw-2023.2.5/invenio_config_tuw.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 docs/usage.rst
 invenio_config_tuw/__init__.py
 invenio_config_tuw/config.py
 invenio_config_tuw/ext.py
 invenio_config_tuw/formatters.py
 invenio_config_tuw/forms.py
 invenio_config_tuw/startup.py
+invenio_config_tuw/tasks.py
 invenio_config_tuw/utils.py
 invenio_config_tuw.egg-info/PKG-INFO
 invenio_config_tuw.egg-info/SOURCES.txt
 invenio_config_tuw.egg-info/dependency_links.txt
 invenio_config_tuw.egg-info/entry_points.txt
 invenio_config_tuw.egg-info/not-zip-safe
 invenio_config_tuw.egg-info/requires.txt
@@ -45,9 +46,12 @@
 invenio_config_tuw/auth/__init__.py
 invenio_config_tuw/auth/config.py
 invenio_config_tuw/auth/handlers.py
 invenio_config_tuw/auth/utils.py
 invenio_config_tuw/permissions/__init__.py
 invenio_config_tuw/permissions/generators.py
 invenio_config_tuw/permissions/policies.py
+invenio_config_tuw/tiss/__init__.py
+invenio_config_tuw/tiss/models.py
+invenio_config_tuw/tiss/utils.py
 tests/conftest.py
 tests/test_invenio_config_tuw.py
```

### Comparing `invenio-config-tuw-2023.2.4/setup.cfg` & `invenio-config-tuw-2023.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/tests/conftest.py` & `invenio-config-tuw-2023.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-config-tuw-2023.2.4/tests/test_invenio_config_tuw.py` & `invenio-config-tuw-2023.2.5/tests/test_invenio_config_tuw.py`

 * *Files identical despite different names*

