# Comparing `tmp/django-waffle-3.0.0.tar.gz` & `tmp/django-waffle-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-waffle-3.0.0.tar", last modified: Tue Aug 30 17:29:03 2022, max compression
+gzip compressed data, was "django-waffle-4.0.0.tar", last modified: Wed Jul 26 04:58:34 2023, max compression
```

## Comparing `django-waffle-3.0.0.tar` & `django-waffle-4.0.0.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.842712 django-waffle-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-08-30 17:28:57.000000 django-waffle-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-08-30 17:28:57.000000 django-waffle-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-08-30 17:29:03.842712 django-waffle-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-08-30 17:28:57.000000 django-waffle-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.834711 django-waffle-3.0.0/django_waffle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-08-30 17:29:03.000000 django-waffle-3.0.0/django_waffle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1663 2022-08-30 17:29:03.000000 django-waffle-3.0.0/django_waffle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-30 17:29:03.000000 django-waffle-3.0.0/django_waffle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-30 17:29:03.000000 django-waffle-3.0.0/django_waffle.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-30 17:29:03.000000 django-waffle-3.0.0/django_waffle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-08-30 17:29:03.842712 django-waffle-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-08-30 17:28:57.000000 django-waffle-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.834711 django-waffle-3.0.0/test_app/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.834711 django-waffle-3.0.0/test_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     4126 2022-08-30 17:28:57.000000 django-waffle-3.0.0/test_app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     2904 2022-08-30 17:28:57.000000 django-waffle-3.0.0/test_app/migrations/0002_auto_20220717_1934.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 17:28:57.000000 django-waffle-3.0.0/test_app/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.838712 django-waffle-3.0.0/waffle/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1896 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4725 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1895 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/jinja.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.834711 django-waffle-3.0.0/waffle/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.834711 django-waffle-3.0.0/waffle/locale/en_US/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.838712 django-waffle-3.0.0/waffle/locale/en_US/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/locale/en_US/LC_MESSAGES/django.mo
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.834711 django-waffle-3.0.0/waffle/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.838712 django-waffle-3.0.0/waffle/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     4257 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/locale/it/LC_MESSAGES/django.mo
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.834711 django-waffle-3.0.0/waffle/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.838712 django-waffle-3.0.0/waffle/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     5757 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/locale/ru/LC_MESSAGES/django.mo
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.838712 django-waffle-3.0.0/waffle/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.838712 django-waffle-3.0.0/waffle/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1836 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/management/commands/waffle_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)     7095 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/management/commands/waffle_flag.py
--rw-r--r--   0 runner    (1001) docker     (121)     2225 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/management/commands/waffle_sample.py
--rw-r--r--   0 runner    (1001) docker     (121)     2275 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/management/commands/waffle_switch.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/managers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.838712 django-waffle-3.0.0/waffle/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     4472 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/migrations/0002_auto_20161201_0958.py
--rw-r--r--   0 runner    (1001) docker     (121)     6755 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/migrations/0003_update_strings_for_i18n.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/migrations/0004_update_everyone_nullbooleanfield.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)    16951 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.834711 django-waffle-3.0.0/waffle/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.838712 django-waffle-3.0.0/waffle/templates/waffle/
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/templates/waffle/waffle.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.838712 django-waffle-3.0.0/waffle/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/templatetags/waffle_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 17:29:03.842712 django-waffle-3.0.0/waffle/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/tests/base.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7149 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     5286 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)    13010 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)     3650 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2378 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (121)    12443 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/tests/test_testutils.py
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4357 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)    32392 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/tests/test_waffle.py
--rw-r--r--   0 runner    (1001) docker     (121)     2977 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/testutils.py
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2028 2022-08-30 17:28:57.000000 django-waffle-3.0.0/waffle/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.863829 django-waffle-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-26 04:58:24.000000 django-waffle-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-26 04:58:24.000000 django-waffle-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-26 04:58:34.863829 django-waffle-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-26 04:58:24.000000 django-waffle-4.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.847829 django-waffle-4.0.0/django_waffle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-26 04:58:34.000000 django-waffle-4.0.0/django_waffle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-26 04:58:34.000000 django-waffle-4.0.0/django_waffle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 04:58:34.000000 django-waffle-4.0.0/django_waffle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 04:58:34.000000 django-waffle-4.0.0/django_waffle.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 04:58:34.000000 django-waffle-4.0.0/django_waffle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 04:58:34.000000 django-waffle-4.0.0/django_waffle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-26 04:58:24.000000 django-waffle-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 04:58:34.863829 django-waffle-4.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.839829 django-waffle-4.0.0/test_app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.847829 django-waffle-4.0.0/test_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-07-26 04:58:24.000000 django-waffle-4.0.0/test_app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-26 04:58:24.000000 django-waffle-4.0.0/test_app/migrations/0002_auto_20220717_1934.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:24.000000 django-waffle-4.0.0/test_app/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.851829 django-waffle-4.0.0/waffle/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2310 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4747 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/jinja.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.839829 django-waffle-4.0.0/waffle/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.839829 django-waffle-4.0.0/waffle/locale/en_US/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.855829 django-waffle-4.0.0/waffle/locale/en_US/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/locale/en_US/LC_MESSAGES/django.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.839829 django-waffle-4.0.0/waffle/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.855829 django-waffle-4.0.0/waffle/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/locale/it/LC_MESSAGES/django.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.839829 django-waffle-4.0.0/waffle/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.855829 django-waffle-4.0.0/waffle/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/locale/ru/LC_MESSAGES/django.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.855829 django-waffle-4.0.0/waffle/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.855829 django-waffle-4.0.0/waffle/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/management/commands/waffle_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/management/commands/waffle_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/management/commands/waffle_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/management/commands/waffle_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.859829 django-waffle-4.0.0/waffle/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/migrations/0002_auto_20161201_0958.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/migrations/0003_update_strings_for_i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/migrations/0004_update_everyone_nullbooleanfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.843829 django-waffle-4.0.0/waffle/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.859829 django-waffle-4.0.0/waffle/templates/waffle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/templates/waffle/waffle.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.859829 django-waffle-4.0.0/waffle/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/templatetags/waffle_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:34.863829 django-waffle-4.0.0/waffle/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/tests/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7149 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/tests/test_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32392 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/tests/test_waffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-26 04:58:24.000000 django-waffle-4.0.0/waffle/views.py
```

### Comparing `django-waffle-3.0.0/LICENSE` & `django-waffle-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/PKG-INFO` & `django-waffle-4.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-waffle
-Version: 3.0.0
+Version: 4.0.0
 Summary: A feature flipper for Django.
