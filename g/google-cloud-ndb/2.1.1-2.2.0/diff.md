# Comparing `tmp/google-cloud-ndb-2.1.1.tar.gz` & `tmp/google-cloud-ndb-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-ndb-2.1.1.tar", last modified: Wed Mar 15 17:41:48 2023, max compression
+gzip compressed data, was "google-cloud-ndb-2.2.0.tar", last modified: Wed Jul 26 16:33:29 2023, max compression
```

## Comparing `google-cloud-ndb-2.1.1.tar` & `google-cloud-ndb-2.2.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-15 17:41:48.164897 google-cloud-ndb-2.1.1/
--rw-rw-r--   0 root         (0)     1003      370 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/AUTHORS
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/LICENSE
--rw-r--r--   0 root         (0)     1003     2400 2023-03-15 17:41:48.164897 google-cloud-ndb-2.1.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     1279 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/README.md
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-15 17:41:48.156896 google-cloud-ndb-2.1.1/google/
--rw-rw-r--   0 root         (0)     1003      748 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-15 17:41:48.160897 google-cloud-ndb-2.1.1/google/cloud/
--rw-rw-r--   0 root         (0)     1003      748 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-15 17:41:48.164897 google-cloud-ndb-2.1.1/google/cloud/ndb/
--rw-rw-r--   0 root         (0)     1003     8239 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/__init__.py
--rw-rw-r--   0 root         (0)     1003     2208 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/_batch.py
--rw-rw-r--   0 root         (0)     1003    23276 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/_cache.py
--rw-rw-r--   0 root         (0)     1003    38957 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/_datastore_api.py
--rw-rw-r--   0 root         (0)     1003    35353 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/_datastore_query.py
--rw-rw-r--   0 root         (0)     1003     2850 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/_datastore_types.py
--rw-rw-r--   0 root         (0)     1003    14996 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/_eventloop.py
--rw-rw-r--   0 root         (0)     1003    28421 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/_gql.py
--rw-rw-r--   0 root         (0)     1003    19538 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/_legacy_entity_pb.py
--rw-rw-r--   0 root         (0)     1003     5557 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/_legacy_protocol_buffer.py
--rw-rw-r--   0 root         (0)     1003     7728 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/_options.py
--rw-rw-r--   0 root         (0)     1003     2814 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/_remote.py
--rw-rw-r--   0 root         (0)     1003     5562 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/_retry.py
--rw-rw-r--   0 root         (0)     1003    17072 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/_transaction.py
--rw-rw-r--   0 root         (0)     1003     4382 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/blobstore.py
--rw-rw-r--   0 root         (0)     1003     9126 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/client.py
--rw-rw-r--   0 root         (0)     1003    23154 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/context.py
--rw-rw-r--   0 root         (0)     1003      993 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/django_middleware.py
--rw-rw-r--   0 root         (0)     1003     4045 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/exceptions.py
--rw-rw-r--   0 root         (0)     1003    27391 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/global_cache.py
--rw-rw-r--   0 root         (0)     1003    55949 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/key.py
--rw-rw-r--   0 root         (0)     1003    10973 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/metadata.py
--rw-rw-r--   0 root         (0)     1003   242140 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/model.py
--rw-rw-r--   0 root         (0)     1003      938 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/msgprop.py
--rw-rw-r--   0 root         (0)     1003     9157 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/polymodel.py
--rw-rw-r--   0 root         (0)     1003    85835 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/query.py
--rw-rw-r--   0 root         (0)     1003    15713 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/stats.py
--rw-rw-r--   0 root         (0)     1003    21299 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/tasklets.py
--rw-rw-r--   0 root         (0)     1003     4938 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/google/cloud/ndb/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-15 17:41:48.164897 google-cloud-ndb-2.1.1/google_cloud_ndb.egg-info/
--rw-r--r--   0 root         (0)     1003     2400 2023-03-15 17:41:48.000000 google-cloud-ndb-2.1.1/google_cloud_ndb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1243 2023-03-15 17:41:48.000000 google-cloud-ndb-2.1.1/google_cloud_ndb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-15 17:41:48.000000 google-cloud-ndb-2.1.1/google_cloud_ndb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-15 17:41:48.000000 google-cloud-ndb-2.1.1/google_cloud_ndb.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-15 17:41:48.000000 google-cloud-ndb-2.1.1/google_cloud_ndb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      332 2023-03-15 17:41:48.000000 google-cloud-ndb-2.1.1/google_cloud_ndb.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-15 17:41:48.000000 google-cloud-ndb-2.1.1/google_cloud_ndb.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-03-15 17:41:48.164897 google-cloud-ndb-2.1.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2898 2023-03-15 17:39:07.000000 google-cloud-ndb-2.1.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-26 16:33:29.116542 google-cloud-ndb-2.2.0/
+-rw-rw-r--   0 root         (0)     1003      370 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/AUTHORS
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/LICENSE
+-rw-r--r--   0 root         (0)     1003     2400 2023-07-26 16:33:29.112542 google-cloud-ndb-2.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     1279 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/README.md
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-26 16:33:29.104541 google-cloud-ndb-2.2.0/google/
+-rw-rw-r--   0 root         (0)     1003      748 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-26 16:33:29.108541 google-cloud-ndb-2.2.0/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      748 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-26 16:33:29.112542 google-cloud-ndb-2.2.0/google/cloud/ndb/
+-rw-rw-r--   0 root         (0)     1003     8239 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2208 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/_batch.py
+-rw-rw-r--   0 root         (0)     1003    23276 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/_cache.py
+-rw-rw-r--   0 root         (0)     1003    41403 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/_datastore_api.py
+-rw-rw-r--   0 root         (0)     1003    35515 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/_datastore_query.py
+-rw-rw-r--   0 root         (0)     1003     2850 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/_datastore_types.py
+-rw-rw-r--   0 root         (0)     1003    14996 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/_eventloop.py
+-rw-rw-r--   0 root         (0)     1003    28515 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/_gql.py
+-rw-rw-r--   0 root         (0)     1003    19538 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/_legacy_entity_pb.py
+-rw-rw-r--   0 root         (0)     1003     5557 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/_legacy_protocol_buffer.py
+-rw-rw-r--   0 root         (0)     1003     7728 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/_options.py
+-rw-rw-r--   0 root         (0)     1003     2814 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/_remote.py
+-rw-rw-r--   0 root         (0)     1003     5562 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/_retry.py
+-rw-rw-r--   0 root         (0)     1003    17072 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/_transaction.py
+-rw-rw-r--   0 root         (0)     1003     4382 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/blobstore.py
+-rw-rw-r--   0 root         (0)     1003     9401 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/client.py
+-rw-rw-r--   0 root         (0)     1003    23154 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/context.py
+-rw-rw-r--   0 root         (0)     1003      993 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/django_middleware.py
+-rw-rw-r--   0 root         (0)     1003     4045 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/exceptions.py
+-rw-rw-r--   0 root         (0)     1003    27391 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/global_cache.py
+-rw-rw-r--   0 root         (0)     1003    59314 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/key.py
+-rw-rw-r--   0 root         (0)     1003    10973 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/metadata.py
+-rw-rw-r--   0 root         (0)     1003   242646 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/model.py
+-rw-rw-r--   0 root         (0)     1003      938 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/msgprop.py
+-rw-rw-r--   0 root         (0)     1003     9157 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/polymodel.py
+-rw-rw-r--   0 root         (0)     1003    86296 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/query.py
+-rw-rw-r--   0 root         (0)     1003    15713 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/stats.py
+-rw-rw-r--   0 root         (0)     1003    21299 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/tasklets.py
+-rw-rw-r--   0 root         (0)     1003     4938 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/google/cloud/ndb/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-26 16:33:29.112542 google-cloud-ndb-2.2.0/google_cloud_ndb.egg-info/
+-rw-r--r--   0 root         (0)     1003     2400 2023-07-26 16:33:29.000000 google-cloud-ndb-2.2.0/google_cloud_ndb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1243 2023-07-26 16:33:29.000000 google-cloud-ndb-2.2.0/google_cloud_ndb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-26 16:33:29.000000 google-cloud-ndb-2.2.0/google_cloud_ndb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-26 16:33:29.000000 google-cloud-ndb-2.2.0/google_cloud_ndb.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-26 16:33:29.000000 google-cloud-ndb-2.2.0/google_cloud_ndb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      333 2023-07-26 16:33:29.000000 google-cloud-ndb-2.2.0/google_cloud_ndb.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-26 16:33:29.000000 google-cloud-ndb-2.2.0/google_cloud_ndb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-07-26 16:33:29.116542 google-cloud-ndb-2.2.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2900 2023-07-26 16:30:52.000000 google-cloud-ndb-2.2.0/setup.py
```

### Comparing `google-cloud-ndb-2.1.1/LICENSE` & `google-cloud-ndb-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/PKG-INFO` & `google-cloud-ndb-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-ndb
-Version: 2.1.1
+Version: 2.2.0
 Summary: NDB library for Google Cloud Datastore
 Home-page: https://github.com/googleapis/python-ndb
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Project-URL: Documentation, https://googleapis.dev/python/python-ndb/latest
 Project-URL: Issue Tracker, https://github.com/googleapis/python-ndb/issues
