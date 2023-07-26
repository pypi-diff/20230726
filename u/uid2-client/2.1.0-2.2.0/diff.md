# Comparing `tmp/uid2_client-2.1.0.tar.gz` & `tmp/uid2_client-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uid2_client-2.1.0.tar", last modified: Thu Jul 20 21:08:29 2023, max compression
+gzip compressed data, was "uid2_client-2.2.0.tar", last modified: Wed Jul 26 18:40:33 2023, max compression
```

## Comparing `uid2_client-2.1.0.tar` & `uid2_client-2.2.0.tar`

### file list

```diff
@@ -1,34 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:08:29.198895 uid2_client-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-07-20 21:08:21.000000 uid2_client-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-20 21:08:29.198895 uid2_client-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-20 21:08:21.000000 uid2_client-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-20 21:08:21.000000 uid2_client-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-20 21:08:29.202895 uid2_client-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 21:08:21.000000 uid2_client-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:08:29.198895 uid2_client-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12130 2023-07-20 21:08:21.000000 uid2_client-2.1.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29296 2023-07-20 21:08:21.000000 uid2_client-2.1.0/tests/test_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-20 21:08:21.000000 uid2_client-2.1.0/tests/test_key_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-20 21:08:21.000000 uid2_client-2.1.0/tests/test_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-20 21:08:21.000000 uid2_client-2.1.0/tests/test_sharing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-20 21:08:21.000000 uid2_client-2.1.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:08:29.198895 uid2_client-2.1.0/uid2_client/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/advertising_token_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/auto_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/euid_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/identity_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/identity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/request_response_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/uid2_base64_url_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-20 21:08:21.000000 uid2_client-2.1.0/uid2_client/uid2_client_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 21:08:29.198895 uid2_client-2.1.0/uid2_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-07-20 21:08:29.000000 uid2_client-2.1.0/uid2_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-20 21:08:29.000000 uid2_client-2.1.0/uid2_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:08:29.000000 uid2_client-2.1.0/uid2_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 21:08:29.000000 uid2_client-2.1.0/uid2_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 21:08:29.000000 uid2_client-2.1.0/uid2_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 21:08:28.000000 uid2_client-2.1.0/uid2_client.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:40:33.931265 uid2_client-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-07-26 18:40:24.000000 uid2_client-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-26 18:40:33.931265 uid2_client-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-26 18:40:24.000000 uid2_client-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-26 18:40:24.000000 uid2_client-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-26 18:40:33.931265 uid2_client-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 18:40:24.000000 uid2_client-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:40:33.931265 uid2_client-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12130 2023-07-26 18:40:24.000000 uid2_client-2.2.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29296 2023-07-26 18:40:24.000000 uid2_client-2.2.0/tests/test_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-07-26 18:40:24.000000 uid2_client-2.2.0/tests/test_key_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-26 18:40:24.000000 uid2_client-2.2.0/tests/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-07-26 18:40:24.000000 uid2_client-2.2.0/tests/test_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10696 2023-07-26 18:40:24.000000 uid2_client-2.2.0/tests/test_publisher_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-07-26 18:40:24.000000 uid2_client-2.2.0/tests/test_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-26 18:40:24.000000 uid2_client-2.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:40:33.931265 uid2_client-2.2.0/uid2_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/advertising_token_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/auto_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/euid_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/identity_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/identity_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/identity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/input_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/publisher_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/request_response_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/token_generate_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/token_generate_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/token_refresh_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/uid2_base64_url_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-26 18:40:24.000000 uid2_client-2.2.0/uid2_client/uid2_client_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:40:33.931265 uid2_client-2.2.0/uid2_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-26 18:40:33.000000 uid2_client-2.2.0/uid2_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-26 18:40:33.000000 uid2_client-2.2.0/uid2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:40:33.000000 uid2_client-2.2.0/uid2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 18:40:33.000000 uid2_client-2.2.0/uid2_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 18:40:33.000000 uid2_client-2.2.0/uid2_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:40:33.000000 uid2_client-2.2.0/uid2_client.egg-info/zip-safe
```

### Comparing `uid2_client-2.1.0/LICENSE` & `uid2_client-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uid2_client-2.1.0/pyproject.toml` & `uid2_client-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools >= 40.9.0",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uid2_client"
-version = "2.1.0"
+version = "2.2.0"
 authors = [
     { name = "UID2 team", email = "unifiedid-admin@thetradedesk.com" }
 ]
 description = "UID2 SDK for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `uid2_client-2.1.0/setup.cfg` & `uid2_client-2.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `uid2_client-2.1.0/tests/test_client.py` & `uid2_client-2.2.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.1.0/tests/test_encryption.py` & `uid2_client-2.2.0/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.1.0/tests/test_key_parse.py` & `uid2_client-2.2.0/tests/test_key_parse.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.1.0/tests/test_keys.py` & `uid2_client-2.2.0/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.1.0/tests/test_sharing.py` & `uid2_client-2.2.0/tests/test_sharing.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.1.0/tests/test_utils.py` & `uid2_client-2.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.1.0/uid2_client/auto_refresh.py` & `uid2_client-2.2.0/uid2_client/auto_refresh.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.1.0/uid2_client/client.py` & `uid2_client-2.2.0/uid2_client/client.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.1.0/uid2_client/encryption.py` & `uid2_client-2.2.0/uid2_client/encryption.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
     Raises:
         ValueError: if invalid parameter combinations are specified through **kwargs
         EncryptionError: if advertising_token cannot be decrypted, no key can be found
                          for the site_id, or the key has expired
 
     The keyword arguments key, keys, site_id and advertising_token can only be used in
     the following combinations:
