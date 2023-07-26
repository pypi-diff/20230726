# Comparing `tmp/cog-airflow-notify-sns-2.0.0.tar.gz` & `tmp/cog-airflow-notify-sns-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cog-airflow-notify-sns-2.0.0.tar", last modified: Wed Jul 26 03:09:32 2023, max compression
+gzip compressed data, was "cog-airflow-notify-sns-2.0.1.tar", last modified: Wed Jul 26 03:18:47 2023, max compression
```

## Comparing `cog-airflow-notify-sns-2.0.0.tar` & `cog-airflow-notify-sns-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-07-26 03:09:32.832805 cog-airflow-notify-sns-2.0.0/
--rw-rw-r--   0 werneck   (1000) werneck   (1000)     1073 2023-07-24 09:36:46.000000 cog-airflow-notify-sns-2.0.0/LICENSE
--rw-rw-r--   0 werneck   (1000) werneck   (1000)     2497 2023-07-26 03:09:32.828806 cog-airflow-notify-sns-2.0.0/PKG-INFO
--rw-rw-r--   0 werneck   (1000) werneck   (1000)     2011 2023-07-24 09:36:46.000000 cog-airflow-notify-sns-2.0.0/README.md
-drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-07-26 03:09:32.824806 cog-airflow-notify-sns-2.0.0/airflow_notify_sns/
--rw-rw-r--   0 werneck   (1000) werneck   (1000)       38 2023-07-24 09:36:46.000000 cog-airflow-notify-sns-2.0.0/airflow_notify_sns/__init__.py
--rw-rw-r--   0 werneck   (1000) werneck   (1000)     3870 2023-07-24 14:32:55.000000 cog-airflow-notify-sns-2.0.0/airflow_notify_sns/notify.py
-drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-07-26 03:09:32.828806 cog-airflow-notify-sns-2.0.0/cog_airflow_notify_sns.egg-info/
--rw-rw-r--   0 werneck   (1000) werneck   (1000)     2497 2023-07-26 03:09:32.000000 cog-airflow-notify-sns-2.0.0/cog_airflow_notify_sns.egg-info/PKG-INFO
--rw-rw-r--   0 werneck   (1000) werneck   (1000)      315 2023-07-26 03:09:32.000000 cog-airflow-notify-sns-2.0.0/cog_airflow_notify_sns.egg-info/SOURCES.txt
--rw-rw-r--   0 werneck   (1000) werneck   (1000)        1 2023-07-26 03:09:32.000000 cog-airflow-notify-sns-2.0.0/cog_airflow_notify_sns.egg-info/dependency_links.txt
--rw-rw-r--   0 werneck   (1000) werneck   (1000)        1 2023-07-26 03:09:32.000000 cog-airflow-notify-sns-2.0.0/cog_airflow_notify_sns.egg-info/not-zip-safe
--rw-rw-r--   0 werneck   (1000) werneck   (1000)       19 2023-07-26 03:09:32.000000 cog-airflow-notify-sns-2.0.0/cog_airflow_notify_sns.egg-info/top_level.txt
--rw-rw-r--   0 werneck   (1000) werneck   (1000)       38 2023-07-26 03:09:32.832805 cog-airflow-notify-sns-2.0.0/setup.cfg
--rwxrwxr-x   0 werneck   (1000) werneck   (1000)      917 2023-07-24 14:55:35.000000 cog-airflow-notify-sns-2.0.0/setup.py
+drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-07-26 03:18:47.436557 cog-airflow-notify-sns-2.0.1/
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     1073 2023-07-24 09:36:46.000000 cog-airflow-notify-sns-2.0.1/LICENSE
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     2497 2023-07-26 03:18:47.436557 cog-airflow-notify-sns-2.0.1/PKG-INFO
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     2011 2023-07-24 09:36:46.000000 cog-airflow-notify-sns-2.0.1/README.md
+drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-07-26 03:18:47.432557 cog-airflow-notify-sns-2.0.1/airflow_notify_sns/
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)       66 2023-07-26 03:17:58.000000 cog-airflow-notify-sns-2.0.1/airflow_notify_sns/__init__.py
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     3870 2023-07-24 14:32:55.000000 cog-airflow-notify-sns-2.0.1/airflow_notify_sns/notify.py
+drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-07-26 03:18:47.436557 cog-airflow-notify-sns-2.0.1/cog_airflow_notify_sns.egg-info/
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     2497 2023-07-26 03:18:47.000000 cog-airflow-notify-sns-2.0.1/cog_airflow_notify_sns.egg-info/PKG-INFO
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)      315 2023-07-26 03:18:47.000000 cog-airflow-notify-sns-2.0.1/cog_airflow_notify_sns.egg-info/SOURCES.txt
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)        1 2023-07-26 03:18:47.000000 cog-airflow-notify-sns-2.0.1/cog_airflow_notify_sns.egg-info/dependency_links.txt
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)        1 2023-07-26 03:18:47.000000 cog-airflow-notify-sns-2.0.1/cog_airflow_notify_sns.egg-info/not-zip-safe
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)       19 2023-07-26 03:18:47.000000 cog-airflow-notify-sns-2.0.1/cog_airflow_notify_sns.egg-info/top_level.txt
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)       38 2023-07-26 03:18:47.436557 cog-airflow-notify-sns-2.0.1/setup.cfg
+-rwxrwxr-x   0 werneck   (1000) werneck   (1000)      917 2023-07-26 03:18:20.000000 cog-airflow-notify-sns-2.0.1/setup.py
```

### Comparing `cog-airflow-notify-sns-2.0.0/LICENSE` & `cog-airflow-notify-sns-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cog-airflow-notify-sns-2.0.0/PKG-INFO` & `cog-airflow-notify-sns-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cog-airflow-notify-sns
-Version: 2.0.0
+Version: 2.0.1
 Summary: Publish Airflow notification errors to SNS Topic
 Home-page: https://github.com/cognitivo/cog.dataplatform.service.system.airflow.notification
 Author: Cognitivo.ai
 Author-email: engenharia@cognitivo.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cog-airflow-notify-sns-2.0.0/README.md` & `cog-airflow-notify-sns-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cog-airflow-notify-sns-2.0.0/airflow_notify_sns/notify.py` & `cog-airflow-notify-sns-2.0.1/airflow_notify_sns/notify.py`

 * *Files identical despite different names*

### Comparing `cog-airflow-notify-sns-2.0.0/cog_airflow_notify_sns.egg-info/PKG-INFO` & `cog-airflow-notify-sns-2.0.1/cog_airflow_notify_sns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cog-airflow-notify-sns
-Version: 2.0.0
+Version: 2.0.1
 Summary: Publish Airflow notification errors to SNS Topic
 Home-page: https://github.com/cognitivo/cog.dataplatform.service.system.airflow.notification
 Author: Cognitivo.ai
 Author-email: engenharia@cognitivo.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cog-airflow-notify-sns-2.0.0/setup.py` & `cog-airflow-notify-sns-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 MYDIR = path.abspath(path.dirname(__file__))
 
 cmdclass = {}
 ext_modules = []
 
 setup(
     name='cog-airflow-notify-sns',  
-    version='2.0.0',
+    version='2.0.1',
     author="Cognitivo.ai",
     author_email="engenharia@cognitivo.ai",
     description="Publish Airflow notification errors to SNS Topic",
     url='https://github.com/cognitivo/cog.dataplatform.service.system.airflow.notification',
     long_description=io.open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests']),
```

