# Comparing `tmp/pyramid_formencode_classic-0.5.0.tar.gz` & `tmp/pyramid_formencode_classic-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyramid_formencode_classic-0.5.0.tar", last modified: Wed Jul 26 18:22:20 2023, max compression
+gzip compressed data, was "pyramid_formencode_classic-0.5.1.tar", last modified: Wed Jul 26 19:32:17 2023, max compression
```

## Comparing `pyramid_formencode_classic-0.5.0.tar` & `pyramid_formencode_classic-0.5.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/
--rw-r--r--   0 jvanasco   (501) admin       (80)     8177 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/CHANGES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       82 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/pyproject.toml
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)   119760 2023-06-16 19:20:00.000000 pyramid_formencode_classic-0.5.0/tests/test_core.py
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2018-07-06 19:51:51.000000 pyramid_formencode_classic-0.5.0/tests/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/tests/fixtures/
--rw-r--r--   0 jvanasco   (501) admin       (80)      254 2018-07-09 21:19:45.000000 pyramid_formencode_classic-0.5.0/tests/fixtures/form_a-html_error_placeholder-none.mako
--rw-r--r--   0 jvanasco   (501) admin       (80)      305 2019-04-29 17:59:54.000000 pyramid_formencode_classic-0.5.0/tests/fixtures/form_a-html_error_placeholder-explicit.mako
--rw-r--r--   0 jvanasco   (501) admin       (80)      293 2018-07-09 19:58:30.000000 pyramid_formencode_classic-0.5.0/tests/fixtures/form_a-html_error_placeholder-default.mako
--rw-r--r--   0 jvanasco   (501) admin       (80)      676 2018-07-10 22:33:13.000000 pyramid_formencode_classic-0.5.0/tests/fixtures/form_b-multi.mako
--rw-r--r--   0 jvanasco   (501) admin       (80)      304 2019-04-29 17:59:50.000000 pyramid_formencode_classic-0.5.0/tests/fixtures/form_a-html_error_placeholder-alt.mako
--rw-r--r--   0 jvanasco   (501) admin       (80)    26396 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)     2032 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/setup.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    20888 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/tox.ini
--rw-r--r--   0 jvanasco   (501) admin       (80)      583 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)      163 2021-03-25 20:34:20.000000 pyramid_formencode_classic-0.5.0/MANIFEST.in
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/panels/
--rwxrwxrwx   0 jvanasco   (501) admin       (80)        0 2017-12-05 16:49:40.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/panels/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/panels/templates/
--rw-r--r--   0 jvanasco   (501) admin       (80)     3235 2019-09-05 21:50:23.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/panels/templates/formencode_classic.dbtmako
--rw-r--r--   0 jvanasco   (501) admin       (80)     1371 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/panels/formencode_classic.py
--rwxr-xr-x   0 jvanasco   (501) admin       (80)      422 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1691 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/formatters.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     2040 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      144 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/_defaults.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    14242 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/api.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1542 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/utils.py
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/py.typed
--rw-r--r--   0 jvanasco   (501) admin       (80)     2057 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/exceptions.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    16571 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/objects.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      208 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/_utils.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 20:40:15.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)    26396 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       68 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       27 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/top_level.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     1351 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-07-26 18:22:20.000000 pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/dependency_links.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.299528 pyramid_formencode_classic-0.5.1/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     8177 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/CHANGES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      163 2021-03-25 20:34:20.000000 pyramid_formencode_classic-0.5.1/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)    21773 2023-07-26 19:32:17.299937 pyramid_formencode_classic-0.5.1/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)    20888 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)       82 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/pyproject.toml
+-rw-r--r--   0 jvanasco   (501) admin       (80)      583 2023-07-26 19:32:17.301509 pyramid_formencode_classic-0.5.1/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2032 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.240047 pyramid_formencode_classic-0.5.1/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.263735 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2071 2023-07-26 19:32:05.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      144 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/_defaults.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      208 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/_utils.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    14242 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/api.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.275559 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/
+-rwxr-xr-x   0 jvanasco   (501) admin       (80)      422 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/__init__.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.277864 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/panels/
+-rwxrwxrwx   0 jvanasco   (501) admin       (80)        0 2017-12-05 16:49:40.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/panels/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1371 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/panels/formencode_classic.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.279227 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/panels/templates/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3235 2019-09-05 21:50:23.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/panels/templates/formencode_classic.dbtmako
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2057 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/exceptions.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1691 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/formatters.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    16571 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/objects.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/py.typed
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1542 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/utils.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.272593 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)    21773 2023-07-26 19:32:17.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1351 2023-07-26 19:32:17.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-07-26 19:32:17.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 20:40:15.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)       68 2023-07-26 19:32:17.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       27 2023-07-26 19:32:17.000000 pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/top_level.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.282225 pyramid_formencode_classic-0.5.1/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2018-07-06 19:51:51.000000 pyramid_formencode_classic-0.5.1/tests/__init__.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-07-26 19:32:17.297868 pyramid_formencode_classic-0.5.1/tests/fixtures/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      304 2019-04-29 17:59:50.000000 pyramid_formencode_classic-0.5.1/tests/fixtures/form_a-html_error_placeholder-alt.mako
+-rw-r--r--   0 jvanasco   (501) admin       (80)      293 2018-07-09 19:58:30.000000 pyramid_formencode_classic-0.5.1/tests/fixtures/form_a-html_error_placeholder-default.mako
+-rw-r--r--   0 jvanasco   (501) admin       (80)      305 2019-04-29 17:59:54.000000 pyramid_formencode_classic-0.5.1/tests/fixtures/form_a-html_error_placeholder-explicit.mako
+-rw-r--r--   0 jvanasco   (501) admin       (80)      254 2018-07-09 21:19:45.000000 pyramid_formencode_classic-0.5.1/tests/fixtures/form_a-html_error_placeholder-none.mako
+-rw-r--r--   0 jvanasco   (501) admin       (80)      676 2018-07-10 22:33:13.000000 pyramid_formencode_classic-0.5.1/tests/fixtures/form_b-multi.mako
+-rw-r--r--   0 jvanasco   (501) admin       (80)   119760 2023-06-16 19:20:00.000000 pyramid_formencode_classic-0.5.1/tests/test_core.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-07-26 18:22:00.000000 pyramid_formencode_classic-0.5.1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyramid_formencode_classic-0.5.0/CHANGES.txt` & `pyramid_formencode_classic-0.5.1/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.0/tests/test_core.py` & `pyramid_formencode_classic-0.5.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.0/tests/fixtures/form_b-multi.mako` & `pyramid_formencode_classic-0.5.1/tests/fixtures/form_b-multi.mako`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.0/setup.py` & `pyramid_formencode_classic-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.0/README.md` & `pyramid_formencode_classic-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.0/setup.cfg` & `pyramid_formencode_classic-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/panels/templates/formencode_classic.dbtmako` & `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/panels/templates/formencode_classic.dbtmako`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/debugtoolbar/panels/formencode_classic.py` & `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/debugtoolbar/panels/formencode_classic.py`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/formatters.py` & `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/formatters.py`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/__init__.py` & `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # pypi
 import webob.compat
 
 # local
 from .api import form_reprint  # noqa: F401 ; maintain API
 from .api import form_validate  # noqa: F401 ; maintain API
 from .exceptions import FormInvalid  # noqa: F401 ; maintain API
+from .objects import FormStash
 from .objects import FormStashList
 
 if TYPE_CHECKING:
     from pyramid.config import Configurator
     from pyramid.request import Request
 
 # ==============================================================================
@@ -28,15 +29,15 @@
 
 def warn_user(message):
     warnings.warn(message, UserWarning, stacklevel=2)
 """
 
 
 # defaults
-__VERSION__ = "0.5.0"
+__VERSION__ = "0.5.1"
 
 AUTOMATIC_CLEANUP = True
 
 log = logging.getLogger(__name__)
 
 
 # ------------------------------------------------------------------------------
```

### Comparing `pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/api.py` & `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/api.py`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/utils.py` & `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/utils.py`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/exceptions.py` & `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic/objects.py` & `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic/objects.py`

 * *Files identical despite different names*

### Comparing `pyramid_formencode_classic-0.5.0/src/pyramid_formencode_classic.egg-info/SOURCES.txt` & `pyramid_formencode_classic-0.5.1/src/pyramid_formencode_classic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