```

### Comparing `google-cloud-ndb-2.1.1/README.md` & `google-cloud-ndb-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/__init__.py` & `google-cloud-ndb-2.2.0/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/__init__.py` & `google-cloud-ndb-2.2.0/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/__init__.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/_batch.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/_batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/_cache.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/_cache.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/_datastore_api.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/_datastore_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 """Functions that interact with Datastore backend."""
 
 import grpc
 import itertools
 import logging
 
 from google.api_core import exceptions as core_exceptions
+from google.api_core import gapic_v1
 from google.cloud.datastore import helpers
 from google.cloud.datastore_v1.types import datastore as datastore_pb2
 from google.cloud.datastore_v1.types import entity as entity_pb2
 
 from google.cloud.ndb import context as context_module
 from google.cloud.ndb import _batch
 from google.cloud.ndb import _cache
@@ -52,26 +53,28 @@
         :class:`~google.cloud.datastore_v1.proto.datastore_pb2_grpc.DatastoreStub`:
             The stub instance.
     """
     context = context_module.get_context()
     return context.client.stub
 
 
-def make_call(rpc_name, request, retries=None, timeout=None):
+def make_call(rpc_name, request, retries=None, timeout=None, metadata=()):
     """Make a call to the Datastore API.
 
     Args:
         rpc_name (str): Name of the remote procedure to call on Datastore.
         request (Any): An appropriate request object for the call, eg,
             `entity_pb2.LookupRequest` for calling ``Lookup``.
         retries (int): Number of times to potentially retry the call. If
             :data:`None` is passed, will use :data:`_retry._DEFAULT_RETRIES`.
             If :data:`0` is passed, the call is attempted only once.
         timeout (float): Timeout, in seconds, to pass to gRPC call. If
             :data:`None` is passed, will use :data:`_DEFAULT_TIMEOUT`.
+        metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
 
     Returns:
         tasklets.Future: Future for the eventual response for the API call.
     """
     api = stub()
     method = getattr(api, rpc_name)
 
@@ -81,15 +84,15 @@
     if timeout is None:
         timeout = _DEFAULT_TIMEOUT
 
     @tasklets.tasklet
     def rpc_call():
         context = context_module.get_toplevel_context()
 
-        call = method.future(request, timeout=timeout)
+        call = method.future(request, timeout=timeout, metadata=metadata)
         rpc = _remote.RemoteCall(call, rpc_name)
         utils.logging_debug(log, rpc)
         utils.logging_debug(log, "timeout={}", timeout)
         utils.logging_debug(log, request)
 
         try:
             result = yield rpc
@@ -278,39 +281,45 @@
         for result in results.found:
             entity = result.entity
             todo_key = entity.key._pb.SerializeToString()
             for future in self.todo[todo_key]:
                 future.set_result(entity)
 
 
-def _datastore_lookup(keys, read_options, retries=None, timeout=None):
+def _datastore_lookup(keys, read_options, retries=None, timeout=None, metadata=()):
     """Issue a Lookup call to Datastore using gRPC.
 
     Args:
         keys (Iterable[entity_pb2.Key]): The entity keys to
             look up.
         read_options (Union[datastore_pb2.ReadOptions, NoneType]): Options for
             the request.
         retries (int): Number of times to potentially retry the call. If
             :data:`None` is passed, will use :data:`_retry._DEFAULT_RETRIES`.
             If :data:`0` is passed, the call is attempted only once.
         timeout (float): Timeout, in seconds, to pass to gRPC call. If
             :data:`None` is passed, will use :data:`_DEFAULT_TIMEOUT`.
+        metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
 
     Returns:
         tasklets.Future: Future object for eventual result of lookup.
     """
     client = context_module.get_context().client
     request = datastore_pb2.LookupRequest(
         project_id=client.project,
+        database_id=client.database,
         keys=[key for key in keys],
         read_options=read_options,
     )
+    metadata = _add_routing_info(metadata, request)
 
-    return make_call("lookup", request, retries=retries, timeout=timeout)
+    return make_call(
+        "lookup", request, retries=retries, timeout=timeout, metadata=metadata
+    )
 
 
 def get_read_options(options, default_read_consistency=None):
     """Get the read options for a request.
 
     Args:
         options (_options.ReadOptions): The options for the request. May
@@ -839,47 +848,53 @@
         element = key_pb.path[-1]
         if element.id or element.name:
             return True
 
     return False
 
 
-def _datastore_commit(mutations, transaction, retries=None, timeout=None):
+def _datastore_commit(mutations, transaction, retries=None, timeout=None, metadata=()):
     """Call Commit on Datastore.
 
     Args:
         mutations (List[datastore_pb2.Mutation]): The changes to persist to
             Datastore.
         transaction (Union[bytes, NoneType]): The identifier for the
             transaction for this commit, or :data:`None` if no transaction is
             being used.
         retries (int): Number of times to potentially retry the call. If
             :data:`None` is passed, will use :data:`_retry._DEFAULT_RETRIES`.
             If :data:`0` is passed, the call is attempted only once.
         timeout (float): Timeout, in seconds, to pass to gRPC call. If
             :data:`None` is passed, will use :data:`_DEFAULT_TIMEOUT`.
+        metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
 
     Returns:
         tasklets.Tasklet: A future for
             :class:`google.cloud.datastore_v1.datastore_pb2.CommitResponse`
     """
     if transaction is None:
         mode = datastore_pb2.CommitRequest.Mode.NON_TRANSACTIONAL
     else:
         mode = datastore_pb2.CommitRequest.Mode.TRANSACTIONAL
 
     client = context_module.get_context().client
     request = datastore_pb2.CommitRequest(
         project_id=client.project,
+        database_id=client.database,
         mode=mode,
         mutations=mutations,
         transaction=transaction,
     )
+    metadata = _add_routing_info(metadata, request)
 
