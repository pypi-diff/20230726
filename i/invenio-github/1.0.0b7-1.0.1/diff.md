# Comparing `tmp/invenio-github-1.0.0b7.tar.gz` & `tmp/invenio-github-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-github-1.0.0b7.tar", last modified: Mon Jul 24 09:24:01 2023, max compression
+gzip compressed data, was "dist/invenio-github-1.0.1.tar", last modified: Wed Jul 26 08:13:39 2023, max compression
```

## Comparing `invenio-github-1.0.0b7.tar` & `invenio-github-1.0.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      973 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2509 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/.lgtm
--rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/MAINTAINERS
--rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5058 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/RELEASE-NOTES.rst
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/babel.ini
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/constraints-pypi.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10770 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/alembic/
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/alembic/5a5428312b2b_create_github_branch.py
--rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/alembic/b0eaee37b545_create_github_tables.py
--rw-r--r--   0 runner    (1001) docker     (122)    23408 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/assets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/assets/semantic-ui/js/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)     3388 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/assets/semantic-ui/js/invenio_github/index.js
--rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/ext.py
--rw-r--r--   0 runner    (1001) docker     (122)     7738 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/oauth/
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/oauth/handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/oauth/remote_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/proxies.py
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/receivers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/helpers.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     2656 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
--rw-r--r--   0 runner    (1001) docker     (122)     6538 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
--rw-r--r--   0 runner    (1001) docker     (122)    15814 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/view.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/it/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github/views/
--rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3596 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/views/badge.py
--rw-r--r--   0 runner    (1001) docker     (122)     8272 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/views/github.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/invenio_github/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5058 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      944 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/invenio_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      347 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/run-i18n-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)     1840 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3247 2023-07-24 09:24:01.000000 invenio-github-1.0.0b7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-24 09:23:56.000000 invenio-github-1.0.0b7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-26 08:13:26.000000 invenio-github-1.0.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      973 2023-07-26 08:13:26.000000 invenio-github-1.0.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2509 2023-07-26 08:13:26.000000 invenio-github-1.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-26 08:13:26.000000 invenio-github-1.0.1/.lgtm
+-rw-r--r--   0 runner    (1001) docker     (122)     2747 2023-07-26 08:13:26.000000 invenio-github-1.0.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-26 08:13:26.000000 invenio-github-1.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1826 2023-07-26 08:13:26.000000 invenio-github-1.0.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3464 2023-07-26 08:13:26.000000 invenio-github-1.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-07-26 08:13:26.000000 invenio-github-1.0.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-07-26 08:13:26.000000 invenio-github-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-26 08:13:26.000000 invenio-github-1.0.1/MAINTAINERS
+-rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-07-26 08:13:26.000000 invenio-github-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5260 2023-07-26 08:13:38.000000 invenio-github-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-26 08:13:26.000000 invenio-github-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-07-26 08:13:26.000000 invenio-github-1.0.1/RELEASE-NOTES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-07-26 08:13:26.000000 invenio-github-1.0.1/babel.ini
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-07-26 08:13:26.000000 invenio-github-1.0.1/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-07-26 08:13:26.000000 invenio-github-1.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-26 08:13:26.000000 invenio-github-1.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-26 08:13:26.000000 invenio-github-1.0.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-26 08:13:26.000000 invenio-github-1.0.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10770 2023-07-26 08:13:26.000000 invenio-github-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1013 2023-07-26 08:13:26.000000 invenio-github-1.0.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-26 08:13:26.000000 invenio-github-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-26 08:13:26.000000 invenio-github-1.0.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      867 2023-07-26 08:13:26.000000 invenio-github-1.0.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-07-26 08:13:26.000000 invenio-github-1.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-26 08:13:26.000000 invenio-github-1.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-07-26 08:13:26.000000 invenio-github-1.0.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1138 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/alembic/
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/alembic/5a5428312b2b_create_github_branch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/alembic/b0eaee37b545_create_github_tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23408 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/assets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/assets/semantic-ui/js/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)     5255 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/assets/semantic-ui/js/invenio_github/index.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7759 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/oauth/
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/oauth/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/oauth/remote_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6382 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/templates/semantic-ui/invenio_github/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/templates/semantic-ui/invenio_github/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/templates/semantic-ui/invenio_github/helpers.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/templates/semantic-ui/invenio_github/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/templates/semantic-ui/invenio_github/settings/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5022 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/templates/semantic-ui/invenio_github/settings/helpers.html
+-rw-r--r--   0 runner    (1001) docker     (122)     7220 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/templates/semantic-ui/invenio_github/settings/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/templates/semantic-ui/invenio_github/settings/index_item.html
+-rw-r--r--   0 runner    (1001) docker     (122)    15564 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/templates/semantic-ui/invenio_github/settings/view.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1338 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1556 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/translations/it/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      949 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3596 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/views/badge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8212 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/views/github.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-26 08:13:26.000000 invenio-github-1.0.1/invenio_github/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5260 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      944 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-26 08:13:38.000000 invenio-github-1.0.1/invenio_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-07-26 08:13:26.000000 invenio-github-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-26 08:13:26.000000 invenio-github-1.0.1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      347 2023-07-26 08:13:26.000000 invenio-github-1.0.1/run-i18n-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1840 2023-07-26 08:13:26.000000 invenio-github-1.0.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3247 2023-07-26 08:13:39.000000 invenio-github-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-07-26 08:13:26.000000 invenio-github-1.0.1/setup.py
```

### Comparing `invenio-github-1.0.0b7/.github/workflows/pypi-publish.yml` & `invenio-github-1.0.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/.github/workflows/tests.yml` & `invenio-github-1.0.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/.travis.yml` & `invenio-github-1.0.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/AUTHORS.rst` & `invenio-github-1.0.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/CHANGES.rst` & `invenio-github-1.0.1/CHANGES.rst`

 * *Files 13% similar despite different names*

```diff
@@ -21,14 +21,22 @@
     waive the privileges and immunities granted to it by virtue of its status
     as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 
 Changes
 =======
 
