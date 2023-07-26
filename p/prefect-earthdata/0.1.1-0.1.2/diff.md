# Comparing `tmp/prefect-earthdata-0.1.1.tar.gz` & `tmp/prefect-earthdata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-earthdata-0.1.1.tar", last modified: Tue Jul 25 21:14:46 2023, max compression
+gzip compressed data, was "prefect-earthdata-0.1.2.tar", last modified: Wed Jul 26 14:53:42 2023, max compression
```

## Comparing `prefect-earthdata-0.1.1.tar` & `prefect-earthdata-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:14:46.424977 prefect-earthdata-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-25 21:13:54.000000 prefect-earthdata-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-25 21:13:54.000000 prefect-earthdata-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-25 21:14:46.428977 prefect-earthdata-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-07-25 21:13:54.000000 prefect-earthdata-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:14:46.428977 prefect-earthdata-0.1.1/prefect_earthdata/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-25 21:13:54.000000 prefect-earthdata-0.1.1/prefect_earthdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-25 21:14:46.428977 prefect-earthdata-0.1.1/prefect_earthdata/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-25 21:13:54.000000 prefect-earthdata-0.1.1/prefect_earthdata/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-25 21:13:54.000000 prefect-earthdata-0.1.1/prefect_earthdata/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:14:46.424977 prefect-earthdata-0.1.1/prefect_earthdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-25 21:14:46.000000 prefect-earthdata-0.1.1/prefect_earthdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-25 21:14:46.000000 prefect-earthdata-0.1.1/prefect_earthdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:14:46.000000 prefect-earthdata-0.1.1/prefect_earthdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 21:14:46.000000 prefect-earthdata-0.1.1/prefect_earthdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-25 21:14:46.000000 prefect-earthdata-0.1.1/prefect_earthdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 21:14:46.000000 prefect-earthdata-0.1.1/prefect_earthdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-25 21:13:54.000000 prefect-earthdata-0.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 21:13:54.000000 prefect-earthdata-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-25 21:14:46.428977 prefect-earthdata-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-25 21:13:54.000000 prefect-earthdata-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:14:46.424977 prefect-earthdata-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-25 21:13:54.000000 prefect-earthdata-0.1.1/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-25 21:13:54.000000 prefect-earthdata-0.1.1/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-25 21:13:54.000000 prefect-earthdata-0.1.1/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-07-25 21:13:54.000000 prefect-earthdata-0.1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:42.540606 prefect-earthdata-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-26 14:52:42.000000 prefect-earthdata-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-26 14:52:42.000000 prefect-earthdata-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-26 14:53:42.540606 prefect-earthdata-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-07-26 14:52:42.000000 prefect-earthdata-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:42.544606 prefect-earthdata-0.1.2/prefect_earthdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-26 14:52:42.000000 prefect-earthdata-0.1.2/prefect_earthdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-26 14:53:42.544606 prefect-earthdata-0.1.2/prefect_earthdata/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-26 14:52:42.000000 prefect-earthdata-0.1.2/prefect_earthdata/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-26 14:52:42.000000 prefect-earthdata-0.1.2/prefect_earthdata/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:42.540606 prefect-earthdata-0.1.2/prefect_earthdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-26 14:53:42.000000 prefect-earthdata-0.1.2/prefect_earthdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-26 14:53:42.000000 prefect-earthdata-0.1.2/prefect_earthdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:53:42.000000 prefect-earthdata-0.1.2/prefect_earthdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 14:53:42.000000 prefect-earthdata-0.1.2/prefect_earthdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-26 14:53:42.000000 prefect-earthdata-0.1.2/prefect_earthdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 14:53:42.000000 prefect-earthdata-0.1.2/prefect_earthdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-26 14:52:42.000000 prefect-earthdata-0.1.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-26 14:52:42.000000 prefect-earthdata-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-26 14:53:42.544606 prefect-earthdata-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-26 14:52:42.000000 prefect-earthdata-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:42.540606 prefect-earthdata-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-26 14:52:42.000000 prefect-earthdata-0.1.2/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-26 14:52:42.000000 prefect-earthdata-0.1.2/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-26 14:52:42.000000 prefect-earthdata-0.1.2/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-07-26 14:52:42.000000 prefect-earthdata-0.1.2/versioneer.py
```

### Comparing `prefect-earthdata-0.1.1/LICENSE` & `prefect-earthdata-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-earthdata-0.1.1/PKG-INFO` & `prefect-earthdata-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-earthdata
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prefect integrations with NASA Earthdata.
 Home-page: https://github.com/giorgiobasile/prefect-earthdata
 Author: Giorgio Basile
 Author-email: giorgiobasile@users.noreply.github.com
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-earthdata-0.1.1/README.md` & `prefect-earthdata-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `prefect-earthdata-0.1.1/prefect_earthdata/credentials.py` & `prefect-earthdata-0.1.2/prefect_earthdata/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Authentication is handled via the `earthaccess` module.
     Refer to the [earthaccess docs](https://nsidc.github.io/earthaccess/)
     for more info about the possible credential configurations.
 
     Example:
         Load stored Earthdata credentials:
         ```python
-        from prefect_earthdata.credentials import EarthdataCredentials
+        from prefect_earthdata import EarthdataCredentials
 
         ed_credentials_block = EarthdataCredentials.load("BLOCK_NAME")
         ```
     """  # noqa E501
 
     _logo_url = "https://yt3.googleusercontent.com/ytc/AGIKgqPjIUeAw3_hrkHWZgixdwD5jc-hTWweoCA6bJMhUg=s176-c-k-c0x00ffffff-no-rj"  # noqa
     _block_type_name = "NASA Earthdata Credentials"
@@ -46,15 +46,15 @@
         Returns an authenticated session with NASA Earthdata using
         the [`earthaccess.login()`](https://nsidc.github.io/earthaccess/user-reference/api/api/#earthaccess.api.login) function
 
         Example:
             Authenticates with NASA Earthdata using the credentials.
 
             ```python
-            from prefect_earthdata.credentials import EarthdataCredentials
+            from prefect_earthdata import EarthdataCredentials
 
             earthdata_credentials_block = EarthdataCredentials(
                 earthdata_username = "username",
                 earthdata_password = "password"
             )
             earthdata_auth = earthdata_credentials_block.login()
             ```
```

### Comparing `prefect-earthdata-0.1.1/prefect_earthdata/tasks.py` & `prefect-earthdata-0.1.2/prefect_earthdata/tasks.py`

 * *Files identical despite different names*

### Comparing `prefect-earthdata-0.1.1/prefect_earthdata.egg-info/PKG-INFO` & `prefect-earthdata-0.1.2/prefect_earthdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-earthdata
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prefect integrations with NASA Earthdata.
 Home-page: https://github.com/giorgiobasile/prefect-earthdata
 Author: Giorgio Basile
 Author-email: giorgiobasile@users.noreply.github.com
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-earthdata-0.1.1/prefect_earthdata.egg-info/SOURCES.txt` & `prefect-earthdata-0.1.2/prefect_earthdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-earthdata-0.1.1/setup.cfg` & `prefect-earthdata-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-earthdata-0.1.1/setup.py` & `prefect-earthdata-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-earthdata-0.1.1/tests/test_block_standards.py` & `prefect-earthdata-0.1.2/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-earthdata-0.1.1/tests/test_tasks.py` & `prefect-earthdata-0.1.2/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `prefect-earthdata-0.1.1/versioneer.py` & `prefect-earthdata-0.1.2/versioneer.py`

 * *Files identical despite different names*