-Home-page: http://github.com/django-waffle/django-waffle
-Author: James Socol
-Author-email: me@jamessocol.com
+Author-email: James Socol <me@jamessocol.com>
 License: BSD
-Description: ======
-        README
-        ======
-        
-        Django Waffle is (yet another) feature flipper for Django. You can
-        define the conditions for which a flag should be active, and use it in
-        a number of ways.
-        
-        .. image:: https://github.com/django-waffle/django-waffle/workflows/Python%20package/badge.svg?branch=master
-           :target: https://github.com/django-waffle/django-waffle/actions
-           :alt: Build Status
-        .. image:: https://badge.fury.io/py/django-waffle.svg
-           :target: https://badge.fury.io/py/django-waffle
-           :alt: PyPI status badge
-        
-        :Code:          https://github.com/django-waffle/django-waffle
-        :License:       BSD; see LICENSE file
-        :Issues:        https://github.com/django-waffle/django-waffle/issues
-        :Documentation: https://waffle.readthedocs.io/
-        
-Platform: UNKNOWN
+Project-URL: Homepage, http://github.com/django-waffle/django-waffle
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+======
+README
+======
+
+Django Waffle is (yet another) feature flipper for Django. You can
+define the conditions for which a flag should be active, and use it in
+a number of ways.
+
+.. image:: https://github.com/django-waffle/django-waffle/workflows/Python%20package/badge.svg?branch=master
+   :target: https://github.com/django-waffle/django-waffle/actions
+   :alt: Build Status
+.. image:: https://badge.fury.io/py/django-waffle.svg
+   :target: https://badge.fury.io/py/django-waffle
+   :alt: PyPI status badge
+
+:Code:          https://github.com/django-waffle/django-waffle
+:License:       BSD; see LICENSE file
+:Issues:        https://github.com/django-waffle/django-waffle/issues
+:Documentation: https://waffle.readthedocs.io/
```

### Comparing `django-waffle-3.0.0/README.rst` & `django-waffle-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/django_waffle.egg-info/PKG-INFO` & `django-waffle-4.0.0/django_waffle.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-waffle
-Version: 3.0.0
+Version: 4.0.0
 Summary: A feature flipper for Django.
-Home-page: http://github.com/django-waffle/django-waffle
-Author: James Socol
-Author-email: me@jamessocol.com
+Author-email: James Socol <me@jamessocol.com>
 License: BSD
-Description: ======
-        README
-        ======
-        
-        Django Waffle is (yet another) feature flipper for Django. You can
-        define the conditions for which a flag should be active, and use it in
-        a number of ways.
-        
-        .. image:: https://github.com/django-waffle/django-waffle/workflows/Python%20package/badge.svg?branch=master
-           :target: https://github.com/django-waffle/django-waffle/actions
-           :alt: Build Status
-        .. image:: https://badge.fury.io/py/django-waffle.svg
-           :target: https://badge.fury.io/py/django-waffle
-           :alt: PyPI status badge
-        
-        :Code:          https://github.com/django-waffle/django-waffle
-        :License:       BSD; see LICENSE file
-        :Issues:        https://github.com/django-waffle/django-waffle/issues
-        :Documentation: https://waffle.readthedocs.io/
-        
-Platform: UNKNOWN
+Project-URL: Homepage, http://github.com/django-waffle/django-waffle
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+======
+README
+======
+
+Django Waffle is (yet another) feature flipper for Django. You can
+define the conditions for which a flag should be active, and use it in
+a number of ways.
+
+.. image:: https://github.com/django-waffle/django-waffle/workflows/Python%20package/badge.svg?branch=master
+   :target: https://github.com/django-waffle/django-waffle/actions
+   :alt: Build Status
+.. image:: https://badge.fury.io/py/django-waffle.svg
+   :target: https://badge.fury.io/py/django-waffle
+   :alt: PyPI status badge
+
+:Code:          https://github.com/django-waffle/django-waffle
+:License:       BSD; see LICENSE file
+:Issues:        https://github.com/django-waffle/django-waffle/issues
+:Documentation: https://waffle.readthedocs.io/
```

### Comparing `django-waffle-3.0.0/django_waffle.egg-info/SOURCES.txt` & `django-waffle-4.0.0/django_waffle.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 LICENSE
 MANIFEST.in
 README.rst
-setup.cfg
-setup.py
+pyproject.toml
 django_waffle.egg-info/PKG-INFO
 django_waffle.egg-info/SOURCES.txt
 django_waffle.egg-info/dependency_links.txt
 django_waffle.egg-info/not-zip-safe
+django_waffle.egg-info/requires.txt
 django_waffle.egg-info/top_level.txt
 test_app/migrations/0001_initial.py
 test_app/migrations/0002_auto_20220717_1934.py
 test_app/migrations/__init__.py
 waffle/__init__.py
 waffle/admin.py
 waffle/apps.py
 waffle/decorators.py
 waffle/defaults.py
 waffle/jinja.py
 waffle/managers.py
 waffle/middleware.py
 waffle/mixins.py
 waffle/models.py