+Version v1.0.1 (released 2023-07-26)
+
+- ui: layout and styling improvements
+
+Version v1.0.0 (released 2023-07-24)
+
+- inital public release
+
 Version v1.0.0b7 (released 2023-07-24)
 
 - handlers: fix oauthclient import
 
 Version v1.0.0b6 (released 2023-07-21)
 
 - add github badges
```

### Comparing `invenio-github-1.0.0b7/CONTRIBUTING.rst` & `invenio-github-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/LICENSE` & `invenio-github-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/MANIFEST.in` & `invenio-github-1.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/PKG-INFO` & `invenio-github-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0b7
+Version: 1.0.1
 Summary: "Invenio module that adds GitHub integration to the platform."
 Home-page: https://github.com/inveniosoftware/invenio-github
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -79,14 +79,22 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         
         Changes
         =======
         
+        Version v1.0.1 (released 2023-07-26)
+        
+        - ui: layout and styling improvements
+        
+        Version v1.0.0 (released 2023-07-24)
+        
+        - inital public release
+        
         Version v1.0.0b7 (released 2023-07-24)
         
         - handlers: fix oauthclient import
         
         Version v1.0.0b6 (released 2023-07-21)
         
         - add github badges
```

### Comparing `invenio-github-1.0.0b7/README.rst` & `invenio-github-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/RELEASE-NOTES.rst` & `invenio-github-1.0.1/RELEASE-NOTES.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/docs/Makefile` & `invenio-github-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/docs/api.rst` & `invenio-github-1.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/docs/authors.rst` & `invenio-github-1.0.1/docs/authors.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/docs/changes.rst` & `invenio-github-1.0.1/docs/changes.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/docs/conf.py` & `invenio-github-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/docs/contributing.rst` & `invenio-github-1.0.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/docs/index.rst` & `invenio-github-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/docs/installation.rst` & `invenio-github-1.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/docs/license.rst` & `invenio-github-1.0.1/docs/license.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/docs/make.bat` & `invenio-github-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/docs/usage.rst` & `invenio-github-1.0.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/__init__.py` & `invenio-github-1.0.1/invenio_github/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,10 +22,10 @@
 # waive the privileges and immunities granted to it by virtue of its status
 # as an Intergovernmental Organization or submit itself to any jurisdiction.
 
 """Invenio module that adds GitHub integration to the platform."""
 
 from .ext import InvenioGitHub
 