-    return make_call("commit", request, retries=retries, timeout=timeout)
+    return make_call(
+        "commit", request, retries=retries, timeout=timeout, metadata=metadata
+    )
 
 
 def allocate(keys, options):
     """Allocate ids for incomplete keys.
 
     Args:
         key (key.Key): The incomplete key.
@@ -969,34 +984,41 @@
                 future.set_exception(exception)
             return
 
         for key, future in zip(rpc.result().keys, self.futures):
             future.set_result(key)
 
 
-def _datastore_allocate_ids(keys, retries=None, timeout=None):
+def _datastore_allocate_ids(keys, retries=None, timeout=None, metadata=()):
     """Calls ``AllocateIds`` on Datastore.
 
     Args:
         keys (List[google.cloud.datastore_v1.entity_pb2.Key]): List of
             incomplete keys to allocate.
         retries (int): Number of times to potentially retry the call. If
             :data:`None` is passed, will use :data:`_retry._DEFAULT_RETRIES`.
             If :data:`0` is passed, the call is attempted only once.
         timeout (float): Timeout, in seconds, to pass to gRPC call. If
             :data:`None` is passed, will use :data:`_DEFAULT_TIMEOUT`.
+        metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
 
     Returns:
         tasklets.Future: A future for
             :class:`google.cloud.datastore_v1.datastore_pb2.AllocateIdsResponse`
     """
     client = context_module.get_context().client
-    request = datastore_pb2.AllocateIdsRequest(project_id=client.project, keys=keys)
+    request = datastore_pb2.AllocateIdsRequest(
+        project_id=client.project, database_id=client.database, keys=keys
+    )
+    metadata = _add_routing_info(metadata, request)
 
-    return make_call("allocate_ids", request, retries=retries, timeout=timeout)
+    return make_call(
+        "allocate_ids", request, retries=retries, timeout=timeout, metadata=metadata
+    )
 
 
 @tasklets.tasklet
 def begin_transaction(read_only, retries=None, timeout=None):
     """Start a new transaction.
 
     Args:
@@ -1014,25 +1036,27 @@
     """
     response = yield _datastore_begin_transaction(
         read_only, retries=retries, timeout=timeout
     )
     raise tasklets.Return(response.transaction)
 
 
-def _datastore_begin_transaction(read_only, retries=None, timeout=None):
+def _datastore_begin_transaction(read_only, retries=None, timeout=None, metadata=()):
     """Calls ``BeginTransaction`` on Datastore.
 
     Args:
         read_only (bool): Whether to start a read-only or read-write
             transaction.
         retries (int): Number of times to potentially retry the call. If
             :data:`None` is passed, will use :data:`_retry._DEFAULT_RETRIES`.
             If :data:`0` is passed, the call is attempted only once.
         timeout (float): Timeout, in seconds, to pass to gRPC call. If
             :data:`None` is passed, will use :data:`_DEFAULT_TIMEOUT`.
+        metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
 
     Returns:
         tasklets.Tasklet: A future for
             :class:`google.cloud.datastore_v1.datastore_pb2.BeginTransactionResponse`
     """
     client = context_module.get_context().client
     if read_only:
@@ -1041,18 +1065,27 @@
         )
     else:
         options = datastore_pb2.TransactionOptions(
             read_write=datastore_pb2.TransactionOptions.ReadWrite()
         )
 
     request = datastore_pb2.BeginTransactionRequest(
-        project_id=client.project, transaction_options=options
+        project_id=client.project,
+        database_id=client.database,
+        transaction_options=options,
     )
+    metadata = _add_routing_info(metadata, request)
 
-    return make_call("begin_transaction", request, retries=retries, timeout=timeout)
+    return make_call(
+        "begin_transaction",
+        request,
+        retries=retries,
+        timeout=timeout,
+        metadata=metadata,
+    )
 
 
 @tasklets.tasklet
 def rollback(transaction, retries=None, timeout=None):
     """Rollback a transaction.
 
     Args:
@@ -1065,28 +1098,64 @@
 
     Returns:
         tasklets.Future: Future completes when rollback is finished.
     """
     yield _datastore_rollback(transaction, retries=retries, timeout=timeout)
 
 
-def _datastore_rollback(transaction, retries=None, timeout=None):
+def _datastore_rollback(transaction, retries=None, timeout=None, metadata=()):
     """Calls Rollback in Datastore.
 
     Args:
         transaction (bytes): Transaction id.
         retries (int): Number of times to potentially retry the call. If
             :data:`None` is passed, will use :data:`_retry._DEFAULT_RETRIES`.
             If :data:`0` is passed, the call is attempted only once.
         timeout (float): Timeout, in seconds, to pass to gRPC call. If
             :data:`None` is passed, will use :data:`_DEFAULT_TIMEOUT`.
+        metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
 
     Returns:
         tasklets.Tasklet: Future for
             :class:`google.cloud.datastore_v1.datastore_pb2.RollbackResponse`
     """
     client = context_module.get_context().client
     request = datastore_pb2.RollbackRequest(
-        project_id=client.project, transaction=transaction
+        project_id=client.project,
+        database_id=client.database,
+        transaction=transaction,
+    )
+    metadata = _add_routing_info(metadata, request)
+
+    return make_call(
+        "rollback", request, retries=retries, timeout=timeout, metadata=metadata
     )
 
-    return make_call("rollback", request, retries=retries, timeout=timeout)
+
+def _add_routing_info(metadata, request):
+    """Adds routing header info to the given metadata.
+
+    Args:
+        metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata. Not modified.
+        request (Any): An appropriate request object for the call, eg,
+            `entity_pb2.LookupRequest` for calling ``Lookup``.
+
+    Returns:
+        Sequence[Tuple[str, str]]: Sequence with routing info added,
+            if it is included in the request.
+    """
+    header_params = {}
+
+    if request.project_id:
+        header_params["project_id"] = request.project_id
+
+    if request.database_id:
+        header_params["database_id"] = request.database_id
+
+    if header_params:
+        return tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata(header_params),
+        )
+
+    return tuple(metadata)
```

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/_datastore_query.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/_datastore_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1006,25 +1006,30 @@
         query (query.QueryOptions): The query spec.
 
     Returns:
         tasklets.Future:
     """
     query_pb = _query_to_protobuf(query)
     partition_id = entity_pb2.PartitionId(
-        project_id=query.project, namespace_id=query.namespace
+        project_id=query.project,
+        database_id=query.database,
+        namespace_id=query.namespace,
     )
     read_options = _datastore_api.get_read_options(query)
     request = datastore_pb2.RunQueryRequest(
         project_id=query.project,
+        database_id=query.database,
         partition_id=partition_id,
         query=query_pb,
         read_options=read_options,
     )
+    metadata = _datastore_api._add_routing_info((), request)
+
     response = yield _datastore_api.make_call(
-        "run_query", request, timeout=query.timeout
+        "run_query", request, timeout=query.timeout, metadata=metadata
     )
     utils.logging_debug(log, response)
     raise tasklets.Return(response)
 
 
 class Cursor(object):
     """Cursor.
```

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/_datastore_types.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/_datastore_types.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/_eventloop.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/_eventloop.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/_gql.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/_gql.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,15 @@
     _hint = ""
 
     def __init__(self, query_string, _app=None, _auth_domain=None, namespace=None):
         """Parses the input query into the class as a pre-compiled query.
 
         Args:
             query_string (str): properly formatted GQL query string.
