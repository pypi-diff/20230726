# Comparing `tmp/gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6.tar.gz` & `tmp/gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6.tar", last modified: Tue Jul 25 19:21:54 2023, max compression
+gzip compressed data, was "gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7.tar", last modified: Wed Jul 26 19:22:51 2023, max compression
```

## Comparing `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6.tar` & `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:21:54.101671 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-25 19:21:36.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 19:21:36.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-25 19:21:54.101671 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-25 19:21:36.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 19:21:36.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:21:54.101671 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-25 19:21:36.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:21:54.097670 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:21:54.097670 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:21:54.097670 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer/aws_daily_cloud_watch_logs_archiver/
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-25 19:21:36.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer/aws_daily_cloud_watch_logs_archiver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:21:54.097670 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer/aws_daily_cloud_watch_logs_archiver/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-25 19:21:36.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer/aws_daily_cloud_watch_logs_archiver/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28204 2023-07-25 19:21:36.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer/aws_daily_cloud_watch_logs_archiver/_jsii/aws-daily-cloud-watch-logs-archiver@0.11.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:21:36.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer/aws_daily_cloud_watch_logs_archiver/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:21:54.097670 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-25 19:21:54.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-25 19:21:54.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:21:54.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-25 19:21:54.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 19:21:54.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:22:51.022872 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-26 19:22:35.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 19:22:35.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-26 19:22:51.022872 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-26 19:22:35.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 19:22:35.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:22:51.022872 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-26 19:22:35.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:22:51.022872 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:22:51.022872 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:22:51.022872 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer/aws_daily_cloud_watch_logs_archiver/
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-26 19:22:35.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer/aws_daily_cloud_watch_logs_archiver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:22:51.022872 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer/aws_daily_cloud_watch_logs_archiver/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-26 19:22:35.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer/aws_daily_cloud_watch_logs_archiver/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28206 2023-07-26 19:22:35.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer/aws_daily_cloud_watch_logs_archiver/_jsii/aws-daily-cloud-watch-logs-archiver@0.11.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:22:35.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer/aws_daily_cloud_watch_logs_archiver/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:22:51.022872 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-26 19:22:50.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-26 19:22:50.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:22:50.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-26 19:22:50.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 19:22:50.000000 gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/top_level.txt
```

### Comparing `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/LICENSE` & `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/PKG-INFO` & `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-daily-cloud-watch-logs-archiver
-Version: 0.11.6
+Version: 0.11.7
 Summary: AWS CloudWatch Logs daily archive to s3 bucket
 Home-page: https://github.com/yicr/aws-daily-cloud-watch-logs-archiver.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-daily-cloud-watch-logs-archiver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/README.md` & `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/setup.py` & `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-daily-cloud-watch-logs-archiver",
-    "version": "0.11.6",
+    "version": "0.11.7",
     "description": "AWS CloudWatch Logs daily archive to s3 bucket",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-daily-cloud-watch-logs-archiver.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "gammarer.aws_daily_cloud_watch_logs_archiver",
         "gammarer.aws_daily_cloud_watch_logs_archiver._jsii"
     ],
     "package_data": {
         "gammarer.aws_daily_cloud_watch_logs_archiver._jsii": [
-            "aws-daily-cloud-watch-logs-archiver@0.11.6.jsii.tgz"
+            "aws-daily-cloud-watch-logs-archiver@0.11.7.jsii.tgz"
         ],
         "gammarer.aws_daily_cloud_watch_logs_archiver": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.66.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "gammarer.aws-secure-bucket>=0.9.8, <0.10.0",
-        "gammarer.aws-secure-log-bucket>=0.9.8, <0.10.0",
+        "gammarer.aws-secure-bucket>=0.9.9, <0.10.0",
+        "gammarer.aws-secure-log-bucket>=0.9.9, <0.10.0",
         "jsii>=1.85.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer/aws_daily_cloud_watch_logs_archiver/__init__.py` & `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer/aws_daily_cloud_watch_logs_archiver/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer/aws_daily_cloud_watch_logs_archiver/_jsii/__init__.py` & `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer/aws_daily_cloud_watch_logs_archiver/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import aws_cdk._jsii
 import constructs._jsii
 import gammarer.aws_secure_bucket._jsii
 import gammarer.aws_secure_log_bucket._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-daily-cloud-watch-logs-archiver",
-    "0.11.6",
+    "0.11.7",
     __name__[0:-6],
-    "aws-daily-cloud-watch-logs-archiver@0.11.6.jsii.tgz",
+    "aws-daily-cloud-watch-logs-archiver@0.11.7.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/PKG-INFO` & `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-daily-cloud-watch-logs-archiver
-Version: 0.11.6
+Version: 0.11.7
 Summary: AWS CloudWatch Logs daily archive to s3 bucket
 Home-page: https://github.com/yicr/aws-daily-cloud-watch-logs-archiver.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-daily-cloud-watch-logs-archiver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.6/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/SOURCES.txt` & `gammarer.aws-daily-cloud-watch-logs-archiver-0.11.7/src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/SOURCES.txt
 src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/dependency_links.txt
 src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/requires.txt
 src/gammarer.aws_daily_cloud_watch_logs_archiver.egg-info/top_level.txt
 src/gammarer/aws_daily_cloud_watch_logs_archiver/__init__.py
 src/gammarer/aws_daily_cloud_watch_logs_archiver/py.typed
 src/gammarer/aws_daily_cloud_watch_logs_archiver/_jsii/__init__.py
-src/gammarer/aws_daily_cloud_watch_logs_archiver/_jsii/aws-daily-cloud-watch-logs-archiver@0.11.6.jsii.tgz
+src/gammarer/aws_daily_cloud_watch_logs_archiver/_jsii/aws-daily-cloud-watch-logs-archiver@0.11.7.jsii.tgz
```

