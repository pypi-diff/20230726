# Comparing `tmp/qwak_inference-0.1.6.tar.gz` & `tmp/qwak_inference-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_inference-0.1.6.tar", max compression
+gzip compressed data, was "qwak_inference-0.1.7.tar", max compression
```

## Comparing `qwak_inference-0.1.6.tar` & `qwak_inference-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    10480 2023-07-09 06:43:09.509103 qwak_inference-0.1.6/LICENSE
--rw-r--r--   0        0        0      267 2023-07-09 06:43:09.509103 qwak_inference-0.1.6/README.md
--rw-r--r--   0        0        0     1893 2023-07-09 06:44:01.485719 qwak_inference-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      804 2023-07-09 06:44:01.485719 qwak_inference-0.1.6/qwak_inference/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/batch_client/__init__.py
--rw-r--r--   0        0        0    20136 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/batch_client/batch_client.py
--rw-r--r--   0        0        0     2172 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/batch_client/file_serialization.py
--rw-r--r--   0        0        0     1497 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/batch_client/instance_validation.py
--rw-r--r--   0        0        0      739 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/batch_client/s3.py
--rw-r--r--   0        0        0       95 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/configuration/__init__.py
--rw-r--r--   0        0        0     3127 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/configuration/account.py
--rw-r--r--   0        0        0     2676 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/configuration/auth.py
--rw-r--r--   0        0        0      929 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/configuration/session.py
--rw-r--r--   0        0        0      688 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/constants.py
--rw-r--r--   0        0        0     1592 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/exceptions.py
--rw-r--r--   0        0        0     1999 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/feedback_client.py
--rw-r--r--   0        0        0       65 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/realtime_client/__init__.py
--rw-r--r--   0        0        0     4811 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/realtime_client/client.py
--rw-r--r--   0        0        0     2346 2023-07-09 06:43:09.513104 qwak_inference-0.1.6/qwak_inference/realtime_client/rest_helpers.py
--rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 qwak_inference-0.1.6/setup.py
--rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 qwak_inference-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    10480 2023-07-26 10:34:32.413627 qwak_inference-0.1.7/LICENSE
+-rw-r--r--   0        0        0      267 2023-07-26 10:34:32.413627 qwak_inference-0.1.7/README.md
+-rw-r--r--   0        0        0     2192 2023-07-26 10:35:34.786138 qwak_inference-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      804 2023-07-26 10:35:34.786138 qwak_inference-0.1.7/qwak_inference/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 10:34:32.413627 qwak_inference-0.1.7/qwak_inference/batch_client/__init__.py
+-rw-r--r--   0        0        0    20136 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/batch_client/batch_client.py
+-rw-r--r--   0        0        0     2172 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/batch_client/file_serialization.py
+-rw-r--r--   0        0        0     1497 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/batch_client/instance_validation.py
+-rw-r--r--   0        0        0      739 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/batch_client/s3.py
+-rw-r--r--   0        0        0       95 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/configuration/__init__.py
+-rw-r--r--   0        0        0     3127 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/configuration/account.py
+-rw-r--r--   0        0        0     2676 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/configuration/auth.py
+-rw-r--r--   0        0        0      929 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/configuration/session.py
+-rw-r--r--   0        0        0      688 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/constants.py
+-rw-r--r--   0        0        0     1592 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/exceptions.py
+-rw-r--r--   0        0        0     1999 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/feedback_client.py
+-rw-r--r--   0        0        0       65 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/realtime_client/__init__.py
+-rw-r--r--   0        0        0     4811 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/realtime_client/client.py
+-rw-r--r--   0        0        0     2346 2023-07-26 10:34:32.417627 qwak_inference-0.1.7/qwak_inference/realtime_client/rest_helpers.py
+-rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 qwak_inference-0.1.7/setup.py
+-rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 qwak_inference-0.1.7/PKG-INFO
```

### Comparing `qwak_inference-0.1.6/LICENSE` & `qwak_inference-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.6/pyproject.toml` & `qwak_inference-0.1.7/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 [tool.poetry]
 name = "qwak-inference"