-            namespace (str): the namespace to use for this query.
-
+            namespace (str): The namespace to use for this query. Defaults to the client's value.
         Raises:
             exceptions.BadQueryError: if the query is not parsable.
         """
         self._app = _app
 
         self._namespace = namespace
 
@@ -849,15 +848,18 @@
 
 
 def _key_function(values):
     if not len(values) % 2:
         context = context_module.get_context()
         client = context.client
         return key.Key(
-            *values, namespace=context.get_namespace(), project=client.project
+            *values,
+            project=client.project,
+            database=client.database,
+            namespace=context.get_namespace(),
         )
     _raise_cast_error(
         "Key requires even number of operands or single string, {}".format(values)
     )
 
 
 FUNCTIONS = {
```

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/_legacy_entity_pb.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/_legacy_entity_pb.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/_legacy_protocol_buffer.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/_legacy_protocol_buffer.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/_options.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/_options.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/_remote.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/_remote.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/_retry.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/_retry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/_transaction.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/_transaction.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/blobstore.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/blobstore.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/client.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""A client for NDB which manages credentials, project, namespace."""
+"""A client for NDB which manages credentials, project, namespace, and database."""
 
 import contextlib
 import grpc
 import os
 import requests
 
 import google.api_core.client_options
@@ -88,25 +88,33 @@
         namespace (Optional[str]): Namespace to pass to proxied API methods.
         credentials (Optional[:class:`~google.auth.credentials.Credentials`]):
             The OAuth2 Credentials to use for this client. If not passed, falls
             back to the default inferred from the environment.
         client_options (Optional[:class:`~google.api_core.client_options.ClientOptions` or :class:`dict`])
             Client options used to set user options on the client.
             API Endpoint should be set through client_options.
+        database (Optional[str]): Database to access. Defaults to the (default) database.
     """
 
     SCOPE = ("https://www.googleapis.com/auth/datastore",)
     """The scopes required for authenticating as a Cloud Datastore consumer."""
 
     def __init__(
-        self, project=None, namespace=None, credentials=None, client_options=None
+        self,
+        project=None,
+        namespace=None,
+        credentials=None,
+        client_options=None,
+        database=None,
     ):
         self.namespace = namespace
+        self.host = os.environ.get(environment_vars.GCD_HOST, DATASTORE_API_HOST)
         self.client_info = _CLIENT_INFO
         self._client_options = client_options
+        self.database = database
 
         # Use insecure connection when using Datastore Emulator, otherwise
         # use secure connection
         emulator = bool(os.environ.get(environment_vars.GCD_HOST))
         self.secure = not emulator
 
         # Use Datastore API host from client_options if provided, otherwise use default
```

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/context.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/context.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/django_middleware.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/django_middleware.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/exceptions.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/global_cache.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/global_cache.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/key.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/key.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,20 +20,26 @@
 
 A key encapsulates the following pieces of information, which together
 uniquely designate a (possible) entity in Google Cloud Datastore:
 
 * a Google Cloud Platform project (a string)
 * a list of one or more ``(kind, id)`` pairs where ``kind`` is a string
   and ``id`` is either a string or an integer
+* an optional database (a string)
 * an optional namespace (a string)
 
 The application ID must always be part of the key, but since most
 applications can only access their own entities, it defaults to the
 current application ID and you rarely need to worry about it.
 
+The database is an optional database ID. If unspecified, it defaults
+to that of the client.
+For usage in Cloud NDB, the default database should always be referred
+to as an empty string; please do not use "(default)".
+
 The namespace designates a top-level partition of the key space for a
 particular application. If you've never heard of namespaces, you can
 safely ignore this feature.
 
 Most of the action is in the ``(kind, id)`` pairs. A key must have at
 least one ``(kind, id)`` pair. The last ``(kind, id)`` pair gives the kind
 and the ID of the entity that the key refers to, the others merely
@@ -91,22 +97,22 @@
 import google.cloud.datastore
 
 from google.cloud.ndb import exceptions
 from google.cloud.ndb import _options
 from google.cloud.ndb import tasklets
 from google.cloud.ndb import utils
 
-
 __all__ = ["Key", "UNDEFINED"]
 _APP_ID_ENVIRONMENT = "APPLICATION_ID"
 _APP_ID_DEFAULT = "_"
 _WRONG_TYPE = "Cannot construct Key reference on non-Key class; received {!r}"
 _REFERENCE_APP_MISMATCH = (
     "Key reference constructed uses a different app {!r} than the one specified {!r}"
 )
+_REFERENCE_DATABASE_MISMATCH = "Key reference constructed uses a different database {!r} than the one specified {!r}"
 _REFERENCE_NAMESPACE_MISMATCH = (
     "Key reference constructed uses a different namespace {!r} than "
     "the one specified {!r}"
 )
 _INVALID_ID_TYPE = "Key ID must be a string or a number; received {!r}"
 _NO_LEGACY = "The `google.appengine.ext.db` module is not available."
 _MAX_INTEGER_ID = 0x7FFFFFFFFFFFFFFF  # 2 ** 63 - 1
@@ -116,17 +122,17 @@
 _BAD_STRING_ID = (
     "Key name strings must be non-empty strings up to {:d} bytes; received {}"
 )
 
 UNDEFINED = object()
 """Sentinel value.
 
-Used to indicate a namespace hasn't been explicitly set in key construction.
+Used to indicate a database or namespace hasn't been explicitly set in key construction.
 Used to distinguish between not passing a value and passing `None`, which
-indicates the default namespace.
+indicates the default database/namespace.
 """
 
 
 class Key(object):
     """An immutable datastore key.
 
     For flexibility and convenience, multiple constructor signatures are
@@ -136,17 +142,18 @@
 
     .. testsetup:: *
 
         from unittest import mock
         from google.cloud.ndb import context as context_module
         client = mock.Mock(
             project="testing",
+            database=None,
             namespace=None,
             stub=mock.Mock(spec=()),
-            spec=("project", "namespace", "stub"),
+            spec=("project", "database", "namespace", "stub"),
         )
         context = context_module.Context(client).use()
         context.__enter__()
         kind1, id1 = "Parent", "C"
         kind2, id2 = "Child", 42
 
     .. testcleanup:: *
@@ -265,14 +272,17 @@
         project (Optional[str]): The Google Cloud Platform project (previously
             on Google App Engine, this was called the Application ID).
         app (Optional[str]): DEPRECATED: Synonym for ``project``.
         namespace (Optional[str]): The namespace for the key.
         parent (Optional[Key]): The parent of the key being
             constructed. If provided, the key path will be **relative** to the
             parent key's path.
+        database (Optional[str]): The database to use.
+            Defaults to that of the client if a parent was specified, and
+            to the default database if it was not.
 
     Raises:
         TypeError: If none of ``reference``, ``serialized``, ``urlsafe``,
             ``pairs`` or ``flat`` is provided as an argument and no positional
             arguments were given with the path.
     """
 
@@ -313,63 +323,66 @@
         key._reference = None
         return key
 
     def __repr__(self):
         """String representation used by :class:`str() <str>` and :func:`repr`.
 
         We produce a short string that conveys all relevant information,
-        suppressing project and namespace when they are equal to the default.
-        In many cases, this string should be able to be used to invoke the
-        constructor.
+        suppressing project, database, and namespace when they are equal to their
+        respective defaults.
+
+        In many cases, this string should be able to be used to invoke the constructor.
 
         For example:
 
         .. doctest:: key-repr
 
             >>> key = ndb.Key("hi", 100)
             >>> repr(key)
             "Key('hi', 100)"
             >>>
             >>> key = ndb.Key(
-            ...     "bye", "hundred", project="specific", namespace="space"
+            ...     "bye", "hundred", project="specific", database="db", namespace="space",
             ... )
             >>> str(key)
