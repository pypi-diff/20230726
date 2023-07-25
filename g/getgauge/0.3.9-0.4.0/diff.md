# Comparing `tmp/getgauge-0.3.9.tar.gz` & `tmp/getgauge-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/getgauge-0.3.9.tar", last modified: Thu Apr 23 06:18:25 2020, max compression
+gzip compressed data, was "getgauge-0.4.0.tar", last modified: Tue Jul 25 22:58:18 2023, max compression
```

## Comparing `getgauge-0.3.9.tar` & `getgauge-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-23 06:18:25.000000 getgauge-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (116)     1081 2020-04-23 06:18:12.000000 getgauge-0.3.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)      826 2020-04-23 06:18:25.000000 getgauge-0.3.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-23 06:18:25.000000 getgauge-0.3.9/getgauge/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2541 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/executor.py
--rw-r--r--   0 runner    (1001) docker     (116)     3104 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/handlers.py
--rw-r--r--   0 runner    (1001) docker     (116)     3799 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/impl_loader.py
--rw-r--r--   0 runner    (1001) docker     (116)      479 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-23 06:18:25.000000 getgauge-0.3.9/getgauge/messages/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)   114200 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/messages/messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (116)    14870 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/messages/services_pb2.py
--rw-r--r--   0 runner    (1001) docker     (116)    31017 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/messages/services_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (116)    95903 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/messages/spec_pb2.py
--rw-r--r--   0 runner    (1001) docker     (116)     2720 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/parser.py
--rw-r--r--   0 runner    (1001) docker     (116)     7539 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/parser_parso.py
--rw-r--r--   0 runner    (1001) docker     (116)     6011 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/parser_redbaron.py
--rw-r--r--   0 runner    (1001) docker     (116)     8285 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/processor.py
--rw-r--r--   0 runner    (1001) docker     (116)    10387 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/python.py
--rw-r--r--   0 runner    (1001) docker     (116)     1381 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/refactor.py
--rw-r--r--   0 runner    (1001) docker     (116)     8807 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/registry.py
--rw-r--r--   0 runner    (1001) docker     (116)      845 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/static_loader.py
--rw-r--r--   0 runner    (1001) docker     (116)     1596 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/util.py
--rw-r--r--   0 runner    (1001) docker     (116)     2146 2020-04-23 06:18:12.000000 getgauge-0.3.9/getgauge/validator.py
--rw-r--r--   0 runner    (1001) docker     (116)     1109 2020-04-23 06:18:25.000000 getgauge-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:58:18.446948 getgauge-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-25 22:58:06.670871 getgauge-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-25 22:58:18.446948 getgauge-0.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:58:18.442948 getgauge-0.4.0/getgauge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 22:58:06.670871 getgauge-0.4.0/getgauge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/impl_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:58:18.446948 getgauge-0.4.0/getgauge/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19941 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/messages/messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/messages/services_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60546 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/messages/services_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17111 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/messages/spec_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10387 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/static_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-25 22:58:06.674871 getgauge-0.4.0/getgauge/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-25 22:58:18.098948 getgauge-0.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `getgauge-0.3.9/LICENSE.txt` & `getgauge-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `getgauge-0.3.9/PKG-INFO` & `getgauge-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: getgauge
-Version: 0.3.9
+Version: 0.4.0
 Summary: Enables Python support for Gauge
 Home-page: https://github.com/getgauge/gauge-python
 Author: Gauge Team
 Author-email: getgauge@outlook.com
 License: MIT
-Download-URL: https://github.com/getgauge/gauge-python/archive/v0.3.9.zip
+Download-URL: https://github.com/getgauge/gauge-python/archive/v0.4.0.zip
 Description: UNKNOWN
 Keywords: testing,gauge,gauge-python,getgauge,automation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `getgauge-0.3.9/getgauge/executor.py` & `getgauge-0.4.0/getgauge/executor.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.3.9/getgauge/handlers.py` & `getgauge-0.4.0/getgauge/handlers.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.3.9/getgauge/impl_loader.py` & `getgauge-0.4.0/getgauge/impl_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,15 @@
         if len(classes) > 0:
             for c in classes:
                 file = inspect.getfile(c[1])
                 # Create instance of step implementation class.
                 if _has_methods_with_gauge_decoratores(c[1]):
                     update_step_resgistry_with_class(c[1](), file_path) # c[1]() will create a new instance of the class
     except:
-        logger.error('Exception occurred while loading step implementations from file: {}.'.format(rel_path))
-        logger.error(traceback.format_exc())
+        logger.fatal('Exception occurred while loading step implementations from file: {}.\n{}'.format(rel_path, traceback.format_exc()))
 
 # Inject instace in each class method (hook/step)
 def update_step_resgistry_with_class(instance, file_path):
     for info in registry.get_all_methods_in(file_path):
         class_methods = [x[0] for x in inspect.getmembers(instance, inspect.ismethod)]
         if info.impl.__name__ in class_methods:
             info.instance = instance
```

### Comparing `getgauge-0.3.9/getgauge/parser_redbaron.py` & `getgauge-0.4.0/getgauge/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-import six
 from getgauge import logger
 from redbaron import RedBaron
 
 
-class RedbaronPythonFile(object):
+class Parser(object):
 
     @staticmethod
     def parse(file_path, content=None):
         """
-        Create a PythonFile object with specified file_path and content.
+        Create a Parser object with specified file_path and content.
         If content is None then, it is loaded from the file_path method.
         Otherwise, file_path is only used for reporting errors.
         """
         try:
             if content is None:
