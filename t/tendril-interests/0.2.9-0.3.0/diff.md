# Comparing `tmp/tendril-interests-0.2.9.tar.gz` & `tmp/tendril-interests-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tendril-interests-0.2.9.tar", last modified: Thu Mar 30 03:19:56 2023, max compression
+gzip compressed data, was "tendril-interests-0.3.0.tar", last modified: Wed Jul 26 11:05:27 2023, max compression
```

## Comparing `tendril-interests-0.2.9.tar` & `tendril-interests-0.3.0.tar`

### file list

```diff
@@ -1,86 +1,105 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.048756 tendril-interests-0.2.9/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3982 2023-03-30 03:19:56.048756 tendril-interests-0.2.9/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.036757 tendril-interests-0.2.9/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.036757 tendril-interests-0.2.9/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.036757 tendril-interests-0.2.9/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-interests-0.2.9/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-03-30 03:19:56.048756 tendril-interests-0.2.9/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3246 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.032757 tendril-interests-0.2.9/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.2.9/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.2.9/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.2.9/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2137 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/apiserver/routers/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/apiserver/templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-02-18 15:16:12.000000 tendril-interests-0.2.9/src/tendril/apiserver/templates/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      102 2023-02-18 22:08:54.000000 tendril-interests-0.2.9/src/tendril/apiserver/templates/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    17841 2023-03-30 03:05:21.000000 tendril-interests-0.2.9/src/tendril/apiserver/templates/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril-interests-0.2.9/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/authz/roles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril-interests-0.2.9/src/tendril/authz/roles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    12188 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/authz/roles/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril-interests-0.2.9/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/authz/scopes/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.040757 tendril-interests-0.2.9/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.044757 tendril-interests-0.2.9/src/tendril/common/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/common/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3851 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/common/interests/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6577 2023-03-30 02:19:26.000000 tendril-interests-0.2.9/src/tendril/common/interests/memberships.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      172 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/common/interests/states.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.044757 tendril-interests-0.2.9/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1762 2023-03-16 06:15:55.000000 tendril-interests-0.2.9/src/tendril/config/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.044757 tendril-interests-0.2.9/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.2.9/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.044757 tendril-interests-0.2.9/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril-interests-0.2.9/src/tendril/db/controllers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9884 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/db/controllers/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.044757 tendril-interests-0.2.9/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril-interests-0.2.9/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4112 2023-03-27 15:41:29.000000 tendril-interests-0.2.9/src/tendril/db/models/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.044757 tendril-interests-0.2.9/src/tendril/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril-interests-0.2.9/src/tendril/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    15664 2023-03-15 16:01:38.000000 tendril-interests-0.2.9/src/tendril/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5735 2023-03-27 17:44:29.000000 tendril-interests-0.2.9/src/tendril/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.048756 tendril-interests-0.2.9/src/tendril/libraries/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril-interests-0.2.9/src/tendril/libraries/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.048756 tendril-interests-0.2.9/src/tendril/libraries/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril-interests-0.2.9/src/tendril/libraries/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4140 2023-03-30 03:05:21.000000 tendril-interests-0.2.9/src/tendril/libraries/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1596 2023-02-18 15:08:06.000000 tendril-interests-0.2.9/src/tendril/libraries/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.048756 tendril-interests-0.2.9/src/tendril_interests.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3982 2023-03-30 03:19:55.000000 tendril-interests-0.2.9/src/tendril_interests.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1775 2023-03-30 03:19:55.000000 tendril-interests-0.2.9/src/tendril_interests.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-03-30 03:19:55.000000 tendril-interests-0.2.9/src/tendril_interests.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      558 2023-03-30 03:19:55.000000 tendril-interests-0.2.9/src/tendril_interests.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-03-30 03:19:55.000000 tendril-interests-0.2.9/src/tendril_interests.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-03-30 03:19:56.048756 tendril-interests-0.2.9/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril-interests-0.2.9/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.132869 tendril-interests-0.3.0/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2023-07-26 11:05:27.132869 tendril-interests-0.3.0/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.124869 tendril-interests-0.3.0/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril-interests-0.3.0/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-07-26 11:05:27.132869 tendril-interests-0.3.0/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3261 2023-06-27 18:08:50.000000 tendril-interests-0.3.0/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.124869 tendril-interests-0.3.0/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.3.0/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.3.0/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril-interests-0.3.0/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3703 2023-07-20 18:33:13.000000 tendril-interests-0.3.0/src/tendril/apiserver/routers/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/src/tendril/apiserver/templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 03:48:56.000000 tendril-interests-0.3.0/src/tendril/apiserver/templates/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      102 2023-02-18 22:08:54.000000 tendril-interests-0.3.0/src/tendril/apiserver/templates/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    21379 2023-07-25 18:59:57.000000 tendril-interests-0.3.0/src/tendril/apiserver/templates/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7395 2023-07-26 09:37:44.000000 tendril-interests-0.3.0/src/tendril/apiserver/templates/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril-interests-0.3.0/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/src/tendril/authz/approvals/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      249 2023-07-19 03:39:36.000000 tendril-interests-0.3.0/src/tendril/authz/approvals/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1649 2023-07-19 03:44:45.000000 tendril-interests-0.3.0/src/tendril/authz/approvals/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      949 2023-07-19 05:11:01.000000 tendril-interests-0.3.0/src/tendril/authz/approvals/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/src/tendril/authz/roles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril-interests-0.3.0/src/tendril/authz/roles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13869 2023-07-21 18:06:15.000000 tendril-interests-0.3.0/src/tendril/authz/roles/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      620 2023-07-19 07:05:51.000000 tendril-interests-0.3.0/src/tendril/authz/roles/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril-interests-0.3.0/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril-interests-0.3.0/src/tendril/authz/scopes/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.3.0/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/src/tendril/common/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril-interests-0.3.0/src/tendril/common/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3581 2023-07-21 17:21:15.000000 tendril-interests-0.3.0/src/tendril/common/interests/approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4287 2023-07-21 16:56:09.000000 tendril-interests-0.3.0/src/tendril/common/interests/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     8613 2023-07-20 19:30:39.000000 tendril-interests-0.3.0/src/tendril/common/interests/memberships.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      347 2023-07-20 16:55:21.000000 tendril-interests-0.3.0/src/tendril/common/interests/representations.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2023-04-12 09:49:34.000000 tendril-interests-0.3.0/src/tendril/common/states.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril-interests-0.3.0/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1762 2023-03-16 06:15:55.000000 tendril-interests-0.3.0/src/tendril/config/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril-interests-0.3.0/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril-interests-0.3.0/src/tendril/db/controllers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9944 2023-07-20 16:04:26.000000 tendril-interests-0.3.0/src/tendril/db/controllers/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4684 2023-07-20 16:05:06.000000 tendril-interests-0.3.0/src/tendril/db/controllers/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.128869 tendril-interests-0.3.0/src/tendril/db/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-30 15:19:11.000000 tendril-interests-0.3.0/src/tendril/db/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      429 2023-06-30 17:10:42.000000 tendril-interests-0.3.0/src/tendril/db/mixins/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.132869 tendril-interests-0.3.0/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril-interests-0.3.0/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4751 2023-07-18 17:03:54.000000 tendril-interests-0.3.0/src/tendril/db/models/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2069 2023-07-21 16:00:50.000000 tendril-interests-0.3.0/src/tendril/db/models/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.132869 tendril-interests-0.3.0/src/tendril/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril-interests-0.3.0/src/tendril/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    19016 2023-07-26 02:49:51.000000 tendril-interests-0.3.0/src/tendril/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7344 2023-07-19 05:16:07.000000 tendril-interests-0.3.0/src/tendril/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.132869 tendril-interests-0.3.0/src/tendril/interests/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-19 16:39:46.000000 tendril-interests-0.3.0/src/tendril/interests/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    17711 2023-07-26 11:04:17.000000 tendril-interests-0.3.0/src/tendril/interests/mixins/approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.132869 tendril-interests-0.3.0/src/tendril/libraries/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril-interests-0.3.0/src/tendril/libraries/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.132869 tendril-interests-0.3.0/src/tendril/libraries/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril-interests-0.3.0/src/tendril/libraries/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6009 2023-07-16 08:29:12.000000 tendril-interests-0.3.0/src/tendril/libraries/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2644 2023-04-09 05:14:23.000000 tendril-interests-0.3.0/src/tendril/libraries/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.132869 tendril-interests-0.3.0/src/tendril/libraries/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 15:54:08.000000 tendril-interests-0.3.0/src/tendril/libraries/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      418 2023-07-18 18:38:25.000000 tendril-interests-0.3.0/src/tendril/libraries/mixins/interests_approvals.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.132869 tendril-interests-0.3.0/src/tendril_interests.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3542 2023-07-26 11:05:27.000000 tendril-interests-0.3.0/src/tendril_interests.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2417 2023-07-26 11:05:27.000000 tendril-interests-0.3.0/src/tendril_interests.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-07-26 11:05:27.000000 tendril-interests-0.3.0/src/tendril_interests.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      566 2023-07-26 11:05:27.000000 tendril-interests-0.3.0/src/tendril_interests.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-07-26 11:05:27.000000 tendril-interests-0.3.0/src/tendril_interests.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-07-26 11:05:27.132869 tendril-interests-0.3.0/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril-interests-0.3.0/tox.ini
```

### Comparing `tendril-interests-0.2.9/.gitignore` & `tendril-interests-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/.readthedocs.yml` & `tendril-interests-0.3.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/.travis.yml` & `tendril-interests-0.3.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/LICENSE` & `tendril-interests-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/PKG-INFO` & `tendril-interests-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.2.9
+Version: 0.3.0
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-interests
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-interests.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-interests
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-interests.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-interests
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-interests.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-interests
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-interests.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-interests
-        
-        .. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
-            :target: https://www.codacy.com/app/chintal/tendril-interests
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-interests.svg
-            :target: https://requires.io/github/tendril-framework/tendril-interests/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-interests.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
-        
-        
-        
-        .. inclusion-marker-do-not-remove
-        
-        Introduction
-        ------------
-        
-        TODO Some brief introduction
-        
-        
-        Package Information
-        -------------------
-        
-        The latest version of the documentation, including installation, usage, and
-        API/developer notes can be found at
-        `ReadTheDocs <https://tendril-interests.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-interests>`_. Please use 
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-interests`` is Chintalagiri Shashank. The 
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-interests`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
-        
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -81,7 +25,63 @@
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
 Provides-Extra: publish
 Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-interests.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-interests
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-interests.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-interests
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-interests.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-interests
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-interests.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-interests
+
+.. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-interests
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-interests.svg
+    :target: https://requires.io/github/tendril-framework/tendril-interests/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-interests.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
+
+
+
+.. inclusion-marker-do-not-remove
+
+Introduction
+------------
+
+TODO Some brief introduction
+
+
+Package Information
+-------------------
+
+The latest version of the documentation, including installation, usage, and
+API/developer notes can be found at
+`ReadTheDocs <https://tendril-interests.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-interests>`_. Please use 
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-interests`` is Chintalagiri Shashank. The 
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-interests`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
+
```