-            "Key('bye', 'hundred', project='specific', namespace='space')"
+            "Key('bye', 'hundred', project='specific', database='db', namespace='space')"
         """
         args = ["{!r}".format(item) for item in self.flat()]
         if self.project() != _project_from_app(None):
             args.append("project={!r}".format(self.app()))
+        if self.database():
+            args.append("database={!r}".format(self.database()))
         if self.namespace() is not None:
             args.append("namespace={!r}".format(self.namespace()))
 
         return "Key({})".format(", ".join(args))
 
     def __str__(self):
         """Alias for :meth:`__repr__`."""
         return self.__repr__()
 
     def __hash__(self):
         """Hash value, for use in dictionary lookups.
 
         .. note::
 
-            This ignores ``app`` and ``namespace``. Since :func:`hash` isn't
+            This ignores ``app``, ``database``, and ``namespace``. Since :func:`hash` isn't
             expected to return a unique value (it just reduces the chance of
             collision), this doesn't try to increase entropy by including other
             values. The primary concern is that hashes of equal keys are
             equal, not the other way around.
         """
         hash_value = self._hash_value
         if hash_value is None:
             self._hash_value = hash_value = hash(self.pairs())
         return hash_value
 
     def _tuple(self):
         """Helper to return an orderable tuple."""
-        return (self.app(), self.namespace(), self.pairs())
+        return (self.app(), self.namespace(), self.database() or "", self.pairs())
 
     def __eq__(self, other):
         """Equality comparison operation."""
         if not isinstance(other, Key):
             return NotImplemented
 
         return self._tuple() == other._tuple()
@@ -405,33 +418,36 @@
         return not self < other
 
     def __getstate__(self):
         """Private API used for pickling.
 
         Returns:
             Tuple[Dict[str, Any]]: A tuple containing a single dictionary of
-            state to pickle. The dictionary has three keys ``pairs``, ``app``
-            and ``namespace``.
+            state to pickle. The dictionary has four keys: ``pairs``, ``app``,
+            ``database``, and ``namespace``.
         """
-        return (
+        to_pickle = (
             {
                 "pairs": self.pairs(),
                 "app": self.app(),
                 "namespace": self.namespace(),
             },
         )
+        if self.database():
+            to_pickle[0]["database"] = self.database()
+        return to_pickle
 
     def __setstate__(self, state):
         """Private API used for unpickling.
 
         Args:
             state (Tuple[Dict[str, Any]]): A tuple containing a single
                 dictionary of pickled state. This should match the signature
                 returned from :func:`__getstate__`, in particular, it should
-                have three keys ``pairs``, ``app`` and ``namespace``.
+                have four keys: ``pairs``, ``app``, ``database``, and ``namespace``.
 
         Raises:
             TypeError: If the ``state`` does not have length 1.
             TypeError: If the single element in ``state`` is not a dictionary.
         """
         if len(state) != 1:
             msg = "Invalid state length, expected 1; received {:d}".format(len(state))
@@ -443,37 +459,46 @@
                 "Key accepts a dict of keyword arguments as state; "
                 "received {!r}".format(kwargs)
             )
 
         flat = _get_path(None, kwargs["pairs"])
         _clean_flat_path(flat)
         project = _project_from_app(kwargs["app"])
+
+        database = None
+        if "database" in kwargs:
+            database = kwargs["database"]
+
         self._key = _key_module.Key(
-            *flat, project=project, namespace=kwargs["namespace"]
+            *flat,
+            project=project,
+            namespace=kwargs["namespace"],
+            database=database,
         )
         self._reference = None
 
     def __getnewargs__(self):
         """Private API used to specify ``__new__`` arguments when unpickling.
 
         .. note::
 
             This method is provided for backwards compatibility, though it
             isn't needed.
 
         Returns:
             Tuple[Dict[str, Any]]: A tuple containing a single dictionary of
-            state to pickle. The dictionary has three keys ``pairs``, ``app``
-            and ``namespace``.
+            state to pickle. The dictionary has four keys: ``pairs``, ``app``,
+            ``database`` and ``namespace``.
         """
         return (
             {
                 "pairs": self.pairs(),
                 "app": self.app(),
                 "namespace": self.namespace(),
+                "database": self.database() if self.database() is not None else None,
             },
         )
 
     def parent(self):
         """Parent key constructed from all but the last ``(kind, id)`` pairs.
 
         If there is only one ``(kind, id)`` pair, return :data:`None`.
@@ -561,14 +586,25 @@
             >>> key.project()
             'example'
         """
         return self._key.project
 
     app = project
 
+    def database(self):
+        """The database ID for the key.
+
+        .. doctest:: key-database
+
+           >>> key = ndb.Key("A", "B", database="mydb")
+           >>> key.database()
+           'mydb'
+        """
+        return self._key.database
+
     def id(self):
         """The string or integer ID in the last ``(kind, id)`` pair, if any.
 
         .. doctest:: key-id
 
             >>> key_int = ndb.Key("A", 37)
             >>> key_int.id()
@@ -674,42 +710,51 @@
         """The ``Reference`` protobuf object for this key.
 
         The return value will be stored on the current key, so the caller
         promises not to mutate it.
 
         .. doctest:: key-reference
 
-            >>> key = ndb.Key("Trampoline", 88, project="xy", namespace="zt")
+            >>> key = ndb.Key("Trampoline", 88, project="xy", database="wv", namespace="zt")
             >>> key.reference()
             app: "xy"
             name_space: "zt"
             path {
               element {
                 type: "Trampoline"
                 id: 88
               }
             }
+            database_id: "wv"
             <BLANKLINE>
         """
         if self._reference is None:
-            self._reference = _app_engine_key_pb2.Reference(
-                app=self._key.project,
-                path=_to_legacy_path(self._key.path),
-                name_space=self._key.namespace,
-            )
+            if self._key.database:
+                self._reference = _app_engine_key_pb2.Reference(
+                    app=self._key.project,
+                    path=_to_legacy_path(self._key.path),
+                    database_id=self._key.database,
+                    name_space=self._key.namespace,
+                )
+            else:
+                self._reference = _app_engine_key_pb2.Reference(
+                    app=self._key.project,
+                    path=_to_legacy_path(self._key.path),
+                    name_space=self._key.namespace,
+                )
         return self._reference
 
     def serialized(self):
         """A ``Reference`` protobuf serialized to bytes.
 
         .. doctest:: key-serialized
 
-            >>> key = ndb.Key("Kind", 1337, project="example")
+            >>> key = ndb.Key("Kind", 1337, project="example", database="example-db")
             >>> key.serialized()
-            b'j\\x07exampler\\x0b\\x0b\\x12\\x04Kind\\x18\\xb9\\n\\x0c'
+            b'j\\x07exampler\\x0b\\x0b\\x12\\x04Kind\\x18\\xb9\\n\\x0c\\xba\\x01\\nexample-db'
         """
         reference = self.reference()
         return reference.SerializeToString()
 
     def urlsafe(self):
         """A ``Reference`` protobuf serialized and encoded as urlsafe base 64.
 
@@ -726,29 +771,34 @@
         """
         A urlsafe serialized ``Reference`` protobuf with an App Engine prefix.
 
         This will produce a urlsafe string which includes an App Engine
         location prefix ("partition"), compatible with the Google Datastore
         admin console.
 