-__version__ = "1.0.0b7"
+__version__ = "1.0.1"
 
 __all__ = ("__version__", "InvenioGitHub")
```

### Comparing `invenio-github-1.0.0b7/invenio_github/alembic/5a5428312b2b_create_github_branch.py` & `invenio-github-1.0.1/invenio_github/alembic/5a5428312b2b_create_github_branch.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/alembic/b0eaee37b545_create_github_tables.py` & `invenio-github-1.0.1/invenio_github/alembic/b0eaee37b545_create_github_tables.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/api.py` & `invenio-github-1.0.1/invenio_github/api.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/config.py` & `invenio-github-1.0.1/invenio_github/config.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/errors.py` & `invenio-github-1.0.1/invenio_github/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/ext.py` & `invenio-github-1.0.1/invenio_github/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/models.py` & `invenio-github-1.0.1/invenio_github/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,27 +40,27 @@
     "PROCESSING": _("Processing"),
     "PUBLISHED": _("Published"),
     "FAILED": _("Failed"),
     "DELETED": _("Deleted"),
 }
 
 RELEASE_STATUS_ICON = {
-    "RECEIVED": "spinner icon",
-    "PROCESSING": "spinner icon",
+    "RECEIVED": "spinner loading icon",
+    "PROCESSING": "spinner loading icon",
     "PUBLISHED": "check icon",
     "FAILED": "times icon",
     "DELETED": "times icon",
 }
 
 RELEASE_STATUS_COLOR = {
-    "RECEIVED": "default",
-    "PROCESSING": "default",
-    "PUBLISHED": "success",
-    "FAILED": "danger",
-    "DELETED": "danger",
+    "RECEIVED": "warning",
+    "PROCESSING": "warning",
+    "PUBLISHED": "positive",
+    "FAILED": "negative",
+    "DELETED": "negative",
 }
 
 
 class ReleaseStatus(Enum):
     """Constants for possible status of a Release."""
 
     __order__ = "RECEIVED PROCESSING PUBLISHED FAILED DELETED"
```

### Comparing `invenio-github-1.0.0b7/invenio_github/oauth/handlers.py` & `invenio-github-1.0.1/invenio_github/oauth/handlers.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/oauth/remote_app.py` & `invenio-github-1.0.1/invenio_github/oauth/remote_app.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/proxies.py` & `invenio-github-1.0.1/invenio_github/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/receivers.py` & `invenio-github-1.0.1/invenio_github/receivers.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/tasks.py` & `invenio-github-1.0.1/invenio_github/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/templates/semantic-ui/invenio_github/settings/index.html` & `invenio-github-1.0.1/invenio_github/templates/semantic-ui/invenio_github/settings/index.html`

 * *Files 22% similar despite different names*

```diff
@@ -10,159 +10,170 @@
 {%- if not request.is_xhr %}
   {%- extends config.GITHUB_SETTINGS_TEMPLATE %}
 {%- endif %}
 
 {%- block settings_content %}
   {%- if connected %}
     {%- block repositories_get_started %}
-      {{ helpers.panel_start(_('GitHub Repositories') ,
-        with_body=False,
-        icon="github icon",
-        btn=_('Sync now ...'),
-        btn_icon='sync alternate icon',
-        btn_id='sync_repos',
-        btn_name='sync-repos',
-        btn_text=_('(updated {})').format(last_sync|naturaltime),
-        id="github-view",
-      ) }}
+      {{
+        helpers.panel_start(
+          _('GitHub Repositories'),
+          icon="github icon",
+          btn_text=_('Sync now'),
+          btn_loading_text=_('Syncing'),
+          btn_icon='sync alternate icon',
+          btn_id='sync_repos',
+          btn_name='sync-repos',
+          btn_help_text=_('(updated {})').format(last_sync|naturaltime),
+          loaded_message_id='sync-result-message',
+          id="github-view",
+        )
+      }}
+
       <div class="ui segment">
-        <div class="ui two column centered grid">
-          <div class="column">
-            <h1 class="ui center aligned header">
-              <i class="github icon"></i>{{ _("Get started") }}
-            </h1>
+        <div class="ui grid">
+          <div class="sixteen wide centered column">
+            <h3 class="ui large header mt-10">
+              <i class="github icon" aria-hidden="true"></i>{{ _("Get started") }}
+            </h3>
           </div>