### Comparing `tendril-interests-0.2.9/README.rst` & `tendril-interests-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/docs/Makefile` & `tendril-interests-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/docs/_static/custom.css` & `tendril-interests-0.3.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/docs/_static/favicon.ico` & `tendril-interests-0.3.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/docs/_static/logo.png` & `tendril-interests-0.3.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/docs/_static/logo_packed.png` & `tendril-interests-0.3.0/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/docs/_templates/about.html` & `tendril-interests-0.3.0/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/docs/conf.py` & `tendril-interests-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/docs/index.rst` & `tendril-interests-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/docs/installation.rst` & `tendril-interests-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/setup.py` & `tendril-interests-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 core_dependencies = [
     'tendril-utils-db>=0.4.3',
     'tendril-auth',
     'networkx',
     'polars',
     'makefun',
+    'asgiref',
 ]
 
 install_requires = core_dependencies + ['wheel']
 
 setup_requires = ['setuptools_scm']
 
 doc_requires = setup_requires + ['sphinx', 'sphinx-argparse', 'alabaster']
```

### Comparing `tendril-interests-0.2.9/src/tendril/apiserver/routers/interests.py` & `tendril-interests-0.3.0/src/tendril/apiserver/routers/interests.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 
 
+from typing import List
+from typing import Optional
 from fastapi import APIRouter
 from fastapi import Depends
 
 from tendril.authn.users import auth_spec
 from tendril.authn.users import authn_dependency
 from tendril.authn.users import AuthUserModel
 
 from tendril.libraries import interests
 from tendril.interests import type_spec
+from tendril.common.states import LifecycleStatus
+
+from tendril.db.controllers.interests import get_interest
+from tendril.common.interests.representations import rewrap_interest
+from tendril.common.interests.representations import get_interest_stub
+
 from tendril.common.interests.memberships import user_memberships
 from tendril.common.interests.memberships import UserMembershipsTModel
+
 from tendril.config import INTERESTS_API_ENABLED
 
+from tendril.utils.db import get_session
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEFAULT)
 
 
 interests_router = APIRouter(prefix='/interests',
                              tags=["Common Interests API"],
                              dependencies=[Depends(authn_dependency),
@@ -30,37 +40,62 @@
 
 
 @interests_router.get("/types")
 async def get_interest_types():
     return {'interest_types': type_spec}
 
 
-def get_interest_stub(interest):
-    return {
-        'type_name': interest.type_name,
-        'name': interest.name,
-        'id': interest.id,
-    }
+@interests_router.get("/{id}/stub")
+async def interest_stubs(id: int,
+                         user: AuthUserModel = auth_spec()):
+    with get_session() as session:
+        interest = get_interest(id=id, session=session)
+        interest = rewrap_interest(interest)
+
+        # We can't expect the user to have permissions on the interest, for
+        # instance when looking at platform information from the content
+        # interest's perspective for approvals. The stub will have to be
+        # treated as public (any logged in user).
+        # interest.export(auth_user=user, probe_only=True, session=session)
+        return get_interest_stub(interest)
 
 
-@interests_router.get("/memberships", response_model=UserMembershipsTModel)
+@interests_router.post("/memberships", response_model=UserMembershipsTModel)
 async def get_user_memberships(user: AuthUserModel = auth_spec(),
                                include_delegated: bool = False,
-                               include_inherited: bool = False):
+                               include_inherited: bool = False,
+                               interest_types: Optional[List[str]] = [],
+                               statuses:Optional[List[LifecycleStatus]] = [],
+                               roles:Optional[List[str]] = []):
+    kwargs = {}
+    if interest_types:
+        kwargs['interest_types'] = interest_types
+    if statuses:
+        kwargs['include_statuses'] = [x.value for x in statuses]
+    if roles:
+        kwargs['include_roles'] = roles
     return user_memberships(user,
                             include_delegated=include_delegated,
-                            include_inherited=include_inherited).render()
+                            include_inherited=include_inherited,
+                            **kwargs).render()
+
+
+@interests_router.get("/name_available", response_model=bool)
+async def check_name_available(name: str):
+    return interests.name_available(name)
 
 
 def _generate_routers():
     interest_routers = []
-    for itype in interests.defined_types:
-        ilib = getattr(interests, itype)
-        generated_routers = ilib.api_generator().generate(f'{itype}')
-        interest_routers.extend(generated_routers)
+    for libname in interests.libraries:
+        ilib = getattr(interests, libname)
+        api_generators = ilib.api_generators()
+        for generator in api_generators:
+            generated_routers = generator.generate(f'{libname}')
+            interest_routers.extend(generated_routers)
     return interest_routers
 
 
 if INTERESTS_API_ENABLED:
     routers = [
         interests_router
     ] + _generate_routers()
```

### Comparing `tendril-interests-0.2.9/src/tendril/apiserver/templates/interests.py` & `tendril-interests-0.3.0/src/tendril/apiserver/templates/interests.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 
 
 from typing import List
 from typing import Dict
 from typing import Union
 
-from pydantic import Field
 from inspect import signature
 from makefun import create_function
 
 from fastapi import APIRouter
 from fastapi import Request
 from fastapi import Depends
+from fastapi import BackgroundTasks
 from fastapi.responses import JSONResponse
 
 from tendril.authn.users import auth_spec
 from tendril.authn.users import AuthUserModel
 from tendril.authn.users import authn_dependency
 
 from tendril.authn.pydantic import UserReferenceTModel
 from tendril.authz.roles.interests import MembershipInfoTModel
-from tendril.common.interests.states import InterestLifecycleStatus
+from tendril.common.states import LifecycleStatus
 from tendril.utils.db import get_session
 
 from .base import ApiRouterGenerator
 
 
 class InterestLibraryRouterGenerator(ApiRouterGenerator):
     def __init__(self, actual):
@@ -80,15 +80,15 @@
          - **include_roles :** Include the user's roles in the response.
          - **include_permissions :** Include the user's permissions in the response.
         """
         with get_session() as session:
             rv = [x.export(session=session,
                            include_roles=include_roles,
                            include_permissions=include_permissions)
-                  for x in self._actual.items(state=InterestLifecycleStatus.NEW,
+                  for x in self._actual.items(state=LifecycleStatus.NEW,
                                               session=session)]
         return rv
 
     async def item(self, request: Request, id: int,
                    user: AuthUserModel = auth_spec(),
                    include_roles: bool = False,
                    include_permissions: bool = False):
@@ -112,26 +112,43 @@
         with get_session() as session:
             rv = self._actual.item(id=id, session=session).\
                 export(auth_user=user, session=session,
                        include_roles=include_roles,
                        include_permissions=include_permissions)
         return rv
 
+    async def find_possible_parents(self, request: Request,
+                                    user: AuthUserModel = auth_spec()):
+        """
+        Get possible parents for new items in this library.
+
+        All user memberships in possible parents for this library's interest
+        type which allow creation of a child of this type are returned.
+
+        - **user :* The requesting user, identified by the access token.
+        """
+        with get_session() as session:
+            result = self._actual.possible_parents(user=user, session=session)
+            return [x.export(auth_user=user, session=session,
+                             include_roles=False,
+                             include_permissions=False) for x in result]
+
     def _inject_create_model(self, ep, param='item'):
         orig_sig = signature(ep)
         params = list(orig_sig.parameters.values())
         orig_param = next(p for p in params if p.name == param)
         index = params.index(orig_param)
         new_param = orig_param.replace(name=orig_param.name, default=orig_param.default, kind=orig_param.kind,
                                        annotation=self._actual.interest_class.tmodel_create)
         params[index] = new_param
         new_sig = orig_sig.replace(parameters=params)
         return create_function(func_signature=new_sig, func_impl=ep)
 
-    def create_item(self, item, user: AuthUserModel = auth_spec()):
+    def create_item(self, item,
+                    user: AuthUserModel = auth_spec()):
         """
         Create an Interest.
 
         This endpoint does not enforce interest access controls, and allows
         any user with the create scope for this interest type to create an
         interest.
 
