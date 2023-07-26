# Comparing `tmp/bento_lib-7.1.0.tar.gz` & `tmp/bento_lib-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_lib-7.1.0.tar", last modified: Mon Jul 24 20:34:43 2023, max compression
+gzip compressed data, was "bento_lib-7.2.0.tar", last modified: Wed Jul 26 19:51:22 2023, max compression
```

## Comparing `bento_lib-7.1.0.tar` & `bento_lib-7.2.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.293377 bento_lib-7.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-24 20:34:33.000000 bento_lib-7.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-24 20:34:33.000000 bento_lib-7.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-24 20:34:43.293377 bento_lib-7.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-24 20:34:33.000000 bento_lib-7.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.289377 bento_lib-7.1.0/bento_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.289377 bento_lib-7.1.0/bento_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.289377 bento_lib-7.1.0/bento_lib/auth/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/middleware/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/middleware/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/middleware/django.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/middleware/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/auth/middleware/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.289377 bento_lib-7.1.0/bento_lib/drs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/drs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.289377 bento_lib-7.1.0/bento_lib/events/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/events/_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/events/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/package.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.293377 bento_lib-7.1.0/bento_lib/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/responses/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/responses/fastapi_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/responses/flask_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.293377 bento_lib-7.1.0/bento_lib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/schemas/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/schemas/bento.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/schemas/bento_data_use.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/schemas/bento_ingest.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/schemas/ga4gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/schemas/ga4gh_service_info.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.293377 bento_lib-7.1.0/bento_lib/search/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/search/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/search/data_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/search/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/search/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-24 20:34:33.000000 bento_lib-7.1.0/bento_lib/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 20:34:43.289377 bento_lib-7.1.0/bento_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-24 20:34:43.000000 bento_lib-7.1.0/bento_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-24 20:34:43.000000 bento_lib-7.1.0/bento_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 20:34:43.000000 bento_lib-7.1.0/bento_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-24 20:34:43.000000 bento_lib-7.1.0/bento_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-24 20:34:43.000000 bento_lib-7.1.0/bento_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 20:34:43.293377 bento_lib-7.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-24 20:34:33.000000 bento_lib-7.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.226414 bento_lib-7.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-26 19:51:11.000000 bento_lib-7.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 19:51:11.000000 bento_lib-7.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-26 19:51:22.226414 bento_lib-7.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-26 19:51:11.000000 bento_lib-7.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.222414 bento_lib-7.2.0/bento_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.222414 bento_lib-7.2.0/bento_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.226414 bento_lib-7.2.0/bento_lib/auth/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/middleware/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/middleware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/middleware/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/middleware/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/auth/middleware/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.226414 bento_lib-7.2.0/bento_lib/drs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/drs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.226414 bento_lib-7.2.0/bento_lib/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/events/_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/events/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/package.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.226414 bento_lib-7.2.0/bento_lib/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/responses/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/responses/fastapi_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/responses/flask_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.226414 bento_lib-7.2.0/bento_lib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/schemas/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/schemas/bento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/schemas/bento_data_use.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/schemas/bento_ingest.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/schemas/ga4gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/schemas/ga4gh_service_info.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.226414 bento_lib-7.2.0/bento_lib/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/search/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/search/data_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/search/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/search/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-26 19:51:11.000000 bento_lib-7.2.0/bento_lib/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:51:22.222414 bento_lib-7.2.0/bento_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-26 19:51:22.000000 bento_lib-7.2.0/bento_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-26 19:51:22.000000 bento_lib-7.2.0/bento_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:51:22.000000 bento_lib-7.2.0/bento_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-26 19:51:22.000000 bento_lib-7.2.0/bento_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 19:51:22.000000 bento_lib-7.2.0/bento_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:51:22.226414 bento_lib-7.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-26 19:51:11.000000 bento_lib-7.2.0/setup.py
```

### Comparing `bento_lib-7.1.0/LICENSE` & `bento_lib-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/PKG-INFO` & `bento_lib-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento_lib
-Version: 7.1.0
+Version: 7.2.0
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `bento_lib-7.1.0/README.md` & `bento_lib-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/bento_lib/auth/middleware/base.py` & `bento_lib-7.2.0/bento_lib/auth/middleware/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,26 +12,28 @@
 
 class BaseAuthMiddleware(ABC):
     def __init__(
         self,
         bento_authz_service_url: str,
         drs_compat: bool = False,
         sr_compat: bool = False,
+        beacon_meta_callback: Callable[[], dict] | None = None,
         debug_mode: bool = False,
         enabled: bool = True,
         logger: logging.Logger | None = None,
     ):
         self._debug: bool = debug_mode
         self._verify_ssl: bool = not debug_mode
 
         self._enabled: bool = enabled
         self._logger: logging.Logger | None = logger
 
         self._drs_compat: bool = drs_compat
         self._sr_compat: bool = sr_compat
+        self._beacon_meta_callback: Callable[[], dict] | None = beacon_meta_callback
 
         self._bento_authz_service_url: str = bento_authz_service_url
 
     @property
     def enabled(self) -> bool:
         return self._enabled
```