+waffle/py.typed
 waffle/signals.py
 waffle/testutils.py
 waffle/urls.py
 waffle/utils.py
 waffle/views.py
 waffle/locale/en_US/LC_MESSAGES/django.mo
 waffle/locale/it/LC_MESSAGES/django.mo
```

### Comparing `django-waffle-3.0.0/test_app/migrations/0001_initial.py` & `django-waffle-4.0.0/test_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/test_app/migrations/0002_auto_20220717_1934.py` & `django-waffle-4.0.0/test_app/migrations/0002_auto_20220717_1934.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/__init__.py` & `django-waffle-4.0.0/waffle/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,54 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 import django
 from django.core.exceptions import ImproperlyConfigured
+from django.http import HttpRequest
 
 from waffle.utils import get_setting
 from django.apps import apps as django_apps
 
-VERSION = (3, 0, 0)
-__version__ = '.'.join(map(str, VERSION))
+if TYPE_CHECKING:
+    from waffle.models import AbstractBaseFlag, AbstractBaseSample, AbstractBaseSwitch
+
+__version__ = '4.0.0'
 
 
-def flag_is_active(request, flag_name, read_only=False):
+def flag_is_active(request: HttpRequest, flag_name: str, read_only: bool = False) -> bool | None:
     flag = get_waffle_flag_model().get(flag_name)
     return flag.is_active(request, read_only=read_only)
 
 
-def switch_is_active(switch_name):
+def switch_is_active(switch_name: str) -> bool:
     switch = get_waffle_switch_model().get(switch_name)
     return switch.is_active()
 
 
-def sample_is_active(sample_name):
+def sample_is_active(sample_name: str) -> bool:
     sample = get_waffle_sample_model().get(sample_name)
     return sample.is_active()
 
 
-def get_waffle_flag_model():
+def get_waffle_flag_model() -> type[AbstractBaseFlag]:
     return get_waffle_model('FLAG_MODEL')
 
 
-def get_waffle_switch_model():
+def get_waffle_switch_model() -> type[AbstractBaseSwitch]:
     return get_waffle_model('SWITCH_MODEL')
 
 
-def get_waffle_sample_model():
+def get_waffle_sample_model() -> type[AbstractBaseSample]:
     return get_waffle_model('SAMPLE_MODEL')
 
 
-def get_waffle_model(setting_name):
+def get_waffle_model(setting_name: str) -> (
+    type[AbstractBaseFlag] | type[AbstractBaseSwitch] | type[AbstractBaseSample]
+):
     """
     Returns the waffle Flag model that is active in this project.
     """
     default_model = {
         'FLAG_MODEL': 'waffle.Flag',
         'SWITCH_MODEL': 'waffle.Switch',
         'SAMPLE_MODEL': 'waffle.Sample',
```

### Comparing `django-waffle-3.0.0/waffle/admin.py` & `django-waffle-4.0.0/waffle/admin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+from __future__ import annotations
+
+from typing import Any
+
 from django.contrib import admin
 from django.contrib.admin.models import LogEntry, CHANGE, DELETION
 from django.contrib.admin.widgets import ManyToManyRawIdWidget
 from django.contrib.contenttypes.models import ContentType
+from django.http import HttpRequest
 from django.utils.html import escape
 from django.utils.translation import gettext_lazy as _
 
 from waffle.models import Flag, Sample, Switch
 from waffle.utils import get_setting
 
 
 class BaseAdmin(admin.ModelAdmin):
     search_fields = ('name', 'note')
 
-    def get_actions(self, request):
+    def get_actions(self, request: HttpRequest) -> dict[str, Any]:
         actions = super().get_actions(request)
         if 'delete_selected' in actions:
             del actions['delete_selected']
         return actions
 
 
 def _add_log_entry(user, model, description, action_flag):
@@ -25,53 +30,56 @@
         content_type=ContentType.objects.get_for_model(type(model)),
         object_id=model.id,
         object_repr=model.name + " " + description,
         action_flag=action_flag
     )
 
 
+@admin.action(
+    description=_('Enable selected flags for everyone'),
+    permissions=('change',),
+)
 def enable_for_all(ma, request, qs):
     # Iterate over all objects to cause cache invalidation.
     for f in qs.all():
         _add_log_entry(request.user, f, "on", CHANGE)
         f.everyone = True
         f.save()
 
 
+@admin.action(
+    description=_('Disable selected flags for everyone'),
+    permissions=('change',),
+)
 def disable_for_all(ma, request, qs):
     # Iterate over all objects to cause cache invalidation.
     for f in qs.all():
         _add_log_entry(request.user, f, "off", CHANGE)
         f.everyone = False
         f.save()
 
 
+@admin.action(
+    description=_('Delete selected'),
+    permissions=('delete',),
+)
 def delete_individually(ma, request, qs):
     # Iterate over all objects to cause cache invalidation.
     for f in qs.all():
         _add_log_entry(request.user, f, "deleted", DELETION)
         f.delete()
 
 
-enable_for_all.short_description = _('Enable selected flags for everyone')
-disable_for_all.short_description = _('Disable selected flags for everyone')
-delete_individually.short_description = _('Delete selected')
-
-enable_for_all.allowed_permissions = ('change',)
-disable_for_all.allowed_permissions = ('change',)
-delete_individually.allowed_permissions = ('delete',)
-
-
 class InformativeManyToManyRawIdWidget(ManyToManyRawIdWidget):
     """Widget for ManyToManyField to Users.
 
     Will display the names of the users in a parenthesised list after the
     input field. This widget works with all models that have a "name" field.
     """
-    def label_and_url_for_value(self, values):
+    def label_and_url_for_value(self, values: Any) -> tuple[str, str]:
         names = []
         key = self.rel.get_related_field().name
         for value in values:
             try:
                 name = self.rel.model._default_manager \
                     .using(self.db) \
                     .get(**{key: value})
