# Comparing `tmp/snitch-protos-0.0.48.tar.gz` & `tmp/snitch-protos-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snitch-protos-0.0.48.tar", last modified: Wed Jul 26 20:59:58 2023, max compression
+gzip compressed data, was "snitch-protos-0.0.49.tar", last modified: Wed Jul 26 21:44:48 2023, max compression
```

## Comparing `snitch-protos-0.0.48.tar` & `snitch-protos-0.0.49.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:58.970237 snitch-protos-0.0.48/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 20:59:58.970237 snitch-protos-0.0.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-26 20:59:28.000000 snitch-protos-0.0.48/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 20:59:58.970237 snitch-protos-0.0.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-26 20:59:58.000000 snitch-protos-0.0.48/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:58.970237 snitch-protos-0.0.48/snitch_protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:28.000000 snitch-protos-0.0.48/snitch_protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:58.970237 snitch-protos-0.0.48/snitch_protos/protos/
--rw-r--r--   0 runner    (1001) docker     (123)    32411 2023-07-26 20:59:28.000000 snitch-protos-0.0.48/snitch_protos/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:58.970237 snitch-protos-0.0.48/snitch_protos/protos/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-26 20:59:28.000000 snitch-protos-0.0.48/snitch_protos/protos/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:59:58.970237 snitch-protos-0.0.48/snitch_protos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 20:59:58.000000 snitch-protos-0.0.48/snitch_protos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-26 20:59:58.000000 snitch-protos-0.0.48/snitch_protos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:59:58.000000 snitch-protos-0.0.48/snitch_protos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 20:59:58.000000 snitch-protos-0.0.48/snitch_protos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:44:48.173422 snitch-protos-0.0.49/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 21:44:48.173422 snitch-protos-0.0.49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-26 21:44:14.000000 snitch-protos-0.0.49/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 21:44:48.173422 snitch-protos-0.0.49/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-26 21:44:47.000000 snitch-protos-0.0.49/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:44:48.173422 snitch-protos-0.0.49/snitch_protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:44:14.000000 snitch-protos-0.0.49/snitch_protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:44:48.173422 snitch-protos-0.0.49/snitch_protos/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)    32523 2023-07-26 21:44:14.000000 snitch-protos-0.0.49/snitch_protos/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:44:48.173422 snitch-protos-0.0.49/snitch_protos/protos/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-26 21:44:14.000000 snitch-protos-0.0.49/snitch_protos/protos/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:44:48.173422 snitch-protos-0.0.49/snitch_protos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-26 21:44:48.000000 snitch-protos-0.0.49/snitch_protos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-26 21:44:48.000000 snitch-protos-0.0.49/snitch_protos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:44:48.000000 snitch-protos-0.0.49/snitch_protos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 21:44:48.000000 snitch-protos-0.0.49/snitch_protos.egg-info/top_level.txt
```

### Comparing `snitch-protos-0.0.48/PKG-INFO` & `snitch-protos-0.0.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.48
+Version: 0.0.49
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `snitch-protos-0.0.48/setup.py` & `snitch-protos-0.0.49/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='snitch-protos',
-    version='0.0.48',
+    version='0.0.49',
     description='Protobuf python package for Streamdal.com Snitch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/streamdal/snitch-protos',
     author='Streamdal.com',
     author_email='engineering@streamdal.com',
     license='MIT',
```

### Comparing `snitch-protos-0.0.48/snitch_protos/protos/__init__.py` & `snitch-protos-0.0.49/snitch_protos/protos/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,19 +390,21 @@
     pipeline_id: str = betterproto.string_field(1)
     audience: "Audience" = betterproto.message_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class PausePipelineRequest(betterproto.Message):
     pipeline_id: str = betterproto.string_field(1)
+    audience: "Audience" = betterproto.message_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class ResumePipelineRequest(betterproto.Message):
     pipeline_id: str = betterproto.string_field(1)
+    audience: "Audience" = betterproto.message_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class TestRequest(betterproto.Message):
     input: str = betterproto.string_field(1)
```

### Comparing `snitch-protos-0.0.48/snitch_protos/protos/steps/__init__.py` & `snitch-protos-0.0.49/snitch_protos/protos/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `snitch-protos-0.0.48/snitch_protos.egg-info/PKG-INFO` & `snitch-protos-0.0.49/snitch_protos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snitch-protos
-Version: 0.0.48
+Version: 0.0.49
 Summary: Protobuf python package for Streamdal.com Snitch
 Home-page: https://github.com/streamdal/snitch-protos
 Author: Streamdal.com
 Author-email: engineering@streamdal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