@@ -150,14 +167,15 @@
         """
         with get_session() as session:
             item = self._actual.add_item(item, session=session)
             rv = item.export(session=session)
         return rv
 
     async def activate_item(self, request: Request, id: int,
+                            background_tasks: BackgroundTasks,
                             user: AuthUserModel = auth_spec()):
         """
         Activate a specified interest.
 
         This endpoint enforces interest access control, and executes only if
         the logged-in user (identified by the access token) has the necessary
         permissions.
@@ -182,21 +200,55 @@
         The endpoint parameters are:
 
          - **id :** The id of the interest to be activated
          - **user :** The requesting user, identified by the access token.
         """
         with get_session() as session:
             item = self._actual.item(id, session=session)
-            item.activate(auth_user=user, session=session)
+            result, msg = item.activate(background_tasks=background_tasks,
+                                        auth_user=user, session=session)
+        if result:
+            status_code = 200
+        else:
+            status_code = 406
+        return JSONResponse(
+            status_code=status_code,
+            content={'message': msg}
+        )
+
+    async def deactivate_item(self, request: Request, id: int,
+                              user: AuthUserModel = auth_spec()):
+        """
+        Deactivate a specified interest.
+
+        This endpoint enforces interest access control, and executes only if
+        the logged-in user (identified by the access token) has the necessary
+        permissions.
+
+        Activated interests disallow most modifying operations to be carried out
+        on them. Usually, the operations needed to modify the interest in a
+        significant was is only allowed when the interest is new.
+
+        Note that such changes may also (independent of this endpoint) rescind
+        approvals granted to the interest in the past.
+
+        The endpoint parameters are:
+
+         - **id :** The id of the interest to be activated
+         - **user :** The requesting user, identified by the access token.
+        """
+        with get_session() as session:
+            item = self._actual.item(id, session=session)
+            msg = item.deactivate(auth_user=user, session=session)
         return JSONResponse(
             status_code=200,
-            content={'message': f"{self._actual.interest_class.model.role_spec.prefix} "
-                                f"{id} Activated"}
+            content={'message': msg}
         )
 
+
     async def item_members(self, request: Request, id: int,
                            user: AuthUserModel = auth_spec(),
                            include_effective: bool=False,
                            include_inherited: bool=True):
         """
         Get all users with privileges for a specified interest.
 
@@ -306,64 +358,91 @@
         return rv
 
     def item_add_child(self, request: Request, id: int,
                        child_id: int, limited: bool = False,
                        user: AuthUserModel = auth_spec()):
         with get_session() as session:
             item = self._actual.item(id, session=session)
-            asn = item.add_child(child_id, limited=limited,
-                                 auth_user=user, session=session)
+            return item.add_child(child_id, limited=limited,
+                                  auth_user=user, session=session)
 
     async def update_item(self):
         raise NotImplementedError
 
     async def delete_item(self):
         raise NotImplementedError
 
     def generate(self, name):
         desc = f'{name} Interest API'
         prefix = self._actual.interest_class.model.role_spec.prefix
+        from tendril import interests
+        parent_models = [interests.type_codes[x].tmodel for x in interests.possible_parents[prefix]]
+
         router = APIRouter(prefix=f'/{name}', tags=[desc],
                            dependencies=[Depends(authn_dependency)])
         router.add_api_route("", self.items, methods=["GET"],
                              response_model=List[self._actual.interest_class.tmodel],
+                             response_model_exclude_none=True,
                              dependencies=[auth_spec(scopes=[f'{prefix}:read'])],)