@@ -96,35 +104,36 @@
                 InformativeManyToManyRawIdWidget(db_field.remote_field,
                                                  self.admin_site,
                                                  using=kwargs.get("using"))
             return db_field.formfield(**kwargs)
         return super().formfield_for_dbfield(db_field, **kwargs)
 
 
+@admin.action(
+    description=_('Enable selected switches'),
+    permissions=('change',),
+)
 def enable_switches(ma, request, qs):
     for switch in qs:
         _add_log_entry(request.user, switch, "on", CHANGE)
         switch.active = True
         switch.save()
 
 
+@admin.action(
+    description=_('Disable selected switches'),
+    permissions=('change',),
+)
 def disable_switches(ma, request, qs):
     for switch in qs:
         _add_log_entry(request.user, switch, "off", CHANGE)
         switch.active = False
         switch.save()
 
 
-enable_switches.short_description = _('Enable selected switches')
-disable_switches.short_description = _('Disable selected switches')
-
-enable_switches.allowed_permissions = ('change',)
-disable_switches.allowed_permissions = ('change',)
-
-
 class SwitchAdmin(BaseAdmin):
     actions = [enable_switches, disable_switches, delete_individually]
     list_display = ('name', 'active', 'note', 'created', 'modified')
     list_filter = ('active',)
     ordering = ('-id',)
```

### Comparing `django-waffle-3.0.0/waffle/defaults.py` & `django-waffle-4.0.0/waffle/defaults.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/jinja.py` & `django-waffle-4.0.0/waffle/jinja.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from waffle.views import _generate_waffle_js
 
 
 try:
     from jinja2 import pass_context
 except ImportError:
     # NOTE: We can get rid of this when we stop supporting Jinja2 < 3.
-    from jinja2 import contextfunction as pass_context
+    from jinja2 import contextfunction as pass_context  # type: ignore
 
 
 @pass_context
 def flag_helper(context, flag_name):
     return flag_is_active(context['request'], flag_name)
```

### Comparing `django-waffle-3.0.0/waffle/locale/it/LC_MESSAGES/django.mo` & `django-waffle-4.0.0/waffle/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/locale/ru/LC_MESSAGES/django.mo` & `django-waffle-4.0.0/waffle/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/management/commands/waffle_delete.py` & `django-waffle-4.0.0/waffle/management/commands/waffle_delete.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from django.core.management.base import BaseCommand
+from typing import Any
+
+from django.core.management.base import BaseCommand, CommandParser
 
 from waffle import (
     get_waffle_flag_model,
     get_waffle_switch_model,
     get_waffle_sample_model,
 )
 
 
 class Command(BaseCommand):
-    def add_arguments(self, parser):
+    def add_arguments(self, parser: CommandParser) -> None:
         parser.add_argument(
             '--flags',
             action='store',
             dest='flag_names',
             nargs='*',
             help='List of flag names to delete.')
         parser.add_argument(
@@ -26,15 +28,15 @@
             action='store',
             dest='switch_names',
             nargs='*',
             help='List of switch names to delete.')
 
     help = 'Delete flags, samples, and switches from database'
 
-    def handle(self, *args, **options):
+    def handle(self, *args: Any, **options: Any) -> None:
         flags = options['flag_names']
         if flags:
             flag_queryset = get_waffle_flag_model().objects.filter(name__in=flags)
             flag_count = flag_queryset.count()
             flag_queryset.delete()
             self.stdout.write('Deleted %s Flags' % flag_count)
```

### Comparing `django-waffle-3.0.0/waffle/management/commands/waffle_flag.py` & `django-waffle-4.0.0/waffle/management/commands/waffle_flag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from typing import Any
+
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Group
-from django.core.management.base import BaseCommand, CommandError
+from django.core.management.base import BaseCommand, CommandError, CommandParser
 from django.db.models import Q
 
 from waffle import get_waffle_flag_model
 
 UserModel = get_user_model()
 
 
 class Command(BaseCommand):
-    def add_arguments(self, parser):
+    def add_arguments(self, parser: CommandParser) -> None:
         parser.add_argument(
             'name',
             nargs='?',
             help='The name of the flag.')
         parser.add_argument(
             '-l', '--list',
             action='store_true',
@@ -87,15 +89,15 @@
             dest='create',
             default=False,
             help='If the flag doesn\'t exist, create it.')
         parser.set_defaults(everyone=None)
 
     help = 'Modify a flag.'
 
-    def handle(self, *args, **options):
+    def handle(self, *args: Any, **options: Any) -> None:
         if options['list_flags']:
             self.stdout.write('Flags:')
             for flag in get_waffle_flag_model().objects.iterator():
                 self.stdout.write('NAME: %s' % flag.name)
                 self.stdout.write('SUPERUSERS: %s' % flag.superusers)
                 self.stdout.write('EVERYONE: %s' % flag.everyone)
                 self.stdout.write('AUTHENTICATED: %s' % flag.authenticated)
@@ -104,15 +106,15 @@
                 self.stdout.write('ROLLOUT: %s' % flag.rollout)
                 self.stdout.write('STAFF: %s' % flag.staff)
                 self.stdout.write('GROUPS: %s' % list(
                     flag.groups.values_list('name', flat=True))
                 )
                 self.stdout.write('USERS: %s' % list(
                     flag.users.values_list(UserModel.USERNAME_FIELD, flat=True))
-                                  )
+                )
                 self.stdout.write('')
             return
 
         flag_name = options['name']
 
         if not flag_name:
             raise CommandError('You need to specify a flag name.')
```

### Comparing `django-waffle-3.0.0/waffle/management/commands/waffle_sample.py` & `django-waffle-4.0.0/waffle/management/commands/waffle_sample.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from django.core.management.base import BaseCommand, CommandError
+from typing import Any
+
+from django.core.management.base import BaseCommand, CommandError, CommandParser
 
 from waffle import get_waffle_sample_model
 