### Comparing `bento_lib-7.1.0/bento_lib/auth/middleware/django.py` & `bento_lib-7.2.0/bento_lib/auth/middleware/django.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,21 @@
                     return self._make_auth_error(exc)
                 return None
 
         return InnerMiddleware
 
     def _make_auth_error(self, e: BentoAuthException) -> JsonResponse:
         return JsonResponse(
-            http_error(e.status_code, e.message, drs_compat=self._drs_compat, sr_compat=self._sr_compat),
+            http_error(
+                e.status_code,
+                e.message,
+                drs_compat=self._drs_compat,
+                sr_compat=self._sr_compat,
+                beacon_meta_callback=self._beacon_meta_callback,
+            ),
             status=e.status_code)
 
     async def dispatch(
         self,
         get_response: Callable[[HttpRequest], Awaitable[HttpResponse]],
         request: HttpRequest,
     ) -> HttpResponse:
```

### Comparing `bento_lib-7.1.0/bento_lib/auth/middleware/fastapi.py` & `bento_lib-7.2.0/bento_lib/auth/middleware/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,21 @@
                 # Next in response chain didn't properly think about auth; return 403
                 raise BentoAuthException(status_code=status.HTTP_403_FORBIDDEN, message="Forbidden")
 
         except BentoAuthException as e:
             self.mark_authz_done(request)
             return JSONResponse(
                 status_code=e.status_code,
-                content=http_error(e.status_code, e.message, drs_compat=self._drs_compat, sr_compat=self._sr_compat))
+                content=http_error(
+                    e.status_code,
+                    e.message,
+                    drs_compat=self._drs_compat,
+                    sr_compat=self._sr_compat,
+                    beacon_meta_callback=self._beacon_meta_callback,
+                ))
 
         # Otherwise, return the response as normal
         return res
 
     def get_authz_header_value(self, request: Request) -> str | None:
         return request.headers.get("Authorization")
```

### Comparing `bento_lib-7.1.0/bento_lib/auth/middleware/flask.py` & `bento_lib-7.2.0/bento_lib/auth/middleware/flask.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,21 @@
             g.bento_determined_authz = False
 
     def _make_auth_error(self, e: BentoAuthException) -> Response:
         # returning an error, so mark authz flow as 'done' (rejecting in one way or another):
         self.mark_authz_done(request)
         # return error response:
         return Response(
-            json.dumps(http_error(e.status_code, e.message, drs_compat=self._drs_compat, sr_compat=self._sr_compat)),
+            json.dumps(http_error(
+                e.status_code,
+                e.message,
+                drs_compat=self._drs_compat,
+                sr_compat=self._sr_compat,
+                beacon_meta_callback=self._beacon_meta_callback,
+            )),
             status=e.status_code,
             content_type="application/json")
 
     def _make_forbidden(self) -> Response:
         return self._make_auth_error(BentoAuthException("Forbidden", status_code=403))
 
     def middleware_post(self, response: Response) -> Response:
```

### Comparing `bento_lib-7.1.0/bento_lib/drs/utils.py` & `bento_lib-7.2.0/bento_lib/drs/utils.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/bento_lib/events/_event_bus.py` & `bento_lib-7.2.0/bento_lib/events/_event_bus.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/bento_lib/events/notifications.py` & `bento_lib-7.2.0/bento_lib/events/notifications.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/bento_lib/events/types.py` & `bento_lib-7.2.0/bento_lib/events/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/bento_lib/responses/errors.py` & `bento_lib-7.2.0/bento_lib/responses/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import datetime
 from functools import partial
 from werkzeug.http import HTTP_STATUS_CODES
 
+from typing import Callable
+
 
 __all__ = [
     "http_error",
 
     "bad_request_error",
     "unauthorized_error",
     "forbidden_error",
@@ -16,21 +18,29 @@
 ]
 
 
 def _error_message(message):
     return {"message": message}
 
 
-def http_error(code: int, *errors, drs_compat: bool = False, sr_compat: bool = False):
+def http_error(
+    code: int,
+    *errors,
+    drs_compat: bool = False,
+    sr_compat: bool = False,
+    beacon_meta_callback: Callable[[], dict] | None = None,
+):
     """
     Builds a dictionary for an HTTP error JSON response.
     :param code: The error status code to embed in the response.
     :param errors: A list of error descriptions (human-readable) to explain the error.
     :param drs_compat: Whether to generate a GA4GH DRS schema backwards-compatible response.
     :param sr_compat: Whether to generate a GA4GH Service Registry backwards-compatible response.
+    :param beacon_meta_callback: Callback for generating GA4GH Beacon V2 backwards-compatible meta field for
+           error response. If this is specified, Beacon V2-compatible errors will be enabled.
     :return: A dictionary to encode in JSON for the error response.
     """
 
     if code not in HTTP_STATUS_CODES:
         print(f"[Bento Lib] Error: Could not find code {code} in valid HTTP status codes.")
         code = 500
         errors = (*errors, f"An invalid status code of {code} was specified by the service.")
@@ -55,14 +65,23 @@
         # The Service Registry spec *also* has a slightly different error
         # specification; do the same thing as above.
         **({
             "status": code,
             "title": message,
             **({"detail": " | ".join(errors)} if errors else {}),
         } if sr_compat else {}),
+
+        # ... why so many "standards"? Here's a Beacon V2-compatible error specification
+        **({
+            "meta": beacon_meta_callback(),
+            "error": {
+                "errorCode": code,
+                **({"errorMessage": " | ".join(errors)} if errors else {}),
+            },
+        } if beacon_meta_callback is not None else {}),
     }
 
 
 _e = partial(partial, http_error)
 
 bad_request_error = _e(400)
 unauthorized_error = _e(401)
```

### Comparing `bento_lib-7.1.0/bento_lib/responses/fastapi_errors.py` & `bento_lib-7.2.0/bento_lib/responses/fastapi_errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,46 +23,50 @@
     if code == status.HTTP_500_INTERNAL_SERVER_ERROR:
         logger.error(f"Encountered error:\n{traceback.format_exception(type(exc), exc, exc.__traceback__)}")
 
 
 def http_exception_handler_factory(
     logger: logging.Logger,
     authz: FastApiAuthMiddleware | None = None,
+    **kwargs,
 ) -> Callable[[Request, HTTPException], Response]:
     def http_exception_handler(request: Request, exc: HTTPException) -> JSONResponse:
         if authz:
             authz.mark_authz_done(request)
         code = exc.status_code
         _log_if_500(logger, code, exc)