+        This only supports the default database. For a named database,
+        please use urlsafe() instead.
+
         Arguments:
             location_prefix (str): A location prefix ("partition") to be
                 prepended to the key's `project` when serializing the key. A
                 typical value is "s~", but "e~" or other partitions are
                 possible depending on the project's region and other factors.
 
         .. doctest:: key-legacy-urlsafe
 
             >>> key = ndb.Key("Kind", 1337, project="example")
             >>> key.to_legacy_urlsafe("s~")
             b'aglzfmV4YW1wbGVyCwsSBEtpbmQYuQoM'
         """
+        if self._key.database:
+            raise ValueError("to_legacy_urlsafe only supports the default database")
         return google.cloud.datastore.Key(
             *self.flat(),
-            **{"namespace": self._key.namespace, "project": self._key.project}
+            **{"namespace": self._key.namespace, "project": self._key.project},
         ).to_legacy_urlsafe(location_prefix=location_prefix)
 
     @_options.ReadOptions.options
     @utils.positional(1)
     def get(
         self,
         read_consistency=None,
@@ -1081,15 +1131,15 @@
 
     # NOTE: This is the same behavior as in the helper
     #       ``google.cloud.datastore.key._clean_app()``.
     parts = app.split("~", 1)
     return parts[-1]
 
 
-def _from_reference(reference, app, namespace):
+def _from_reference(reference, app, namespace, database):
     """Convert Reference protobuf to :class:`~google.cloud.datastore.key.Key`.
 
     This is intended to work with the "legacy" representation of a
     datastore "Key" used within Google App Engine (a so-called
     "Reference"). This assumes that ``serialized`` was created within an App
     Engine app via something like ``ndb.Key(...).reference()``.
 
@@ -1098,68 +1148,81 @@
     ``google.appengine.datastore.entity_pb.Reference``.
 
     Args:
         serialized (bytes): A reference protobuf serialized to bytes.
         app (Optional[str]): The application ID / project ID for the
             constructed key.
         namespace (Optional[str]): The namespace for the constructed key.
+        database (Optional[str]): The database for the constructed key.
 
     Returns:
         google.cloud.datastore.key.Key: The key corresponding to
         ``serialized``.
 
     Raises:
         RuntimeError: If ``app`` is not :data:`None`, but not the same as
             ``reference.app``.
+        RuntimeError: If ``database`` is not :data:`None`, but not the same as
+            ``reference.database_id``.
         RuntimeError: If ``namespace`` is not :data:`None`, but not the same as
             ``reference.name_space``.
     """
     project = _project_from_app(reference.app)
     if app is not None:
         if _project_from_app(app) != project:
             raise RuntimeError(_REFERENCE_APP_MISMATCH.format(reference.app, app))
 
+    parsed_database = _key_module._get_empty(reference.database_id, "")
+    if database is not None:
+        if database != parsed_database:
+            raise RuntimeError(
+                _REFERENCE_DATABASE_MISMATCH.format(reference.database_id, database)
+            )
+
     parsed_namespace = _key_module._get_empty(reference.name_space, "")
     if namespace is not None:
         if namespace != parsed_namespace:
             raise RuntimeError(
                 _REFERENCE_NAMESPACE_MISMATCH.format(reference.name_space, namespace)
             )
 
-    _key_module._check_database_id(reference.database_id)
     flat_path = _key_module._get_flat_path(reference.path)
     return google.cloud.datastore.Key(
-        *flat_path, project=project, namespace=parsed_namespace
+        *flat_path,
+        project=project,
+        database=parsed_database,
+        namespace=parsed_namespace,
     )
 
 
-def _from_serialized(serialized, app, namespace):
+def _from_serialized(serialized, app, namespace, database):
     """Convert serialized protobuf to :class:`~google.cloud.datastore.key.Key`.
 
     This is intended to work with the "legacy" representation of a
     datastore "Key" used within Google App Engine (a so-called
     "Reference"). This assumes that ``serialized`` was created within an App
     Engine app via something like ``ndb.Key(...).serialized()``.
 
     Args:
         serialized (bytes): A reference protobuf serialized to bytes.
         app (Optional[str]): The application ID / project ID for the
             constructed key.
         namespace (Optional[str]): The namespace for the constructed key.
+        database (Optional[str]): The database for the constructed key.
 
     Returns:
         Tuple[google.cloud.datastore.key.Key, .Reference]: The key
         corresponding to ``serialized`` and the Reference protobuf.
     """
     reference = _app_engine_key_pb2.Reference()
     reference.ParseFromString(serialized)
-    return _from_reference(reference, app, namespace), reference
+    return _from_reference(reference, app, namespace, database), reference
 
 
-def _from_urlsafe(urlsafe, app, namespace):
+def _from_urlsafe(urlsafe, app, namespace, database):
     """Convert urlsafe string to :class:`~google.cloud.datastore.key.Key`.
 
     .. note::
 
        This is borrowed from
        :meth:`~google.cloud.datastore.key.Key.from_legacy_urlsafe`.
        It is provided here, rather than calling that method, since component
@@ -1172,25 +1235,26 @@
 
     Args:
         urlsafe (Union[bytes, str]): The base64 encoded (ASCII) string
             corresponding to a datastore "Key" / "Reference".
         app (Optional[str]): The application ID / project ID for the
             constructed key.
         namespace (Optional[str]): The namespace for the constructed key.
+        database (Optional[str]): The database for the constructed key.
 
     Returns:
         Tuple[google.cloud.datastore.key.Key, .Reference]: The key
         corresponding to ``urlsafe`` and the Reference protobuf.
     """
     if isinstance(urlsafe, six.string_types):  # pragma: NO BRANCH
         urlsafe = urlsafe.encode("ascii")
     padding = b"=" * (-len(urlsafe) % 4)
     urlsafe += padding
     raw_bytes = base64.urlsafe_b64decode(urlsafe)
-    return _from_serialized(raw_bytes, app, namespace)
+    return _from_serialized(raw_bytes, app, namespace, database)
 
 
 def _constructor_handle_positional(path_args, kwargs):
     """Properly handle positional arguments to Key constructor.
 
     This will modify ``kwargs`` in a few cases:
 