-                with open(file_path) as f:
+                with open(file_path, encoding='utf-8') as f:
                     content = f.read()
             py_tree = RedBaron(content)
-            return RedbaronPythonFile(file_path, py_tree)
+            return Parser(file_path, py_tree)
         except Exception as ex:
             # Trim parsing error message to only include failure location
             msg = str(ex)
             marker = "<---- here\n"
             marker_pos = msg.find(marker)
             if marker_pos > 0:
                 msg = msg[:marker_pos + len(marker)]
@@ -69,20 +68,20 @@
         args = decorator.call.value
         step = None
         if len(args) == 1:
             try:
                 step = args[0].value.to_python()
             except (ValueError, SyntaxError):
                 pass
-            if isinstance(step, six.string_types + (list,)):
+            if isinstance(step, str) or isinstance(step, list):
                 return step
             logger.error("Decorator step accepts either a string or a list of \
-                strings - %s".format(self.file_path))
+                strings - {0}".format(self.file_path))
         else:
-            logger.error("Decorator step accepts only one argument - %s".format(self.file_path))
+            logger.error("Decorator step accepts only one argument - {0}".format(self.file_path))
 
     def iter_steps(self):
         """Iterate over steps in the parsed file."""
         for func, decorator in self._iter_step_func_decorators():
             step = self._step_decorator_args(decorator)
             if step:
                 yield step, func.name, self._span_for_node(func, True)
```

### Comparing `getgauge-0.3.9/getgauge/processor.py` & `getgauge-0.4.0/getgauge/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import traceback
 from os import environ, path
 from threading import Timer
 
-import ptvsd
 from getgauge import logger
 from getgauge.executor import (create_execution_status_response,
                                execute_method, run_hook)
 from getgauge.impl_loader import load_impls
 from getgauge.messages.messages_pb2 import *
 from getgauge.messages.spec_pb2 import Parameter, Span
 from getgauge.python import Table, create_execution_context_from, data_store
```

### Comparing `getgauge-0.3.9/getgauge/python.py` & `getgauge-0.4.0/getgauge/python.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.3.9/getgauge/refactor.py` & `getgauge-0.4.0/getgauge/refactor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from getgauge.messages.messages_pb2 import RefactorResponse, TextDiff
 from getgauge.messages.spec_pb2 import Span
-from getgauge.parser import PythonFile
+from getgauge.parser import Parser
 from getgauge.registry import registry
 
 
 def refactor_step(request, response):
     if registry.has_multiple_impls(request.oldStepValue.stepValue):
         raise Exception('Multiple Implementation found for `{}`'.format(
             request.oldStepValue.parameterizedStepValue
         ))
     info = registry.get_info_for(request.oldStepValue.stepValue)
-    impl_file = PythonFile.parse(info.file_name)
+    impl_file = Parser.parse(info.file_name)
     diffs = impl_file.refactor_step(
         info.step_text,
         request.newStepValue.parameterizedStepValue,
         _new_parameter_positions(request),
     )
     content = impl_file.get_code()
     if request.saveChanges:
```

### Comparing `getgauge-0.3.9/getgauge/registry.py` & `getgauge-0.4.0/getgauge/registry.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.3.9/getgauge/static_loader.py` & `getgauge-0.4.0/getgauge/static_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 from getgauge.registry import registry
-from getgauge.parser import PythonFile
+from getgauge.parser import Parser
 
 
 def load_steps(python_file):
     for funcStep in python_file.iter_steps():
         registry.add_step(funcStep[0], funcStep[1],
                           python_file.file_path, funcStep[2])
 
 
 def reload_steps(file_path, content=None):
-    pf = PythonFile.parse(file_path, content)
+    pf = Parser.parse(file_path, content)
     if pf:
         registry.remove_steps(file_path)
         load_steps(pf)
 
 
 def load_files(step_impl_dirs):
     for step_impl_dir in step_impl_dirs:
         for dirpath, _, files in os.walk(step_impl_dir):
                 py_files = (os.path.join(dirpath, f) for f in files if f.endswith('.py'))
                 for file_path in py_files:
-                        pf = PythonFile.parse(file_path)
+                        pf = Parser.parse(file_path)
                         if pf:
                                 load_steps(pf)
```

### Comparing `getgauge-0.3.9/getgauge/util.py` & `getgauge-0.4.0/getgauge/util.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.3.9/getgauge/validator.py` & `getgauge-0.4.0/getgauge/validator.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.3.9/setup.py` & `getgauge-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from distutils.core import setup
 
 setup(
     name='getgauge',
     packages=['getgauge', 'getgauge/messages'],
-    version='0.3.9',
+    version='0.4.0',
     description='Enables Python support for Gauge',
     author='Gauge Team',
     author_email='getgauge@outlook.com',
     url='https://github.com/getgauge/gauge-python',
-    download_url='https://github.com/getgauge/gauge-python/archive/v0.3.9.zip',
+    download_url='https://github.com/getgauge/gauge-python/archive/v0.4.0.zip',
     keywords=['testing', 'gauge', 'gauge-python', 'getgauge', 'automation'],
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
     ],
-    install_requires=['redBaron', 'parso', 'ptvsd==4.3.2', 'grpcio==1.28.1', 'protobuf>=3.5.2', 'six'],
+    install_requires=['redBaron', 'debugpy', 'grpcio>=1.39.0', 'protobuf>=3.5.2'],
     extras_require={
 		':python_version == "2.7"': ['futures']
 	},
 )
```