+
 class Command(BaseCommand):
-    def add_arguments(self, parser):
+    def add_arguments(self, parser: CommandParser) -> None:
         parser.add_argument(
             'name',
             nargs='?',
             help='The name of the sample.')
         parser.add_argument(
             'percent',
             nargs='?',
@@ -22,15 +25,15 @@
             action='store_true',
             dest='create',
             default=False,
             help='If the sample does not exist, create it.')
 
     help = 'Change percentage of a sample.'
 
-    def handle(self, *args, **options):
+    def handle(self, *args: Any, **options: Any) -> None:
         if options['list_samples']:
             self.stdout.write('Samples:')
             for sample in get_waffle_sample_model().objects.iterator():
                 self.stdout.write(f'{sample.name}: {sample.percent:.1f}%')
             self.stdout.write('')
             return
```

### Comparing `django-waffle-3.0.0/waffle/management/commands/waffle_switch.py` & `django-waffle-4.0.0/waffle/management/commands/waffle_switch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from typing import Any
+
 from argparse import ArgumentTypeError
-from django.core.management.base import BaseCommand, CommandError
+from django.core.management.base import BaseCommand, CommandError, CommandParser
 
 from waffle import get_waffle_switch_model
 
 
-def on_off_bool(string):
+def on_off_bool(string: str) -> bool:
     if string not in ['on', 'off']:
         raise ArgumentTypeError("invalid choice: %r (choose from 'on', "
                                 "'off')" % string)
     return string == 'on'
 
 
 class Command(BaseCommand):
-    def add_arguments(self, parser):
+    def add_arguments(self, parser: CommandParser) -> None:
         parser.add_argument(
             'name',
             nargs='?',
             help='The name of the switch.')
         parser.add_argument(
             'state',
             nargs='?',
@@ -33,15 +35,15 @@
             action='store_true',
             dest='create',
             default=False,
             help='If the switch does not exist, create it.')
 
     help = 'Activate or deactivate a switch.'
 
-    def handle(self, *args, **options):
+    def handle(self, *args: Any, **options: Any) -> None:
         if options['list_switches']:
             self.stdout.write('Switches:')
             for switch in get_waffle_switch_model().objects.iterator():
                 self.stdout.write(
                     '{}: {}'.format(switch.name, 'on' if switch.active else 'off')
                 )
             self.stdout.write('')
```

### Comparing `django-waffle-3.0.0/waffle/middleware.py` & `django-waffle-4.0.0/waffle/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from django.http import HttpRequest, HttpResponse
 from django.utils.deprecation import MiddlewareMixin
 from django.utils.encoding import smart_str
 
 from waffle.utils import get_setting
 
 
 class WaffleMiddleware(MiddlewareMixin):
-    def process_response(self, request, response):
+    def process_response(self, request: HttpRequest, response: HttpResponse) -> HttpResponse:
         secure = get_setting('SECURE')
         max_age = get_setting('MAX_AGE')
 
         if hasattr(request, 'waffles'):
             for k in request.waffles:
                 name = smart_str(get_setting('COOKIE') % k)
                 active, rollout = request.waffles[k]
```

### Comparing `django-waffle-3.0.0/waffle/migrations/0001_initial.py` & `django-waffle-4.0.0/waffle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/migrations/0003_update_strings_for_i18n.py` & `django-waffle-4.0.0/waffle/migrations/0003_update_strings_for_i18n.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/migrations/0004_update_everyone_nullbooleanfield.py` & `django-waffle-4.0.0/waffle/migrations/0004_update_everyone_nullbooleanfield.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/mixins.py` & `django-waffle-4.0.0/waffle/mixins.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from functools import partial
 
 from django.http import Http404
 
 from waffle import switch_is_active, flag_is_active, sample_is_active
 
 
@@ -20,15 +22,15 @@
 
 class WaffleFlagMixin(BaseWaffleMixin):
     """
     Checks that as flag is active, or 404. Operates like the FBV decorator
     waffle_flag
     """
 
-    waffle_flag = None
+    waffle_flag: str | None = None
 
     def dispatch(self, request, *args, **kwargs):
         func = partial(flag_is_active, request)
         active = self.validate_waffle(self.waffle_flag, func)
 
         if not active:
             return self.invalid_waffle()
@@ -38,15 +40,15 @@
 
 class WaffleSampleMixin(BaseWaffleMixin):
     """
     Checks that as switch is active, or 404. Operates like the FBV decorator
     waffle_sample.
     """
 
-    waffle_sample = None
+    waffle_sample: str | None = None
 
     def dispatch(self, request, *args, **kwargs):
         active = self.validate_waffle(self.waffle_sample, sample_is_active)
 
         if not active:
             return self.invalid_waffle()
 
@@ -55,15 +57,15 @@
 
 class WaffleSwitchMixin(BaseWaffleMixin):
     """
     Checks that as switch is active, or 404. Operates like the FBV decorator
     waffle_switch.
     """
 
-    waffle_switch = None
+    waffle_switch: str | None = None
 
     def dispatch(self, request, *args, **kwargs):
         active = self.validate_waffle(self.waffle_switch, switch_is_active)
 
         if not active:
             return self.invalid_waffle()
```

### Comparing `django-waffle-3.0.0/waffle/models.py` & `django-waffle-4.0.0/waffle/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from __future__ import annotations
+
+import logging
 import random
 from decimal import Decimal
-import logging
+from typing import Any, TypeVar
 
 from django.conf import settings
-from django.contrib.auth.models import Group
+from django.contrib.auth.models import AbstractBaseUser, Group
 from django.db import models, router, transaction