@@ -1248,14 +1312,15 @@
 def _parse_from_ref(
     klass,
     reference=None,
     serialized=None,
     urlsafe=None,
     app=None,
     namespace=None,
+    database: str = None,
     **kwargs
 ):
     """Construct a key from a Reference.
 
     This makes sure that **exactly** one of ``reference``, ``serialized`` and
     ``urlsafe`` is specified (all three are different representations of a
     ``Reference`` protobuf).
@@ -1269,14 +1334,15 @@
             reference protobuf representing a key.
         serialized (Optional[bytes]): A reference protobuf serialized to bytes.
         urlsafe (Optional[bytes]): A reference protobuf serialized to bytes. The
             raw bytes are then converted to a websafe base64-encoded string.
         app (Optional[str]): The Google Cloud Platform project (previously
             on Google App Engine, this was called the Application ID).
         namespace (Optional[str]): The namespace for the key.
+        database (Optional[str]): The database for the Key.
         kwargs (Dict[str, Any]): Any extra keyword arguments not covered by
             the explicitly provided ones. These are passed through to indicate
             to the user that the wrong combination of arguments was used, e.g.
             if ``parent`` and ``urlsafe`` were used together.
 
     Returns:
         Tuple[~.datastore.Key, \
@@ -1295,29 +1361,35 @@
 
     if kwargs or not _exactly_one_specified(reference, serialized, urlsafe):
         raise TypeError(
             "Cannot construct Key reference from incompatible " "keyword arguments."
         )
 
     if reference:
-        ds_key = _from_reference(reference, app, namespace)
+        ds_key = _from_reference(reference, app, namespace, database)
     elif serialized:
-        ds_key, reference = _from_serialized(serialized, app, namespace)
+        ds_key, reference = _from_serialized(serialized, app, namespace, database)
     else:
         # NOTE: We know here that ``urlsafe`` is truth-y;
         #       ``_exactly_one_specified()`` guarantees this.
-        ds_key, reference = _from_urlsafe(urlsafe, app, namespace)
+        ds_key, reference = _from_urlsafe(urlsafe, app, namespace, database)
 
     return ds_key, reference
 
 
 def _parse_from_args(
-    pairs=None, flat=None, project=None, app=None, namespace=UNDEFINED, parent=None
+    pairs=None,
+    flat=None,
+    project=None,
+    app=None,
+    namespace=UNDEFINED,
+    parent=None,
+    database=UNDEFINED,
 ):
-    """Construct a key the path (and possibly a parent key).
+    """Construct a key from the path (and possibly a parent key).
 
     Args:
         pairs (Optional[Iterable[Tuple[str, Union[str, int]]]]): An iterable
             of (kind, ID) pairs.
         flat (Optional[Iterable[Union[str, int]]]): An iterable of the
             (kind, ID) pairs but flattened into a single value. For example,
             the pairs ``[("Parent", 1), ("Child", "a")]`` would be flattened to
@@ -1325,14 +1397,17 @@
         project (Optional[str]): The Google Cloud Platform project (previously
             on Google App Engine, this was called the Application ID).
         app (Optional[str]): DEPRECATED: Synonym for ``project``.
         namespace (Optional[str]): The namespace for the key.
         parent (Optional[~.ndb.key.Key]): The parent of the key being
             constructed. If provided, the key path will be **relative** to the
             parent key's path.
+        database (Optional[str]): The database for the key.
+            Defaults to that of the client if a parent was specified, and
+            to the default database if it was not.
 
     Returns:
         ~.datastore.Key: The constructed key.
 
     Raises:
         .BadValueError: If ``parent`` is passed but is not a ``Key``.
     """
@@ -1346,36 +1421,49 @@
         raise TypeError("Can't specify both 'project' and 'app'. They are synonyms.")
     elif not app:
         app = project
 
     parent_ds_key = None
     if parent is None:
         project = _project_from_app(app)
+
         if namespace is UNDEFINED:
-            context = context_module.get_context()
-            namespace = context.get_namespace()
+            namespace = context_module.get_context().get_namespace()
+
+        if database is UNDEFINED:
+            database = context_module.get_context().client.database
 
     else:
         project = _project_from_app(app, allow_empty=True)
         if not isinstance(parent, Key):
             raise exceptions.BadValueError(
                 "Expected Key instance, got {!r}".format(parent)
             )
 
         if namespace is UNDEFINED:
             namespace = None
 
+        if database is UNDEFINED:
+            database = None
+
         # Offload verification of parent to ``google.cloud.datastore.Key()``.
         parent_ds_key = parent._key
 
+    if database == "":
+        database = None
+
     if namespace == "":
         namespace = None
 
     return google.cloud.datastore.Key(
-        *flat, parent=parent_ds_key, project=project, namespace=namespace
+        *flat,
+        parent=parent_ds_key,
+        project=project,
+        database=database,
+        namespace=namespace,
     )
 
 
 def _get_path(flat, pairs):
     """Get a flat path of key arguments.
 
     Does this from exactly one of ``flat`` or ``pairs``.
```

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/metadata.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/metadata.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/model.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 
     from unittest import mock
     from google.cloud import ndb
     from google.cloud.ndb import context as context_module
 
     client = mock.Mock(
         project="testing",
+        database=None,
         namespace=None,
         stub=mock.Mock(spec=()),
-        spec=("project", "namespace", "stub"),
+        spec=("project", "namespace", "database", "stub"),
     )
     context = context_module.Context(client).use()
     context.__enter__()
 
 .. testcleanup:: *
 
     context.__exit__(None, None, None)
@@ -4692,21 +4693,22 @@
         >>> class MyModel(ndb.Model):
         ...     value = ndb.FloatProperty()
         ...     description = ndb.StringProperty()
         ...
         >>> MyModel(value=7.34e22, description="Mass of the moon")
         MyModel(description='Mass of the moon', value=7.34e+22)
 
-    In addition to user-defined properties, there are six accepted keyword
+    In addition to user-defined properties, there are seven accepted keyword
     arguments:
 
     * ``key``
     * ``id``
     * ``app``
     * ``namespace``
+    * ``database``
     * ``parent``
     * ``projection``
 
     Of these, ``key`` is a public attribute on :class:`Model` instances:
 
     .. testsetup:: model-key
 
@@ -4804,20 +4806,21 @@
         id (str): Key ID for this model. If ``id`` is used, ``key`` must be
             :data:`None`.
         parent (Key): The parent model or :data:`None` for a top-level model.
             If ``parent`` is used, ``key`` must be :data:`None`.
         namespace (str): Namespace for the entity key.
         project (str): Project ID for the entity key.
         app (str): DEPRECATED: Synonym for ``project``.
+        database (str): Database for the entity key.
         kwargs (Dict[str, Any]): Additional keyword arguments. These should map
             to properties of this model.
 
     Raises:
         .BadArgumentError: If the constructor is called with ``key`` and one
-            of ``id``, ``app``, ``namespace`` or ``parent`` specified.
+            of ``id``, ``app``, ``namespace``, ``database``, or ``parent`` specified.
     """
 
     # Class variables updated by _fix_up_properties()
     _properties = None
     _has_repeated = False
     _kind_map = {}  # Dict mapping {kind: Model subclass}
 
@@ -4857,14 +4860,15 @@
         # NOTE: We use ``_self`` rather than ``self`` so users can define a
         #       property named 'self'.
         self = _self
         key = self._get_arg(kwargs, "key")
         id_ = self._get_arg(kwargs, "id")
         project = self._get_arg(kwargs, "project")
         app = self._get_arg(kwargs, "app")
+        database = self._get_arg(kwargs, "database", key_module.UNDEFINED)
         namespace = self._get_arg(kwargs, "namespace", key_module.UNDEFINED)
         parent = self._get_arg(kwargs, "parent")
         projection = self._get_arg(kwargs, "projection")
 
         if app and project:
             raise exceptions.BadArgumentError(
                 "Can't specify both 'app' and 'project'. They are synonyms."
@@ -4873,29 +4877,31 @@
         if not project:
             project = app
 
         key_parts_unspecified = (
             id_ is None
             and parent is None
             and project is None
+            and database is key_module.UNDEFINED
             and namespace is key_module.UNDEFINED
         )
         if key is not None:
             if not key_parts_unspecified:
                 raise exceptions.BadArgumentError(
                     "Model constructor given 'key' does not accept "
-                    "'id', 'project', 'app', 'namespace', or 'parent'."
+                    "'id', 'project', 'app', 'namespace', 'database', or 'parent'."
                 )
             self._key = _validate_key(key, entity=self)
         elif not key_parts_unspecified:
             self._key = Key(
                 self._get_kind(),
                 id_,
                 parent=parent,
                 project=project,
+                database=database,
                 namespace=namespace,
             )
 
         self._values = {}
         self._set_attributes(kwargs)
         # Set the projection last, otherwise it will prevent _set_attributes().
         if projection:
@@ -5710,14 +5716,15 @@
         global_cache_timeout=None,
         use_datastore=None,
         use_memcache=None,
         memcache_timeout=None,
         max_memcache_items=None,
         force_writes=None,
         _options=None,
+        database=None,
     ):
         """Get an instance of Model class by ID.
 
         This really just a shorthand for ``Key(cls, id, ....).get()``.
 
         Args:
             id (Union[int, str]): ID of the entity to load.
@@ -5753,25 +5760,28 @@
                 cache; overrides global cache timeout policy for this
                 operation.
             use_memcache (bool): DEPRECATED: Synonym for ``use_global_cache``.
             memcache_timeout (int): DEPRECATED: Synonym for
                 ``global_cache_timeout``.
             max_memcache_items (int): No longer supported.
             force_writes (bool): No longer supported.
+            database (Optional[str]): Database for the entity to load. If not
+                passed, uses the client's value.
 
         Returns:
             Optional[Model]: The retrieved entity, if one is found.
         """
         return cls._get_by_id_async(
             id,
             parent=parent,
             namespace=namespace,
             project=project,
             app=app,
             _options=_options,
+            database=database,
         ).result()
 
     get_by_id = _get_by_id
 
     @classmethod
     @options_module.ReadOptions.options
     @utils.positional(6)