-        router.add_api_route("/new", self.new_items, methods=["GET"],
-                             response_model=List[self._actual.interest_class.tmodel],
-                             dependencies=[auth_spec(scopes=[f'{prefix}:create'])], )
-        router.add_api_route("/{id}", self.item, methods=["GET"],
+
+        if self._actual.enable_creation_api:
+            router.add_api_route("/create", self._inject_create_model(self.create_item), methods=['PUT'],
+                                 response_model=self._actual.interest_class.tmodel,
+                                 response_model_exclude_none=True,
+                                 dependencies=[auth_spec(scopes=[f'{prefix}:create'])], )
+
+        if self._actual.enable_activation_api:
+            router.add_api_route("/new", self.new_items, methods=["GET"],
+                                 response_model=List[self._actual.interest_class.tmodel],
+                                 response_model_exclude_none=True,
+                                 dependencies=[auth_spec(scopes=[f'{prefix}:create'])], )
+
+            if len(parent_models):
+                router.add_api_route("/possible_parents", self.find_possible_parents, methods=['GET'],
+                                     response_model=List[Union[tuple(parent_models)]],
+                                     response_model_exclude_none=True,
+                                     dependencies=[auth_spec(scopes=[f'{prefix}:create'])])
+
+            router.add_api_route("/{id:int}/activate", self.activate_item, methods=['POST'],
+                                 dependencies=[auth_spec(scopes=[f'{prefix}:write'])])
+            router.add_api_route("/{id:int}/deactivate", self.deactivate_item, methods=['POST'],
+                                 dependencies=[auth_spec(scopes=[f'{prefix}:write'])])
+
+        router.add_api_route("/{id:int}", self.item, methods=["GET"],
                              response_model=self._actual.interest_class.tmodel,
+                             response_model_exclude_none=True,
                              dependencies=[auth_spec(scopes=[f'{prefix}:read'])])
-        router.add_api_route("/create", self._inject_create_model(self.create_item), methods=['PUT'],
-                             response_model=self._actual.interest_class.tmodel,
-                             dependencies=[auth_spec(scopes=[f'{prefix}:create'])], )
-        router.add_api_route("/{id}/activate", self.activate_item, methods=['POST'],
-                             dependencies=[auth_spec(scopes=[f'{prefix}:write'])])
-        router.add_api_route("/{id}/members", self.item_members, methods=["GET"],
-                             response_model=Dict[str, List[MembershipInfoTModel]],
-                             dependencies=[auth_spec(scopes=[f'{prefix}:read'])], )
-        router.add_api_route("/{id}/members/{role}", self.item_role_members, methods=["GET"],
-                             response_model=List[MembershipInfoTModel],
-                             dependencies=[auth_spec(scopes=[f'{prefix}:read'])], )
-        router.add_api_route("/{id}/members/{role}/add", self.item_grant_role, methods=["POST"],
-                             response_model=self._actual.interest_class.tmodel,
-                             dependencies=[auth_spec(scopes=[f'{prefix}:write'])], )
 
-        from tendril import interests
-        parent_models = [interests.type_codes[x].tmodel for x in interests.possible_parents[prefix]]
+        if self._actual.enable_membership_api:
+            router.add_api_route("/{id:int}/members", self.item_members, methods=["GET"],
+                                 response_model=Dict[str, List[MembershipInfoTModel]],
+                                 response_model_exclude_none=True,
+                                 dependencies=[auth_spec(scopes=[f'{prefix}:read'])], )
+            router.add_api_route("/{id:int}/members/{role}", self.item_role_members, methods=["GET"],
+                                 response_model=List[MembershipInfoTModel],
+                                 response_model_exclude_none=True,
+                                 dependencies=[auth_spec(scopes=[f'{prefix}:read'])], )
+
+        if self._actual.enable_membership_edit_api:
+            router.add_api_route("/{id:int}/members/{role}/add", self.item_grant_role, methods=["POST"],
+                                 response_model=self._actual.interest_class.tmodel,
+                                 response_model_exclude_none=True,
+                                 dependencies=[auth_spec(scopes=[f'{prefix}:write'])], )
 
         if len(parent_models):
-            router.add_api_route("/{id}/parents", self.item_parents, methods=["GET"],
+            router.add_api_route("/{id:int}/parents", self.item_parents, methods=["GET"],
                                  response_model=List[Union[tuple(parent_models)]],
+                                 response_model_exclude_none=True,
                                  dependencies=[auth_spec(scopes=[f'{prefix}:read'])],)
 
         ac = self._actual.interest_class.model.role_spec.allowed_children
         if '*' in ac:
             ac = interests.type_codes.keys()
         child_models = [interests.type_codes[x].tmodel for x in ac]
         if len(child_models):
-            router.add_api_route("/{id}/children", self.item_children, methods=["GET"],
+            router.add_api_route("/{id:int}/children", self.item_children, methods=["GET"],
                                  response_model=List[Union[tuple(child_models)]],
+                                 response_model_exclude_none=True,
                                  dependencies=[auth_spec(scopes=[f'{prefix}:read'])])
-            router.add_api_route("/{id}/children/add", self.item_add_child, methods=["POST"],
+            router.add_api_route("/{id:int}/children/add", self.item_add_child, methods=["POST"],
                                  dependencies=[auth_spec(scopes=[f'{prefix}:write'])])
         return [router]
```

### Comparing `tendril-interests-0.2.9/src/tendril/authz/roles/interests.py` & `tendril-interests-0.3.0/src/tendril/authz/roles/interests.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import enum
 from collections.abc import Iterable
 from functools import cached_property
 from functools import wraps
 from tendril.authn.pydantic import UserStubTModel
 from tendril.utils.pydantic import TendrilTBaseModel
-from tendril.common.interests.states import InterestLifecycleStatus
+from tendril.common.states import LifecycleStatus
 from tendril.common.interests.exceptions import InterestStateException
 from tendril.common.interests.exceptions import AuthorizationRequiredError
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEBUG)
 
 
 class MembershipInfoTModel(TendrilTBaseModel):
@@ -46,29 +46,36 @@
     authz_write_role = None
     authz_write_peers = False
 
     child_read_role = None
     child_add_role = None
     child_delete_role = None
 
+    artefact_read_role = None
+    artefact_add_role = None
+    artefact_delete_role = None
+
     child_read_roles = {}
     child_add_roles = {}
     child_delete_roles = {}
 
     inherits_from_parent = True
 
     custom_delegations = {}
     additional_roles_required = []
     parent_required = True
 
+    mixin_scopes = {}
+    mixin_actions = {}
+
     @cached_property
     def activation_requirements(self):
         rv = {'roles_required': [self.apex_role] + self.additional_roles_required,
               'parent_required': self.parent_required,
-              'allowed_states': [InterestLifecycleStatus.NEW]}
+              'allowed_states': [LifecycleStatus.NEW, LifecycleStatus.APPROVAL]}
         return rv
 
     @cached_property
     def role_delegations(self):
         rv = {self.apex_role: [r for r in self.roles if r != self.apex_role]}
         rv.update(self.custom_delegations)
         for role in self.roles:
@@ -90,21 +97,38 @@
         return {
             f'{self.prefix}:create': f"Create operations on '{self.prefix}' interests",
             f'{self.prefix}:read': f"Read operations on '{self.prefix}' interests",
             f'{self.prefix}:write': f"Write operations on '{self.prefix}' interests",
             f'{self.prefix}:delete': f"Delete operations on '{self.prefix}' interests",
         }
 
+    def _mixin_scopes(self):
+        try:
+            mro = list(self.__class__.__mro__)
+            mro.reverse()
+        except AttributeError:
+            print(f"There isn't an __mro__ on {self.__class__}. "
+                  f"This is probably a classic class. We don't support this.")
+            return self.mixin_scopes
+        rv = {}
+        for cls in mro:
+            v = getattr(cls, 'mixin_scopes', {})
+            if hasattr(v, '__get__'):
+                v = v.__get__(self)
+            rv.update(v)
+        return rv
+
     def _custom_scopes(self):
         return {}
 
     @cached_property
     def scopes(self):
         rv = {}
         rv.update(self._standard_scopes())
+        rv.update(self._mixin_scopes())
         rv.update(self._custom_scopes())
         return rv
 
     def _crud_actions(self):
         rv = {'read': (self.read_role or self.apex_role, f'{self.prefix}:read'),
               'edit': (self.edit_role or self.apex_role, f'{self.prefix}:write'),
               # 'delete': (self.delete_role or self.apex_role, f'{self.prefix}:delete'),
@@ -157,29 +181,46 @@
             rv[f'remove_child:{ctype}'] = (self.child_delete_roles.get(ctype, None)
                                            or self.child_delete_role
                                            or self.apex_role, f'{self.prefix}:write')
         return rv
 
     def _artefact_actions(self):
         return {
-            'read_artefacts': ('Member', f'{self.prefix}:read'),
-            'add_artefact': ('Owner', f'{self.prefix}:write'),
-            'delete_artefact': ('Owner', f'{self.prefix}:delete'),
+            'read_artefacts': (self.artefact_read_role or self.base_role, f'{self.prefix}:read'),
+            'add_artefact': (self.artefact_add_role or self.apex_role, f'{self.prefix}:write'),
+            'delete_artefact': (self.artefact_delete_role or self.apex_role, f'{self.prefix}:delete'),
         }
 
+    def _mixin_actions(self):
+        try:
+            mro = list(self.__class__.__mro__)
+            mro.reverse()
+        except AttributeError:
+            print(f"There isn't an __mro__ on {self.__class__}. "
+                  f"This is probably a classic class. We don't support this.")
+            return self.mixin_actions
+        rv = {}
+        for cls in mro:
+            v = getattr(cls, 'mixin_actions', {})
+            if hasattr(v, '__get__'):
+                v = v.__get__(self)
+            rv.update(v)
+        return rv
+
     def _custom_actions(self):
         return {}
 
     @cached_property
     def actions(self):
         rv = {}
         rv.update(self._crud_actions())
         rv.update(self._authz_actions())
         rv.update(self._hierarchy_actions())
         rv.update(self._artefact_actions())
+        rv.update(self._mixin_actions())
         rv.update(self._custom_actions())
         return rv
 
     def get_delegated_roles(self, role):
         return self.role_delegations.get(role, [])
 
     def get_effective_roles(self, role):
@@ -219,17 +260,20 @@
     def get_roles_permissions(self, roles):
         allowed = set()
         for role in roles:
             allowed.update(self.get_role_permissions(role))
         return allowed
 
     def get_permitted_roles(self, action):
-        while action not in self.actions.keys():
+        if action not in self.actions.keys():
             if ':' in action:
-                action = action.rsplit(':', 1)[0]
+               action = action.rsplit(':', 1)[0]
+        if action not in self.actions.keys():
+            raise ValueError(f"Action {action} does not seem to be "
+                             f"recognized by {self.__class__.__name__}")
         return set(self.get_accepted_roles(self.actions[action][0]))
 
     def check_permitted(self, action, roles):
         permitted = self.get_permitted_roles(action)
         for role in roles:
             if role in permitted:
                 return True
@@ -264,48 +308,51 @@
 
 def require_permission(action,
                        specifier=None, preprocessor=lambda x: x,
                        strip_auth=True, required=True,
                        exceptions=[]):
     def decorator(func):
         @wraps(func)
-        def permission_check(self, *args, **kwargs):
+        def permission_check(self, *args, probe_only=False, **kwargs):
             if strip_auth:
                 auth_user = kwargs.pop('auth_user', None)
             else:
                 auth_user = kwargs.get('auth_user', None)
 
             in_exception = False
             for exception in exceptions:
                 for predicate in exception:
                     if not _check_predicate(predicate, self, kwargs):
-                        print(predicate)
                         break
                 else:
                     in_exception = True
                     break
 
             if not in_exception and required and auth_user is None:
                 raise AttributeError("auth_user is required to execute "
                                      "this interest instance method")
             if not auth_user:
+                if probe_only:
+                    return True
                 return func(self, *args, **kwargs)
             session = kwargs.get('session', None)
             if specifier:
                 s = kwargs.get(specifier, None)
                 if callable(s):
                     s = s(self, *args, **kwargs)
                 if s:
                     laction = f'{action}:{preprocessor(s)}'
                 else:
                     laction = action
             else:
                 laction = action
             # logger.debug(f"Checking permissions of {auth_user} for '{laction}' on {self}")
             if in_exception or self.check_user_access(user=auth_user, action=laction, session=session):
+                if probe_only:
+                    return True
                 return func(self, *args, **kwargs)
             else:
                 raise AuthorizationRequiredError(auth_user, laction, self.id, self.name)
         return permission_check
     return decorator
```

### Comparing `tendril-interests-0.2.9/src/tendril/common/interests/exceptions.py` & `tendril-interests-0.3.0/src/tendril/common/interests/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -111,10 +111,22 @@
 
     def __init__(self, type_name, name, id=None):
         self.type_name = type_name
         self.name = name
         self.i_id = id
 
     def __str__(self):
-        return f"Interest of type '{self.type_name}' with name '{self.name}' (id={self.i_id}) could not " \
-               f"be found."
+        return f"Interest of type '{self.type_name}' with " \
+               f"name '{self.name}' (id={self.i_id}) could not be found."
 
+
+class InterestTypeUnsupported(HTTPCodedException):
+    status_code = 406
+
+    def __init__(self, required=None, id='<unspecified>', name='<unspecified>'):
+        self.required = required
+        self.i_id = id
+        self.name = name
+
+    def __str__(self):
+        return f"Interest with name '{self.name}' (id={self.i_id} does not seem to be " \
+               f"of a supported type for this operation. Required : {self.required}."
```

### Comparing `tendril-interests-0.2.9/src/tendril/common/interests/memberships.py` & `tendril-interests-0.3.0/src/tendril/common/interests/memberships.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 
 
 import polars
+from polars.exceptions import ColumnNotFoundError
 from typing import Dict
 from typing import List
+from tendril import interests
 from tendril.utils.pydantic import TendrilTBaseModel
-from tendril.utils.db import get_session
+from tendril.common.states import LifecycleStatus
+from tendril.db.controllers.interests import get_interest
+from tendril.utils.db import with_db
 
 
 class UserMembershipTModel(TendrilTBaseModel):
     role: str
     delegated: bool
     inherited: bool
 
 
 class UserMembershipsInterestTModel(TendrilTBaseModel):
     id: int
     name: str
+    status: LifecycleStatus
     roles: List[UserMembershipTModel]
 
 
 UserMembershipsInterestsContainerTModel = List[UserMembershipsInterestTModel]
 UserMembershipsTModel = Dict[str, UserMembershipsInterestsContainerTModel]
 
 
@@ -28,66 +33,100 @@
         self._raw_data = []
         self.df = None
 
     def add_membership(self, interest, role, delegated, inherited):
         self._raw_data.append({'type': interest.type_name,
                                'interest.id': interest.id,
                                'interest.name': interest.name,
+                               'interest.status': interest.status.value,
                                'role.name': role,
                                'role.delegated': delegated,
                                'role.inherited': inherited})
 
     def process(self):
         self.df = polars.DataFrame(self._raw_data)
 
+    def apply_status_filter(self, include_statuses):
+        # TODO This will mess with caching!
+        self.df = self.df.filter(polars.col('interest.status').is_in(include_statuses))
+
+    def apply_role_filter(self, include_roles):
+        # TODO This will mess with caching!
+        self.df = self.df.filter(polars.col('role.name').is_in(include_roles))
+
     def _pack_interest_role(self, df):
         # TODO This calculation is wrong.
         return {'role': df[0]['role.name'].item(),
                 'delegated': bool(df.select(polars.col('role.delegated')).min().item()),
                 'inherited': bool(df.select(polars.col('role.inherited')).min().item())}
 
     def _pack_interest_memberships(self, df):
         roles = []
         for role in df.select(polars.col('role.name').unique()).rows():
             role_df = df.filter(polars.col('role.name') == role[0])\
                         .select(['role.name', 'role.delegated', 'role.inherited'])
             roles.append(self._pack_interest_role(role_df))
         idict = {'id': df[0]['interest.id'].item(),
                  'name': df[0]['interest.name'].item(),
+                 'status': df[0]['interest.status'].item(),
                  'roles': roles}
         return idict
 
     def _pack_itype_memberships(self, df):
         rv = []
         for interest_id in df.select(polars.col('interest.id').unique()).rows():
             interest_df = df.filter(polars.col('interest.id') == interest_id[0])
             rv.append(self._pack_interest_memberships(interest_df))
         return rv
 
     def render(self):
         rv = {}
-        for itype in self.df.select(polars.col("type").unique()).rows():
-            itype_df = self.df.filter(polars.col("type") == itype[0])\
-                              .select(['interest.id', 'interest.name',
-                                       'role.name', 'role.delegated', 'role.inherited'])
-            rv[itype[0]] = self._pack_itype_memberships(itype_df)
-        return rv
+        try:
+            for itype in self.df.select(polars.col("type").unique()).rows():
+                itype_df = self.df.filter(polars.col("type") == itype[0])\
+                                  .select(['interest.id', 'interest.name', 'interest.status',
+                                           'role.name', 'role.delegated', 'role.inherited'])
+                rv[itype[0]] = self._pack_itype_memberships(itype_df)
+            return rv
+        except ColumnNotFoundError:
+            return {}
 
     def interest_ids(self):
         if not self.df.select(polars.count()).item():
             return []
-        return self.df.select(polars.col('interest.id').unique()).rows()[0]
+        return list(self.df.select(polars.col('interest.id').unique()).get_column(name='interest.id'))
+
+    @with_db
+    def _get_interest(self, iid, itype, session=None):
+        interest_type = interests.type_codes[itype]
+        return interest_type(get_interest(id=iid, type=interest_type.model, session=session))
+
+    @with_db
+    def interests(self, filter_criteria=None, sort_heuristics=None, session=None):
+        if not self.df.select(polars.count()).item():
+            return []
+        i_itype = self.df.select(polars.col(['interest.id', 'type'])).unique()
+        cand_interests = [self._get_interest(iid=iid, itype=type_name, session=session)
+                          for iid, type_name in i_itype.rows()]
+        if filter_criteria:
+            cand_interests = [x for x in cand_interests
+                              if all([getattr(x, acc)(**kw) for acc, kw in filter_criteria])]
+        if sort_heuristics:
+            for acc, reflist in sort_heuristics:
+                ranks = dict((value, idx) for idx, value in enumerate(reflist))
+                cand_interests = sorted(cand_interests, key=lambda x: ranks[x.type_name])
+        return cand_interests
 
 
 def _rewrap_interest(model):
-    from tendril.interests import type_codes
     type_name = model.type
-    return type_codes[type_name](model)
+    return interests.type_codes[type_name](model)
 
 
+@with_db
 def _get_interest_user_memberships(collector, interest, user_id,
                                    include_delegated=True,
                                    include_inherited=True,
                                    is_inherited=False,
                                    inherited_roles=None,
                                    interest_types=None,
                                    parent_types=None,
@@ -125,34 +164,39 @@
                                            include_inherited=include_inherited,
                                            is_inherited=True, inherited_roles=to_inherit,
                                            interest_types=interest_types,
                                            parent_types=parent_types,
                                            session=session)
 
 
+@with_db
 def user_memberships(user_id, interest_types=None,
-                     include_delegated=True,
-                     include_inherited=True):
-    from tendril.interests import possible_parents
+                     include_statuses=None, include_roles=None,
+                     include_delegated=True, include_inherited=True,
+                     session=None):
+    from tendril.interests import possible_ancestors
     from tendril.db.controllers import interests
 
     parent_types = None
     if interest_types:
         parent_types = set(interest_types)
         for t in interest_types:
-            parent_types.update(possible_parents[t])
+            parent_types.update(possible_ancestors[t])
 
-    with get_session() as session:
-        memberships = interests.get_user_memberships(user=user_id, session=session)
-        rv = UserMembershipCollector()
-        for m in memberships:
-            if parent_types and m.interest.type_name not in parent_types:
-                continue
-            _get_interest_user_memberships(rv, _rewrap_interest(m.interest), user_id,
-                                           include_delegated=include_delegated,
-                                           include_inherited=include_inherited,
-                                           is_inherited=False, inherited_roles=[],
-                                           interest_types=interest_types,
-                                           parent_types=parent_types,
-                                           session=session)
-        rv.process()
+    memberships = interests.get_user_memberships(user=user_id, session=session)
+    rv = UserMembershipCollector()
+    for m in memberships:
+        if parent_types and m.interest.type_name not in parent_types:
+            continue
+        _get_interest_user_memberships(rv, _rewrap_interest(m.interest), user_id,
+                                       include_delegated=include_delegated,
+                                       include_inherited=include_inherited,
+                                       is_inherited=False, inherited_roles=[],
+                                       interest_types=interest_types,
+                                       parent_types=parent_types,
+                                       session=session)
+    rv.process()
+    if include_roles:
+        rv.apply_role_filter(include_roles)
+    if include_statuses:
+        rv.apply_status_filter(include_statuses)
     return rv
```

### Comparing `tendril-interests-0.2.9/src/tendril/config/__init__.py` & `tendril-interests-0.3.0/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/src/tendril/config/interests.py` & `tendril-interests-0.3.0/src/tendril/config/interests.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/src/tendril/db/controllers/interests.py` & `tendril-interests-0.3.0/src/tendril/db/controllers/interests.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,16 @@
     if isinstance(interest, int):
         return interest
     elif isinstance(interest, str):
         interest = get_interest(name=interest, type=type, session=session)
         return interest.id
     elif isinstance(interest, InterestModel):
         return interest.id
-
+    elif hasattr(interest, 'id'):
+        return interest.id
 
 @with_db
 def get_membership(interest, user, role, session=None):
     interest_id = preprocess_interest(interest, session=session)
     user_id = preprocess_user(user, session=session)
     role_id = preprocess_role(role, session=session)
     q = session.query(InterestMembershipModel)\
```

### Comparing `tendril-interests-0.2.9/src/tendril/db/models/interests.py` & `tendril-interests-0.3.0/src/tendril/db/models/interests.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from sqlalchemy.orm import mapped_column
 from sqlalchemy_json import mutable_json_type
 from sqlalchemy.ext.declarative import declared_attr
 from sqlalchemy.dialects.postgresql import JSONB
 
 from tendril.authz.roles.interests import InterestRoleSpec
 
-from tendril.common.interests.states import InterestLifecycleStatus
+from tendril.common.states import LifecycleStatus
 
 from tendril.utils.db import DeclBase
 from tendril.utils.db import BaseMixin
 from tendril.utils.db import TimestampMixin
 from tendril.authn.db.mixins import UserMixin
 
 from tendril.utils import log
@@ -37,32 +37,49 @@
     type_name = "interest"
     role_spec = InterestRoleSpec()
 
     type = Column(String(50), nullable=False, default=type_name)
     name = Column(String(255), nullable=False)
     descriptive_name = Column(String(255), nullable=True)
 
-    status = Column(Enum(InterestLifecycleStatus), nullable=False,
-                    default=InterestLifecycleStatus.NEW)
+    status = Column(Enum(LifecycleStatus), nullable=False,
+                    default=LifecycleStatus.NEW)
     info = Column(mutable_json_type(dbtype=JSONB))
 
+    @property
+    def actual(self):
+        if not hasattr(self, '_actual'):
+            from tendril.interests import type_codes
+            self._actual = type_codes[self.type_name](self)
+        return self._actual
+
     # @declared_attr
     # def parent(cls):
     #     return relationship("InterestModel", remote_side=[cls.id])
 
     @declared_attr
     def memberships(cls):
         return relationship("InterestMembershipModel", back_populates='interest', lazy='dynamic')
 
     @declared_attr
+    def approvals(cls):
+        return relationship("InterestApprovalModel", back_populates='context', lazy='select',
+                            foreign_keys='InterestApprovalModel.interest_id')
+
+    @declared_attr
+    def child_approvals(cls):
+        return relationship("InterestApprovalModel", back_populates='interest', lazy='select',
+                            foreign_keys='InterestApprovalModel.context_id')
+
+    @declared_attr
     def children(cls):
         return relationship("InterestModel", secondary="InterestAssociation",
                             primaryjoin="InterestModel.id == InterestAssociationModel.parent_id",
                             secondaryjoin="InterestModel.id == InterestAssociationModel.child_id",
-                            backref="parents")
+                            backref="parents", lazy='dynamic')
 
     # @declared_attr
     # def artefacts(cls):
     #     return relationship('ArtefactModel', back_populates="interest")
 
     @declared_attr
     def logs(cls):
```

### Comparing `tendril-interests-0.2.9/src/tendril/interests/base.py` & `tendril-interests-0.3.0/src/tendril/interests/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 from functools import cached_property
 from pydantic import Field
 
 from tendril.utils.pydantic import TendrilTBaseModel
 
 from tendril.authn.db.controller import get_user_by_id
 from tendril.db.models.interests import InterestModel
-from tendril.db.models.interests import InterestLifecycleStatus
 
-from tendril.common.interests.exceptions import InterestStateException
+from tendril.common.states import LifecycleStatus
 from tendril.common.interests.exceptions import RequiredRoleNotPresent
 from tendril.common.interests.exceptions import RequiredParentNotPresent
 from tendril.common.interests.exceptions import ActivationNotAllowedFromState
 from tendril.common.interests.exceptions import AuthorizationRequiredError
 
 from tendril.db.controllers.interests import get_interest
 from tendril.db.controllers.interests import upsert_interest
@@ -37,44 +36,47 @@
 from tendril.utils.db import with_db
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEFAULT)
 
 
 class InterestBaseCreateTModel(TendrilTBaseModel):
     name: str = Field(..., max_length=255)