+from django.http import HttpRequest
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
 
 from waffle import (
     get_waffle_sample_model,
     get_waffle_switch_model,
     get_waffle_flag_model,
@@ -16,33 +20,37 @@
 )
 from waffle.utils import get_setting, keyfmt, get_cache
 
 logger = logging.getLogger('waffle')
 
 CACHE_EMPTY = '-'
 
+
+_BaseModelType = TypeVar("_BaseModelType", bound="BaseModel")
+
+
 class BaseModel(models.Model):
     SINGLE_CACHE_KEY = ''
     ALL_CACHE_KEY = ''
 
     class Meta:
         abstract = True
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.name
 
-    def natural_key(self):
+    def natural_key(self) -> tuple[str]:
         return (self.name,)
 
     @classmethod
-    def _cache_key(cls, name):
+    def _cache_key(cls, name: str) -> str:
         return keyfmt(get_setting(cls.SINGLE_CACHE_KEY), name)
 
     @classmethod
-    def get(cls, name):
+    def get(cls: type[_BaseModelType], name: str) -> _BaseModelType:
         cache = get_cache()
         cache_key = cls._cache_key(name)
         cached = cache.get(cache_key)
         if cached == CACHE_EMPTY:
             return cls(name=name)
         if cached:
             return cached
@@ -53,22 +61,22 @@
             cache.add(cache_key, CACHE_EMPTY)
             return cls(name=name)
 
         cache.add(cache_key, obj)
         return obj
 
     @classmethod
-    def get_from_db(cls, name):
+    def get_from_db(cls: type[_BaseModelType], name: str) -> _BaseModelType:
         objects = cls.objects
         if get_setting('READ_FROM_WRITE_DB'):
             objects = objects.using(router.db_for_write(cls))
         return objects.get(name=name)
 
     @classmethod
-    def get_all(cls):
+    def get_all(cls: type[_BaseModelType]) -> list[_BaseModelType]:
         cache = get_cache()
         cache_key = get_setting(cls.ALL_CACHE_KEY)
         cached = cache.get(cache_key)
         if cached == CACHE_EMPTY:
             return []
         if cached:
             return cached
@@ -78,47 +86,47 @@
             cache.add(cache_key, CACHE_EMPTY)
             return []
 
         cache.add(cache_key, objs)
         return objs
 
     @classmethod
-    def get_all_from_db(cls):
+    def get_all_from_db(cls: type[_BaseModelType]) -> list[_BaseModelType]:
         objects = cls.objects
         if get_setting('READ_FROM_WRITE_DB'):
             objects = objects.using(router.db_for_write(cls))
         return list(objects.all())
 
-    def flush(self):
+    def flush(self) -> None:
         cache = get_cache()
         keys = [
             self._cache_key(self.name),
             get_setting(self.ALL_CACHE_KEY),
         ]
         cache.delete_many(keys)
 
-    def save(self, *args, **kwargs):
+    def save(self, *args: Any, **kwargs: Any) -> None:
         self.modified = timezone.now()
         ret = super().save(*args, **kwargs)
         if hasattr(transaction, 'on_commit'):
             transaction.on_commit(self.flush)
         else:
             self.flush()
         return ret
 
-    def delete(self, *args, **kwargs):
+    def delete(self, *args: Any, **kwargs: Any) -> tuple[int, dict[str, int]]:
         ret = super().delete(*args, **kwargs)
         if hasattr(transaction, 'on_commit'):
             transaction.on_commit(self.flush)
         else:
             self.flush()
         return ret
 
 
-def set_flag(request, flag_name, active=True, session_only=False):
+def set_flag(request: HttpRequest, flag_name: str, active: bool | None = True, session_only: bool = False) -> None:
     """Set a flag value on a request object."""
     if not hasattr(request, 'waffles'):
         request.waffles = {}
     request.waffles[flag_name] = [active, session_only]
 
 
 class AbstractBaseFlag(BaseModel):
@@ -204,54 +212,54 @@
     ALL_CACHE_KEY = 'ALL_FLAGS_CACHE_KEY'
 
     class Meta:
         abstract = True
         verbose_name = _('Flag')
         verbose_name_plural = _('Flags')
 
-    def flush(self):
+    def flush(self) -> None:
         cache = get_cache()
         keys = self.get_flush_keys()
         cache.delete_many(keys)
 
-    def get_flush_keys(self, flush_keys=None):
+    def get_flush_keys(self, flush_keys: list[str] | None = None) -> list[str]:
         flush_keys = flush_keys or []
         flush_keys.extend([
             self._cache_key(self.name),
             get_setting('ALL_FLAGS_CACHE_KEY'),
         ])
         return flush_keys
 
-    def is_active_for_user(self, user):
+    def is_active_for_user(self, user: AbstractBaseUser) -> bool | None:
         if self.authenticated and user.is_authenticated:
             return True
 
         if self.staff and getattr(user, 'is_staff', False):
             return True
 
         if self.superusers and getattr(user, 'is_superuser', False):
             return True
 
         return None
 
-    def _is_active_for_user(self, request):
+    def _is_active_for_user(self, request: HttpRequest) -> bool | None:
         user = getattr(request, "user", None)
         if user:
             return self.is_active_for_user(user)
         return False
 
-    def _is_active_for_language(self, request):
+    def _is_active_for_language(self, request: HttpRequest) -> bool | None:
         if self.languages:
             languages = [ln.strip() for ln in self.languages.split(',')]
             if (hasattr(request, 'LANGUAGE_CODE') and
                     request.LANGUAGE_CODE in languages):
                 return True
         return None
 
-    def is_active(self, request, read_only=False):
+    def is_active(self, request: HttpRequest, read_only: bool = False) -> bool | None:
         if not self.pk:
             log_level = get_setting('LOG_MISSING_FLAGS')
             if log_level:
                 logger.log(log_level, 'Flag %s not found', self.name)
             if get_setting('CREATE_MISSING_FLAGS'):
                 flag, _created = get_waffle_flag_model().objects.get_or_create(
                     name=self.name,
@@ -337,23 +345,23 @@
     )
 
     class Meta(AbstractBaseFlag.Meta):
         abstract = True
         verbose_name = _('Flag')
         verbose_name_plural = _('Flags')
 
