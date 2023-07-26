# Comparing `tmp/invenio-formatter-2.0.0.tar.gz` & `tmp/invenio-formatter-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-formatter-2.0.0.tar", last modified: Wed Jul 19 14:55:35 2023, max compression
+gzip compressed data, was "dist/invenio-formatter-2.0.1.tar", last modified: Wed Jul 26 07:28:52 2023, max compression
```

## Comparing `invenio-formatter-2.0.0.tar` & `invenio-formatter-2.0.1.tar`

### file list

```diff
@@ -1,273 +1,273 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (122)      458 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (122)      494 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1289 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3755 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      803 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3400 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     7453 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10113 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/docs/examplesapp.rst
--rw-r--r--   0 runner    (1001) docker     (122)      845 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7003 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/examples/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/examples/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/examples/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/
--rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/context_processors/
--rw-r--r--   0 runner    (1001) docker     (122)      329 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/context_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3550 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/context_processors/badges.py
--rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/filters/datetime.py
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/filters/html.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/templates/invenio_formatter/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/templates/invenio_formatter/macros/
--rw-r--r--   0 runner    (1001) docker     (122)     1194 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/templates/invenio_formatter/macros/badges.html
--rw-r--r--   0 runner    (1001) docker     (122)     2306 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/templates/invenio_formatter/macros/meta.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/templates/semantic-ui/invenio_formatter/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html
--rw-r--r--   0 runner    (1001) docker     (122)     2306 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/meta.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1615 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1693 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      464 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      533 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      490 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/en_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      767 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      719 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1632 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1627 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      567 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      590 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1616 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1627 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      590 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1748 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      651 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ne/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      519 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1760 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      655 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      684 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      777 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1877 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      757 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1855 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      525 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (122)     2274 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/invenio_formatter/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/invenio_formatter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3400 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7310 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-19 14:55:34.000000 invenio-formatter-2.0.0/invenio_formatter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      577 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-19 14:55:35.000000 invenio-formatter-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/tests/test_examples_app.py
--rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/tests/test_invenio_formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/tests/test_template_context_processors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/tests/test_template_macros.py
--rw-r--r--   0 runner    (1001) docker     (122)     3234 2023-07-19 14:55:26.000000 invenio-formatter-2.0.0/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/.tx/
+-rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (122)      494 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1357 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3755 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      803 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      499 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7453 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10113 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/docs/examplesapp.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      845 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7003 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/examples/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/examples/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/examples/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/context_processors/
+-rw-r--r--   0 runner    (1001) docker     (122)      329 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/context_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3550 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/context_processors/badges.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/filters/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/filters/html.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/templates/invenio_formatter/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/templates/invenio_formatter/macros/
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/templates/invenio_formatter/macros/badges.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2306 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/templates/invenio_formatter/macros/meta.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/templates/semantic-ui/invenio_formatter/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/badges.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2306 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/meta.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1926 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1615 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1693 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      464 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1667 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1798 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1632 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1627 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1616 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1627 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1748 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1633 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1654 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      651 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1760 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      571 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1669 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      777 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1877 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1839 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1855 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1747 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-07-26 07:28:51.000000 invenio-formatter-2.0.1/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2274 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/invenio_formatter/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7310 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/invenio_formatter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      577 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 07:28:52.000000 invenio-formatter-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/tests/test_examples_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/tests/test_invenio_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/tests/test_template_context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2882 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/tests/test_template_macros.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3234 2023-07-26 07:28:39.000000 invenio-formatter-2.0.1/tests/test_views.py
```

### Comparing `invenio-formatter-2.0.0/.editorconfig` & `invenio-formatter-2.0.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/.github/workflows/pypi-publish.yml` & `invenio-formatter-2.0.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/.github/workflows/tests.yml` & `invenio-formatter-2.0.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/.tx/config` & `invenio-formatter-2.0.1/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/CHANGES.rst` & `invenio-formatter-2.0.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.0.1 (released 2023-07-26)
+
+- badges: semantic html Fixes
+
 Version 2.0.0 (released 2023-07-19)
 
 - setup: bump pillow minimum version
 
 Version 1.3.0 (released 2023-07-17)
 
 - add template filter for human readable time
```

### Comparing `invenio-formatter-2.0.0/CONTRIBUTING.rst` & `invenio-formatter-2.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/INSTALL.rst` & `invenio-formatter-2.0.1/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/LICENSE` & `invenio-formatter-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/MANIFEST.in` & `invenio-formatter-2.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/PKG-INFO` & `invenio-formatter-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-formatter
-Version: 2.0.0
+Version: 2.0.1
 Summary: "Jinja utilities for Invenio."
 Home-page: https://github.com/inveniosoftware/invenio-formatter
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -41,14 +41,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.0.1 (released 2023-07-26)
+        
+        - badges: semantic html Fixes
+        
         Version 2.0.0 (released 2023-07-19)
         
         - setup: bump pillow minimum version
         
         Version 1.3.0 (released 2023-07-17)
         
         - add template filter for human readable time