-version = "0.1.6"
+version = "0.1.7"
 description = "Qwak Inference is a Python library for running predictions again Qwak Models."
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.10"
+python = ">=3.7.1,<3.12"
 requests = "^2.0.0"
-qwak-core = { version=">=0.0.102", optional=true}
+qwak-core = [
+    { version=">=0.0.102", python=">=3.7.1,<3.10", optional=true},
+    { version=">=0.0.147", python=">=3.10", optional=true}
+]
 boto3 = { version="^1.24.89", optional=true }
+numpy = [
+    { version = ">=1.21.6", python = ">=3.7.1,<3.10" },
+    { version = ">=1.24.0", python = ">=3.10" }
+]
 pandas = [
     {version="<1.4", python=">=3.7.1,<3.8", optional=true},
-    {version=">=1.4.3,<2.0.0", python=">=3.8,<3.10", optional=true}
+    { version = ">=1.4.0", python = ">=3.8,<3.12", optional=true }
 ]
 joblib = { version="^1.1.0", optional=true }
 pyarrow = { version=">=6.0.0, <11.0.0", optional=true }
 
 [tool.poetry.dev-dependencies]
 pytest = "7.2.1"
 black = "23.1.0"
```

### Comparing `qwak_inference-0.1.6/qwak_inference/__init__.py` & `qwak_inference-0.1.7/qwak_inference/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     print(
         "Notice that BatchInferenceClient and FeedbackClient are not available in the skinny package. "
         'In order to use them, please install them as extras: pip install "qwak-inference[batch,feedback]".'
     )
 
 __all__ = clients
 
-__version__ = "0.1.6"
+__version__ = "0.1.7"
```

### Comparing `qwak_inference-0.1.6/qwak_inference/batch_client/batch_client.py` & `qwak_inference-0.1.7/qwak_inference/batch_client/batch_client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.6/qwak_inference/batch_client/file_serialization.py` & `qwak_inference-0.1.7/qwak_inference/batch_client/file_serialization.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.6/qwak_inference/batch_client/instance_validation.py` & `qwak_inference-0.1.7/qwak_inference/batch_client/instance_validation.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.6/qwak_inference/batch_client/s3.py` & `qwak_inference-0.1.7/qwak_inference/batch_client/s3.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.6/qwak_inference/configuration/account.py` & `qwak_inference-0.1.7/qwak_inference/configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.6/qwak_inference/configuration/auth.py` & `qwak_inference-0.1.7/qwak_inference/configuration/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.6/qwak_inference/configuration/session.py` & `qwak_inference-0.1.7/qwak_inference/configuration/session.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.6/qwak_inference/constants.py` & `qwak_inference-0.1.7/qwak_inference/constants.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.6/qwak_inference/exceptions.py` & `qwak_inference-0.1.7/qwak_inference/exceptions.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.6/qwak_inference/feedback_client.py` & `qwak_inference-0.1.7/qwak_inference/feedback_client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.6/qwak_inference/realtime_client/client.py` & `qwak_inference-0.1.7/qwak_inference/realtime_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.6/qwak_inference/realtime_client/rest_helpers.py` & `qwak_inference-0.1.7/qwak_inference/realtime_client/rest_helpers.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.6/setup.py` & `qwak_inference-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,42 +10,48 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.0.0,<3.0.0']
 
 extras_require = \