-    descriptive_name : Optional[str] = Field(..., max_length=255)
+    descriptive_name: Optional[str] = Field(..., max_length=255)
     type: Literal['interest']
     info: dict
 
 
 class InterestBaseReadTMixin(TendrilTBaseModel):
     id: int
     roles: Optional[List[str]]
     permissions: Optional[List[str]]
-    status: InterestLifecycleStatus
+    status: LifecycleStatus
 
 
 class InterestBaseTModel(InterestBaseCreateTModel,
                          InterestBaseReadTMixin):
     ...
 
 
 class InterestBase(object):
     model = InterestModel
     tmodel_create = InterestBaseCreateTModel
     tmodel = InterestBaseTModel
     additional_fields = []
+    additional_creation_fields = []
+    additional_export_fields = []
+    additional_activation_checks = []
 
     def __init__(self, name, info=None, must_create=False,
                  can_create=True, session=None):
         self._name = None
         self._descriptive_name = None
         self._info = None
         self._model_instance: InterestModel = None
-        self._status: InterestLifecycleStatus = None
+        self._status: LifecycleStatus = None
         if isinstance(name, InterestModel):
             if must_create:
                 raise AttributeError("Expected a name, not an object")
             self._model_instance = name
         else:
             self._name = name
             self._info = info or {}