-    def get_flush_keys(self, flush_keys=None):
+    def get_flush_keys(self, flush_keys: list[str] | None = None) -> list[str]:
         flush_keys = super().get_flush_keys(flush_keys)
         flush_keys.extend([
             keyfmt(get_setting('FLAG_USERS_CACHE_KEY'), self.name),
             keyfmt(get_setting('FLAG_GROUPS_CACHE_KEY'), self.name),
         ])
         return flush_keys
 
-    def _get_user_ids(self):
+    def _get_user_ids(self) -> set[Any]:
         cache = get_cache()
         cache_key = keyfmt(get_setting('FLAG_USERS_CACHE_KEY'), self.name)
         cached = cache.get(cache_key)
         if cached == CACHE_EMPTY:
             return set()
         if cached:
             return cached
@@ -362,15 +370,15 @@
         if not user_ids:
             cache.add(cache_key, CACHE_EMPTY)
             return set()
 
         cache.add(cache_key, user_ids)
         return user_ids
 
-    def _get_group_ids(self):
+    def _get_group_ids(self) -> set[Any]:
         cache = get_cache()
         cache_key = keyfmt(get_setting('FLAG_GROUPS_CACHE_KEY'), self.name)
         cached = cache.get(cache_key)
         if cached == CACHE_EMPTY:
             return set()
         if cached:
             return cached
@@ -379,15 +387,15 @@
         if not group_ids:
             cache.add(cache_key, CACHE_EMPTY)
             return set()
 
         cache.add(cache_key, group_ids)
         return group_ids
 
-    def is_active_for_user(self, user):
+    def is_active_for_user(self, user: AbstractBaseUser) -> bool | None:
         is_active = super().is_active_for_user(user)
         if is_active:
             return is_active
 
         user_ids = self._get_user_ids()
         if hasattr(user, 'pk') and user.pk in user_ids:
             return True
@@ -455,15 +463,15 @@
     ALL_CACHE_KEY = 'ALL_SWITCHES_CACHE_KEY'
 
     class Meta:
         abstract = True
         verbose_name = _('Switch')
         verbose_name_plural = _('Switches')
 
