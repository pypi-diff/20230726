# Comparing `tmp/dx_profiler-0.0.1.tar.gz` & `tmp/dx_profiler-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dx_profiler-0.0.1.tar", max compression
+gzip compressed data, was "dx_profiler-0.1.0.tar", max compression
```

## Comparing `dx_profiler-0.0.1.tar` & `dx_profiler-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1473 2023-07-26 07:38:50.384156 dx_profiler-0.0.1/README.md
--rw-r--r--   0        0        0     3887 2023-07-26 07:38:50.384156 dx_profiler-0.0.1/dx_profiler/cli.py
--rw-r--r--   0        0        0      556 2023-07-26 07:38:50.384156 dx_profiler-0.0.1/inference/file_writer.py
--rw-r--r--   0        0        0     1784 2023-07-26 07:38:50.384156 dx_profiler-0.0.1/inference/inference.py
--rw-r--r--   0        0        0     1024 2023-07-26 07:38:50.384156 dx_profiler-0.0.1/inference/nats_listener.py
--rw-r--r--   0        0        0     9352 2023-07-26 07:38:50.384156 dx_profiler-0.0.1/player/player.py
--rw-r--r--   0        0        0     8818 2023-07-26 07:38:50.384156 dx_profiler-0.0.1/proto_py/dx_pb2.py
--rw-r--r--   0        0        0    10004 2023-07-26 07:38:50.384156 dx_profiler-0.0.1/proto_py/dx_pb2.pyi
--rw-r--r--   0        0        0    25768 2023-07-26 07:38:50.384156 dx_profiler-0.0.1/proto_py/dx_pb2_grpc.py
--rw-r--r--   0        0        0      692 2023-07-26 07:38:50.384156 dx_profiler-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2148 1970-01-01 00:00:00.000000 dx_profiler-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1473 2023-07-26 07:47:35.674613 dx_profiler-0.1.0/README.md
+-rw-r--r--   0        0        0     3887 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/dx_profiler/cli.py
+-rw-r--r--   0        0        0      556 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/inference/file_writer.py
+-rw-r--r--   0        0        0     1784 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/inference/inference.py
+-rw-r--r--   0        0        0     1024 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/inference/nats_listener.py
+-rw-r--r--   0        0        0     9352 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/player/player.py
+-rw-r--r--   0        0        0     8818 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/proto_py/dx_pb2.py
+-rw-r--r--   0        0        0    10004 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/proto_py/dx_pb2.pyi
+-rw-r--r--   0        0        0    25768 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/proto_py/dx_pb2_grpc.py
+-rw-r--r--   0        0        0      692 2023-07-26 07:47:35.678613 dx_profiler-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2148 1970-01-01 00:00:00.000000 dx_profiler-0.1.0/PKG-INFO
```

### Comparing `dx_profiler-0.0.1/README.md` & `dx_profiler-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.0.1/dx_profiler/cli.py` & `dx_profiler-0.1.0/dx_profiler/cli.py`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.0.1/inference/file_writer.py` & `dx_profiler-0.1.0/inference/file_writer.py`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.0.1/inference/inference.py` & `dx_profiler-0.1.0/inference/inference.py`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.0.1/inference/nats_listener.py` & `dx_profiler-0.1.0/inference/nats_listener.py`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.0.1/player/player.py` & `dx_profiler-0.1.0/player/player.py`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.0.1/proto_py/dx_pb2.py` & `dx_profiler-0.1.0/proto_py/dx_pb2.py`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.0.1/proto_py/dx_pb2.pyi` & `dx_profiler-0.1.0/proto_py/dx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.0.1/proto_py/dx_pb2_grpc.py` & `dx_profiler-0.1.0/proto_py/dx_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dx_profiler-0.0.1/pyproject.toml` & `dx_profiler-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dx-profiler"
-version = "0.0.1"
+version = "0.1.0"
 description = "Profile Dx App"
 authors = ["SangHyeukYoon <shyoon@snuailab.ai>"]
 readme = "README.md"
 packages = [{include = "dx_profiler"}, {include = "proto_py"}, {include = "inference"}, {include = "player"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dx_profiler-0.0.1/PKG-INFO` & `dx_profiler-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dx-profiler
-Version: 0.0.1
+Version: 0.1.0
 Summary: Profile Dx App
 Author: SangHyeukYoon
 Author-email: shyoon@snuailab.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

