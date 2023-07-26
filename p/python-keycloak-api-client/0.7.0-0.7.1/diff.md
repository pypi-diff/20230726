# Comparing `tmp/python-keycloak-api-client-0.7.0.tar.gz` & `tmp/python-keycloak-api-client-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-keycloak-api-client-0.7.0.tar", last modified: Mon Jun  5 10:37:27 2023, max compression
+gzip compressed data, was "python-keycloak-api-client-0.7.1.tar", last modified: Wed Jul 26 07:51:47 2023, max compression
```

## Comparing `python-keycloak-api-client-0.7.0.tar` & `python-keycloak-api-client-0.7.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-05 10:37:27.221013 python-keycloak-api-client-0.7.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1065 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2145 2023-06-05 10:37:27.221013 python-keycloak-api-client-0.7.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1072 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-05 10:37:27.221013 python-keycloak-api-client-0.7.0/keycloak_api_client/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/keycloak_api_client/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16448 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/keycloak_api_client/api_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1008 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/keycloak_api_client/data_classes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/keycloak_api_client/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1017 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/keycloak_api_client/factories.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-05 10:37:27.221013 python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2145 2023-06-05 10:37:27.000000 python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1328 2023-06-05 10:37:27.000000 python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-05 10:37:27.000000 python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       58 2023-06-05 10:37:27.000000 python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2023-06-05 10:37:27.000000 python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      135 2023-06-05 10:37:27.225013 python-keycloak-api-client-0.7.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1017 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-05 10:37:27.221013 python-keycloak-api-client-0.7.0/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17086 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/api_client_test.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-05 10:37:27.221013 python-keycloak-api-client-0.7.0/tests/cassettes/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12289 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_count_users.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    28025 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_create_client_and_create_mapper.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9991 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_delete_client.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6942 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_get_existing_user.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6950 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_get_existing_user_by_keycloak_id.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6512 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_get_not_existing_user.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6513 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_get_not_existing_user_by_id.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6954 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_get_not_existing_user_when_partially_matching_emails_returned.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12066 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_get_user_tokens.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    37491 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_password_reset.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23632 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_register_then_update_then_get_user.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9710 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_search_clients_by_client_id.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7379 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_search_for_existing_user.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6945 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_search_for_existing_user_with_limit_and_offset.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15948 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/cassettes/test_send_verification_email.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3344 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tests/factories_test.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      274 2023-06-05 10:37:26.000000 python-keycloak-api-client-0.7.0/tox.ini
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 07:51:47.348333 python-keycloak-api-client-0.7.1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1065 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       76 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2229 2023-07-26 07:51:47.348333 python-keycloak-api-client-0.7.1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1132 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 07:51:47.344332 python-keycloak-api-client-0.7.1/keycloak_api_client/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       61 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/keycloak_api_client/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16432 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/keycloak_api_client/api_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1008 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/keycloak_api_client/data_classes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/keycloak_api_client/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1017 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/keycloak_api_client/factories.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 07:51:47.348333 python-keycloak-api-client-0.7.1/python_keycloak_api_client.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2229 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/python_keycloak_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1328 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/python_keycloak_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/python_keycloak_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       58 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/python_keycloak_api_client.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/python_keycloak_api_client.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      135 2023-07-26 07:51:47.348333 python-keycloak-api-client-0.7.1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1017 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 07:51:47.348333 python-keycloak-api-client-0.7.1/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17086 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/api_client_test.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 07:51:47.348333 python-keycloak-api-client-0.7.1/tests/cassettes/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12289 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/cassettes/test_count_users.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    28025 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/cassettes/test_create_client_and_create_mapper.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9991 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/cassettes/test_delete_client.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6942 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/cassettes/test_get_existing_user.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6950 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/cassettes/test_get_existing_user_by_keycloak_id.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6512 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/cassettes/test_get_not_existing_user.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6513 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/cassettes/test_get_not_existing_user_by_id.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6954 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/cassettes/test_get_not_existing_user_when_partially_matching_emails_returned.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12066 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/cassettes/test_get_user_tokens.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    37491 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/cassettes/test_password_reset.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23632 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/cassettes/test_register_then_update_then_get_user.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9710 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/cassettes/test_search_clients_by_client_id.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7379 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/cassettes/test_search_for_existing_user.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6945 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/cassettes/test_search_for_existing_user_with_limit_and_offset.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15948 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/cassettes/test_send_verification_email.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3344 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tests/factories_test.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      274 2023-07-26 07:51:47.000000 python-keycloak-api-client-0.7.1/tox.ini
```

### Comparing `python-keycloak-api-client-0.7.0/LICENSE.txt` & `python-keycloak-api-client-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/PKG-INFO` & `python-keycloak-api-client-0.7.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-keycloak-api-client
-Version: 0.7.0
+Version: 0.7.1
 Summary: Client for Keycloak Api (mostly users and impersonation)
 Home-page: https://github.com/masterplandev/python-keycloak-api-client
 Author: Szymon Marcinkowski
 Author-email: szymon@masterhub.com
 License: MIT
 Description: # Python Keycloak Client
         
@@ -27,14 +27,17 @@
         
         ```bash
         $ pip install -e .
         ```
         
         ## Changelog
         
+        ### v0.7.1
+        - Change `client_id` value in `get_user_tokens`
+        
         ### v0.7.0
         - Added methods `search_clients_by_client_id` and `delete_client`
         - Added `KeycloakClient` dataclass
         
         ### v0.6.0
         - Added methods `create_client` and `create_mapper_for_client`
```

### Comparing `python-keycloak-api-client-0.7.0/README.md` & `python-keycloak-api-client-0.7.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 
 ```bash
 $ pip install -e .
 ```
 
 ## Changelog
 