-    def is_active(self):
+    def is_active(self) -> bool:
         if not self.pk:
             log_level = get_setting('LOG_MISSING_SWITCHES')
             if log_level:
                 logger.log(log_level, 'Switch %s not found', self.name)
             if get_setting('CREATE_MISSING_SWITCHES'):
                 switch, _created = get_waffle_switch_model().objects.get_or_create(
                     name=self.name, defaults={"active": get_setting("SWITCH_DEFAULT")}
@@ -520,15 +528,15 @@
     ALL_CACHE_KEY = 'ALL_SAMPLES_CACHE_KEY'
 
     class Meta:
         abstract = True
         verbose_name = _('Sample')
         verbose_name_plural = _('Samples')
 
-    def is_active(self):
+    def is_active(self) -> bool:
         if not self.pk:
             log_level = get_setting('LOG_MISSING_SAMPLES')
             if log_level:
                 logger.log(log_level, 'Sample %s not found', self.name)
             if get_setting('CREATE_MISSING_SAMPLES'):
 
                 default_percent = 100 if get_setting('SAMPLE_DEFAULT') else 0
```

### Comparing `django-waffle-3.0.0/waffle/signals.py` & `django-waffle-4.0.0/waffle/signals.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/templates/waffle/waffle.js` & `django-waffle-4.0.0/waffle/templates/waffle/waffle.js`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/templatetags/waffle_tags.py` & `django-waffle-4.0.0/waffle/templatetags/waffle_tags.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/tests/base.py` & `django-waffle-4.0.0/waffle/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/tests/test_admin.py` & `django-waffle-4.0.0/waffle/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/tests/test_decorators.py` & `django-waffle-4.0.0/waffle/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/tests/test_management.py` & `django-waffle-4.0.0/waffle/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/tests/test_middleware.py` & `django-waffle-4.0.0/waffle/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/tests/test_mixin.py` & `django-waffle-4.0.0/waffle/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/tests/test_models.py` & `django-waffle-4.0.0/waffle/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/tests/test_templates.py` & `django-waffle-4.0.0/waffle/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/tests/test_testutils.py` & `django-waffle-4.0.0/waffle/tests/test_testutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,39 +193,39 @@
         with override_sample('foo', active=True):
             assert waffle.sample_is_active('foo')
 
         with override_sample('foo', active=False):
             assert not waffle.sample_is_active('foo')
 
         self.assertEqual(Decimal('100.0'),
-                          waffle.get_waffle_sample_model().objects.get(name='foo').percent)
+                         waffle.get_waffle_sample_model().objects.get(name='foo').percent)
 
     def test_sample_existed_and_was_0(self):
         waffle.get_waffle_sample_model().objects.create(name='foo', percent='0.0')
 
         with override_sample('foo', active=True):
             assert waffle.sample_is_active('foo')
 
         with override_sample('foo', active=False):
             assert not waffle.sample_is_active('foo')
 
         self.assertEqual(Decimal('0.0'),
-                          waffle.get_waffle_sample_model().objects.get(name='foo').percent)
+                         waffle.get_waffle_sample_model().objects.get(name='foo').percent)
 
     def test_sample_existed_and_was_50(self):
         waffle.get_waffle_sample_model().objects.create(name='foo', percent='50.0')
 
         with override_sample('foo', active=True):
             assert waffle.sample_is_active('foo')
 
         with override_sample('foo', active=False):
             assert not waffle.sample_is_active('foo')
 
         self.assertEqual(Decimal('50.0'),
-                          waffle.get_waffle_sample_model().objects.get(name='foo').percent)
+                         waffle.get_waffle_sample_model().objects.get(name='foo').percent)
 
     def test_sample_did_not_exist(self):
         assert not waffle.get_waffle_sample_model().objects.filter(name='foo').exists()
 
         with override_sample('foo', active=True):
             assert waffle.sample_is_active('foo')
```

### Comparing `django-waffle-3.0.0/waffle/tests/test_utils.py` & `django-waffle-4.0.0/waffle/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/tests/test_views.py` & `django-waffle-4.0.0/waffle/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/tests/test_waffle.py` & `django-waffle-4.0.0/waffle/tests/test_waffle.py`

 * *Files identical despite different names*

### Comparing `django-waffle-3.0.0/waffle/testutils.py` & `django-waffle-4.0.0/waffle/testutils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,54 @@
+from typing import Generic, Optional, TypeVar, Union
+
 from django.test.utils import TestContextDecorator
 
 from waffle import (
     get_waffle_flag_model,
     get_waffle_sample_model,
     get_waffle_switch_model,
 )
 from waffle.models import Switch, Sample
 
 
 __all__ = ['override_flag', 'override_sample', 'override_switch']
 
+_T = TypeVar("_T")
+
 
-class _overrider(TestContextDecorator):
-    def __init__(self, name, active):
+class _overrider(TestContextDecorator, Generic[_T]):
+    def __init__(self, name: str, active: _T):
         super().__init__()
         self.name = name
         self.active = active
 
-    def get(self):
+    def get(self) -> None:
         self.obj, self.created = self.cls.objects.get_or_create(name=self.name)
 
-    def update(self, active):
+    def update(self, active: _T) -> None:
         raise NotImplementedError
 
-    def get_value(self):
+    def get_value(self) -> _T:
         raise NotImplementedError
 
-    def enable(self):
+    def enable(self) -> None:
         self.get()
         self.old_value = self.get_value()
         if self.old_value != self.active:
             self.update(self.active)
 
-    def disable(self):
+    def disable(self) -> None:
         if self.created:
             self.obj.delete()
             self.obj.flush()
         else:
             self.update(self.old_value)
 
 
-class override_switch(_overrider):
+class override_switch(_overrider[bool]):
     """
     override_switch is a contextmanager for easier testing of switches.
 
     It accepts two parameters, name of the switch and it's state. Example
     usage::
 
         with override_switch('happy_mode', active=True):
@@ -60,60 +64,60 @@
         @override_switch('happy_mode', active=True)
         def test_happy_mode_enabled():
             ...
 
     """
     cls = get_waffle_switch_model()
 
-    def update(self, active):
+    def update(self, active: bool) -> None:
         obj = self.cls.objects.get(pk=self.obj.pk)
         obj.active = active
         obj.save()
         obj.flush()
 
-    def get_value(self):
+    def get_value(self) -> bool:
         return self.obj.active
 
 
-class override_flag(_overrider):
+class override_flag(_overrider[Optional[bool]]):
     cls = get_waffle_flag_model()
 
-    def update(self, active):
+    def update(self, active: Optional[bool]) -> None:
         obj = self.cls.objects.get(pk=self.obj.pk)
         obj.everyone = active
         obj.save()
         obj.flush()
 
-    def get_value(self):
+    def get_value(self) -> Optional[bool]:
         return self.obj.everyone
 
 
-class override_sample(_overrider):
+class override_sample(_overrider[Union[bool, float]]):
     cls = get_waffle_sample_model()
 
-    def get(self):
+    def get(self) -> None:
         try:
             self.obj = self.cls.objects.get(name=self.name)
             self.created = False
         except self.cls.DoesNotExist:
             self.obj = self.cls.objects.create(name=self.name, percent='0.0')
             self.created = True
 
-    def update(self, active):
+    def update(self, active: Union[bool, float]) -> None:
         if active is True:
             p = 100.0
         elif active is False:
             p = 0.0
         else:
             p = active
         obj = self.cls.objects.get(pk=self.obj.pk)
         obj.percent = f'{p}'
         obj.save()
         obj.flush()
 
-    def get_value(self):
+    def get_value(self) -> Union[bool, float]:
         p = self.obj.percent
         if p == 100.0:
             return True
         if p == 0.0:
             return False
         return p
```

### Comparing `django-waffle-3.0.0/waffle/views.py` & `django-waffle-4.0.0/waffle/views.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-from django.http import HttpResponse, JsonResponse
+from __future__ import annotations
+
+from typing import Any
+
+from django.http import HttpRequest, HttpResponse, JsonResponse
 from django.template import loader
 from django.views.decorators.cache import never_cache
 
 from waffle import get_waffle_flag_model, get_waffle_switch_model, get_waffle_sample_model
 from waffle.utils import get_setting
 
 
 @never_cache
 def wafflejs(request):
     return HttpResponse(_generate_waffle_js(request),
                         content_type='application/x-javascript')
 
 
-def _generate_waffle_js(request):
+def _generate_waffle_js(request: HttpRequest) -> str:
     flags = get_waffle_flag_model().get_all()
     flag_values = [(f.name, f.is_active(request)) for f in flags]
 
     switches = get_waffle_switch_model().get_all()
     switch_values = [(s.name, s.is_active()) for s in switches]
 
     samples = get_waffle_sample_model().get_all()
@@ -33,15 +37,15 @@
 
 
 @never_cache
 def waffle_json(request):
     return JsonResponse(_generate_waffle_json(request))
 
 
-def _generate_waffle_json(request):
+def _generate_waffle_json(request: HttpRequest) -> dict[str, dict[str, Any]]:
     flags = get_waffle_flag_model().get_all()
     flag_values = {
         f.name: {
             'is_active': f.is_active(request),
             'last_modified': f.modified,
         }
         for f in flags
```