@@ -127,39 +129,95 @@
 
     @status.setter
     def status(self, value):
         self._status = value
         self._commit_to_db()
 
     @with_db
-    @require_permission('edit')
-    def activate(self, session=None):
+    def _check_activation_requirements(self, session=None):
         if self.status not in self.model.role_spec.activation_requirements['allowed_states']:
             raise ActivationNotAllowedFromState(self.status, self.id, self.name)
         for role in self.model.role_spec.activation_requirements['roles_required']:
             users = self.get_role_accepted_users(role, session=session)
             if not len(users):
                 raise RequiredRoleNotPresent(role, self.id, self.name)
         if self.model.role_spec.activation_requirements['parent_required']:
             if not len(self.parents(limited=False, session=session)):
                 raise RequiredParentNotPresent(self.id, self.name)
-        logger.info(f"Activating {self.model.type_name} Interest {self.id} {self.name}")
-        self._model_instance.status = InterestLifecycleStatus.ACTIVE
+
+    @property
+    def _additional_activation_checks(self):
+        try:
+            mro = list(self.__class__.__mro__)
+        except AttributeError:
+            print(f"There isn't an __mro__ on {self.__class__}. "
+                  f"This is probably a classic class. We don't support this.")
+            return self.additional_activation_checks
+        rv = []
+        for cls in mro:
+            if hasattr(cls, 'additional_activation_checks'):
+                for check_fn in cls.additional_activation_checks:
+                    rv.append(check_fn)
+        return rv
+
+    @with_db
+    @require_permission('edit', strip_auth=False, required=False)
+    @require_state([LifecycleStatus.NEW, LifecycleStatus.APPROVAL, LifecycleStatus.ACTIVE])
+    def activate(self, background_tasks=None, auth_user=None, session=None):
+        # logger.debug(f"Attempting to activate {self.type_name} {self.id}")
+        if self.model_instance.status == LifecycleStatus.ACTIVE:
+            msg = f"{self.model.type_name} Interest {self.id} {self.name} is already active"
+            logger.info(msg)
+            return False, msg
+
+        # logger.debug(f"Checking Activation Requirements for {self.type_name} {self.id}")
+        self._check_activation_requirements(session=session)
+
+        for check_fn_orig in self._additional_activation_checks:
+            # logger.debug(f"Trying Additional Activation Check for {self.type_name} {self.id} : {check_fn_orig}")
+            if not callable(check_fn_orig):
+                check_fn = getattr(self, check_fn_orig)
+            else:
+                check_fn = check_fn_orig
+            result = check_fn(auth_user=auth_user, session=session)
+            if not result:
+                msg = f"Additional activation check '{check_fn_orig}' failed. " \
+                      f"Will not activate."
+                logger.debug(msg)
+                return False, msg
+            # else:
+            #   logger.debug(f"Additional activation check '{check_fn_orig}' passed. Got {result}.")
+
+        logger.debug(f"Passed all activation checks. Activating {self.type_name} {self.id}")
+        self._model_instance.status = LifecycleStatus.ACTIVE
         session.add(self._model_instance)
+        msg = f"Activated {self.model.type_name} Interest {self.id} {self.name}"
+        logger.info(msg)
+        return True, msg
+
+    @with_db
+    @require_permission('edit', strip_auth=False, required=False)
+    @require_state([LifecycleStatus.ACTIVE, LifecycleStatus.APPROVAL])
+    def deactivate(self, auth_user=None, session=None):
+        self._model_instance.status = LifecycleStatus.NEW
+        session.add(self.model_instance)
+        msg = f"Deactivated {self.model.type_name} Interest {self.id} {self.name}"
+        logger.info(msg)
+        return msg
 
     @property
     def roles(self):
         return self._model_instance.role_spec.roles
 
     @property
     def allowed_children(self):
         return self._model_instance.role_spec.allowed_children
 
     @with_db