-        - key: use the specied key
+        - key: use the specified key
         - keys and site_id: find the key for the specified site_id
         - keys and advertising_token: extract site_id from the token and find a key for it
     """
     now = kwargs.get("now")
     if now is None:
         now = dt.datetime.now(tz=timezone.utc)
     keys = kwargs.get("keys")
```

### Comparing `uid2_client-2.1.0/uid2_client/keys.py` & `uid2_client-2.2.0/uid2_client/keys.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.1.0/uid2_client/request_response_util.py` & `uid2_client-2.2.0/uid2_client/request_response_util.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.1.0/uid2_client/uid2_base64_url_coder.py` & `uid2_client-2.2.0/uid2_client/uid2_base64_url_coder.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.1.0/uid2_client.egg-info/SOURCES.txt` & `uid2_client-2.2.0/uid2_client.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,26 +3,34 @@
 pyproject.toml
 setup.cfg
 setup.py
 tests/test_client.py
 tests/test_encryption.py
 tests/test_key_parse.py
 tests/test_keys.py
+tests/test_normalization.py
+tests/test_publisher_client.py
 tests/test_sharing.py
 tests/test_utils.py
 uid2_client/__init__.py
 uid2_client/advertising_token_version.py
 uid2_client/auto_refresh.py
 uid2_client/client.py
 uid2_client/encryption.py
 uid2_client/euid_client_factory.py
 uid2_client/identity_scope.py
+uid2_client/identity_tokens.py
 uid2_client/identity_type.py
+uid2_client/input_util.py
 uid2_client/keys.py
+uid2_client/publisher_client.py
 uid2_client/request_response_util.py
+uid2_client/token_generate_input.py
+uid2_client/token_generate_response.py
+uid2_client/token_refresh_response.py
 uid2_client/uid2_base64_url_coder.py
 uid2_client/uid2_client_factory.py
 uid2_client.egg-info/PKG-INFO
 uid2_client.egg-info/SOURCES.txt
 uid2_client.egg-info/dependency_links.txt
 uid2_client.egg-info/requires.txt
 uid2_client.egg-info/top_level.txt
```