-        return JSONResponse(http_error(code, exc.detail), status_code=code)
+        return JSONResponse(http_error(code, exc.detail, **kwargs), status_code=code)
 
     return http_exception_handler
 
 
 def bento_auth_exception_handler_factory(
     logger: logging.Logger,
     authz: FastApiAuthMiddleware | None = None,
+    **kwargs,
 ) -> Callable[[Request, BentoAuthException], Response]:
     def bento_auth_exception_handler(request: Request, exc: BentoAuthException) -> JSONResponse:
         if authz:
             authz.mark_authz_done(request)
         code = exc.status_code
         _log_if_500(logger, code, exc)
-        return JSONResponse(http_error(code, exc.message), status_code=code)
+        return JSONResponse(http_error(code, exc.message, **kwargs), status_code=code)
 
     return bento_auth_exception_handler
 
 
 def validation_exception_handler_factory(
     authz: FastApiAuthMiddleware | None = None,
+    **kwargs,
 ) -> Callable[[Request, RequestValidationError], Response]:
     def validation_exception_handler(request: Request, exc: RequestValidationError) -> JSONResponse:
         if authz:
             authz.mark_authz_done(request)
         code = status.HTTP_400_BAD_REQUEST
         return JSONResponse(
             http_error(
                 code,
                 *((".".join(map(str, e["loc"])) + ": " + e["msg"])
-                  if e.get("loc") else e["msg"] for e in exc.errors())),
+                  if e.get("loc") else e["msg"] for e in exc.errors()),
+                **kwargs),
             status_code=code)
     return validation_exception_handler
```

### Comparing `bento_lib-7.1.0/bento_lib/responses/flask_errors.py` & `bento_lib-7.2.0/bento_lib/responses/flask_errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,16 +68,16 @@
         if authz:
             authz.mark_authz_done(request)
         return fn(str(e), *args, **kwargs)
 
     return handle_error
 
 
-def flask_error(code: int, *errs, drs_compat: bool = False, sr_compat: bool = False):
-    return jsonify(errors.http_error(code, *errs, drs_compat=drs_compat, sr_compat=sr_compat)), code
+def flask_error(code: int, *errs, **kwargs):
+    return jsonify(errors.http_error(code, *errs, **kwargs)), code
 
 
 def _flask_error(code: int) -> Callable:
     return partial(flask_error, code)
 
 
 flask_bad_request_error = _flask_error(400)
```

### Comparing `bento_lib-7.1.0/bento_lib/schemas/bento_data_use.schema.json` & `bento_lib-7.2.0/bento_lib/schemas/bento_data_use.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/bento_lib/schemas/bento_ingest.schema.json` & `bento_lib-7.2.0/bento_lib/schemas/bento_ingest.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/bento_lib/schemas/ga4gh_service_info.schema.json` & `bento_lib-7.2.0/bento_lib/schemas/ga4gh_service_info.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/bento_lib/search/data_structure.py` & `bento_lib-7.2.0/bento_lib/search/data_structure.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/bento_lib/search/operations.py` & `bento_lib-7.2.0/bento_lib/search/operations.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/bento_lib/search/postgres.py` & `bento_lib-7.2.0/bento_lib/search/postgres.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/bento_lib/search/queries.py` & `bento_lib-7.2.0/bento_lib/search/queries.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/bento_lib/types.py` & `bento_lib-7.2.0/bento_lib/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/bento_lib/workflows.py` & `bento_lib-7.2.0/bento_lib/workflows.py`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/bento_lib.egg-info/PKG-INFO` & `bento_lib-7.2.0/bento_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bento-lib
-Version: 7.1.0
+Version: 7.2.0
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `bento_lib-7.1.0/bento_lib.egg-info/SOURCES.txt` & `bento_lib-7.2.0/bento_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bento_lib-7.1.0/setup.py` & `bento_lib-7.2.0/setup.py`

 * *Files identical despite different names*