-    @require_state(InterestLifecycleStatus.ACTIVE,
+    @require_state(LifecycleStatus.ACTIVE,
                    exceptions=[(('status', 'NEW'),)])
     @require_permission('add_member', specifier='role', required=False,
                         preprocessor=normalize_role_name, strip_auth=False,
                         exceptions=[(('status', 'NEW'), ('role', 'self.model.role_spec.apex_role'))])
     def assign_role(self, role=None, user=None, reference=None, auth_user=None, session=None):
         if not reference:
             reference = {}
@@ -202,14 +260,15 @@
 
     @with_db
     def get_role_accepted_users(self, role, session=None):
         return self.memberships(role=role, session=session)
 
     @with_db
     def check_user_access(self, user, action, session=None):
+        logger.debug(f"Checking permissions to '{action}' on '{self}' for user '{user.id}'")
         action_roles = self.model.role_spec.get_permitted_roles(action)
         user_roles = set(self.get_user_effective_roles(user, session=session))
         return any(x in user_roles for x in action_roles)
 
     @staticmethod
     def _build_ms_info_dict(user, prov):
         from tendril.authn.users import get_user_stub
@@ -291,14 +350,24 @@
     @require_permission('read', required=False)
     def parents(self, limited=None, session=None):
         return self._repack_interest_list(
             get_parents(self.id, limited=limited, session=session)
         )
 
     @with_db
+    @require_permission('read', strip_auth=False, required=False)
+    def ancestors(self, auth_user=None, session=None):
+        rv = []
+        parents = self.parents(auth_user=auth_user, session=session)
+        rv.extend(parents)
+        for parent in parents:
+            rv.extend(parent.ancestors(auth_user=auth_user, session=session))
+        return rv
+
+    @with_db
     @require_permission('read_children', strip_auth=False, required=False,
                         specifier='child_type', preprocessor=normalize_type_name)
     def children(self, child_type=None, limited=None, auth_user=None, session=None):
         return self._repack_interest_list(
             get_children(self.id, self.type_name,
                          child_type=child_type, limited=limited, session=session)
         )
@@ -306,15 +375,15 @@
     @staticmethod
     def _get_child_type(cls, child, *a, **k):
         if isinstance(child, int):
             child = get_interest(id=child)
         return child.type_name
 
     @with_db
-    @require_state(InterestLifecycleStatus.ACTIVE)
+    @require_state(LifecycleStatus.ACTIVE)
     @require_permission('add_child', specifier=_get_child_type, preprocessor=normalize_type_name)
     def add_child(self, child, limited=False, session=None):
         return add_child(child, self.id, self.type_name,
                          limited=limited, session=session)
 
     @with_db
     def add_artefact(self, artefact, session=None):
@@ -341,34 +410,42 @@
     def artefacts(self, artefact_type, session=None):
         pass
 
     @with_db
     @require_permission(action='read', strip_auth=False, required=False)
     def export(self, session=None, auth_user=None,
                include_permissions=False,
-               include_roles=False):
+               include_roles=False, **kwargs):
         rv = {
             'name': self.name,
             'type': self.type_name,
             'id': self.id,
             'info': self.info,
             'status': self.status,
             'descriptive_name': self.descriptive_name,
         }
         for field in self.additional_fields:
             rv[field] = getattr(self, field)
+        for field in self.additional_export_fields:
+            rv[field] = getattr(self, field)
         if include_roles or include_permissions:
             user_roles = self.get_user_effective_roles(auth_user, session=session)
-        if include_roles:
-            rv['roles'] = sorted(user_roles)
-        if include_permissions:
-            rv['permissions'] = sorted(self.model.role_spec.get_roles_permissions(user_roles))
+            if include_roles:
+                rv['roles'] = sorted(user_roles)
+            if include_permissions:
+                rv['permissions'] = sorted(self.model.role_spec.get_roles_permissions(user_roles))
+        if hasattr(super(), 'export'):
+            rv.update(super().export(session=session, auth_user=auth_user, **kwargs))
         return rv
 
     @property
