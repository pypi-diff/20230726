# Comparing `tmp/vmware-aria-operations-integration-sdk-lib-0.7.3.tar.gz` & `tmp/vmware-aria-operations-integration-sdk-lib-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmware-aria-operations-integration-sdk-lib-0.7.3.tar", last modified: Wed May 10 14:54:52 2023, max compression
+gzip compressed data, was "vmware-aria-operations-integration-sdk-lib-0.7.4.tar", last modified: Wed Jul 26 21:09:02 2023, max compression
```

## Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3.tar` & `vmware-aria-operations-integration-sdk-lib-0.7.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-05-10 14:54:52.175380 vmware-aria-operations-integration-sdk-lib-0.7.3/
--rw-r--r--   0 kylerokos   (501) staff       (20)    10449 2022-10-27 15:46:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/LICENSE
--rw-r--r--   0 kylerokos   (501) staff       (20)      411 2022-10-27 15:46:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/NOTICE
--rw-r--r--   0 kylerokos   (501) staff       (20)     3020 2023-05-10 14:54:52.175682 vmware-aria-operations-integration-sdk-lib-0.7.3/PKG-INFO
--rw-r--r--   0 kylerokos   (501) staff       (20)     2199 2023-04-20 17:56:10.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/README.md
--rw-r--r--   0 kylerokos   (501) staff       (20)      141 2023-01-11 16:15:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/pyproject.toml
--rw-r--r--   0 kylerokos   (501) staff       (20)      929 2023-05-10 14:54:52.177217 vmware-aria-operations-integration-sdk-lib-0.7.3/setup.cfg
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-05-10 14:54:52.098170 vmware-aria-operations-integration-sdk-lib-0.7.3/src/
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-05-10 14:54:52.103989 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/
--rw-r--r--   0 kylerokos   (501) staff       (20)       70 2022-11-22 14:51:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/__init__.py
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-05-10 14:54:52.123404 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/
--rw-r--r--   0 kylerokos   (501) staff       (20)      281 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/__init__.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     3522 2023-02-01 19:20:02.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/adapter_instance.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     2948 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/adapter_logging.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     2910 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/data.py
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-05-10 14:54:52.149748 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/
--rw-r--r--   0 kylerokos   (501) staff       (20)       70 2022-11-30 20:30:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/__init__.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    12374 2023-05-09 21:05:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/adapter_definition.py
--rw-r--r--   0 kylerokos   (501) staff       (20)      531 2022-11-22 14:51:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/assertions.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     7217 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/attribute.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     9884 2023-05-09 21:05:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/credential_type.py
--rw-r--r--   0 kylerokos   (501) staff       (20)      198 2022-11-30 20:30:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/exceptions.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    11446 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/group.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     6442 2023-05-09 21:05:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/object_type.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     6916 2023-05-09 21:05:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/parameter.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    17902 2023-03-04 23:38:33.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/units.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     2449 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/event.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    17112 2023-03-04 23:31:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/object.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     1183 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/pipe_utils.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    13941 2023-02-03 17:27:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/result.py
--rw-r--r--   0 kylerokos   (501) staff       (20)    13784 2023-04-19 11:57:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/suite_api_client.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     4259 2023-04-19 11:57:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/timer.py
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-05-10 14:54:52.158528 vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/
--rw-r--r--   0 kylerokos   (501) staff       (20)     3020 2023-05-10 14:54:52.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/PKG-INFO
--rw-r--r--   0 kylerokos   (501) staff       (20)     1155 2023-05-10 14:54:52.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/SOURCES.txt
--rw-r--r--   0 kylerokos   (501) staff       (20)        1 2023-05-10 14:54:52.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/dependency_links.txt
--rw-r--r--   0 kylerokos   (501) staff       (20)       14 2023-05-10 14:54:52.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/requires.txt
--rw-r--r--   0 kylerokos   (501) staff       (20)        5 2023-05-10 14:54:52.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/top_level.txt
-drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-05-10 14:54:52.174455 vmware-aria-operations-integration-sdk-lib-0.7.3/tests/
--rw-r--r--   0 kylerokos   (501) staff       (20)    12006 2023-02-03 17:27:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/tests/test_collect_result.py
--rw-r--r--   0 kylerokos   (501) staff       (20)      406 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/tests/test_event.py
--rw-r--r--   0 kylerokos   (501) staff       (20)     1809 2023-03-04 23:31:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/tests/test_object_key.py
--rw-r--r--   0 kylerokos   (501) staff       (20)      663 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.3/tests/test_result.py
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-07-26 21:09:02.302285 vmware-aria-operations-integration-sdk-lib-0.7.4/
+-rw-r--r--   0 kylerokos   (501) staff       (20)    10449 2022-10-27 15:46:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/LICENSE
+-rw-r--r--   0 kylerokos   (501) staff       (20)      411 2022-10-27 15:46:24.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/NOTICE
+-rw-r--r--   0 kylerokos   (501) staff       (20)     3020 2023-07-26 21:09:02.302427 vmware-aria-operations-integration-sdk-lib-0.7.4/PKG-INFO
+-rw-r--r--   0 kylerokos   (501) staff       (20)     2199 2023-04-20 17:56:10.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/README.md
+-rw-r--r--   0 kylerokos   (501) staff       (20)      141 2023-07-20 19:18:18.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/pyproject.toml
+-rw-r--r--   0 kylerokos   (501) staff       (20)      929 2023-07-26 21:09:02.303255 vmware-aria-operations-integration-sdk-lib-0.7.4/setup.cfg
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-07-26 21:09:02.273456 vmware-aria-operations-integration-sdk-lib-0.7.4/src/
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-07-26 21:09:02.279772 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/
+-rw-r--r--   0 kylerokos   (501) staff       (20)       70 2022-11-22 14:51:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/__init__.py
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-07-26 21:09:02.288034 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/
+-rw-r--r--   0 kylerokos   (501) staff       (20)      281 2023-01-25 18:53:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/__init__.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     3564 2023-06-07 18:47:56.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/adapter_instance.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     3599 2023-06-07 18:47:56.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/adapter_logging.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     3081 2023-06-07 18:47:56.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/data.py
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-07-26 21:09:02.294877 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/
+-rw-r--r--   0 kylerokos   (501) staff       (20)       70 2022-11-30 20:30:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/__init__.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    12892 2023-06-07 18:47:56.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/adapter_definition.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)      531 2022-11-22 14:51:39.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/assertions.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     7593 2023-06-07 18:47:56.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/attribute.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    10381 2023-06-07 18:47:56.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/credential_type.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)      198 2022-11-30 20:30:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/exceptions.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    11992 2023-06-07 18:47:56.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/group.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     6678 2023-06-07 18:47:56.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/object_type.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     7259 2023-06-07 18:47:56.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/parameter.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    17902 2023-03-04 23:38:33.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/units.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     2844 2023-06-07 18:47:56.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/event.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    17498 2023-06-07 18:47:56.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/object.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     1622 2023-06-07 18:47:56.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/pipe_utils.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    14697 2023-06-07 18:47:56.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/result.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)    14310 2023-06-07 18:47:56.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/suite_api_client.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     4259 2023-04-19 11:57:28.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/timer.py
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-07-26 21:09:02.298614 vmware-aria-operations-integration-sdk-lib-0.7.4/src/vmware_aria_operations_integration_sdk_lib.egg-info/
+-rw-r--r--   0 kylerokos   (501) staff       (20)     3020 2023-07-26 21:09:02.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/vmware_aria_operations_integration_sdk_lib.egg-info/PKG-INFO
+-rw-r--r--   0 kylerokos   (501) staff       (20)     1155 2023-07-26 21:09:02.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/vmware_aria_operations_integration_sdk_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 kylerokos   (501) staff       (20)        1 2023-07-26 21:09:02.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/vmware_aria_operations_integration_sdk_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 kylerokos   (501) staff       (20)       14 2023-07-26 21:09:02.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/vmware_aria_operations_integration_sdk_lib.egg-info/requires.txt
+-rw-r--r--   0 kylerokos   (501) staff       (20)        5 2023-07-26 21:09:02.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/src/vmware_aria_operations_integration_sdk_lib.egg-info/top_level.txt
+drwxr-xr-x   0 kylerokos   (501) staff       (20)        0 2023-07-26 21:09:02.301713 vmware-aria-operations-integration-sdk-lib-0.7.4/tests/
+-rw-r--r--   0 kylerokos   (501) staff       (20)    12006 2023-02-03 17:27:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/tests/test_collect_result.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)      406 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/tests/test_event.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)     1809 2023-03-04 23:31:20.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/tests/test_object_key.py
+-rw-r--r--   0 kylerokos   (501) staff       (20)      663 2023-01-11 16:15:44.000000 vmware-aria-operations-integration-sdk-lib-0.7.4/tests/test_result.py
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/LICENSE` & `vmware-aria-operations-integration-sdk-lib-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/PKG-INFO` & `vmware-aria-operations-integration-sdk-lib-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-aria-operations-integration-sdk-lib
-Version: 0.7.3
+Version: 0.7.4
 Summary: Object model for interacting with the VMware Aria Operations Containerized API
 Home-page: https://github.com/vmware/vmware-aria-operations-integration-sdk
 Author: VMware, Inc.
 Author-email: krokos@vmware.com
 Project-URL: Bug Tracker, https://github.com/vmware/vmware-aria-operations-integration-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/README.md` & `vmware-aria-operations-integration-sdk-lib-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/setup.cfg` & `vmware-aria-operations-integration-sdk-lib-0.7.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vmware-aria-operations-integration-sdk-lib
-version = 0.7.3
+version = 0.7.4
 author = VMware, Inc.
 author_email = krokos@vmware.com
 description = Object model for interacting with the VMware Aria Operations Containerized API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/vmware/vmware-aria-operations-integration-sdk
 project_urls =
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/adapter_instance.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/adapter_instance.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,23 +64,27 @@
 
         self.collection_number: Optional[int] = json.get("collection_number", None)
         self.collection_window: Optional[Dict] = json.get("collection_window", None)
 
     def get_credential_type(self) -> Optional[str]:
         """Get the type (key) of credential. This is useful if an adapter supports multiple types of credentials.
 
-        :return: the type of the credential used by this adapter instance, or None if the adapter instance does not have a credential.
+        Returns:
+            the type of the credential used by this adapter instance, or None if the adapter instance does not have a credential.
         """
         return self.credential_type  # type: ignore[no-any-return]
 
     def get_credential_value(self, credential_key: str) -> Optional[str]:
         """Retrieve the value of a given credential
 
-        :param credential_key: Key of the credential field
-        :return: value associated with the credential field, or None if a credential field with the given key does not exist.
+        Args:
+            credential_key (str): Key of the credential field
+
+        Returns:
+            value associated with the credential field, or None if a credential field with the given key does not exist.
         """
         return self.credentials.get(credential_key)
 
     @classmethod
     def from_input(cls, infile: str = sys.argv[-2]) -> AdapterInstance:
         # The server always invokes methods with the input file as the second to last argument
         return cls(read_from_pipe(infile))
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/adapter_logging.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/adapter_logging.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 from typing import Optional
 
 log_handler: Optional[RotatingFileHandler] = None
 
 
 def setup_logging(filename: str, file_count: int = 5, max_size: int = 0) -> None:
     """
-    :param filename The name of the file to log to
-    :param file_count The total number of files to retain. Defaults to 5.
-    :param max_size The maximum size in bytes of each file before the file
-                    automatically rotates to a new one. Defaults to '0', which will
-                    do no automatic rotation. Requires calling the 'rotate()' function
-                    manually to ensure logs do not become too large.
+    Sets up logging using the given parameters.
+
+    Args:
+        filename (str): The name of the file to log to.
+        file_count (int, optional): The total number of files to retain. Defaults to 5.
+        max_size (int, optional): The maximum size in bytes of each file before the file
+                                  automatically rotates to a new one. Defaults to '0', which will
+                                  do no automatic rotation. Requires calling the 'rotate()' function
+                                  manually to ensure logs do not become too large.
     """
     try:
         global log_handler
         log_handler = RotatingFileHandler(
             os.path.join(os.sep, "var", "log", filename),
             maxBytes=max_size,
             backupCount=file_count,
@@ -33,14 +36,24 @@
         )
         _set_log_levels()
     except Exception:
         logging.basicConfig(level=logging.CRITICAL + 1)
 
 
 def _get_default_log_level(default_level: int = logging.INFO) -> int:
+    """
+    Retrieves the default logging level from a config file, or returns a default value.
+
+    Args:
+        default_level (int, optional): The default logging level if not set in the config file.
+                                        Defaults to logging.INFO.
+
+    Returns:
+        int: The default logging level.
+    """
     default_level_name = logging.getLevelName(default_level)
     log_config_file = os.path.join(os.sep, "var", "log", "loglevels.cfg")
     config = ConfigParser()
     if os.path.isfile(log_config_file):
         config.read(log_config_file)
     modified = False
     if "adapter" not in config["DEFAULT"]:
@@ -59,27 +72,37 @@
             logging.getLevelName(config["DEFAULT"].get("adapter", default_level_name))
         )
     except ValueError:
         return default_level
 
 
 def _set_log_levels() -> None:
+    """
+    Sets the logging levels for each logger as defined in a config file.
+    """
     log_config_file = os.path.join(os.sep, "var", "log", "loglevels.cfg")
     config = ConfigParser()
     config.read(log_config_file)
     for logger in config["adapter"]:
         logging.getLogger(logger).setLevel(config["adapter"][logger])
 
 
 def getLogger(name: str) -> logging.Logger:
-    # convenience function to avoid having to import logging and adapter_logging
+    """
+    A convenience function to get a logger with a specific name.
+
+    Args:
+        name (str): The name of the logger.
+
+    Returns:
+        logging.Logger: The requested logger.
+    """
     return logging.getLogger(name)
 
 
 def rotate() -> None:
     """
     Rotates the current adapter logs to their backups (e.g., `adapter.log` to
     `adapter.log.1`) and starts logging to the new adapter.log file.
-    :return: None
     """
     if log_handler:
         log_handler.doRollover()
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/data.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,92 +1,102 @@
-#  Copyright 2022 VMware, Inc.
+#  Copyright 2023 VMware, Inc.
 #  SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 import time
 from typing import Optional
 from typing import Union
 
 
 class Metric:
     """Class representing a Metric Data Point.
 
     Metrics are numeric values that represent data at a particular point in time. These are stored as time series data.
+
     Examples:
         CPU Utilization
         Disk Capacity
         Current User Session Count
         Cumulative Data Received
     """
 
     def __init__(self, key: str, value: float, timestamp: Optional[int] = None):
-        """Creates a Metric
+        """
+        Creates a Metric.
 
-        :param key: A string representing the type of metric. TODO: Describe how Keys work.
-        :param value: The value of the Metric. Must be type float.
-        :param timestamp: Time in milliseconds since the Epoch when this metric value was recorded.
-            Defaults to the current time.
+        Args:
+            key (str): A string representing the type of metric.
+            value (float): The value of the Metric.
+            timestamp (Optional[int], optional): Time in milliseconds since the Epoch when this metric
+                                                 value was recorded. Defaults to the current time.
         """
         self.key = key
         self.value = value
 
         if timestamp is None:
             self.timestamp = int(time.time() * 1000)
         else:
             self.timestamp = timestamp
 
     def get_json(self) -> dict:
-        """Get a JSON representation of this Metric.
+        """
+        Get a JSON representation of this Metric.
 
         Returns a JSON representation of this Metric in the format required by vROps.
 
-        :return: A JSON representation of this Metric.
+        Returns:
+            dict: A JSON representation of this Metric.
         """
         return {
             "key": self.key,
             "numberValue": float(self.value),
             "timestamp": self.timestamp,
         }
 
 
 class Property:
     """Class representing a Property value.
 
     A Property is a value, usually a string, that will change infrequently or not at all. Only the current value is
     important.
+
     Examples:
         IP Address
         Software Version
         CPU Core Count
     """
 
     def __init__(
         self, key: str, value: Union[float, str], timestamp: Optional[int] = None
     ):
-        """Creates a Property.
+        """
+        Creates a Property.
 
-        :param key: A string representing the type of property. TODO: Describe how Keys work.
-        :param value: The value of the property. Can be str or float.
-        :param timestamp: Time in milliseconds since the Epoch when this property value was recorded.
-            Defaults to the current time.
+        Args:
+            key (str): A string representing the type of property.
+            value (Union[float, str]): The value of the property. Can be str or float.
+            timestamp (Optional[int], optional): Time in milliseconds since the Epoch when this property
+                                                 value was recorded. Defaults to the current time.
         """
         self.key = key
         self.value = value
 
         if timestamp is None:
             self.timestamp = int(time.time() * 1000)
         else:
             self.timestamp = timestamp
 
     def get_json(self) -> dict:
-        """Get a JSON representation of this Property.
+        """
+        Get a JSON representation of this Property.
 
         Returns a JSON representation of this Property in the format required by vROps.
 
-        :return: A JSON representation of this Property.
+        Returns:
+            dict: A JSON representation of this Property.
         """
         if isinstance(self.value, str):
             label = "stringValue"
         else:
             label = "numberValue"
             self.value = float(self.value)
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/adapter_definition.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/adapter_definition.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,22 +25,25 @@
         key: str,
         label: Optional[str] = None,
         adapter_instance_key: Optional[str] = None,
         adapter_instance_label: Optional[str] = None,
         version: int = 1,
     ):
         """
-        :param key: The adapter key is used to identify the adapter and its object types. It must be unique across
-               all Management Packs.
-        :param label: Label that is displayed in the VMware Aria Operations UI for this adapter. Defaults to the key.
-        :param adapter_instance_key: Object type of the adapter instance object. Defaults to
-               '{adapter key}_adapter_instance'.
-        :param adapter_instance_label: Label that is displayed in the VMware Aria Operations UI for the adapter instance
-               object type. Defaults to '{adapter label} Adapter Instance'.
-        :param version: Version of the definition. This should be incremented for new releases of the adapter.
+        Args:
+            key (str): The adapter key is used to identify the adapter and its object types. It must be unique across
+                all Management Packs.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI for this adapter.
+                Defaults to the key.
+            adapter_instance_key (Optional[str]): Object type of the adapter instance object. Defaults to
+                '{adapter key}_adapter_instance'.
+            adapter_instance_label (Optional[str]): Label that is displayed in the VMware Aria Operations UI for the
+                adapter instance object type. Defaults to '{adapter label} Adapter Instance'.
+            version (int): Version of the definition. This should be incremented for new releases of the adapter.
+                Defaults to 1
         """
         key = validate_key(key, "Adapter")
         if not key[0].isalpha():
             raise KeyException("Adapter key must start with a letter.")
         if len(key.split()) > 1:
             raise KeyException("Adapter key cannot contain whitespace.")
         if not all(c.isalnum() or c == "_" for c in key):
@@ -109,22 +112,27 @@
         max_length: int = 512,
         required: bool = True,
         advanced: bool = False,
     ) -> StringParameter:
         """
         Create a new string parameter and add it to the adapter instance. The user will be asked to provide a value for
         this parameter each time a new account/adapter instance is created.
-        :param key: Used to identify the parameter
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param description: More in-depth explanation of the parameter. Displayed as a tooltip in the VMware Aria Operations UI.
-        :param default: The default value of the parameter.
-        :param max_length: The max length of the parameter value. Defaults to 512.
-        :param required: True if user is required to provide this parameter. Defaults to True.
-        :param advanced: True if the parameter should be collapsed by default. Defaults to False.
-        :return The created string parameter definition.
+
+        Args:
+            key (str): Used to identify the parameter
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            description (Optional[str]): More in-depth explanation of the parameter. Displayed as a tooltip in the
+                VMware Aria Operations UI.
+            default (Optional[str]): The default value of the parameter. Defaults to None
+            max_length (int): The max length of the parameter value. Defaults to 512.
+            required (bool): True if user is required to provide this parameter. Defaults to True.
+            advanced (bool): True if the parameter should be collapsed by default. Defaults to False.
+
+        Returns:
+             The created string parameter definition.
         """
         parameter = StringParameter(
             key,
             label,
             description,
             default,
             max_length,
@@ -143,21 +151,25 @@
         default: Optional[int] = None,
         required: bool = True,
         advanced: bool = False,
     ) -> IntParameter:
         """
         Create a new integer parameter and add it to the adapter instance. The user will be asked to provide a value for
         this parameter each time a new account/adapter instance is created.
-        :param key: Used to identify the parameter
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param description: More in-depth explanation of the parameter. Displayed as a tooltip in the VMware Aria Operations UI.
-        :param default: The default value of the parameter.
-        :param required: True if user is required to provide this parameter. Defaults to True.
-        :param advanced: True if the parameter should be collapsed by default. Defaults to False.
-        :return The created int parameter definition.
+
+        Args:
+            key (str): Used to identify the parameter
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            description (Optional[str]): More in-depth explanation of the parameter. Displayed as a tooltip in the VMware Aria Operations UI.
+            default (Optional[int]): The default value of the parameter.
+            required (bool): True if user is required to provide this parameter. Defaults to True.
+            advanced (bool): True if the parameter should be collapsed by default. Defaults to False.
+
+        Returns:
+             The created int parameter definition.
         """
         parameter = IntParameter(
             key,
             label,
             description,
             default,
             required,
@@ -176,23 +188,27 @@
         default: Optional[str] = None,
         required: bool = True,
         advanced: bool = False,
     ) -> EnumParameter:
         """
         Create a new enum parameter and add it to the adapter instance. The user will be asked to provide a value for
         this parameter each time a new account/adapter instance is created.
-        :param key: Used to identify the parameter
-        :param values: An array containing all enum values. If 'default' is specified and not part of this array, it
-               will be added as an additional enum value (values are case-sensitive). Enum values are not localizable.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param description: More in-depth explanation of the parameter. Displayed as a tooltip in the VMware Aria Operations UI.
-        :param default: The default value of the parameter.
-        :param required: True if user is required to provide this parameter. Defaults to True.
-        :param advanced: True if the parameter should be collapsed by default. Defaults to False.
-        :return The created enum parameter definition.
+
+        Args:
+            key (str): Used to identify the parameter
+            values (List[str]): An array containing all enum values. If 'default' is specified and not part of this array, it
+                will be added as an additional enum value (values are case-sensitive). Enum values are not localizable.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            description (Optional[str]): More in-depth explanation of the parameter. Displayed as a tooltip in the VMware Aria Operations UI.
+            default (Optional[str]): The default value of the parameter.
+            required (bool): True if user is required to provide this parameter. Defaults to True.
+            advanced (bool): True if the parameter should be collapsed by default. Defaults to False.
+
+        Returns:
+             The created enum parameter definition.
         """
         parameter = EnumParameter(
             key,
             values,
             label,
             description,
             default,
@@ -203,16 +219,17 @@
         self.add_parameter(parameter)
         return parameter
 
     def add_parameter(self, parameter: Parameter) -> None:
         """
         Add a parameter to the adapter instance. The user will be asked to provide a value for
         this parameter each time a new account/adapter instance is created.
-        :param parameter: The parameter to add to the adapter instance.
-        :return: None
+
+        Args:
+            parameter (Parameter): The parameter to add to the adapter instance.
         """
         key = parameter.key
         if key in self.parameters:
             raise DuplicateKeyException(
                 f"Parameter with key {key} already exists in adapter definition."
             )
         self.parameters[key] = parameter
@@ -220,71 +237,82 @@
     def define_credential_type(
         self, key: str = "default_credential", label: Optional[str] = None
     ) -> CredentialType:
         """
         Create a new credential type and add it to this adapter instance. When more than one credential types are
         present, The user will be required to select the type and then fill in the parameters for that type, as only
         one credential type can be used for any given adapter instance.
-        :param key: Used to identify the credential type
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :return The created credential type.
+
+        Args:
+            key (str): Used to identify the credential type
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+
+        Returns:
+             The created credential type.
         """
         credential = CredentialType(key, label)
         self.add_credential_type(credential)
         return credential
 
     def add_credential_types(self, credential_types: list[CredentialType]) -> None:
         """
         Add a list of credential types to the adapter instance.
-        :param credential_types: A list of credential types to add.
-        :return: None
+
+        Args:
+            credential_types (List[CredentialType]): A list of credential types to add.
         """
         for credential_type in credential_types:
             self.add_credential_type(credential_type)
 
     def add_credential_type(self, credential_type: CredentialType) -> None:
         """
         Add a credential type to the adapter instance. When more than one credential types are present, The user will
         be required to select the type and then fill in the parameters for that type, as only one credential type can be
         used for any given adapter instance.
-        :param credential_type: The credential type to add.
-        :return: None
+
+        Args:
+            credential_type (CredentialType): The credential type to add.
         """
         key = credential_type.key
         if key in self.credentials:
             raise DuplicateKeyException(
                 f"Credential type with key {key} already exists in adapter definition."
             )
         self.credentials[key] = credential_type
 
     def define_object_type(self, key: str, label: Optional[str] = None) -> ObjectType:
         """
         Create a new object type definition and add it to this adapter definition.
-        :param key: The object type
-        :param label: Label that is displayed in the VMware Aria Operations UI for this object type. Defaults to the key.
-        :return: The created object type definition
+
+        Args:
+            key (str): The object type
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI for this object type. Defaults to the key.
+
+        Returns:
+             The created object type definition
         """
         object_type = ObjectType(key, label)
         self.add_object_type(object_type)
         return object_type
 
     def add_object_types(self, object_types: list[ObjectType]) -> None:
         """
         Adds a list of object types to this adapter definition
-        :param object_types: A list of object type definitions.
-        :return: None
+        Args:
+            object_types (List[ObjectType]): A list of object type definitions.
         """
         for object_type in object_types:
             self.add_object_type(object_type)
 
     def add_object_type(self, object_type: ObjectType) -> None:
         """
         Adds an object type to this adapter definition
-        :param object_type: An object type definition.
-        :return: None
+
+        Args:
+            object_type (ObjectType): An object type definition.
         """
         key = object_type.key
         if key in self.object_types:
             raise DuplicateKeyException(
                 f"Object type with key {key} already exists in adapter definition."
             )
         self.object_types[key] = object_type
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/assertions.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/assertions.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/attribute.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/attribute.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,28 +17,30 @@
         is_discrete: bool = False,
         is_kpi: bool = False,
         is_impact: bool = False,
         is_key_attribute: bool = False,
         dashboard_order: int = 0,
     ):
         """
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param unit: Specifies what unit this metric is returned in. This allows the UI to display the units in a
+
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            unit (Optional[str]): Specifies what unit this metric is returned in. This allows the UI to display the units in a
         consistent manner, and perform conversions when appropriate.
-        :param is_rate: Declares this attribute as a rate (e.g., kilobytes per second). If a unit is specified, this
-        will be set automatically. Otherwise, defaults to False.
-        :param is_discrete: Declares that this attribute's range of values is discrete (integer) rather than continuous
-        (floating point)
-        :param is_kpi: If set, threshold breaches for this metric will be used in the calculation of the object's
-        'Self - Health Score' metric, which can affect the 'Anomalies' Badge.
-        :param is_impact: If set, this attribute will never be the 'root cause' of an issue. For example, it could be a
-        proxy to a root cause, but not the root cause itself.
-        :param is_key_attribute: True if the attribute should be shown in some object summary widgets in the UI.
-        :param dashboard_order: Determines the order parameters will be displayed in the UI.
+            is_rate (bool): Declares this attribute as a rate (e.g., kilobytes per second). If a unit is specified, this
+            will be set automatically. Otherwise, defaults to False.
+            is_discrete (bool): Declares that this attribute's range of values is discrete (integer) rather than continuous
+            (floating point). Defaults to False.
+            is_kpi (bool): If set, threshold breaches for this metric will be used in the calculation of the object's
+            'Self - Health Score' metric, which can affect the 'Anomalies' Badge. Defaults to False.
+            is_impact (bool): If set, this attribute will never be the 'root cause' of an issue. For example, it could be a
+            proxy to a root cause, but not the root cause itself. Defaults to False.
+            is_key_attribute (bool): True if the attribute should be shown in some object summary widgets in the UI.
+            dashboard_order (int): Determines the order parameters will be displayed in the UI. Defaults to 0
         """
         self.key = validate_key(key, "Attribute")
         self.label = label
         if label is None:
             self.label = key
         self.unit = unit.value.key if unit else None
         self.is_rate = unit.value.is_rate if unit else is_rate
@@ -72,28 +74,30 @@
         is_discrete: bool = False,
         is_kpi: bool = False,
         is_impact: bool = False,
         is_key_attribute: bool = False,
         dashboard_order: int = 0,
     ):
         """
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param unit: Specifies what unit this metric is returned in. This allows the UI to display the units in a
-        consistent manner, and perform conversions when appropriate.
-        :param is_rate: Declares this attribute as a rate (e.g., kilobytes per second). If a unit is specified, this
-        will be set automatically. Otherwise, defaults to False.
-        :param is_discrete: Declares that this attribute's range of values is discrete (integer) rather than continuous
-        (floating point)
-        :param is_kpi: If set, threshold breaches for this metric will be used in the calculation of the object's
-        'Self - Health Score' metric, which can affect the 'Anomalies' Badge.
-        :param is_impact: If set, this attribute will never be the 'root cause' of an issue. For example, it could be a
-        proxy to a root cause, but not the root cause itself.
-        :param is_key_attribute: True if the attribute should be shown in some object summary widgets in the UI.
-        :param dashboard_order: Determines the order parameters will be displayed in the UI.
+
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            unit (Optional[Unit]): Specifies what unit this metric is returned in. This allows the UI to display the units in a
+                consistent manner, and perform conversions when appropriate.
+            is_rate (bool): Declares this attribute as a rate (e.g., kilobytes per second). If a unit is specified, this
+                will be set automatically. Otherwise, defaults to False.
+            is_discrete (bool): Declares that this attribute's range of values is discrete (integer) rather than continuous
+                (floating point)
+            is_kpi (bool): If set, threshold breaches for this metric will be used in the calculation of the object's
+                'Self - Health Score' metric, which can affect the 'Anomalies' Badge.
+            is_impact (bool): If set, this attribute will never be the 'root cause' of an issue. For example, it could be a
+                proxy to a root cause, but not the root cause itself.
+            is_key_attribute (bool): True if the attribute should be shown in some object summary widgets in the UI.
+            dashboard_order (bool): Determines the order parameters will be displayed in the UI.
         """
         super().__init__(
             key,
             label,
             unit,
             is_rate,
             is_discrete,
@@ -121,29 +125,31 @@
         is_discrete: bool = False,
         is_kpi: bool = False,
         is_impact: bool = False,
         is_key_attribute: bool = False,
         dashboard_order: int = 0,
     ):
         """
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param is_string: Determines if the property is numeric or string (text).
-        :param unit: Specifies what unit this metric is returned in. This allows the UI to display the units in a
-        consistent manner, and perform conversions when appropriate.
-        :param is_rate: Declares this attribute as a rate (e.g., kilobytes per second). If a unit is specified, this
-        will be set automatically. Otherwise, defaults to False.
-        :param is_discrete: Declares that this attribute's range of values is discrete (integer) rather than continuous
-        (floating point). Defaults to False, unless 'is_string' is set, in which case it will always be set to True.
-        :param is_kpi: If set, threshold breaches for this metric will be used in the calculation of the object's
-        'Self - Health Score' metric, which can affect the 'Anomalies' Badge.
-        :param is_impact: If set, this attribute will never be the 'root cause' of an issue. For example, it could be a
-        proxy to a root cause, but not the root cause itself.
-        :param is_key_attribute: True if the attribute should be shown in some object summary widgets in the UI.
-        :param dashboard_order: Determines the order parameters will be displayed in the UI.
+
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            is_string (bool): Determines if the property is numeric or string (text).
+            unit (Optional[Unit]): Specifies what unit this metric is returned in. This allows the UI to display the units in a
+                consistent manner, and perform conversions when appropriate.
+            is_rate (bool): Declares this attribute as a rate (e.g., kilobytes per second). If a unit is specified, this
+                will be set automatically. Otherwise, defaults to False.
+            is_discrete (bool): Declares that this attribute's range of values is discrete (integer) rather than continuous
+                (floating point). Defaults to False, unless 'is_string' is set, in which case it will always be set to True.
+            is_kpi (bool): If set, threshold breaches for this metric will be used in the calculation of the object's
+                'Self - Health Score' metric, which can affect the 'Anomalies' Badge.
+            is_impact (bool): If set, this attribute will never be the 'root cause' of an issue. For example, it could be a
+                proxy to a root cause, but not the root cause itself.
+            is_key_attribute (bool): True if the attribute should be shown in some object summary widgets in the UI.
+            dashboard_order (int): Determines the order parameters will be displayed in the UI.
         """
         super().__init__(
             key,
             label,
             unit,
             is_rate,
             is_discrete,
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/credential_type.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/credential_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,18 +14,19 @@
         self,
         key: str,
         label: Optional[str] = None,
         required: bool = True,
         display_order: int = 0,
     ):
         """
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param required: True if user is required to provide this parameter. Defaults to True.
-        :param display_order: Determines the order parameters will be displayed in the UI.
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            required (bool): True if user is required to provide this parameter. Defaults to True.
+            display_order (0): Determines the order parameters will be displayed in the UI.
         """
         self.key = validate_key(key, "Credential parameter")
         self.label = label
         if label is None:
             self.label = key
         self.required = required
         self.display_order = display_order
@@ -39,18 +40,19 @@
             "enum": False,
             "display_order": self.display_order,
         }
 
 
 class CredentialIntParameter(CredentialParameter):
     """
-    :param key: Used to identify the parameter.
-    :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-    :param required: True if user is required to provide this parameter. Defaults to True.
-    :param display_order: Determines the order parameters will be displayed in the UI.
+    Args:
+        key (str): Used to identify the parameter.
+        label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+        required (bool): True if user is required to provide this parameter. Defaults to True.
+        display_order (int): Determines the order parameters will be displayed in the UI.
     """
 
     def __init__(
         self,
         key: str,
         label: Optional[str] = None,
         required: bool = True,
@@ -69,18 +71,19 @@
         self,
         key: str,
         label: Optional[str] = None,
         required: bool = True,
         display_order: int = 0,
     ):
         """
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param required: True if user is required to provide this parameter. Defaults to True.
-        :param display_order: Determines the order parameters will be displayed in the UI.
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            required (bool): True if user is required to provide this parameter. Defaults to True.
+            display_order (int): Determines the order parameters will be displayed in the UI.
         """
         super().__init__(key, label, required, display_order)
 
     def to_json(self) -> dict:
         return super().to_json() | {
             "type": "string",
         }
@@ -91,37 +94,39 @@
         self,
         key: str,
         label: Optional[str] = None,
         required: bool = True,
         display_order: int = 0,
     ):
         """
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param required: True if user is required to provide this parameter. Defaults to True.
-        :param display_order: Determines the order parameters will be displayed in the UI.
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            required (bool): True if user is required to provide this parameter. Defaults to True.
+            display_order (int): Determines the order parameters will be displayed in the UI.
         """
         super().__init__(key, label, required, display_order)
 
     def to_json(self) -> dict:
         return super().to_json() | {
             "type": "string",
             "password": True,
         }
 
 
 class CredentialEnumParameter(CredentialParameter):
     """
-    :param key: Used to identify the parameter.
-    :param values: An array containing all enum values. If 'default' is specified and not part of this array, it
-           will be added as an additional enum value. Enum values are not localizable.
-    :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-    :param default: The default value of the enum.
-    :param required: True if user is required to provide this parameter. Defaults to True.
-    :param display_order: Determines the order parameters will be displayed in the UI.
+    Args:
+        key (str): Used to identify the parameter.
+        values (list[Union[str, tuple[str,str]]]): An array containing all enum values. If 'default' is specified and
+            not part of this array, it will be added as an additional enum value. Enum values are not localizable.
+        label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+        default (Optional[str]): The default value of the enum.
+        required (bool): True if user is required to provide this parameter. Defaults to True.
+        display_order (int): Determines the order parameters will be displayed in the UI.
     """
 
     def __init__(
         self,
         key: str,
         values: list[Union[str, tuple[str, str]]],
         label: Optional[str] = None,
@@ -164,46 +169,58 @@
         self.credential_parameters: dict = OrderedDict()
 
     def define_string_parameter(
         self, key: str, label: Optional[str] = None, required: bool = True
     ) -> CredentialStringParameter:
         """
         Create a new string credential parameter and apply it to this credential definition.
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param required: True if user is required to provide this parameter. Defaults to True.
-        :return The created string parameter definition.
+
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            required (bool): True if user is required to provide this parameter. Defaults to True.
+
+        Returns:
+             The created string parameter definition.
         """
         field = CredentialStringParameter(key, label, required)
         self.add_parameter(field)
         return field
 
     def define_int_parameter(
         self, key: str, label: Optional[str] = None, required: bool = True
     ) -> CredentialIntParameter:
         """
         Create a new int credential parameter and apply it to this credential definition.
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param required: True if user is required to provide this parameter. Defaults to True.
-        :return The created int parameter definition.
+
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            required (bool): True if user is required to provide this parameter. Defaults to True.
+
+        Returns:
+             The created int parameter definition.
         """
         field = CredentialIntParameter(key, label, required)
         self.add_parameter(field)
         return field
 
     def define_password_parameter(
         self, key: str, label: Optional[str] = None, required: bool = True
     ) -> CredentialPasswordParameter:
         """
         Create a new password credential parameter and apply it to this credential definition.
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param required: True if user is required to provide this parameter. Defaults to True.
-        :return The created password parameter definition.
+
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            required (bool): True if user is required to provide this parameter. Defaults to True.
+
+        Returns:
+            The created password parameter definition.
         """
         field = CredentialPasswordParameter(key, label, required)
         self.add_parameter(field)
         return field
 
     def define_enum_parameter(
         self,
@@ -211,38 +228,42 @@
         values: list[Union[str, tuple[str, str]]],
         label: Optional[str] = None,
         default: Optional[str] = None,
         required: bool = True,
     ) -> CredentialEnumParameter:
         """
         Create a new enum credential parameter and apply it to this credential definition.
-        :param key: Used to identify the parameter.
-        :param values: An array containing all enum values. If 'default' is specified and not part of this array, it
-               will be added as an additional enum value. Enum values are not localizable.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param default: The default value of the enum.
-        :param required: True if user is required to provide this parameter. Defaults to True.
-        :return The created enum parameter definition.
+
+        Args:
+            key (str): Used to identify the parameter.
+            values (list[Union[str, tuple[str, str]]]): An array containing all enum values. If 'default' is specified
+                and not part of this array, it will be added as an additional enum value. Enum values are not localizable.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            default (Optional[str]): The default value of the enum.
+            required (bool): True if user is required to provide this parameter. Defaults to True.
+
+        Returns:
+             The created enum parameter definition.
         """
         field = CredentialEnumParameter(key, values, label, default, required)
         self.add_parameter(field)
         return field
 
     def add_parameters(self, credential_parameters: list[CredentialParameter]) -> None:
         """
-        :param credential_parameters: A list of parameters to add to the credential
-        :return None
+        Args:
+            credential_parameters (list[CredentialParameter]): A list of parameters to add to the credential
         """
         for credential_parameter in credential_parameters:
             self.add_parameter(credential_parameter)
 
     def add_parameter(self, credential_parameter: CredentialParameter) -> None:
         """
-        :param credential_parameter: The parameter to add to the credential
-        :return None
+        Args:
+            credential_parameter (CredentialParameter): The parameter to add to the credential
         """
         key = credential_parameter.key
         if key in self.credential_parameters:
             raise DuplicateKeyException(
                 f"Credential field with key {key} already exists in adapter definition."
             )
         credential_parameter.display_order = len(self.credential_parameters)
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/group.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/group.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,55 +20,65 @@
         self.key: str
         self.attributes: dict[str, Attribute] = OrderedDict()
         self.groups: dict[str, Group] = OrderedDict()
 
     def define_group(self, key: str, label: Optional[str] = None) -> Group:
         """
         Create a new group that can hold attributes and subgroups.
-        :param key: The key for the group.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :return: The created group.
+
+        Args:
+            key (str): The key for the group.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+
+        Returns:
+             The created group.
         """
         group = Group(key, label)
         self.add_group(group)
         return group
 
     def define_instanced_group(
         self, key: str, label: Optional[str] = None, instance_required: bool = True
     ) -> Group:
         """
         Create a new group that can hold attributes and subgroups. This group can be 'instanced', with a value, so that
         its subgroups and attributes can appear multiple times, once for each instance value. For example, a group
         containing metrics for a network interface might be instanced for each discovered interface on the parent
         object.
-        :param key: The key for the group.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param instance_required: If true, then this group must be created with an instance. Otherwise, it can be
-        created both with and without an instance. Creating an instanced group without an instance can be done to
-        provide a location for aggregate metrics across all instances, for example.
-        :return: The created group.
+
+        Args:
+            key (str): The key for the group.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            instance_required (bool): If true, then this group must be created with an instance. Otherwise, it can be
+                created both with and without an instance. Creating an instanced group without an instance can be done
+                to provide a location for aggregate metrics across all instances, for example.
+
+        Returns:
+             The created group.
         """
         group = Group(key, label, instanced=True, instance_required=instance_required)
         self.add_group(group)
         return group
 
     def add_groups(self, groups: list[Group]) -> None:
         """
         Adds a list of groups as subgroups of this group.
-        :param groups: A list of groups.
-        :return: None
+
+        Args:
+            groups (list[Group]): A list of groups.
         """
         for group in groups:
             self.add_group(group)
 
     def add_group(self, group: Group) -> None:
         """
         Adds a group as a subgroup of this group.
-        :param group: A group.
-        :return: None
+
+        Args:
+            group (Group): A group.
         """
         key = group.key
         if key in self.groups:
             raise DuplicateKeyException(
                 f"Group with key {key} already exists in {type(self)} {self.key}."
             )
         self.groups[key] = group
@@ -81,27 +91,28 @@
         is_rate: bool = False,
         is_discrete: bool = False,
         is_kpi: bool = False,
         is_impact: bool = False,
         is_key_attribute: bool = False,
     ) -> MetricAttribute:
         """
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param unit: Specifies what unit this metric is returned in. This allows the UI to display the units in a
-        consistent manner, and perform conversions when appropriate.
-        :param is_rate: Declares this attribute as a rate (e.g., kilobytes per second). If a unit is specified, this
-        will be set automatically. Otherwise, defaults to False.
-        :param is_discrete: Declares that this attribute's range of values is discrete (integer) rather than continuous
-        (floating point)
-        :param is_kpi: If set, threshold breaches for this metric will be used in the calculation of the object's
-        'Self - Health Score' metric, which can affect the 'Anomalies' Badge.
-        :param is_impact: If set, this attribute will never be the 'root cause' of an issue. For example, it could be a
-        proxy to a root cause, but not the root cause itself.
-        :param is_key_attribute: True if the attribute should be shown in some object summary widgets in the UI.
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            unit (Optional[Unit]): Specifies what unit this metric is returned in. This allows the UI to display the
+                units in a consistent manner, and perform conversions when appropriate.
+            is_rate (bool): Declares this attribute as a rate (e.g., kilobytes per second). If a unit is specified, this
+                will be set automatically. Otherwise, defaults to False.
+            is_discrete (bool): Declares that this attribute's range of values is discrete (integer) rather than
+                continuous (floating point)
+            is_kpi (bool): If set, threshold breaches for this metric will be used in the calculation of the object's
+                'Self - Health Score' metric, which can affect the 'Anomalies' Badge.
+            is_impact (bool): If set, this attribute will never be the 'root cause' of an issue. For example, it could
+                be a proxy to a root cause, but not the root cause itself.
+            is_key_attribute (bool): True if the attribute should be shown in some object summary widgets in the UI.
         """
         metric = MetricAttribute(
             key,
             label,
             unit,
             is_rate,
             is_discrete,
@@ -121,27 +132,30 @@
         is_rate: bool = False,
         is_discrete: bool = False,
         is_kpi: bool = False,
         is_impact: bool = False,
         is_key_attribute: bool = False,
     ) -> PropertyAttribute:
         """
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param unit: Specifies what unit this metric is returned in. This allows the UI to display the units in a
-        consistent manner, and perform conversions when appropriate.
-        :param is_rate: Declares this attribute as a rate (e.g., kilobytes per second). If a unit is specified, this
-        will be set automatically. Otherwise, defaults to False.
-        :param is_discrete: Declares that this attribute's range of values is discrete (integer) rather than continuous
-        (floating point). Defaults to False, unless 'is_string' is set, in which case it will always be set to True.
-        :param is_kpi: If set, threshold breaches for this metric will be used in the calculation of the object's
-        'Self - Health Score' metric, which can affect the 'Anomalies' Badge.
-        :param is_impact: If set, this attribute will never be the 'root cause' of an issue. For example, it could be a
-        proxy to a root cause, but not the root cause itself.
-        :param is_key_attribute: True if the attribute should be shown in some object summary widgets in the UI.
+
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            unit (Optional[Unit]): Specifies what unit this metric is returned in. This allows the UI to display the
+                units in a consistent manner, and perform conversions when appropriate.
+            is_rate (bool): Declares this attribute as a rate (e.g., kilobytes per second). If a unit is specified, this
+                will be set automatically. Otherwise, defaults to False.
+            is_discrete (bool): Declares that this attribute's range of values is discrete (integer) rather than
+                continuous (floating point). Defaults to False, unless 'is_string' is set, in which case it will always
+                be set to True.
+            is_kpi (bool): If set, threshold breaches for this metric will be used in the calculation of the object's
+                'Self - Health Score' metric, which can affect the 'Anomalies' Badge.
+            is_impact (bool): If set, this attribute will never be the 'root cause' of an issue. For example, it could
+                be a proxy to a root cause, but not the root cause itself.
+            is_key_attribute (bool): True if the attribute should be shown in some object summary widgets in the UI.
         """
         _property = PropertyAttribute(
             key,
             label,
             True,
             unit,
             is_rate,
@@ -162,27 +176,29 @@
         is_rate: bool = False,
         is_discrete: bool = False,
         is_kpi: bool = False,
         is_impact: bool = False,
         is_key_attribute: bool = False,
     ) -> PropertyAttribute:
         """
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param unit: Specifies what unit this metric is returned in. This allows the UI to display the units in a
-        consistent manner, and perform conversions when appropriate.
-        :param is_rate: Declares this attribute as a rate (e.g., kilobytes per second). If a unit is specified, this
-        will be set automatically. Otherwise, defaults to False.
-        :param is_discrete: Declares that this attribute's range of values is discrete (integer) rather than continuous
-        (floating point). Defaults to False, unless 'is_string' is set, in which case it will always be set to True.
-        :param is_kpi: If set, threshold breaches for this metric will be used in the calculation of the object's
-        'Self - Health Score' metric, which can affect the 'Anomalies' Badge.
-        :param is_impact: If set, this attribute will never be the 'root cause' of an issue. For example, it could be a
-        proxy to a root cause, but not the root cause itself.
-        :param is_key_attribute: True if the attribute should be shown in some object summary widgets in the UI.
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            unit (Optional[Unit]): Specifies what unit this metric is returned in. This allows the UI to display the
+                units in a consistent manner, and perform conversions when appropriate.
+            is_rate (bool): Declares this attribute as a rate (e.g., kilobytes per second). If a unit is specified, this
+                will be set automatically. Otherwise, defaults to False.
+            is_discrete (bool): Declares that this attribute's range of values is discrete (integer) rather than
+                continuous (floating point). Defaults to False, unless 'is_string' is set, in which case it will always
+                be set to True.
+            is_kpi (bool): If set, threshold breaches for this metric will be used in the calculation of the object's
+                'Self - Health Score' metric, which can affect the 'Anomalies' Badge.
+            is_impact (bool): If set, this attribute will never be the 'root cause' of an issue. For example, it could
+                be a proxy to a root cause, but not the root cause itself.
+            is_key_attribute (bool): True if the attribute should be shown in some object summary widgets in the UI.
         """
         _property = PropertyAttribute(
             key,
             label,
             False,
             unit,
             is_rate,
@@ -194,25 +210,27 @@
         )
         self.add_attribute(_property)
         return _property
 
     def add_attributes(self, attributes: list[Attribute]) -> None:
         """
         Adds a list of attributes to this group.
-        :param attributes: A list of attributes (metric or property definitions).
-        :return: None
+
+        Args:
+            attributes (list[Attribute]): A list of attributes (metric or property definitions).
         """
         for attribute in attributes:
             self.add_attribute(attribute)
 
     def add_attribute(self, attribute: Attribute) -> None:
         """
         Adds an attribute to this group.
-        :param attribute: An attribute (metric or property definition).
-        :return: None
+
+        Args:
+            attribute (Attribute): An attribute (metric or property definition).
         """
         key = attribute.key
         if key in self.attributes:
             raise DuplicateKeyException(
                 f"Attribute with key {key} already exists in {type(self)} {self.key}."
             )
 
@@ -233,23 +251,25 @@
         key: str,
         label: Optional[str] = None,
         instanced: bool = False,
         instance_required: bool = True,
     ) -> None:
         """
         Create a new group that can hold attributes and subgroups.
-        :param key: The key for the group.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param instanced: If True, this group can be 'instanced' with a value, so that its subgroups and attributes can
-        appear multiple times, once for each instance value. For example, a group containing
-        metrics for a network interface might be instanced for each discovered interface on the parent object.
-        :param instance_required: If true, then this group must be created with an instance. Otherwise, it can be
-        created both with and without an instance. Creating an instanced group without an instance can be done to
-        provide a location for aggregate metrics across all instances, for example. This does nothing if 'instanced' is
-        False.
+
+        Args:
+            key (str): The key for the group.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            instanced (bool): If True, this group can be 'instanced' with a value, so that its subgroups and attributes
+                can appear multiple times, once for each instance value. For example, a group containing
+                metrics for a network interface might be instanced for each discovered interface on the parent object.
+            instance_required (bool): If true, then this group must be created with an instance. Otherwise, it can be
+                created both with and without an instance. Creating an instanced group without an instance can be done
+                to provide a location for aggregate metrics across all instances, for example. This does nothing if
+                'instanced' is False.
         """
         self.key = validate_key(key, "Group")
         self.label = label
         if label is None:
             self.label = key
         self.instanced = instanced
         self.instance_required = instance_required
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/object_type.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/object_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2022 VMware, Inc.
+#  Copyright 2023 VMware, Inc.
 #  SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 from collections import OrderedDict
 from typing import Optional
 from typing import Union
 
@@ -15,16 +15,18 @@
 from aria.ops.definition.parameter import StringParameter
 
 
 class ObjectType(GroupType):  # type: ignore
     def __init__(self, key: str, label: Optional[str] = None):
         """
         Create a new object type definition
-        :param key: The key of the object type
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+
+        Args:
+            key (str): The key of the object type
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
         """
         self.key = validate_key(key, "Object type")
         self.label = label
         if label is None:
             self.label = key
         self.identifiers: dict = OrderedDict()
         super().__init__()
@@ -37,20 +39,24 @@
         is_part_of_uniqueness: bool = True,
         default: Optional[str] = None,
     ) -> ObjectType:
         """
         Create a new string identifier and apply it to this object type definition.
         All identifiers marked as 'part of uniqueness' are used to determine object identification. If none exist, the
         object name will be used for identification.
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param required: True if this parameter is required. Defaults to True.
-        :param is_part_of_uniqueness: True if the parameter should be used for object identification. Defaults to True.
-        :param default: The default value of the parameter.
-        :return The created String Identifier.
+
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optinal[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            required (bool): True if this parameter is required. Defaults to True.
+            is_part_of_uniqueness (bool): True if the parameter should be used for object identification. Defaults to True.
+            default (Optional[str]): The default value of the parameter.
+
+        Returns:
+             The created String Identifier.
         """
         parameter = StringParameter(
             key,
             label,
             required=required,
             advanced=not is_part_of_uniqueness,
             default=default,
@@ -67,20 +73,23 @@
         is_part_of_uniqueness: bool = True,
         default: Optional[int] = None,
     ) -> ObjectType:
         """
         Create a new int identifier and apply it to this object type definition.
         All identifiers marked 'part of uniqueness' are used to determine object identification. If none exist, the
         object name will be used for identification.
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param required: True if this parameter is required. Defaults to True.
-        :param is_part_of_uniqueness: True if the parameter should be used for object identification. Defaults to True.
-        :param default: The default value of the parameter.
-        :return The created Int Identifier.
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            required (bool): True if this parameter is required. Defaults to True.
+            is_part_of_uniqueness (bool): True if the parameter should be used for object identification. Defaults to True.
+            default ([Optional[int]): The default value of the parameter.
+
+        Returns:
+             The created Int Identifier.
         """
         parameter = IntParameter(
             key,
             label,
             required=required,
             advanced=not is_part_of_uniqueness,
             default=default,
@@ -98,22 +107,24 @@
         is_part_of_uniqueness: bool = True,
         default: Optional[str] = None,
     ) -> ObjectType:
         """
         Create a new enum identifier and apply it to this object type definition.
         All identifiers marked as 'part of uniqueness' are used to determine object identification. If none exist, the
         object name will be used for identification.
-        :param key: Used to identify the parameter.
-        :param values: An array containing all enum values. If 'default' is specified and not part of this array, it
-               will be added as an additional enum value (values are case-sensitive). Enum values are not localizable.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param required: True if this parameter is required. Defaults to True.
-        :param is_part_of_uniqueness: True if the parameter should be used for object identification. Defaults to True.
-        :param default: The default value of the parameter.
-        :return The created Enum Identifier.
+            key (str): Used to identify the parameter.
+            values (list[Union[str, tuple[str, str]]]): An array containing all enum values. If 'default' is specified and not part of this array, it
+            will be added as an additional enum value (values are case-sensitive). Enum values are not localizable.
+            label [Optinal[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            required (bool): True if this parameter is required. Defaults to True.
+            is_part_of_uniqueness (bool): True if the parameter should be used for object identification. Defaults to True.
+            default (Optional[str]): The default value of the parameter.
+
+        Returns:
+            The created Enum Identifier.
         """
         parameter = EnumParameter(
             key,
             values,
             label,
             required=required,
             advanced=not is_part_of_uniqueness,
@@ -121,26 +132,28 @@
             display_order=len(self.identifiers),
         )
         self.add_identifier(parameter)
         return self
 
     def add_identifiers(self, identifiers: list[Parameter]) -> None:
         """
-        :param identifiers: A list of identifiers to add to this object type
-        :return: None
+
+        Args:
+            identifiers: A list of identifiers to add to this object type
         """
         for identifier in identifiers:
             self.add_identifier(identifier)
 
     def add_identifier(self, identifier: Parameter) -> None:
         """
         Add an identifier to this object type. All 'identifying' identifiers are used to determine object uniqueness.
         If no 'identifying' identifiers exist, they object name will be used for uniqueness.
-        :param identifier: The identifier to add to the object type definition.
-        :return: None
+
+        Args:
+            identifier (Parameter): The identifier to add to the object type definition.
         """
         key = identifier.key
         if key in self.identifiers:
             raise DuplicateKeyException(
                 f"Identifier with key {key} already exists in object type {self.key}."
             )
         self.identifiers[key] = identifier
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/parameter.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/parameter.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,21 +18,22 @@
         description: Optional[str] = None,
         default: Optional[Union[str, int]] = None,
         required: bool = True,
         advanced: bool = False,
         display_order: int = 0,
     ) -> None:
         """
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param description: More in-depth explanation of the parameter. Displayed as a tooltip in the VMware Aria Operations UI.
-        :param default: The default value of the parameter.
-        :param required: True if user is required to provide this parameter. Defaults to True.
-        :param advanced: True if the parameter should be collapsed by default. Defaults to False.
-        :param display_order: Determines the order parameters will be displayed in the UI.
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            description (Optional[str]): More in-depth explanation of the parameter. Displayed as a tooltip in the VMware Aria Operations UI.
+            default (Optional[Union[str, int]]): The default value of the parameter.
+            required (bool): True if user is required to provide this parameter. Defaults to True.
+            advanced (bool): True if the parameter should be collapsed by default. Defaults to False.
+            display_order (int): Determines the order parameters will be displayed in the UI.
         """
         self.key = validate_key(key, "Parameter/Identifier")
         self.label = label
         if label is None:
             self.label = key
         self.description = description
         self.default = default
@@ -60,21 +61,23 @@
         description: Optional[str] = None,
         default: Optional[int] = None,
         required: bool = True,
         advanced: bool = False,
         display_order: int = 0,
     ) -> None:
         """
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param description: More in-depth explanation of the parameter. Displayed as a tooltip in the VMware Aria Operations UI.
-        :param default: The default value of the parameter.
-        :param required: True if user is required to provide this parameter. Defaults to True.
-        :param advanced: True if the parameter should be collapsed by default. Defaults to False.
-        :param display_order: Determines the order parameters will be displayed in the UI.
+
+        Args:
+            key (str): Used to identify the parameter.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            description (Optional[str]): More in-depth explanation of the parameter. Displayed as a tooltip in the VMware Aria Operations UI.
+            default (Optional[str]): The default value of the parameter.
+            required (bool): True if user is required to provide this parameter. Defaults to True.
+            advanced (bool): True if the parameter should be collapsed by default. Defaults to False.
+            display_order (int): Determines the order parameters will be displayed in the UI.
         """
         super().__init__(
             key, label, description, default, required, advanced, display_order
         )
 
     def to_json(self) -> dict:
         return super().to_json() | {
@@ -92,22 +95,23 @@
         default: Optional[str] = None,
         max_length: int = 512,
         required: bool = True,
         advanced: bool = False,
         display_order: int = 0,
     ) -> None:
         """
-        :param key: Used to identify the parameter.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param description: More in-depth explanation of the parameter. Displayed as a tooltip in the VMware Aria Operations UI.
-        :param default: The default value of the parameter.
-        :param max_length: The max length of the parameter value. Defaults to 512.
-        :param required: True if user is required to provide this parameter. Defaults to True.
-        :param advanced: True if the parameter should be collapsed by default. Defaults to False.
-        :param display_order: Determines the order parameters will be displayed in the UI.
+        Args:
+           key (str): Used to identify the parameter.
+           label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+           description (Optional[str]): More in-depth explanation of the parameter. Displayed as a tooltip in the VMware Aria Operations UI.
+           default (Optional[str]): The default value of the parameter.
+           max_length (int): The max length of the parameter value. Defaults to 512.
+           required (bool): True if user is required to provide this parameter. Defaults to True.
+           advanced (bool): True if the parameter should be collapsed by default. Defaults to False.
+           display_order (int): Determines the order parameters will be displayed in the UI.
         """
         super().__init__(
             key, label, description, default, required, advanced, display_order
         )
         self.max_length = max_length
 
     def to_json(self) -> dict:
@@ -127,23 +131,27 @@
         description: Optional[str] = None,
         default: Optional[str] = None,
         required: bool = True,
         advanced: bool = False,
         display_order: int = 0,
     ) -> None:
         """
-        :param key: Used to identify the parameter.
-        :param values: An array containing all enum values. If 'default' is specified and not part of this array, it
-               will be added as an additional enum value. Enum values are not localizable.
-        :param label: Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
-        :param description: More in-depth explanation of the parameter. Displayed as a tooltip in the VMware Aria Operations UI.
-        :param default: The default value of the parameter.
-        :param required: True if user is required to provide this parameter. Defaults to True.
-        :param advanced: True if the parameter should be collapsed by default. Defaults to False.
-        :param display_order: Determines the order parameters will be displayed in the UI.
+
+        Args:
+            key (str): Used to identify the parameter.
+            values (list[Union[str, tuple[str, str]]]): An array containing all enum values. If 'default' is specified
+                and not part of this array, it will be added as an additional enum value. Enum values are not
+                localizable.
+            label (Optional[str]): Label that is displayed in the VMware Aria Operations UI. Defaults to the key.
+            description (Optional[str]): More in-depth explanation of the parameter. Displayed as a tooltip in the
+                VMware Aria Operations UI.
+            default (Optional[str]): The default value of the parameter.
+            required (bool): True if user is required to provide this parameter. Defaults to True.
+            advanced (bool): True if the parameter should be collapsed by default. Defaults to False.
+            display_order (int): Determines the order parameters will be displayed in the UI.
         """
         super().__init__(
             key, label, description, default, required, advanced, display_order
         )
         if len(values) > len(set(values)):
             raise DuplicateKeyException(
                 f"Duplicate enum value in parameter {key}: {values}."
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/definition/units.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/definition/units.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/event.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/event.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2022 VMware, Inc.
+#  Copyright 2023 VMware, Inc.
 #  SPDX-License-Identifier: Apache-2.0
 from dataclasses import dataclass
 from enum import Enum
 from typing import Optional
 
 
 class Criticality(Enum):
@@ -12,45 +12,49 @@
     IMMEDIATE = 3
     CRITICAL = 4
     AUTOMATIC = 5
 
 
 @dataclass(frozen=True)
 class Event:
-    """Represents a Aria Operations Event
+    """
+    Represents an Aria Operations Event.
 
-    :param message: The message describes and identifies an event.
-    :param criticality: TODO
-    :param fault_key: TODO
-    :param auto_cancel: TODO
-    :param start_date: TODO
-    :param update_date: TODO
-    :param cancel_date: TODO
-    :param watch_wait_cycle: The number of times this event must be present in a collection before Aria Operations surfaces it
-    in the UI.
-    :param cancel_wait_cycle: The number of times this event must be absent in a collection before Aria Operations removes it
-    from the UI.
+    Args:
+        message (str): The message describes and identifies an event.
+        criticality (Criticality, optional): TODO. Defaults to Criticality.NONE.
+        fault_key (str, optional): TODO. Defaults to None.
+        auto_cancel (bool, optional): TODO. Defaults to False.
+        start_date (int, optional): TODO. Defaults to None.
+        update_date (int, optional): TODO. Defaults to None.
+        cancel_date (int, optional): TODO. Defaults to None.
+        watch_wait_cycle (int, optional): The number of times this event must be present in a collection before Aria
+                                          Operations surfaces it in the UI. Defaults to 1.
+        cancel_wait_cycle (int, optional): The number of times this event must be absent in a collection before Aria
+                                            Operations removes it from the UI. Defaults to 3.
     """
 
     message: str
     criticality: Criticality = Criticality.NONE
     fault_key: Optional[str] = None
     auto_cancel: bool = False
     start_date: Optional[int] = None
     update_date: Optional[int] = None
     cancel_date: Optional[int] = None
     watch_wait_cycle: int = 1
     cancel_wait_cycle: int = 3
 
     def get_json(self) -> dict:
-        """Get a JSON representation of this Event.
+        """
+        Get a JSON representation of this Event.
 
         Returns a JSON representation of this Event in the format required by Aria Operations.
 
-        :return: A JSON representation of this Event.
+        Returns:
+            dict: A JSON representation of this Event.
         """
         # message is the only required field. Other fields are optional but non-nullable if present
         json: dict = {"message": self.message}
 
         if self.criticality is not None:
             json["criticality"] = self.criticality.value
         if self.message is not None:
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/object.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/object.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Optional
 from typing import Set
 
 from aria.ops.data import Metric
 from aria.ops.data import Property
 from aria.ops.event import Event
 
+
 #  Copyright 2022 VMware, Inc.
 #  SPDX-License-Identifier: Apache-2.0
 
 
 class Key:
     """Object's Key class, used for identifying Objects
 
@@ -34,22 +35,23 @@
     def __init__(
         self,
         adapter_kind: str,
         object_kind: str,
         name: str,
         identifiers: Optional[List[Identifier]] = None,
     ) -> None:
-        """Initializes a Key, which uniquely identifies a vROps Object
+        """Initializes a Key, which uniquely identifies a vROps Object.
 
-        :param adapter_kind: The Adapter Kind this Object is associated with.
-        :param object_kind: The Object Kind (e.g., class) of this Object.
-        :param name: A human-readable name for this Object. Should be unique if possible.
-        :param identifiers: A list of :class:`Identifier` that uniquely identify the Object. If none are present than
-            the name must be unique and is used for identification. All Objects with the same adapter kind and Object
-            kind must have the same set of identifiers.
+        Args:
+            adapter_kind: The Adapter Kind this Object is associated with.
+            object_kind: The Object Kind (e.g., class) of this Object.
+            name: A human-readable name for this Object. Should be unique if possible.
+            identifiers: A list of :class:`Identifier` that uniquely identify the Object. If none are present than
+                the name must be unique and is used for identification. All Objects with the same adapter kind and Object
+                kind must have the same set of identifiers.
         """
         self.adapter_kind = adapter_kind
         self.object_kind = object_kind
         self.name = name
         if identifiers is None:
             identifiers = []
         self.identifiers = {identifier.key: identifier for identifier in identifiers}
@@ -81,35 +83,39 @@
 
     def __hash__(self) -> int:
         return hash(self.__key())
 
     def get_identifier(
         self, key: str, default_value: Optional[str] = None
     ) -> Optional[str]:
-        """Return the value for the given identifier key
+        """Return the value for the given identifier key.
 
-        :param key: The identifier key
-        :param default_value: An optional default value
-        :return: The value associated with the identifier.
-        If the value associated with the identifier is empty and 'default_value' is
-        provided, returns 'default_value'.
-        If the identifier does not exist, returns default_value if provided, else 'None'.
+        Args:
+            key: The identifier key.
+            default_value: An optional default value.
+
+        Returns:
+            The value associated with the identifier.
+            If the value associated with the identifier is empty and 'default_value' is
+            provided, returns 'default_value'.
+            If the identifier does not exist, returns default_value if provided, else 'None'.
         """
         if self.identifiers.get(key):
             if self.identifiers[key].value or default_value is None:
                 return self.identifiers[key].value
             return default_value
         return default_value
 
     def get_json(self) -> dict:
-        """Get a JSON representation of this Key
+        """Get a JSON representation of this Key.
 
-        Returns a JSON representation of this Key in the format required by vROps.
+        This method returns a JSON representation of this Key in the format required by vROps.
 
-        :return: A JSON representation of this Key
+        Returns:
+            dict: A JSON representation of this Key.
         """
         return {
             "name": self.name,
             "adapterKind": self.adapter_kind,
             "objectKind": self.object_kind,
             "identifiers": [
                 identifier.get_json() for identifier in self.identifiers.values()
@@ -127,23 +133,24 @@
 
 class Identifier:
     """Represents a piece of data that identifies an Object."""
 
     def __init__(
         self, key: str, value: str, is_part_of_uniqueness: bool = True
     ) -> None:
-        """Creates an identifier which is used as part of an Object's identification in a :class:`Key`
+        """Creates an identifier which is used as part of an Object's identification in a :class:`Key`.
 
-        Represents a piece of data that identifies an Object. If `is_part_of_uniqueness` is False, this data can
-        change over time without creating a new Object. This is primarily used for human-readable values that are useful
-        in identification purposes, but may change at times.
-
-        :param key: A key that determines which identifier the value corresponds to.
-        :param value: The value of the identifier.
-        :param is_part_of_uniqueness: Determines if this key/value pair is used in the identification process
+        This class represents a piece of data that identifies an Object. If `is_part_of_uniqueness` is False, this data
+        can change over time without creating a new Object. This is primarily used for human-readable values that are
+        useful in identification purposes, but may change at times.
+
+        Args:
+            key: A key that determines which identifier the value corresponds to.
+            value: The value of the identifier.
+            is_part_of_uniqueness: Determines if this key/value pair is used in the identification process.
         """
         self.key = key
         self.value = value
         self.is_part_of_uniqueness = is_part_of_uniqueness
 
     def __repr__(self) -> str:
         u = "*" if self.is_part_of_uniqueness else ""
@@ -169,19 +176,20 @@
             return self.__key() == other.__key()
         return False
 
     def __hash__(self) -> int:
         return hash(self.__key())
 
     def get_json(self) -> dict:
-        """Get a JSON representation of this Identifier
+        """Get a JSON representation of this Identifier.
 
-        Returns a JSON representation of this Identifier in the format required by vROps.
+        This method returns a JSON representation of this Identifier in the format required by vROps.
 
-        :return: A JSON representation of this Identifier
+        Returns:
+            dict: A JSON representation of this Identifier.
         """
         return {
             "key": self.key,
             "value": self.value,
             "isPartOfUniqueness": self.is_part_of_uniqueness,
         }
 
@@ -192,288 +200,314 @@
     Contains :class:`Metric`, :class:`Property`, :class:`Event`, and relationships to other Objects. Each Object is
     identified by a unique :class:`Key`.
     """
 
     def __init__(self, key: Key) -> None:
         """Create a new Object with a given Key.
 
-        The preferred way to create a new Object is to call the :class:`Result.object` method on the :class:`Result`
-        class, which ensures that for a given key only one Object exists.
+        This method is the preferred way to create a new Object. It should be called from the :class:`Result.object`
+        method on the :class:`Result` class, which ensures that for a given key only one Object exists.
 
-        :param key: The :class:`Key` that uniquely identifies this Object
+        Args:
+            key: The :class:`Key` that uniquely identifies this Object.
         """
+
         self._key: Key = key
         self._metrics: List[Metric] = []
         self._properties: List[Property] = []
         self._events: Set[Event] = set()
         self._parents: Set[Key] = set()
         self._children: Set[Key] = set()
         self._updated_children: bool = False
 
     def get_key(self) -> Key:
         """Get a copy of the Object's Key.
 
         An object's Key cannot change after it has been created.
 
-        :return: A copy of the object's key
+        Returns:
+            A copy of the object's key.
         """
         return copy.deepcopy(self._key)
 
     def adapter_type(self) -> str:
         """Get the adapter type of this object
 
-        :return: The adapter type of this object
+        Returns:
+             The adapter type of this object
         """
         return self._key.adapter_kind
 
     def object_type(self) -> str:
         """Get the type of this object
 
-        :return: The type of this object
+        Returns:
+             The type of this object
         """
         return self._key.object_kind
 
     def get_identifier_value(
         self, identifier_key: str, default_value: Optional[str] = None
     ) -> Optional[str]:
         """Retrieve the value of a given identifier
 
-        :param identifier_key: Key of the identifier
-        :param default_value: An optional default value
-        :return: The value associated with the identifier.
-        If the value associated with the identifier is empty and 'default_value' is
-        provided, returns 'default_value'.
-        If the identifier does not exist, returns default_value if provided, else 'None'.
+        Args:
+            identifier_key (str): Key of the identifier
+            default_value (str): An optional default value
+
+        Returns:
+            The value associated with the identifier.
+            If the value associated with the identifier is empty and 'default_value' is
+            provided, returns 'default_value'.
+            If the identifier does not exist, returns default_value if provided, else 'None'.
         """
         return self._key.get_identifier(identifier_key, default_value)
 
     def add_metric(self, metric: Metric) -> None:
-        """Method that adds a single Metric data point to this Object
+        """Adds a single Metric data point to this Object.
 
-        :param metric: A :class:`Metric` data point to add to this Object
-        :return: None
+        Args:
+            metric (Metric): A Metric data point to add to this Object.
         """
         self._metrics.append(metric)
 
     def add_metrics(self, metrics: List[Metric]) -> None:
-        """Method that adds a list of Metric data points to this Object
+        """Adds a list of Metric data points to this Object.
 
-        :param metrics: A list of :class:`Metric` data points to add to this Object
-        :return: None
+        Args:
+            metrics (List[Metric]): A list of Metric data points to add to this Object.
         """
         for metric in metrics:
             self.add_metric(metric)
 
     def with_metric(self, *args: Any, **kwargs: Any) -> None:
         """Method that handles creating a :class:`Metric` data point, and adding to this Object.
 
         The signature matches :class:`Metric.__init__`.
-        :return: None
         """
         self.add_metric(Metric(*args, **kwargs))
 
     def get_metric(self, key: str) -> List[Metric]:
         """
 
-        :param key: Metric key of the metric to return.
-        :return: All metrics matching the given key.
+        Args:
+         key (str): Metric key of the metric to return.
+
+        Returns:
+            All metrics matching the given key.
         """
         return list(filter(lambda metric: metric.key == key, self._metrics))
 
     def get_metric_values(self, key: str) -> List[float]:
         """
 
-        :param key: Metric key of the metric to return.
-        :return: A list of the metric values in chronological order.
+        Args:
+            key (str): Metric key of the metric to return.
+
+        Returns (List[float]): A list of the metric values in chronological order.
         """
         # find matching metrics
         metrics = self.get_metric(key)
 
         # sort metrics by timestamp from oldest  to newest
         metrics.sort(key=lambda metric: metric.timestamp)  # type: ignore
 
         return [m.value for m in metrics]
 
     def get_last_metric_value(self, key: str) -> Optional[float]:
         """
 
-        :param key: Metric key of the metric to return.
-        :return: The latest value of the metric or None if no metric exists with the given key.
+        Args:
+            key (str) : Metric key of the metric to return.
+
+        Returns:
+            The latest value of the metric or None if no metric exists with the given key.
         """
         metrics = self.get_metric_values(key)
 
         if not metrics:
             return None
         else:
             return metrics[-1]
 
     def add_property(self, property_: Property) -> None:
         """Method that adds a single Property value to this Object
 
-        :param property_: A :class:`Property` value to add to this Object
-        :return: None
+        Args:
+            property_ (Property): A :class:`Property` value to add to this Object
         """
         self._properties.append(property_)
 
     def add_properties(self, properties: List[Property]) -> None:
         """Method that adds a list of Property values to this Object
 
-        :param properties: A list of :class:`Property` values to add to this Object
-        :return: None
+        Args:
+            properties (List[Property]): A list of :class:`Property` values to add to this Object
         """
         for property_ in properties:
             self.add_property(property_)
 
     def with_property(self, *args: Any, **kwargs: Any) -> None:
         """Method that handles creating a :class:`Property` value, and adding to this Object.
 
         The signature matches :class:`Property.__init__`.
-        :return: None
         """
         self.add_property(Property(*args, **kwargs))
 
     def get_property(self, key: str) -> List[Property]:
         """
 
-        :param key: Property key of the property to return.
-        :return: All properties matching the given key
+        Args:
+            key (str): Property key of the property to return.
+
+        Returns:
+             All properties matching the given key
         """
         return list(filter(lambda property_: property_.key == key, self._properties))
 
     def get_property_values(self, key: str) -> List[str]:
         """
 
-        :param key: Property key of the property to return.
-        :return: A list of the property values in chronological order.
+        Args:
+            key (str): Property key of the property to return.
+
+        Returns:
+            A list of the property values in chronological order.
         """
         # find matching properties
         properties = self.get_property(key)
 
         # sort properties by timestamp from oldest  to newest
         properties.sort(key=lambda property_: property_.timestamp)  # type: ignore
 
         return [p.value for p in properties]
 
     def get_last_property_value(self, key: str) -> Optional[str | float]:
         """
 
-        :param key: Property key of the property to return.
-        :return: The latest value of the property or None if no property exists with the given key.
+        Args:
+            key (str): Property key of the property to return.
+
+        Returns:
+             The latest value of the property or None if no property exists with the given key.
         """
         properties = self.get_property_values(key)
 
         if not properties:
             return None
         else:
             return properties[-1]
 
     def add_event(self, event: Event) -> None:
         """Method that adds a single Event to this Object
 
-        :param event: An :class:`Event` to add to this Object
-        :return: None
+        Args:
+            event: An :class:`Event` to add to this Object
         """
         self._events.add(event)
 
     def add_events(self, events: List[Event]) -> None:
         """Method that adds a list of Events to this Object
 
-        :param events: A list of :class:`Event` to add to this Object
-        :return: None
+        Args:
+            events (List[Event]): A list of :class:`Event` to add to this Object
         """
         for event in events:
             self.add_event(event)
 
     def with_event(self, *args: Any, **kwargs: Any) -> None:
         """Method that handles creating an :class:`Event`, and adding to this Object.
 
         The signature matches :class:`Event.__init__`.
-        :return: None
         """
         self.add_event(Event(*args, **kwargs))
 
     def add_parent(self, parent: Object) -> None:
         """Method that adds a parent Object to this Object.
 
         This Object will also be added as a child to the parent.
 
         Relationship cycles are not permitted.
 
-        :param parent: Parent :class:`Object`
-        :return: None
+        Args:
+            parent (Object): Parent :class:`Object`
         """
         self._parents.add(parent._key)
         parent._children.add(self._key)
 
     def add_parents(self, parents: List[Object]) -> None:
         """Method that adds a list of parent Objects to this Object.
 
         This Object will also be added as a child to each of the parents.
 
         Relationship cycles are not permitted.
 
-        :param parents: A list of parent :class:`Object`
-        :return: None
+        Args:
+            parents (List[Object]): A list of parent :class:`Object`
         """
         for parent in parents:
             self.add_parent(parent)
 
     def get_parents(self) -> Set[Key]:
         """
-        :return: A set of all object keys that are parents of this object
+        Returns:
+         A set of all object keys that are parents of this object
         """
         return self._parents
 
     def add_child(self, child: Object) -> None:
         """Method that adds a child Object to this Object.
 
         This Object will also be added as a parent to the child.
 
         Relationship cycles are not permitted.
 
-        :param child: Child :class:`Object`
-        :return: None
+        Args:
+            child (Object): Child :class:`Object`
         """
         self._updated_children = True
         self._children.add(child._key)
         child._parents.add(self._key)
 
     def add_children(self, children: List[Object]) -> None:
         """Method that adds a list of child Objects to this Object.
 
         This Object will also be added as a parent to each of the children.
 
         Relationship cycles are not permitted.
 
-        :param children: A list of child :class:`Object`
-        :return: None
+        Args:
+            children (List[Object]): A list of child :class:`Object`
         """
         # We want to set this even in the case where the list is empty
         self._updated_children = True
         for child in children:
             self.add_child(child)
 
     def get_children(self) -> Set[Key]:
         """
-        :return: A set of all object keys that are children of this object
+        Returns:
+            A set of all object keys that are children of this object
         """
         return self._children
 
     def has_content(self) -> bool:
         """
-        :return: True if the object contains any metrics, properties or events; False otherwise.
+        Returns:
+             True if the object contains any metrics, properties or events; False otherwise.
         """
         return bool(self._metrics) or bool(self._properties) or bool(self._events)
 
     def get_json(self) -> dict:
         """Get a JSON representation of this Object
 
         Returns a JSON representation of this Object in the format required by vROps.
 
-        :return: A JSON representation of this Object
+        Returns:
+             A JSON representation of this Object
         """
         return {
             "key": self._key.get_json(),
             "metrics": [metric.get_json() for metric in self._metrics],
             "properties": [prop.get_json() for prop in self._properties],
             "events": [event.get_json() for event in self._events],
         }
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/pipe_utils.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/pipe_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,27 +6,41 @@
 import logging
 from typing import Optional
 from typing import Union
 
 logger = logging.getLogger(__name__)
 
 
-def read_from_pipe(input_pipe: str) -> Optional[dict | list]:
+def read_from_pipe(input_pipe: str) -> Optional[Union[dict, list]]:
+    """Reads data from the input pipe.
+
+    Args:
+        input_pipe (str): The path to the input pipe.
+
+    Returns:
+        Optional[Union[dict, list]]: The data read from the input pipe, or None if there was an error.
+    """
     logger.debug(f"Input Pipe: {input_pipe}")
     try:
         with open(input_pipe, "r") as input_file:
             logger.debug(f"Opened {input_file.name}")
             return json.load(input_file)  # type: ignore[no-any-return]
     except Exception as e:
         logger.error("Error when reading from Input Pipe.")
         logger.debug(e)
         return None
 
 
-def write_to_pipe(output_pipe: str, result: Optional[dict | list]) -> None:
+def write_to_pipe(output_pipe: str, result: Optional[Union[dict, list]]) -> None:
+    """Writes data to the output pipe.
+
+    Args:
+        output_pipe (str): The path to the output pipe.
+        result (Optional[Union[dict, list]]): The data to write to the output pipe.
+    """
     logger.debug(repr(result))
     logger.debug(f"Output Pipe: {output_pipe}")
     try:
         with open(output_pipe, "w") as output_file:
             logger.debug(f"Opened {output_pipe}")
             json.dump(result, output_file)
             logger.debug(f"Closing {output_pipe}")
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/result.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/result.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,48 +27,53 @@
     def __init__(self) -> None:
         """Initializes a Result"""
         self._error_message: Optional[str] = None
 
     def is_success(self) -> bool:
         """
 
-        :return: True if the TestResult represents a successful test
+        Returns:
+             True if the TestResult represents a successful test
         """
         return self._error_message is None
 
     def with_error(self, error_message: str) -> None:
         """Set the adapter instance connection test to failed, and display the given
         error message.
 
         If this method is called multiple times, only the most recent error message
         will be recorded. If error_message is set, the test is considered failed.
 
-        :param error_message: A string containing the error message
-        :return: None
+        Args:
+            error_message (str): A string containing the error message
         """
         self._error_message = error_message
 
     def get_json(self) -> dict:
         """Get a JSON representation of this TestResult
 
         Returns a JSON representation of this TestResult in the format required by
         Aria Operations, indicating either a successful test, or a failed test with
         error message.
 
-        :return: A JSON representation of this TestResult
+        Returns:
+             A JSON representation of this TestResult
         """
         if self.is_success():
             return {}
         else:
             return {"errorMessage": self._error_message}
 
     def send_results(self, output_pipe: str = sys.argv[-1]) -> None:
         """Opens the output pipe and sends results directly back to the server
 
         This method can only be called once per collection.
+
+        Args:
+            output_pipe (str): The path to the input pipe. Defaults to sys.argv[-1]
         """
         # The server always invokes methods with the output file as the last argument
         write_to_pipe(output_pipe, self.get_json())
 
 
 class EndpointResult:
     """Class for managing the results of an adapter instance get endpoint URLs call
@@ -86,34 +91,37 @@
     def with_endpoint(self, endpoint_url: str) -> None:
         """Adds an endpoint to the list of endpoints Aria Operations will test for
         certificate validation.
 
         If this method is called multiple times, each url will be called by Aria
         Operations.
 
-        :param endpoint_url: A string containing the url
-
-        :return: None
+        Args:
+            endpoint_url (srt): A string containing the url
         """
         self.endpoints.append(endpoint_url)
 
     def get_json(self) -> dict:
         """Get a JSON representation of this EndpointResult
 
         Returns a JSON representation of this EndpointResult in the format required
         by Aria Operations.
 
-        :return: A JSON representation of this EndpointResult
+        Returns:
+             A JSON representation of this EndpointResult
         """
         return {"endpointUrls": self.endpoints}
 
     def send_results(self, output_pipe: str = sys.argv[-1]) -> None:
         """Opens the output pipe and sends results directly back to the server
 
         This method can only be called once per collection.
+
+        Args:
+            output_pipe (str): The path to the input pipe. Defaults to sys.argv[-1]
         """
         # The server always invokes methods with the output file as the last argument
         write_to_pipe(output_pipe, self.get_json())
 
 
 RelationshipUpdateMode = NewType("RelationshipUpdateMode", int)
 
@@ -162,19 +170,19 @@
     ) -> None:
         """Initializes a Result
 
         A result contains objects, which can be added at initialization or later.
         Each object has a key containing one or more identifiers plus the object type
         and adapter type. Keys must be unique across objects in a Result.
 
-        :param obj_list: an optional list of objects to send to Aria Operations.
-        Objects can be added later using add_object
-
-        :param target_definition: an optional description of the returned objects,
-        used for validation purposes
+        Args:
+            obj_list (Optional[List[Object]]): an optional list of objects to send to Aria Operations. Objects can be
+                added later using add_object. Defaults to None
+            target_definition (AdapterDefinition): an optional description of the returned objects, used for validation
+                purposes. Defaults to None.
         """
         self.objects: dict[Key, Object] = {}
         if type(obj_list) is list:
             self.add_objects(obj_list)
         self.definition: AdapterDefinition = target_definition
         self.adapter_type = None
         if self.definition:
@@ -202,59 +210,73 @@
         If an object with the same key already exists in the result, return that
         object, otherwise create a new object, add it to the result, and return it.
         See discussion on keys in the documentation for the :class:`object.Key` class.
 
         If this method is used to create an object, it does not need to be added
         later using `add_object` (or `add_objects`)
 
-        :param adapter_kind: The adapter kind of the object
-        :param object_kind: The resource kind of the object
-        :param name: The name of the object
-        :param identifiers:
-        :return: The object with the given key
+        Args:
+            adapter_kind (str): The adapter kind of the object
+            object_kind (str): The resource kind of the object
+            name (str): The name of the object
+            identifiers (Optional[List[Identifier]]): An optional list of Identifiers for the object
+
+        Returns:
+             The object with the given key
         """
         obj = Object(Key(adapter_kind, object_kind, name, identifiers))
         return self.objects.setdefault(obj.get_key(), obj)
 
     def get_object(self, obj_key: Key) -> Optional[Object]:
         """Get and return the object corresponding to the given key, if it exists
 
-        :param obj_key: The object key to search for
-        :return: The object with the given key, or None if the key is not in the result
+        Args:
+            obj_key (Key): The object key to search for
+
+        Returns:
+             The object with the given key, or None if the key is not in the result
         """
         return self.objects.get(obj_key, None)
 
     def get_objects_by_type(
         self, object_type: str, adapter_type: Optional[str] = None
     ) -> List[Object]:
         """Returns all objects with the given type. If adapter_type is present,
         the objects must also be from the given adapter type.
 
-        :param object_type: The object type to return
-        :param adapter_type: The adapter type of the objects to return
-        :return: A list of objects matching the object type and adapter type
+        Args:
+            object_type (str): The object type to return
+            adapter_type (Optional[str]): The adapter type of the objects to return. Defaults to None
+
+        Returns:
+             A list of objects matching the object type and adapter type
         """
         return [
             obj
             for obj in self.objects.values()
             if obj.adapter_type() == object_type
             and (adapter_type is None or adapter_type == obj.adapter_type())
         ]
 
     def add_object(self, obj: Object) -> Object:
         """Adds the given object to the Result and returns it.
 
         Adds the given object to the Result and returns it. A different object with
         the same key cannot already exist in the Result. If it does,
-        an :class:`ObjectKeyAlreadyExistsException` will be raised.
+        an ObjectKeyAlreadyExistsException will be raised.
+
+        Args:
+            obj (Object): An object to add to the Result.
+
+        Returns:
+            Object: The object.
 
-        :param obj: An object to add to the Result
-        :return: The object
-        :raises: ObjectKeyAlreadyExistsException if a different object with the same key
-        already exists in the Result
+        Raises:
+            ObjectKeyAlreadyExistsException: If a different object with the same key
+                already exists in the Result.
         """
         o = self.objects.setdefault(obj.get_key(), obj)
         if o is obj:
             return o
         raise ObjectKeyAlreadyExistsException(
             f"A different object with key {obj.get_key()} already exists."
         )
@@ -262,43 +284,49 @@
     def add_objects(self, obj_list: list[Object]) -> None:
         """Adds the given objects to the Result and returns it.
 
         Adds the given objects to the Result. A different object with the same key
         cannot already exist in the Result. If it does, an
         :class:`ObjectKeyAlreadyExistsException` will be raised.
 
-        :param obj_list: A list of objects to add to the Result
-        :return: The object
-        :raises: ObjectKeyAlreadyExistsException if a different object with the same
-        key already exists in the Result
+        Args:
+            obj_list (List[Object]): A list of objects to add to the Result
+
+        Returns:
+            The object
+
+        Raises:
+            ObjectKeyAlreadyExistsException: if a different object with the same
+                key already exists in the Result
         """
         for obj in obj_list:
             self.add_object(obj)
 
     def with_error(self, error_message: str) -> None:
         """Set the Adapter Instance to an error state with the provided message.
 
         If this method is called multiple times, only the most recent error message
         will be recorded. If error_message is set, no results (objects, relationships)
         will be returned.
 
-        :param error_message: A string containing the error message
-        :return: None
+        Args:
+            error_message (str): A string containing the error message
         """
         self._error_message = error_message
 
     def get_json(self) -> dict:
         """Get a JSON representation of this Result
 
         Returns a JSON representation of this Result in the format required by Aria
         Operations. The representation includes all objects (including the object's
         events, properties, and metrics) in the Result. Relationships are returned
         following the update_relationships flag (See RelationshipUpdateMode).
 
-        :return: A JSON representation of this Result
+        Returns:
+            A JSON representation of this Result
         """
         if self._error_message is None:
             result = {
                 "result": [
                     obj.get_json()
                     for obj in self.objects.values()
                     if not self._object_is_external(obj) or obj.has_content()
@@ -339,10 +367,13 @@
         else:
             return {"errorMessage": self._error_message}
 
     def send_results(self, output_pipe: str = sys.argv[-1]) -> None:
         """Opens the output pipe and sends results directly back to the server
 
         This method can only be called once per collection.
+
+        Args:
+            output_pipe (str): The path to the input pipe. Defaults to sys.argv[-1]
         """
         # The server always invokes methods with the output file as the last argument
         write_to_pipe(output_pipe, self.get_json())
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/suite_api_client.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/suite_api_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,18 +26,19 @@
 
 class SuiteApiConnectionParameters:
     def __init__(
         self, host: str, username: str, password: str, auth_source: str = "LOCAL"
     ):
         """Initialize SuiteApi Connection Parameters
 
-        :param host: The host to use for connecting to the SuiteAPI.
-        :param username: Username used to authenticate to SuiteAPI
-        :param password: Password used to authenticate to SuiteAPI
-        :param auth_source: Source of authentication
+        Args:
+            host (str): The host to use for connecting to the SuiteAPI.
+            username (str): Username used to authenticate to SuiteAPI
+            password (str): Password used to authenticate to SuiteAPI
+            auth_source (str): Source of authentication. Defaults to "LOCAL"
         """
         if "http" in host:
             self.host = f"{host}/suite-api/"
         else:
             self.host = f"https://{host}/suite-api/"
         self.username = username
         self.password = password
@@ -59,48 +60,51 @@
         # Code using suiteApiClient goes here
         ...
     """
 
     def __init__(self, connection_params: SuiteApiConnectionParameters):
         """Initializes a SuiteAPI client.
 
-        :param connection_params: Connection parameters for the Suite API.
+        Args:
+             connection_params (SuiteApiConnectionParameters): Connection parameters for the Suite API.
         """
         self.credential = connection_params
         self.token = ""
 
     def __enter__(self) -> SuiteApiClient:
         """Acquire a token upon entering the 'with' context
 
-        :return: self
+        Returns:
+            SuiteApiClient: The current instance of the class.
         """
         self.token = self.get_token()
         return self
 
     def __exit__(
         self,
         exception_type: Optional[Type[BaseException]],
         exception_value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
         """Release the token upon exiting the 'with' context
 
-        :param exception_type: Unused
-        :param exception_value: Unused
-        :param traceback: Unused
-        :return: None
+        Args:
+            exception_type (Optional[Type[BaseException]]): Unused
+            exception_value (Optional[BaseException]): Unused
+            traceback (Optional[TracebackType]): Unused
         """
         self.release_token()
 
     def get_token(self) -> str:
         """Get the authentication token
 
         Gets the current authentication token. If no current token exists, acquires an authentication token first.
 
-        :return: The authentication token
+        Returns:
+             The authentication token
         """
         if self.token == "":
             with self.post(
                 "/api/auth/token/acquire",
                 json={
                     "username": self.credential.username,
                     "password": self.credential.password,
@@ -114,98 +118,117 @@
                     logger.warning(
                         f"Could not acquire SuiteAPI token: {token_response}"
                     )
 
         return self.token
 
     def release_token(self) -> None:
-        """Release the authentication token, if it exists
+        """Release the authentication token, if it exists"""
 
-        :return: None
-        """
         if self.token != "":
             self.post("auth/token/release").close()
             self.token = ""
 
     def get(self, url: str, **kwargs: Any) -> Response:
         """Send a GET request to the SuiteAPI
         The 'Response' object should be used in a 'with' block or
         manually closed after use
 
-        :param url: URL to send GET request to
-        :param kwargs: Additional keyword arguments to pass to request
-        :return: The API response
+        Args:
+            url (str): URL to send GET request to
+            kwargs (Any): Additional keyword arguments to pass to request
+
+        Returns:
+            The API response
         """
         return self._request_wrapper(requests.get, url, **kwargs)
 
     def paged_get(self, url: str, key: str, **kwargs: Any) -> dict:
         """Send a GET request to the SuiteAPI that gets a paged response
 
-        :param url: URL to send GET request to
-        :param key: Json key that contains the paged data
-        :param kwargs: Additional keyword arguments to pass to request
-        :return: The API response
+        Args:
+            url (str): URL to send GET request to
+            key (str): Json key that contains the paged data
+            kwargs (Any): Additional keyword arguments to pass to request
+
+        Returns:
+             The API response
         """
         return self._paged_request(requests.get, url, key, **kwargs)
 
     def post(self, url: str, **kwargs: Any) -> Response:
         """Send a POST request to the SuiteAPI
         The 'Response' object should be used in a 'with' block or
         manually closed after use
 
-        :param url: URL to send POST request to
-        :param kwargs: Additional keyword arguments to pass to request
-        :return: The API response
+        Args:
+            url (str): URL to send POST request to
+            kwargs (Any): Additional keyword arguments to pass to request
+
+        Returns:
+             The API response
         """
         kwargs.setdefault("headers", {})
         kwargs["headers"].setdefault("Content-Type", "application/json")
         return self._request_wrapper(requests.post, url, **kwargs)
 
     def paged_post(self, url: str, key: str, **kwargs: Any) -> dict:
         """Send a POST request to the SuiteAPI that gets a paged response.
 
-        :param url: URL to send POST request to
-        :param key: Json key that contains the paged data
-        :param kwargs: Additional keyword arguments to pass to request
-        :return: The API response
+        Args:
+            url (str): URL to send POST request to
+            key (str): Json key that contains the paged data
+            kwargs (Any): Additional keyword arguments to pass to request
+
+        Returns:
+             The API response
         """
         kwargs.setdefault("headers", {})
         kwargs["headers"].setdefault("Content-Type", "application/json")
         return self._paged_request(requests.post, url, key, **kwargs)
 
     def put(self, url: str, **kwargs: Any) -> Response:
         """Send a PUT request to the SuiteAPI
         The 'Response' object should be used in a 'with' block or
         manually closed after use
 
-        :param url: URL to send PUT request to
-        :param kwargs: Additional keyword arguments to pass to request
-        :return: The API response
+        Args:
+            url (str): URL to send PUT request to
+            kwargs (Any): Additional keyword arguments to pass to request
+
+        Returns:
+             The API response
         """
         return self._request_wrapper(requests.put, url, **kwargs)
 
     def patch(self, url: str, **kwargs: Any) -> Response:
         """Send a PATCH request to the SuiteAPI
         The 'Response' object should be used in a 'with' block or
         manually closed after use
 
-        :param url: URL to send PATCH request to
-        :param kwargs: Additional keyword arguments to pass to request
-        :return: The API response
+        Args:
+            url (str): URL to send PATCH request to
+            kwargs (Any): Additional keyword arguments to pass to request
+
+        Returns:
+            The API response
         """
         return self._request_wrapper(requests.patch, url, **kwargs)
 
     def delete(self, url: str, **kwargs: Any) -> Response:
         """Send a DELETE request to the SuiteAPI
         The 'Response' object should be used in a 'with' block or
         manually closed after use
 
-        :param url: URL to send DELETE request to
-        :param kwargs: Additional keyword arguments to pass to request
-        :return: The API response
+        Args:
+            url (str): URL to send DELETE request to
+            kwargs (Any): Additional keyword arguments to pass to request
+
+        Returns:
+             The API response
         """
         return self._request_wrapper(requests.delete, url, **kwargs)
 
     def _add_paging(self, **kwargs: Any) -> dict:
         kwargs.setdefault("params", {})
         kwargs["params"].setdefault("page", 0)
         kwargs["params"].setdefault("pageSize", 1000)
@@ -224,17 +247,20 @@
         responses to SDK Objects.
 
         Note that not all information from the query is returned. For example, the
         query returns health statuses of each object, but those are not present in
         the resulting Objects. If information other than the Object itself is needed,
         you will need to call the endpoint and process the results manually.
 
-        :param query: json of the resourceQuery, as defined in the SuiteAPI docs:
-        https://[[aria-ops-hostname]]/suite-api/doc/swagger-ui.html#/Resources/getMatchingResourcesUsingPOST
-        :return list of sdk Objects representing each of the returned objects.
+        Args:
+            query (Dict[str, Any]): json of the resourceQuery, as defined in the SuiteAPI docs:
+                https://[[aria-ops-hostname]]/suite-api/doc/swagger-ui.html#/Resources/getMatchingResourcesUsingPOST
+
+        Returns:
+             list of sdk Objects representing each of the returned objects.
         """
         try:
             results = []
             if "name" in query and "regex" in query:
                 # This is behavior in the suite api itself, we're just warning about it
                 # here to avoid confusion.
                 logger.warning(
@@ -273,18 +299,21 @@
         """Send a request to the SuiteAPI that returns a paged response. Each response must have data returned in an
         array at key 'key'. The array from the responses will be combined into a single array and returned in a map of
         the form:
         {
            "{key}": [aggregated data]
         }
 
-        :param url: URL to send request to
-        :param key: Json key that contains the paged data
-        :param kwargs: Additional keyword arguments to pass to request
-        :return: The API response
+        Args:
+            url(str): URL to send request to
+            key (str): Json key that contains the paged data
+            kwargs (Any): Additional keyword arguments to pass to request
+
+        Returns:
+             The API response
         """
         kwargs = self._add_paging(**kwargs)
         with self._request_wrapper(request_func, url, **kwargs) as page_0:
             if page_0.status_code < 300:
                 page_0_body = json.loads(page_0.text)
             else:
                 # _request_wrapper will log the error
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/aria/ops/timer.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/aria/ops/timer.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/PKG-INFO` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/vmware_aria_operations_integration_sdk_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-aria-operations-integration-sdk-lib
-Version: 0.7.3
+Version: 0.7.4
 Summary: Object model for interacting with the VMware Aria Operations Containerized API
 Home-page: https://github.com/vmware/vmware-aria-operations-integration-sdk
 Author: VMware, Inc.
 Author-email: krokos@vmware.com
 Project-URL: Bug Tracker, https://github.com/vmware/vmware-aria-operations-integration-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/src/vmware_aria_operations_integration_sdk_lib.egg-info/SOURCES.txt` & `vmware-aria-operations-integration-sdk-lib-0.7.4/src/vmware_aria_operations_integration_sdk_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/tests/test_collect_result.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/tests/test_collect_result.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/tests/test_object_key.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/tests/test_object_key.py`

 * *Files identical despite different names*

### Comparing `vmware-aria-operations-integration-sdk-lib-0.7.3/tests/test_result.py` & `vmware-aria-operations-integration-sdk-lib-0.7.4/tests/test_result.py`

 * *Files identical despite different names*