-{'batch': ['qwak-core>=0.0.102',
-           'boto3>=1.24.89,<2.0.0',
+{':python_full_version >= "3.7.1" and python_version < "3.10"': ['numpy>=1.21.6'],
+ ':python_version >= "3.10"': ['numpy>=1.24.0'],
+ 'batch': ['boto3>=1.24.89,<2.0.0',
            'joblib>=1.1.0,<2.0.0',
            'pyarrow>=6.0.0,<11.0.0'],
+ 'batch:python_full_version >= "3.7.1" and python_version < "3.10"': ['qwak-core>=0.0.102',
+                                                                      'qwak-core>=0.0.102'],
  'batch:python_full_version >= "3.7.1" and python_version < "3.8"': ['pandas<1.4',
                                                                      'pandas<1.4'],
- 'batch:python_version >= "3.8" and python_version < "3.10"': ['pandas>=1.4.3,<2.0.0',
-                                                               'pandas>=1.4.3,<2.0.0'],
- 'feedback': ['qwak-core>=0.0.102',
-              'boto3>=1.24.89,<2.0.0',
-              'joblib>=1.1.0,<2.0.0'],
+ 'batch:python_version >= "3.10"': ['qwak-core>=0.0.147', 'qwak-core>=0.0.147'],
+ 'batch:python_version >= "3.8" and python_version < "3.12"': ['pandas>=1.4.0',
+                                                               'pandas>=1.4.0'],
+ 'feedback': ['boto3>=1.24.89,<2.0.0', 'joblib>=1.1.0,<2.0.0'],
+ 'feedback:python_full_version >= "3.7.1" and python_version < "3.10"': ['qwak-core>=0.0.102',
+                                                                         'qwak-core>=0.0.102'],
  'feedback:python_full_version >= "3.7.1" and python_version < "3.8"': ['pandas<1.4',
                                                                         'pandas<1.4'],
- 'feedback:python_version >= "3.8" and python_version < "3.10"': ['pandas>=1.4.3,<2.0.0',
-                                                                  'pandas>=1.4.3,<2.0.0']}
+ 'feedback:python_version >= "3.10"': ['qwak-core>=0.0.147',
+                                       'qwak-core>=0.0.147'],
+ 'feedback:python_version >= "3.8" and python_version < "3.12"': ['pandas>=1.4.0',
+                                                                  'pandas>=1.4.0']}
 
 setup_kwargs = {
     'name': 'qwak-inference',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'Qwak Inference is a Python library for running predictions again Qwak Models.',
     'long_description': '# Qwak Inference\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Inference contains tools that allow predicting against the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.7.1,<3.10',
+    'python_requires': '>=3.7.1,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `qwak_inference-0.1.6/PKG-INFO` & `qwak_inference-0.1.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: qwak-inference
-Version: 0.1.6
+Version: 0.1.7
 Summary: Qwak Inference is a Python library for running predictions again Qwak Models.
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
-Requires-Python: >=3.7.1,<3.10
+Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: batch
 Provides-Extra: feedback
 Requires-Dist: boto3 (>=1.24.89,<2.0.0) ; extra == "batch" or extra == "feedback"
 Requires-Dist: joblib (>=1.1.0,<2.0.0) ; extra == "batch" or extra == "feedback"
+Requires-Dist: numpy (>=1.21.6) ; python_full_version >= "3.7.1" and python_version < "3.10"
+Requires-Dist: numpy (>=1.24.0) ; python_version >= "3.10"
 Requires-Dist: pandas (<1.4) ; (python_full_version >= "3.7.1" and python_version < "3.8") and (extra == "batch" or extra == "feedback")
-Requires-Dist: pandas (>=1.4.3,<2.0.0) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "batch" or extra == "feedback")
+Requires-Dist: pandas (>=1.4.0) ; (python_version >= "3.8" and python_version < "3.12") and (extra == "batch" or extra == "feedback")
 Requires-Dist: pyarrow (>=6.0.0,<11.0.0) ; extra == "batch"
-Requires-Dist: qwak-core (>=0.0.102) ; extra == "batch" or extra == "feedback"
+Requires-Dist: qwak-core (>=0.0.102) ; (python_full_version >= "3.7.1" and python_version < "3.10") and (extra == "batch" or extra == "feedback")
+Requires-Dist: qwak-core (>=0.0.147) ; (python_version >= "3.10") and (extra == "batch" or extra == "feedback")
 Requires-Dist: requests (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Qwak Inference
 
 Qwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.
 Qwak Inference contains tools that allow predicting against the Qwak Platform
```