@@ -5793,14 +5803,15 @@
         global_cache_timeout=None,
         use_datastore=None,
         use_memcache=None,
         memcache_timeout=None,
         max_memcache_items=None,
         force_writes=None,
         _options=None,
+        database: str = None,
     ):
         """Get an instance of Model class by ID.
 
         This is the asynchronous version of :meth:`get_by_id`.
 
         Args:
             id (Union[int, str]): ID of the entity to load.
```

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/msgprop.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/msgprop.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/polymodel.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/polymodel.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/query.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                                         cls.age <= max_age))
 
       @classmethod
       def ranked(cls, rank):
           return cls.query(cls.rank == rank).order(cls.age)
 
     for emp in Employee.seniors(42, 5):
-        print emp.name, emp.age, emp.rank
+        print(emp.name, emp.age, emp.rank)
 
 The 'in' operator cannot be overloaded, but is supported through the IN()
 method. For example::
 
     Employee.query().filter(Employee.rank.IN([4, 5, 6]))
 
 Sort orders are supported through the order() method; unary minus is
@@ -129,21 +129,22 @@
 
 Finally, there's an idiom to efficiently loop over the Query results in a
 tasklet, properly yielding when appropriate::
 
     it = query1.iter()
     while (yield it.has_next_async()):
         emp = it.next()
-        print emp.name, emp.age
+        print(emp.name, emp.age)
 """
 
 import functools
 import logging
 import six
 
+from google.cloud.ndb import context as context_module
 from google.cloud.ndb import exceptions
 from google.cloud.ndb import _options
 from google.cloud.ndb import tasklets
 from google.cloud.ndb import utils
 
 
 __all__ = [
@@ -1224,14 +1225,15 @@
         "filters",
         "order_by",
         "orders",
         "distinct_on",
         "group_by",
         "namespace",
         "project",
+        "database",
         # Fetch options
         "keys_only",
         "limit",
         "offset",
         "start_cursor",
         "end_cursor",
         # Both (!?!)
@@ -1262,14 +1264,17 @@
 
         super(QueryOptions, self).__init__(config=config, **kwargs)
 
         if context:
             if not self.project:
                 self.project = context.client.project
 
+            # We always use the client's database, for consistency with python-datastore
+            self.database = context.client.database
+
             if self.namespace is None:
                 if self.ancestor is None:
                     self.namespace = context.get_namespace()
                 else:
                     self.namespace = self.ancestor.namespace()
 
 
@@ -1371,14 +1376,17 @@
             projection = self._option("projection", projection)
             distinct_on = self._option("distinct_on", distinct_on)
             group_by = self._option("group_by", group_by)
             limit = self._option("limit", limit)
             offset = self._option("offset", offset)
             keys_only = self._option("keys_only", keys_only)
 
+        # Except in the case of ancestor queries, we always use the client's database
+        database = context_module.get_context().client.database or None
+
         if ancestor is not None:
             if isinstance(ancestor, ParameterizedThing):
                 if isinstance(ancestor, ParameterizedFunction):
                     if ancestor.func != "key":
                         raise TypeError(
                             "ancestor cannot be a GQL function" "other than Key"
                         )
@@ -1390,25 +1398,29 @@
                 if not ancestor.id():
                     raise ValueError("ancestor cannot be an incomplete key")
                 if project is not None:
                     if project != ancestor.app():
                         raise TypeError("ancestor/project id mismatch")
                 else:
                     project = ancestor.app()
+
+                database = ancestor.database()
+
                 if namespace is not None:
                     # if namespace is the empty string, that means default
                     # namespace, but after a put, if the ancestor is using
                     # the default namespace, its namespace will be None,
                     # so skip the test to avoid a false mismatch error.
                     if namespace == "" and ancestor.namespace() is None:
                         pass
                     elif namespace != ancestor.namespace():
                         raise TypeError("ancestor/namespace mismatch")
                 else:
                     namespace = ancestor.namespace()
+
         if filters is not None:
             if not isinstance(filters, Node):
                 raise TypeError(
                     "filters must be a query Node or None; "
                     "received {}".format(filters)
                 )
         if order_by is not None and orders is not None:
@@ -1427,14 +1439,15 @@
             order_by = self._to_property_orders(order_by)
 
         self.kind = kind
         self.ancestor = ancestor
         self.filters = filters
         self.order_by = order_by
         self.project = project
+        self.database = database
         self.namespace = namespace
         self.limit = limit
         self.offset = offset
         self.keys_only = keys_only
 
         self.projection = None
         if projection is not None:
```

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/stats.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/stats.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/tasklets.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/tasklets.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google/cloud/ndb/utils.py` & `google-cloud-ndb-2.2.0/google/cloud/ndb/utils.py`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/google_cloud_ndb.egg-info/PKG-INFO` & `google-cloud-ndb-2.2.0/google_cloud_ndb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-ndb
-Version: 2.1.1
+Version: 2.2.0
 Summary: NDB library for Google Cloud Datastore
 Home-page: https://github.com/googleapis/python-ndb
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Project-URL: Documentation, https://googleapis.dev/python/python-ndb/latest
 Project-URL: Issue Tracker, https://github.com/googleapis/python-ndb/issues
```

### Comparing `google-cloud-ndb-2.1.1/google_cloud_ndb.egg-info/SOURCES.txt` & `google-cloud-ndb-2.2.0/google_cloud_ndb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-ndb-2.1.1/setup.py` & `google-cloud-ndb-2.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 def main():
     package_root = os.path.abspath(os.path.dirname(__file__))
     readme_filename = os.path.join(package_root, "README.md")
     with io.open(readme_filename, encoding="utf-8") as readme_file:
         readme = readme_file.read()
     dependencies = [
         "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
-        "google-cloud-datastore >= 2.7.2, <3.0.0dev",
+        "google-cloud-datastore >= 2.16.0, < 3.0.0dev",
         "protobuf >= 3.19.5, <5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
         "pymemcache >= 2.1.0, < 5.0.0dev",
         "redis >= 3.0.0, < 5.0.0dev",
         "pytz >= 2018.3"
     ]
 
     setuptools.setup(
         name="google-cloud-ndb",
-        version = "2.1.1",
+        version = "2.2.0",
         description="NDB library for Google Cloud Datastore",
         long_description=readme,
         long_description_content_type="text/markdown",
         author="Google LLC",
         author_email="googleapis-packages@google.com",
         license="Apache 2.0",
         url="https://github.com/googleapis/python-ndb",
```

