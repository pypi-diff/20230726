# Comparing `tmp/gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5.tar.gz` & `tmp/gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5.tar", last modified: Tue Jul 25 18:24:35 2023, max compression
+gzip compressed data, was "gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6.tar", last modified: Wed Jul 26 18:24:39 2023, max compression
```

## Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5.tar` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:35.432511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-25 18:24:35.432511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:24:35.432511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:35.428511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:35.428511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:35.432511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:35.432511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17501 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@0.4.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:24:23.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:24:35.432511 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-25 18:24:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-25 18:24:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:24:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-25 18:24:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 18:24:35.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:39.734343 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-26 18:24:25.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 18:24:25.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-26 18:24:39.730343 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-26 18:24:25.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 18:24:25.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 18:24:39.734343 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-26 18:24:25.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:39.730343 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:39.730343 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:39.730343 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-26 18:24:25.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:39.730343 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-26 18:24:25.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-07-26 18:24:25.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@0.4.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:24:25.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:24:39.730343 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-26 18:24:39.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-26 18:24:39.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:24:39.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 18:24:39.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 18:24:39.000000 gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/top_level.txt
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/LICENSE` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/PKG-INFO` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ecs-fargate-task-termination-detection-event-rule
-Version: 0.4.5
+Version: 0.4.6
 Summary: This an AWS ECS Fargate task termination detection Event Rule.
 Home-page: https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/README.md` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/setup.py` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-ecs-fargate-task-termination-detection-event-rule",
-    "version": "0.4.5",
+    "version": "0.4.6",
     "description": "This an AWS ECS Fargate task termination detection Event Rule.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule",
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule._jsii"
     ],
     "package_data": {
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule._jsii": [
-            "aws-ecs-fargate-task-termination-detection-event-rule@0.4.5.jsii.tgz"
+            "aws-ecs-fargate-task-termination-detection-event-rule@0.4.6.jsii.tgz"
         ],
         "gammarer.aws_ecs_fargate_task_termination_detection_event_rule": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ecs-fargate-task-termination-detection-event-rule
-Version: 0.4.5
+Version: 0.4.6
 Summary: This an AWS ECS Fargate task termination detection Event Rule.
 Home-page: https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ecs-fargate-task-termination-detection-event-rule.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.5/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt` & `gammarer.aws-ecs-fargate-task-termination-detection-event-rule-0.4.6/src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/SOURCES.txt
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/dependency_links.txt
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/requires.txt
 src/gammarer.aws_ecs_fargate_task_termination_detection_event_rule.egg-info/top_level.txt
 src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/__init__.py
 src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/py.typed
 src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/__init__.py
-src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@0.4.5.jsii.tgz
+src/gammarer/aws_ecs_fargate_task_termination_detection_event_rule/_jsii/aws-ecs-fargate-task-termination-detection-event-rule@0.4.6.jsii.tgz
```