```

### Comparing `invenio-formatter-2.0.0/README.rst` & `invenio-formatter-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/docs/Makefile` & `invenio-formatter-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/docs/api.rst` & `invenio-formatter-2.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/docs/conf.py` & `invenio-formatter-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/docs/index.rst` & `invenio-formatter-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/docs/make.bat` & `invenio-formatter-2.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/examples/app.py` & `invenio-formatter-2.0.1/examples/app.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/__init__.py` & `invenio-formatter-2.0.1/invenio_formatter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,10 +66,10 @@
 <http://localhost:5000/badge/ISBN/9780399547331.svg>`_.
 """
 
 from __future__ import absolute_import, print_function
 
 from .ext import InvenioFormatter
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 
 __all__ = ("__version__", "InvenioFormatter")
```

### Comparing `invenio-formatter-2.0.0/invenio_formatter/config.py` & `invenio-formatter-2.0.1/invenio_formatter/config.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/context_processors/badges.py` & `invenio-formatter-2.0.1/invenio_formatter/context_processors/badges.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/ext.py` & `invenio-formatter-2.0.1/invenio_formatter/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/filters/datetime.py` & `invenio-formatter-2.0.1/invenio_formatter/filters/datetime.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/filters/html.py` & `invenio-formatter-2.0.1/invenio_formatter/filters/html.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/templates/invenio_formatter/macros/meta.html` & `invenio-formatter-2.0.1/invenio_formatter/templates/invenio_formatter/macros/meta.html`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/meta.html` & `invenio-formatter-2.0.1/invenio_formatter/templates/semantic-ui/invenio_formatter/macros/meta.html`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/af/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/af/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/ar/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/ar/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/bg/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/bg/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/ca/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/ca/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/cs/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/cs/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/da/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/da/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/de/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/de/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/el/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/el/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/en/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/en_HU/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/es/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/es/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/et/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/et/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/fa/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/fa/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/fr/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/fr/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/gl/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/gl/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/hr/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/hr/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/hu/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/hu/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/it/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/it/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/ja/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/ka/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/ka/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/lt/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/lt/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/messages.pot` & `invenio-formatter-2.0.1/invenio_formatter/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/ne/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/ne/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/ne/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/no/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/no/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/pl/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/pl/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/pt/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/pt/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/ro/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/ro/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/ru/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/ru/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/rw/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/rw/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/sk/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/sk/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/sv/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/sv/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/tr/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/tr/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/uk/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/uk/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-formatter-2.0.1/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-formatter-2.0.1/invenio_formatter/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter/views.py` & `invenio-formatter-2.0.1/invenio_formatter/views.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/invenio_formatter.egg-info/PKG-INFO` & `invenio-formatter-2.0.1/invenio_formatter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-formatter
-Version: 2.0.0
+Version: 2.0.1
 Summary: "Jinja utilities for Invenio."
 Home-page: https://github.com/inveniosoftware/invenio-formatter
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -41,14 +41,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.0.1 (released 2023-07-26)
+        
+        - badges: semantic html Fixes
+        
         Version 2.0.0 (released 2023-07-19)
         
         - setup: bump pillow minimum version
         
         Version 1.3.0 (released 2023-07-17)
         
         - add template filter for human readable time
```

### Comparing `invenio-formatter-2.0.0/invenio_formatter.egg-info/SOURCES.txt` & `invenio-formatter-2.0.1/invenio_formatter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/run-tests.sh` & `invenio-formatter-2.0.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/setup.cfg` & `invenio-formatter-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/tests/conftest.py` & `invenio-formatter-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/tests/test_examples_app.py` & `invenio-formatter-2.0.1/tests/test_examples_app.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/tests/test_filters.py` & `invenio-formatter-2.0.1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/tests/test_invenio_formatter.py` & `invenio-formatter-2.0.1/tests/test_invenio_formatter.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/tests/test_template_context_processors.py` & `invenio-formatter-2.0.1/tests/test_template_context_processors.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/tests/test_template_macros.py` & `invenio-formatter-2.0.1/tests/test_template_macros.py`

 * *Files identical despite different names*

### Comparing `invenio-formatter-2.0.0/tests/test_views.py` & `invenio-formatter-2.0.1/tests/test_views.py`

 * *Files identical despite different names*