+    def role_spec(self):
+        return self.model.role_spec
+
+    @property
     def model_instance(self):
         return self._model_instance
 
     @with_db
     def _commit_to_db(self, must_create=False, can_create=True, session=None):
         kwargs = {'name': self.name,
                   'info': self.info,
```

### Comparing `tendril-interests-0.2.9/src/tendril/interests/manager.py` & `tendril-interests-0.3.0/src/tendril/interests/manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,46 +19,53 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 Tendril Interest Manager (:mod:`tendril.interest.manager`)
 ======================================================
 """
 
 
+import copy
 import importlib
 import networkx
 
 from tendril.utils.db import with_db
 from tendril.utils.db import register_for_create
 from tendril.utils.versions import get_namespace_package_names
 
 from tendril.db.controllers.interests import register_interest_role
+from tendril.db.controllers.interests_approvals import register_approval_type
+from tendril.authz.approvals.interests import ApprovalRequirement
 
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEBUG)
 
 
 class InterestManager(object):
     def __init__(self, prefix):
         self._prefix = prefix
         self._types = {}
         self._type_codes = {}
         self._type_spec = {}
         self.type_tree = None
         self.possible_parents = {}
         self.possible_paths = {}
+        self.possible_ancestors = {}
+        self._approval_types = {}
         self.all_actions = {}
         self._roles = {}
         self._docs = []
         self._load_interests()
 
     def _load_interests(self):
         logger.info("Loading interest types from {0}".format(self._prefix))
         modules = list(get_namespace_package_names(self._prefix))
         for m_name in modules:
-            if m_name in [__name__, f"{self._prefix}.db", f"{self._prefix}.template"]:
+            if m_name in [__name__, f"{self._prefix}.db",
+                          f"{self._prefix}.template",
+                          f'{self._prefix}.mixins']:
                 continue
             m = importlib.import_module(m_name)
             m.load(self)
         logger.info("Done loading interest types from {0}".format(self._prefix))
 
     def register_interest_type(self, name, interest, doc=None):
         logger.info(f"Registering <{interest.__name__}> to handle Interest type '{name}'")
@@ -70,24 +77,41 @@
         self._roles[name] = doc
 
     @with_db
     def commit_interest_roles(self, session=None):
         for name, doc in self._roles.items():
             register_interest_role(name, doc, session=session)
 
+    def register_approval_type(self, approval_type: ApprovalRequirement):
+        logger.info(f"Registering Interest Approval Type '{approval_type.name}'")
+        if approval_type.name in self._approval_types.keys():
+            pass
+        self._approval_types[approval_type.name] = approval_type
+
+    def extract_approval_types(self):
+        for interest_type_name, interest_type in self._types.items():
+            if hasattr(interest_type, 'approval_spec'):
+                for approval_type in interest_type.model.approval_spec.recognized_approvals:
+                    self.register_approval_type(approval_type)
+
+    @with_db
+    def commit_approval_types(self, session=None):
+        for name, approval_type in self._approval_types.items():
+            register_approval_type(approval_type, session=session)
+
     @property
     def types(self):
         return self._types
 
     def _create_tree_edges(self):
         """Creates a graph from the spec dict
         """
         list_of_edges = []
         for item in self._type_spec.keys():
-            allowed_children = self._type_spec[item]['allowed_children']
+            allowed_children = copy.copy(self._type_spec[item]['allowed_children'])
             if allowed_children == ["*"]:
                 allowed_children = [itemtype for itemtype in self._type_spec.keys()]
             while item in allowed_children:
                 allowed_children.remove(item)
             for child in allowed_children:
                 list_of_edges.append((item, child))
         return list_of_edges
@@ -99,21 +123,26 @@
         interest_tree.add_edges_from(self._create_tree_edges())
         return interest_tree
 
     def _possible_type_parents(self, type_name):
         paths = networkx.all_simple_paths(self.type_tree, self._tree_root(), type_name)
         parents = []
         [parents.append(x[-2])
-         for x in sorted(paths, key=lambda x: len(x))
+         for x in sorted(paths, key=lambda x: len(x), reverse=True)
          if x[-2] not in parents]
+        if type_name in self._type_spec[type_name]['allowed_children']:
+            parents.append(type_name)
         return parents
 
     def _possible_type_paths(self, type_name):
         return list(networkx.all_simple_paths(self.type_tree, self._tree_root(), type_name))
 
+    def _possible_type_ancestors(self, type_name):
+        return networkx.ancestors(self.type_tree, type_name)
+
     def _tree_root(self):
         return list(networkx.topological_sort(self.type_tree))[0]
 
     def finalize(self):
         self._type_codes = {
                 x.model.type_name: x
                 for x in self._types.values()
@@ -131,20 +160,26 @@
 
             self.possible_parents = {x: self._possible_type_parents(x)
                                      for x in self._type_codes}
 
             self.possible_paths = {x: self._possible_type_paths(x)
                                    for x in self._type_codes}
 
+            self.possible_ancestors = {x: self._possible_type_ancestors(x)
+                                       for x in self._type_codes}
+
         [self.all_actions.update(
             {f'{t.model.type_name}:{a}': r
              for a, r in t.model.role_spec.actions.items()})
             for t in self._types.values()]
 
+        self.extract_approval_types()
+
         register_for_create(self.commit_interest_roles)
+        register_for_create(self.commit_approval_types)
 
     def __getattr__(self, item):
         if item == '__file__':
             return None
         if item == '__path__':
             return None
         if item == '__len__':
```

### Comparing `tendril-interests-0.2.9/src/tendril/libraries/interests/manager.py` & `tendril-interests-0.3.0/src/tendril/libraries/interests/manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,46 @@
 
 
 import importlib
+from functools import cached_property
+from sqlalchemy.exc import NoResultFound
 
+from tendril.db.controllers.interests import get_interest
+from tendril.common.interests.exceptions import InterestNotFound
 from tendril.utils.versions import get_namespace_package_names
 from tendril.utils import log
 logger = log.get_logger(__name__, log.DEBUG)
 
 
 class InterestLibraryManager(object):
     def __init__(self, prefix):
         self._prefix = prefix
         self._libraries = {}
         self._exc_classes = {}
         self._load_libraries()
 
+    def recognized_idents(self):
+        rv = []
+        for lib in self._libraries.values():
+            rv.extend(lib.idents())
+        return rv
+
+    def recognized_names(self):
+        rv = {}
+        for lname, lib in self._libraries.items():
+            rv.update({x: lname for x in lib.names()})
+        return rv
+
+    def name_available(self, name):
+        i = get_interest(name=name, raise_if_none=False)
+        if i is None:
+            return True
+        else:
+            return False
+
     def _load_libraries(self):
         logger.info("Installing interest libraries from {0}".format(self._prefix))
         modules = list(get_namespace_package_names(self._prefix))
         for m_name in modules:
             if m_name == __name__:
                 continue
             m = importlib.import_module(m_name)
@@ -25,20 +48,30 @@
         logger.info("Done installing interest libraries modules from {0}".format(self._prefix))
 
     def install_library(self, name, library):
         logger.info("Installing interest library '{0}'".format(name))
         self._libraries[name] = library
         
     @property
-    def defined_types(self):
+    def libraries(self):
         return list(self._libraries.keys())
 
+    @cached_property
+    def libraries_by_typename(self):
+        return {x.type_name: x for x in self._libraries.values()}
+
     def install_exc_class(self, name, exc_class):
         self._exc_classes[name] = exc_class
 
+    def find_library(self, id):
+        try:
+            return self.libraries_by_typename[get_interest(id=id).type]
+        except NoResultFound:
+            raise InterestNotFound('<unspecified>', '<unspecified>', id=id)
+
     def __getattr__(self, item):
         if item in self._libraries.keys():
             return self._libraries[item]
         if item in self._exc_classes.keys():
             return self._exc_classes[item]
         raise AttributeError('No attribute {0} in {1}!'
                              ''.format(item, self.__class__.__name__))
```

### Comparing `tendril-interests-0.2.9/src/tendril_interests.egg-info/PKG-INFO` & `tendril-interests-0.3.0/src/tendril_interests.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,17 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.2.9
+Version: 0.3.0
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
-License: UNKNOWN
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-interests
-Description: 
-        
-        .. image:: https://img.shields.io/pypi/v/tendril-interests.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-interests
-        
-        .. image:: https://img.shields.io/pypi/pyversions/tendril-interests.svg?logo=pypi
-            :target: https://pypi.org/project/tendril-interests
-        
-        .. image:: https://img.shields.io/travis/tendril-framework/tendril-interests.svg?logo=travis
-            :target: https://travis-ci.org/tendril-framework/tendril-interests
-        
-        .. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-interests.svg?logo=coveralls
-            :target: https://coveralls.io/github/tendril-framework/tendril-interests
-        
-        .. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
-            :target: https://www.codacy.com/app/chintal/tendril-interests
-        
-        .. image:: https://img.shields.io/requires/github/tendril-framework/tendril-interests.svg
-            :target: https://requires.io/github/tendril-framework/tendril-interests/requirements
-        
-        .. image:: https://img.shields.io/pypi/l/tendril-interests.svg
-            :target: https://www.gnu.org/licenses/agpl-3.0.en.html
-        
-        
-        
-        .. inclusion-marker-do-not-remove
-        
-        Introduction
-        ------------
-        
-        TODO Some brief introduction
-        
-        
-        Package Information
-        -------------------
-        
-        The latest version of the documentation, including installation, usage, and
-        API/developer notes can be found at
-        `ReadTheDocs <https://tendril-interests.readthedocs.io/en/latest/index.html>`_.
-        
-        The latest version of the sources can be found at
-        `GitHub <https://github.com/tendril-framework/tendril-interests>`_. Please use 
-        GitHub's features to report bugs, request features, or submit pull/merge requests.
-        
-        The principle author for ``tendril-interests`` is Chintalagiri Shashank. The 
-        author can be contacted if necessary via the information on the
-        `author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
-        for a full list of collaborators and/or contributing authors, if any.
-        
-        ``tendril-interests`` is distributed under the terms of the
-        `AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
-        A copy of the text of the license is included along with the sources.
-        
-        
-        
 Keywords: tendril
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -81,7 +25,63 @@
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: build
 Provides-Extra: publish
 Provides-Extra: dev
+License-File: LICENSE
+
+
+
+.. image:: https://img.shields.io/pypi/v/tendril-interests.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-interests
+
+.. image:: https://img.shields.io/pypi/pyversions/tendril-interests.svg?logo=pypi
+    :target: https://pypi.org/project/tendril-interests
+
+.. image:: https://img.shields.io/travis/tendril-framework/tendril-interests.svg?logo=travis
+    :target: https://travis-ci.org/tendril-framework/tendril-interests
+
+.. image:: https://img.shields.io/coveralls/github/tendril-framework/tendril-interests.svg?logo=coveralls
+    :target: https://coveralls.io/github/tendril-framework/tendril-interests
+
+.. image:: https://img.shields.io/codacy/grade/363acc44e8c240dc9db79935860191b4?logo=codacy
+    :target: https://www.codacy.com/app/chintal/tendril-interests
+
+.. image:: https://img.shields.io/requires/github/tendril-framework/tendril-interests.svg
+    :target: https://requires.io/github/tendril-framework/tendril-interests/requirements
+
+.. image:: https://img.shields.io/pypi/l/tendril-interests.svg
+    :target: https://www.gnu.org/licenses/agpl-3.0.en.html
+
+
+
+.. inclusion-marker-do-not-remove
+
+Introduction
+------------
+
+TODO Some brief introduction
+
+
+Package Information
+-------------------
+
+The latest version of the documentation, including installation, usage, and
+API/developer notes can be found at
+`ReadTheDocs <https://tendril-interests.readthedocs.io/en/latest/index.html>`_.
+
+The latest version of the sources can be found at
+`GitHub <https://github.com/tendril-framework/tendril-interests>`_. Please use 
+GitHub's features to report bugs, request features, or submit pull/merge requests.
+
+The principle author for ``tendril-interests`` is Chintalagiri Shashank. The 
+author can be contacted if necessary via the information on the
+`author's github profile <https://github.com/chintal>`_ . See the AUTHORS file
+for a full list of collaborators and/or contributing authors, if any.
+
+``tendril-interests`` is distributed under the terms of the
+`AGPLv3 license <https://www.gnu.org/licenses/agpl-3.0.en.html>`_ .
+A copy of the text of the license is included along with the sources.
+
+
```

### Comparing `tendril-interests-0.2.9/src/tendril_interests.egg-info/SOURCES.txt` & `tendril-interests-0.3.0/src/tendril_interests.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -23,38 +23,53 @@
 src/tendril/__init__.py
 src/tendril/apiserver/__init__.py
 src/tendril/apiserver/routers/__init__.py
 src/tendril/apiserver/routers/interests.py
 src/tendril/apiserver/templates/__init__.py
 src/tendril/apiserver/templates/base.py
 src/tendril/apiserver/templates/interests.py
+src/tendril/apiserver/templates/interests_approvals.py
 src/tendril/authz/__init__.py
+src/tendril/authz/approvals/__init__.py
+src/tendril/authz/approvals/interests.py
+src/tendril/authz/approvals/manager.py
 src/tendril/authz/roles/__init__.py
 src/tendril/authz/roles/interests.py
+src/tendril/authz/roles/interests_approvals.py
 src/tendril/authz/scopes/__init__.py
 src/tendril/authz/scopes/interests.py
 src/tendril/common/__init__.py
+src/tendril/common/states.py
 src/tendril/common/interests/__init__.py
+src/tendril/common/interests/approvals.py
 src/tendril/common/interests/exceptions.py
 src/tendril/common/interests/memberships.py
-src/tendril/common/interests/states.py
+src/tendril/common/interests/representations.py
 src/tendril/config/__init__.py
 src/tendril/config/interests.py
 src/tendril/db/__init__.py
 src/tendril/db/controllers/__init__.py
 src/tendril/db/controllers/interests.py
+src/tendril/db/controllers/interests_approvals.py
+src/tendril/db/mixins/__init__.py
+src/tendril/db/mixins/interests.py
 src/tendril/db/models/__init__.py
 src/tendril/db/models/interests.py
+src/tendril/db/models/interests_approvals.py
 src/tendril/interests/__init__.py
 src/tendril/interests/base.py
 src/tendril/interests/manager.py
+src/tendril/interests/mixins/__init__.py
+src/tendril/interests/mixins/approvals.py
 src/tendril/libraries/__init__.py
 src/tendril/libraries/interests/__init__.py
 src/tendril/libraries/interests/base.py
 src/tendril/libraries/interests/manager.py
+src/tendril/libraries/mixins/__init__.py
+src/tendril/libraries/mixins/interests_approvals.py
 src/tendril_interests.egg-info/PKG-INFO
 src/tendril_interests.egg-info/SOURCES.txt
 src/tendril_interests.egg-info/dependency_links.txt
 src/tendril_interests.egg-info/requires.txt
 src/tendril_interests.egg-info/top_level.txt
 tests/__init__.py
 tests/coveralls.py
```

### Comparing `tendril-interests-0.2.9/src/tendril_interests.egg-info/requires.txt` & `tendril-interests-0.3.0/src/tendril_interests.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 tendril-utils-db>=0.4.3
 tendril-auth
 networkx
 polars
 makefun
+asgiref
 wheel
 
 [build]
 setuptools_scm
 sphinx
 sphinx-argparse
 alabaster
```

### Comparing `tendril-interests-0.2.9/tests/coveralls.py` & `tendril-interests-0.3.0/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-interests-0.2.9/tox.ini` & `tendril-interests-0.3.0/tox.ini`

 * *Files identical despite different names*