-          <div class="three column row">
+
+          <div class="three column stackable tablet-mobile row">
             <div class="column">
-              <h2>
-                <strong>1</strong> <small>{{ _("Flip the switch") }}</small>
-              </h2>
+              <h4 class="ui medium header">1 {{ _("Flip the switch") }}</h4>
               <div class="ui divider"></div>
-              {{ _('Select the repository you want to preserve, and toggle
-              the switch below to turn on automatic preservation of your software.') }}
+              <p>
+                {{ _('Select the repository you want to preserve, and toggle
+                the switch below to turn on automatic preservation of your software.') }}
+              </p>
+
+              <div class="text-align-center rel-mt-1">
+                <div class="ui toggle on-off checkbox">
+                  <input
+                    id="example-switch"
+                    name="example-switch"
+                    type="checkbox"
+                    checked
+                  >
+                  <label for="example-switch">
+                    <small class="text-muted ml-5">
+                      {{ _("(example)") }}
+                    </small>
+                  </label>
+                </div>
+              </div>
             </div>
+
             <div class="column">
-              <h2>
-                <strong>2</strong> <small>{{ _("Create a release") }}</small>
-              </h2>
+              <h4 class="ui medium header">2 {{ _("Create a release") }}</h4>
               <div class="ui divider"></div>
-              {{ _('Go to GitHub and <a href="https://help.github.com/articles/creating-releases">create a release</a>. {}
-              will automatically download a .zip-ball of each new release and register a DOI.')
-              .format(config.THEME_SITENAME | default('System')) }}
+              <p>
+                {{ _('Go to GitHub and <a href="https://help.github.com/articles/creating-releases" target="_blank">create a release <i class="small icon external" aria-hidden="true"></i></a>. {}
+                will automatically download a .zip-ball of each new release and register a DOI.')
+                .format(config.THEME_SITENAME | default('System')) }}
+              </p>
             </div>
+
             <div class="column">
-              <h2>
-                <strong>3</strong> <small>{{ _("Get the badge") }}</small>
-              </h2>
+              <h4 class="ui medium header">3 {{ _("Get the badge") }}</h4>
               <div class="ui divider"></div>
-              {{ _('After your first release, a DOI badge that you can include in GitHub
-              README will appear next to your repository below.') }}
-            </div>
-          </div>
-          <div class="three column row">
-            <div class="column centered">
-              <br />
-              <div class="ui toggle checkbox">
-                <input type="checkbox" checked>
-                <label></label>
+              <p>
+                {{ _('After your first release, a DOI badge that you can include in GitHub
+                README will appear next to your repository below.') }}
+              </p>
+
+              <div class="flex align-items-center justify-center rel-mt-1">
+                {#- TODO remove hardcoding Zenodo stuff #}
+                <a href="https://doi.org/10.5281/zenodo.8475">
+                  <img
+                    src="{{ url_for('invenio_formatter_badges.badge', title='doi', value='10.5281/zenodo.8475', ext='svg') }}"
+                    alt="{{ _('Example DOI:') }} 10.5281/zenodo.8475"
+                    class="mt-5 mr-5"
+                  >
+                </a>
+                <small class="text-muted">
+                  {{ _("(example)") }}
+                </small>
               </div>
             </div>
-            <div class="column"></div>
-            <div class="column centered">
-              <br>
-              {#- TODO remove hardcoding Zenodo stuff #}
-              <a href="https://doi.org/10.5281/zenodo.8475">
-                <img src="{{ url_for('invenio_formatter_badges.badge', title='doi', value='10.5281/zenodo.8475', ext='svg') }}" alt="10.5281/zenodo.8475">
-              </a>
-              <br>
-              <small>{{ _("(example)") }}</small>
-            </div>
           </div>
         </div>
       </div>
-      {{ helpers.panel_end(with_body=False) }}
+      {{ helpers.panel_end() }}
     {%- endblock %}
 
     {%- if repos %}
       {%- block enabled_repositories %}
-        {%- for repo_id, repo in repos if repo.instance and repo.instance.hook %}
-          {%- if loop.first %}
-            {{ helpers.panel_start(_('Enabled Repositories') , with_body=False) }}
-            <div class="ui segment">
-          {%- endif %}
-          <div class="repositories-list">
-            {% include "invenio_github/settings/index_item.html" with context %}
-          </div>
-          {%- if loop.last %}
-            </div>
-            {{ helpers.panel_end(with_body=False) }}
-          {%- endif %}
-        {%- endfor %}
+        {{ helpers.panel_start(_('Enabled Repositories')) }}
+
+        <ul class="ui segments no-border no-border-radius-top no-style-list m-0 p-0">
+          {%- for repo_id, repo in repos if repo.instance and repo.instance.hook %}
+            <li class="ui segment {{ 'no-border-radius-top' if loop.last else 'no-border-radius' }} left-border positive m-0">
+              {% include "invenio_github/settings/index_item.html" with context %}
+            </li>
+          {%- endfor %}
+        </ul>
+
+        {{ helpers.panel_end() }}
       {%- endblock %}
     {% endif %}
 
     {%- block disabled_repositories %}
-      {{ helpers.panel_start(_('Repositories') , with_body=False) }}
-      <div class="ui segment">
-        {%- block repositories_tooltip %}
-          <p>
-            <small>
-              {{ _('If your organization\'s repositories do not show up in the list, please
-              ensure you have enabled <a href="https://help.github.com/articles/approving-third-party-applications-for-your-organization/">third-party
-              access</a> to the {} application. Private repositories are not supported.')
-              .format(config.THEME_SITENAME | default('Invenio')) }}
-            </small>
-          </p>
-        {%- endblock %}
-        {%- if not repos %}
-          <p>
-            {{_('You have no repositories on GitHub.
-            <br>
-            Go to <a href="https://github.com/new">GitHub</a> and create your first or
-            click Sync-button to synchronize latest changes from GitHub.')}}
-          </p>
-        {%- else %}
+      {{ helpers.panel_start(_('Repositories')) }}
+
+      {%- block repositories_tooltip %}
+        <p class="ui segment m-0">
+          <small>
+            {{ _('If your organization\'s repositories do not show up in the list, please
+            ensure you have enabled <a href="https://help.github.com/articles/approving-third-party-applications-for-your-organization/" target="_blank">third-party
+            access <i class="small icon external" aria-hidden="true"></i></a> to the {} application. Private repositories are not supported.')
+            .format(config.THEME_SITENAME | default('Invenio')) }}
+          </small>
+        </p>
+      {%- endblock %}
+
+      {%- if not repos %}
+        <p class="ui segment">
+          {{_('You have no repositories on GitHub.') }}
+          <br />
+          <br />
+          {{_('Go to <a href="https://github.com/new" target="_blank">GitHub <i class="small icon external" aria-hidden="true"></i></a> and create your first or
+          click Sync-button to synchronize latest changes from GitHub.')}}
+        </p>
+      {%- else %}
+        <ul class="ui segments no-border no-border-radius-top no-style-list m-0 p-0">
           {%- for repo_id, repo in repos if not repo.instance or not repo.instance.hook %}
-            {%- if loop.first %}
-              <div class="ui divider"></div>
-            {%- endif %}
-            <div class="repositories-list">
+            <li class="ui segment {{ 'no-border-radius-top' if loop.last else 'no-border-radius' }}">
               {% include "invenio_github/settings/index_item.html" with context %}
-            </div>
+            </li>
           {%- endfor %}
-        {% endif %}
-      </div>
-      {{ helpers.panel_end(with_body=False) }}
+        </ul>
+      {% endif %}
+
+      {{ helpers.panel_end() }}
     {%- endblock %}
 
   {#- If the user has not connected his GitHub account... #}
   {%- else %}
     {%- block connect_to_github %}
-      {{ helpers.panel_start(
-        _('GitHub'),
-        icon="github icon",
-      ) }}
-      <div class="ui one column grid">
-        <div class="row">
-          <div class="column centered">
-            <h1>{{ _('Software preservation made simple!') }}</h1>
-          </div>
-        </div>
-        <div class="row">
-          <div class="column centered">
-            <a class="ui basic button" href="{{ url_for('invenio_oauthclient.login', remote_app='github', next=url_for('invenio_github.get_repositories')) }}">
-              <i class="github icon"></i>
-              {{ _('Connect') }}
-            </a>
-          </div>
-        </div>
-        <div class="row">
-          <div class="column centered">
-            <p>{{ _('To get started, click "Connect" and we will get a list of your repositories from GitHub.') }}</p>
-          </div>
+      {{ helpers.panel_start(_('GitHub'), icon="github icon") }}
+      <div class="ui segment">
+        <div class="ui centered container">
+          <h2 class="ui huge header">{{ _('Software preservation made simple!') }}</h2>
+          <a
+            class="ui basic button rel-mt-1"
+            href="{{ url_for('invenio_oauthclient.login', remote_app='github', next=url_for('invenio_github.get_repositories')) }}"
+            aria-label="{{ _('Connect your GitHub account') }}"
+          >
+            <i class="github icon" aria-hidden="True"></i>
+            {{ _('Connect') }}
+          </a>
+          <p class="rel-mt-2">
+            {{ _('To get started, click "Connect" and we will get a list of your repositories from GitHub.') }}
+          </p>
         </div>
       </div>
       {{ helpers.panel_end() }}
     {%- endblock %}
   {%- endif %}
 {%- endblock %}
```

#### html2text {}

```diff
@@ -1,60 +1,61 @@
 {# -*- coding: utf-8 -*- This file is part of Invenio. Copyright (C) 2023 CERN.
 Invenio is free software; you can redistribute it and/or modify it under the
 terms of the MIT License; see LICENSE file for more details. #} {%- import
 "invenio_github/settings/helpers.html" as helpers with context %} {%- if not
 request.is_xhr %} {%- extends config.GITHUB_SETTINGS_TEMPLATE %} {%- endif %}
 {%- block settings_content %} {%- if connected %} {%- block
-repositories_get_started %} {{ helpers.panel_start(_('GitHub Repositories') ,
-with_body=False, icon="github icon", btn=_('Sync now ...'), btn_icon='sync
-alternate icon', btn_id='sync_repos', btn_name='sync-repos', btn_text=_('
-(updated {})').format(last_sync|naturaltime), id="github-view", ) }}
+repositories_get_started %} {{ helpers.panel_start( _('GitHub Repositories'),
+icon="github icon", btn_text=_('Sync now'), btn_loading_text=_('Syncing'),
+btn_icon='sync alternate icon', btn_id='sync_repos', btn_name='sync-repos',
+btn_help_text=_('(updated {})').format(last_sync|naturaltime),
+loaded_message_id='sync-result-message', id="github-view", ) }}
 {{ _("Get started") }}
-***** 1 {{ _("Flip the switch") }} *****
+*** 1 {{ _("Flip the switch") }} ***
 {{ _('Select the repository you want to preserve, and toggle the switch below
 to turn on automatic preservation of your software.') }}
-***** 2 {{ _("Create a release") }} *****
-{{ _('Go to GitHub and create_a_release. {} will automatically download a .zip-
-ball of each new release and register a DOI.') .format(config.THEME_SITENAME |
-default('System')) }}
-***** 3 {{ _("Get the badge") }} *****
+*  {{ _("(example)") }}
+*** 2 {{ _("Create a release") }} ***
+{{ _('Go to GitHub and
+create_a_release
+. {} will automatically download a .zip-ball of each new release and register a
+DOI.') .format(config.THEME_SITENAME | default('System')) }}
+*** 3 {{ _("Get the badge") }} ***
 {{ _('After your first release, a DOI badge that you can include in GitHub
 README will appear next to your repository below.') }}
-
-*
-
-{#- TODO remove hardcoding Zenodo stuff #} [10.5281/zenodo.8475]
-{{ _("(example)") }}
-{{ helpers.panel_end(with_body=False) }} {%- endblock %} {%- if repos %} {%-
-block enabled_repositories %} {%- for repo_id, repo in repos if repo.instance
-and repo.instance.hook %} {%- if loop.first %} {{ helpers.panel_start(_
-('Enabled Repositories') , with_body=False) }}
-{%- endif %}
-{% include "invenio_github/settings/index_item.html" with context %}
-{%- if loop.last %}
-{{ helpers.panel_end(with_body=False) }} {%- endif %} {%- endfor %} {%-
-endblock %} {% endif %} {%- block disabled_repositories %} {
-{ helpers.panel_start(_('Repositories') , with_body=False) }}
-{%- block repositories_tooltip %}
+{#- TODO remove hardcoding Zenodo stuff #} [{{__('Example_DOI:')_}}_10.5281/
+zenodo.8475] {{ _("(example)") }}
+{{ helpers.panel_end() }} {%- endblock %} {%- if repos %} {%- block
+enabled_repositories %} {{ helpers.panel_start(_('Enabled Repositories')) }}
+    * {%- for repo_id, repo in repos if repo.instance and repo.instance.hook %}
+    * {% include "invenio_github/settings/index_item.html" with context %}
+    * {%- endfor %}
+{{ helpers.panel_end() }} {%- endblock %} {% endif %} {%- block
+disabled_repositories %} {{ helpers.panel_start(_('Repositories')) }} {%- block
+repositories_tooltip %}
 {{ _('If your organization\'s repositories do not show up in the list, please
-ensure you have enabled third-party_access to the {} application. Private
-repositories are not supported.') .format(config.THEME_SITENAME | default
-('Invenio')) }}
+ensure you have enabled
+third-party_access
+ to the {} application. Private repositories are not supported.') .format
+(config.THEME_SITENAME | default('Invenio')) }}
 {%- endblock %} {%- if not repos %}
-{{_('You have no repositories on GitHub.
-Go to GitHub and create your first or click Sync-button to synchronize latest
-changes from GitHub.')}}
-{%- else %} {%- for repo_id, repo in repos if not repo.instance or not
-repo.instance.hook %} {%- if loop.first %}
-{%- endif %}
-{% include "invenio_github/settings/index_item.html" with context %}
-{%- endfor %} {% endif %}
-{{ helpers.panel_end(with_body=False) }} {%- endblock %} {#- If the user has
-not connected his GitHub account... #} {%- else %} {%- block connect_to_github
-%} {{ helpers.panel_start( _('GitHub'), icon="github icon", ) }}
-****** {{ _('Software preservation made simple!') }} ******
+{{_('You have no repositories on GitHub.') }}
+
+{{_('Go to
+GitHub
+ and create your first or click Sync-button to synchronize latest changes from
+GitHub.')}}
+{%- else %}
+    * {%- for repo_id, repo in repos if not repo.instance or not
+      repo.instance.hook %}
+    * {% include "invenio_github/settings/index_item.html" with context %}
+    * {%- endfor %}
+{% endif %} {{ helpers.panel_end() }} {%- endblock %} {#- If the user has not
+connected his GitHub account... #} {%- else %} {%- block connect_to_github %} {
+{ helpers.panel_start(_('GitHub'), icon="github icon") }}
+***** {{ _('Software preservation made simple!') }} *****
  {{__('Connect')_}}
 {{ _('To get started, click "Connect" and we will get a list of your
 repositories from GitHub.') }}
 {{ helpers.panel_end() }} {%- endblock %} {%- endif %} {%- endblock %} {%-
 block javascript %} {{ super() }} {{ webpack['invenio-github-init.js'] }} {%-
 endblock javascript %}
```

### Comparing `invenio-github-1.0.0b7/invenio_github/translations/cs/LC_MESSAGES/messages.po` & `invenio-github-1.0.1/invenio_github/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/translations/da/LC_MESSAGES/messages.po` & `invenio-github-1.0.1/invenio_github/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/translations/de/LC_MESSAGES/messages.po` & `invenio-github-1.0.1/invenio_github/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/translations/en/LC_MESSAGES/messages.po` & `invenio-github-1.0.1/invenio_github/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/translations/es/LC_MESSAGES/messages.po` & `invenio-github-1.0.1/invenio_github/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/translations/fr/LC_MESSAGES/messages.po` & `invenio-github-1.0.1/invenio_github/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/translations/it/LC_MESSAGES/messages.po` & `invenio-github-1.0.1/invenio_github/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/translations/messages.pot` & `invenio-github-1.0.1/invenio_github/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/utils.py` & `invenio-github-1.0.1/invenio_github/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/views/__init__.py` & `invenio-github-1.0.1/invenio_github/views/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/views/badge.py` & `invenio-github-1.0.1/invenio_github/views/badge.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github/views/github.py` & `invenio-github-1.0.1/invenio_github/views/github.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # granted to it by virtue of its status as an Intergovernmental Organization
 # or submit itself to any jurisdiction.
 
 """GitHub blueprint for Invenio platform."""
 
 from functools import wraps
 
-from flask import Blueprint, abort, current_app, render_template
+from flask import Blueprint, abort, current_app, render_template, request
 from flask_breadcrumbs import register_breadcrumb
 from flask_login import current_user, login_required
 from flask_menu import register_menu
 from invenio_db import db
 from invenio_i18n import gettext as _
 from invenio_theme.proxies import current_theme_icons
 from speaklater import make_lazy_string
@@ -63,15 +63,16 @@
         "invenio_github",
         __name__,
         static_folder="../static",
         template_folder="../templates",
         url_prefix="/account/settings/github",
     )
     if app.config.get("GITHUB_INTEGRATION_ENABLED", False):
-        register_ui_routes(blueprint)
+        with app.app_context():  # Todo: Temporary fix, it should be removed when inveniosoftware/invenio-theme#355 is merged
+            register_ui_routes(blueprint)
     return blueprint
 
 
 def create_api_blueprint(app):
     """Creates blueprint and registers API endpoints if the integration is enabled."""
     blueprint_api = Blueprint("invenio_github_api", __name__)
     if app.config.get("GITHUB_INTEGRATION_ENABLED", False):
@@ -83,26 +84,22 @@
     """Register ui routes."""
 
     @blueprint.route("/")
     @login_required
     @register_menu(  # TODO modify?
         blueprint,
         "settings.github",
-        # TODO substitute github for icon + 'Github'
-        _("Github"),
-        # _(
-        #     "%(icon)s GitHub",
-        #     icon=make_lazy_string(
-        #         lambda: '<i class="{icon}"></i>'.format(
-        #             icon=current_theme_icons.github
-        #         )  # TODO confirm if icon gets picked
-        #     ),
-        # ),
-        order=10,  # TODO confirm
-        # active_when=lambda: request.endpoint.startswith("invenio_github."),
+        _(
+            "%(icon)s GitHub",
+            icon=make_lazy_string(
+                lambda: f'<i class="{current_theme_icons.github}"></i>'
+            ),
+        ),
+        order=10,
+        active_when=lambda: request.endpoint.startswith("invenio_github."),
     )
     @register_breadcrumb(blueprint, "breadcrumbs.settings.github", _("GitHub"))
     def get_repositories():
         """Display list of the user's repositories."""
         github = GitHubAPI(user_id=current_user.id)
         ctx = dict(connected=False)
         if github.session_token:
```

### Comparing `invenio-github-1.0.0b7/invenio_github/webpack.py` & `invenio-github-1.0.1/invenio_github/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github.egg-info/PKG-INFO` & `invenio-github-1.0.1/invenio_github.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-github
-Version: 1.0.0b7
+Version: 1.0.1
 Summary: "Invenio module that adds GitHub integration to the platform."
 Home-page: https://github.com/inveniosoftware/invenio-github
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -79,14 +79,22 @@
             waive the privileges and immunities granted to it by virtue of its status
             as an Intergovernmental Organization or submit itself to any jurisdiction.
         
         
         Changes
         =======
         
+        Version v1.0.1 (released 2023-07-26)
+        
+        - ui: layout and styling improvements
+        
+        Version v1.0.0 (released 2023-07-24)
+        
+        - inital public release
+        
         Version v1.0.0b7 (released 2023-07-24)
         
         - handlers: fix oauthclient import
         
         Version v1.0.0b6 (released 2023-07-21)
         
         - add github badges
```

### Comparing `invenio-github-1.0.0b7/invenio_github.egg-info/SOURCES.txt` & `invenio-github-1.0.1/invenio_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github.egg-info/entry_points.txt` & `invenio-github-1.0.1/invenio_github.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/invenio_github.egg-info/requires.txt` & `invenio-github-1.0.1/invenio_github.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/requirements-devel.txt` & `invenio-github-1.0.1/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/run-tests.sh` & `invenio-github-1.0.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/setup.cfg` & `invenio-github-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-github-1.0.0b7/setup.py` & `invenio-github-1.0.1/setup.py`

 * *Files identical despite different names*