+### v0.7.1
+- Change `client_id` value in `get_user_tokens`
+
 ### v0.7.0
 - Added methods `search_clients_by_client_id` and `delete_client`
 - Added `KeycloakClient` dataclass
 
 ### v0.6.0
 - Added methods `create_client` and `create_mapper_for_client`
```

### Comparing `python-keycloak-api-client-0.7.0/keycloak_api_client/api_client.py` & `python-keycloak-api-client-0.7.1/keycloak_api_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
             self._get_token_url(),
             data={
                 'audience': self.token_exchange_target_client_id,
                 'grant_type': 'urn:ietf:params:oauth:grant-type'
                               ':token-exchange',
                 'requested_subject': str(keycloak_id),
                 'subject_token': self._get_api_admin_oidc_token(),
-                'client_id': self.token_exchange_target_client_id,
+                'client_id': self.admin_client_id,
                 'client_secret': self.admin_client_secret,
             },
             headers={'Content-Type': 'application/x-www-form-urlencoded'}
         )
 
         if not response.ok:
             raise KeycloakApiClientException(
```

### Comparing `python-keycloak-api-client-0.7.0/keycloak_api_client/data_classes.py` & `python-keycloak-api-client-0.7.1/keycloak_api_client/data_classes.py`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/keycloak_api_client/factories.py` & `python-keycloak-api-client-0.7.1/keycloak_api_client/factories.py`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/PKG-INFO` & `python-keycloak-api-client-0.7.1/python_keycloak_api_client.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-keycloak-api-client
-Version: 0.7.0
+Version: 0.7.1
 Summary: Client for Keycloak Api (mostly users and impersonation)
 Home-page: https://github.com/masterplandev/python-keycloak-api-client
 Author: Szymon Marcinkowski
 Author-email: szymon@masterhub.com
 License: MIT
 Description: # Python Keycloak Client
         
@@ -27,14 +27,17 @@
         
         ```bash
         $ pip install -e .
         ```
         
         ## Changelog
         
+        ### v0.7.1
+        - Change `client_id` value in `get_user_tokens`
+        
         ### v0.7.0
         - Added methods `search_clients_by_client_id` and `delete_client`
         - Added `KeycloakClient` dataclass
         
         ### v0.6.0
         - Added methods `create_client` and `create_mapper_for_client`
```

### Comparing `python-keycloak-api-client-0.7.0/python_keycloak_api_client.egg-info/SOURCES.txt` & `python-keycloak-api-client-0.7.1/python_keycloak_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/setup.py` & `python-keycloak-api-client-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='python-keycloak-api-client',
-    version='0.7.0',
+    version='0.7.1',
     description='Client for Keycloak Api (mostly users and impersonation)',
     keywords='keycloak,client,api',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Szymon Marcinkowski',
     author_email='szymon@masterhub.com',
     license='MIT',
```

### Comparing `python-keycloak-api-client-0.7.0/tests/api_client_test.py` & `python-keycloak-api-client-0.7.1/tests/api_client_test.py`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/cassettes/test_count_users.yaml` & `python-keycloak-api-client-0.7.1/tests/cassettes/test_count_users.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/cassettes/test_create_client_and_create_mapper.yaml` & `python-keycloak-api-client-0.7.1/tests/cassettes/test_create_client_and_create_mapper.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/cassettes/test_delete_client.yaml` & `python-keycloak-api-client-0.7.1/tests/cassettes/test_delete_client.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/cassettes/test_get_existing_user.yaml` & `python-keycloak-api-client-0.7.1/tests/cassettes/test_get_existing_user.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/cassettes/test_get_existing_user_by_keycloak_id.yaml` & `python-keycloak-api-client-0.7.1/tests/cassettes/test_get_existing_user_by_keycloak_id.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/cassettes/test_get_not_existing_user.yaml` & `python-keycloak-api-client-0.7.1/tests/cassettes/test_get_not_existing_user.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/cassettes/test_get_not_existing_user_by_id.yaml` & `python-keycloak-api-client-0.7.1/tests/cassettes/test_get_not_existing_user_by_id.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/cassettes/test_get_not_existing_user_when_partially_matching_emails_returned.yaml` & `python-keycloak-api-client-0.7.1/tests/cassettes/test_get_not_existing_user_when_partially_matching_emails_returned.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/cassettes/test_get_user_tokens.yaml` & `python-keycloak-api-client-0.7.1/tests/cassettes/test_get_user_tokens.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/cassettes/test_password_reset.yaml` & `python-keycloak-api-client-0.7.1/tests/cassettes/test_password_reset.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/cassettes/test_register_then_update_then_get_user.yaml` & `python-keycloak-api-client-0.7.1/tests/cassettes/test_register_then_update_then_get_user.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/cassettes/test_search_clients_by_client_id.yaml` & `python-keycloak-api-client-0.7.1/tests/cassettes/test_search_clients_by_client_id.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/cassettes/test_search_for_existing_user.yaml` & `python-keycloak-api-client-0.7.1/tests/cassettes/test_search_for_existing_user.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/cassettes/test_search_for_existing_user_with_limit_and_offset.yaml` & `python-keycloak-api-client-0.7.1/tests/cassettes/test_search_for_existing_user_with_limit_and_offset.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/cassettes/test_send_verification_email.yaml` & `python-keycloak-api-client-0.7.1/tests/cassettes/test_send_verification_email.yaml`

 * *Files identical despite different names*

### Comparing `python-keycloak-api-client-0.7.0/tests/factories_test.py` & `python-keycloak-api-client-0.7.1/tests/factories_test.py`

 * *Files identical despite different names*

