# Comparing `tmp/cog-airflow-notify-sns-2.0.1.tar.gz` & `tmp/cog-airflow-notify-sns-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cog-airflow-notify-sns-2.0.1.tar", last modified: Wed Jul 26 03:18:47 2023, max compression
+gzip compressed data, was "cog-airflow-notify-sns-2.0.2.tar", last modified: Wed Jul 26 03:49:02 2023, max compression
```

## Comparing `cog-airflow-notify-sns-2.0.1.tar` & `cog-airflow-notify-sns-2.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-07-26 03:18:47.436557 cog-airflow-notify-sns-2.0.1/
--rw-rw-r--   0 werneck   (1000) werneck   (1000)     1073 2023-07-24 09:36:46.000000 cog-airflow-notify-sns-2.0.1/LICENSE
--rw-rw-r--   0 werneck   (1000) werneck   (1000)     2497 2023-07-26 03:18:47.436557 cog-airflow-notify-sns-2.0.1/PKG-INFO
--rw-rw-r--   0 werneck   (1000) werneck   (1000)     2011 2023-07-24 09:36:46.000000 cog-airflow-notify-sns-2.0.1/README.md
-drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-07-26 03:18:47.432557 cog-airflow-notify-sns-2.0.1/airflow_notify_sns/
--rw-rw-r--   0 werneck   (1000) werneck   (1000)       66 2023-07-26 03:17:58.000000 cog-airflow-notify-sns-2.0.1/airflow_notify_sns/__init__.py
--rw-rw-r--   0 werneck   (1000) werneck   (1000)     3870 2023-07-24 14:32:55.000000 cog-airflow-notify-sns-2.0.1/airflow_notify_sns/notify.py
-drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-07-26 03:18:47.436557 cog-airflow-notify-sns-2.0.1/cog_airflow_notify_sns.egg-info/
--rw-rw-r--   0 werneck   (1000) werneck   (1000)     2497 2023-07-26 03:18:47.000000 cog-airflow-notify-sns-2.0.1/cog_airflow_notify_sns.egg-info/PKG-INFO
--rw-rw-r--   0 werneck   (1000) werneck   (1000)      315 2023-07-26 03:18:47.000000 cog-airflow-notify-sns-2.0.1/cog_airflow_notify_sns.egg-info/SOURCES.txt
--rw-rw-r--   0 werneck   (1000) werneck   (1000)        1 2023-07-26 03:18:47.000000 cog-airflow-notify-sns-2.0.1/cog_airflow_notify_sns.egg-info/dependency_links.txt
--rw-rw-r--   0 werneck   (1000) werneck   (1000)        1 2023-07-26 03:18:47.000000 cog-airflow-notify-sns-2.0.1/cog_airflow_notify_sns.egg-info/not-zip-safe
--rw-rw-r--   0 werneck   (1000) werneck   (1000)       19 2023-07-26 03:18:47.000000 cog-airflow-notify-sns-2.0.1/cog_airflow_notify_sns.egg-info/top_level.txt
--rw-rw-r--   0 werneck   (1000) werneck   (1000)       38 2023-07-26 03:18:47.436557 cog-airflow-notify-sns-2.0.1/setup.cfg
--rwxrwxr-x   0 werneck   (1000) werneck   (1000)      917 2023-07-26 03:18:20.000000 cog-airflow-notify-sns-2.0.1/setup.py
+drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-07-26 03:49:02.489455 cog-airflow-notify-sns-2.0.2/
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     1073 2023-07-24 09:36:46.000000 cog-airflow-notify-sns-2.0.2/LICENSE
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     2497 2023-07-26 03:49:02.489455 cog-airflow-notify-sns-2.0.2/PKG-INFO
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     2011 2023-07-24 09:36:46.000000 cog-airflow-notify-sns-2.0.2/README.md
+drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-07-26 03:49:02.473455 cog-airflow-notify-sns-2.0.2/airflow_notify_sns/
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)       66 2023-07-26 03:17:58.000000 cog-airflow-notify-sns-2.0.2/airflow_notify_sns/__init__.py
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     3882 2023-07-26 03:45:50.000000 cog-airflow-notify-sns-2.0.2/airflow_notify_sns/notify.py
+drwxrwxr-x   0 werneck   (1000) werneck   (1000)        0 2023-07-26 03:49:02.489455 cog-airflow-notify-sns-2.0.2/cog_airflow_notify_sns.egg-info/
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)     2497 2023-07-26 03:49:02.000000 cog-airflow-notify-sns-2.0.2/cog_airflow_notify_sns.egg-info/PKG-INFO
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)      315 2023-07-26 03:49:02.000000 cog-airflow-notify-sns-2.0.2/cog_airflow_notify_sns.egg-info/SOURCES.txt
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)        1 2023-07-26 03:49:02.000000 cog-airflow-notify-sns-2.0.2/cog_airflow_notify_sns.egg-info/dependency_links.txt
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)        1 2023-07-26 03:49:02.000000 cog-airflow-notify-sns-2.0.2/cog_airflow_notify_sns.egg-info/not-zip-safe
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)       19 2023-07-26 03:49:02.000000 cog-airflow-notify-sns-2.0.2/cog_airflow_notify_sns.egg-info/top_level.txt
+-rw-rw-r--   0 werneck   (1000) werneck   (1000)       38 2023-07-26 03:49:02.489455 cog-airflow-notify-sns-2.0.2/setup.cfg
+-rwxrwxr-x   0 werneck   (1000) werneck   (1000)      917 2023-07-26 03:48:42.000000 cog-airflow-notify-sns-2.0.2/setup.py
```

### Comparing `cog-airflow-notify-sns-2.0.1/LICENSE` & `cog-airflow-notify-sns-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cog-airflow-notify-sns-2.0.1/PKG-INFO` & `cog-airflow-notify-sns-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cog-airflow-notify-sns
-Version: 2.0.1
+Version: 2.0.2
 Summary: Publish Airflow notification errors to SNS Topic
 Home-page: https://github.com/cognitivo/cog.dataplatform.service.system.airflow.notification
 Author: Cognitivo.ai
 Author-email: engenharia@cognitivo.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cog-airflow-notify-sns-2.0.1/README.md` & `cog-airflow-notify-sns-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cog-airflow-notify-sns-2.0.1/airflow_notify_sns/notify.py` & `cog-airflow-notify-sns-2.0.2/airflow_notify_sns/notify.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             airflow_url: AWS load balancer DNS by airflow
         """
 
         self.aws_sns_topic_arn = aws_sns_topic_arn
         self.airflow_url = airflow_url
 
 
-    def _callback_failure_msg(self, context):
+    def callback_failure_msg(self, context):
         """
             Airflow failure function callback to notify sns
 
             params:
                 context:  Airflow task execution context
             return:
                 Message error formated
@@ -47,15 +47,15 @@
             task=context.get('task_instance').task_id,
             exec_date=context.get('execution_date'),
             log_url=url.replace("localhost:8080", self.airflow_url)
         )
         return msg
 
 
-    def _callback_success_msg(self, context):
+    def callback_success_msg(self, context):
         """
             Airflow success  function callback to notify sns
 
             params:
                 context:  Airflow task execution context
             return:
                 Message success formated
@@ -106,15 +106,15 @@
     notification = Notify(
         aws_sns_topic_arn = ALERTS_CONFIG.get('sns_topic_arn'),
         airflow_url = ALERTS_CONFIG.get('airflow_url')
     )
         
     notification.send(
         msg_subject="ERROR - Airflow task execution failed",
-        msg_content=self._callback_failure_msg(context),
+        msg_content=notification.callback_failure_msg(context),
         context=context
     )
 
 
 def airflow_success_notify(context, **kwargs):
     
     if not ALERTS_CONFIG:
@@ -124,12 +124,12 @@
     notification = Notify(
         aws_sns_topic_arn = ALERTS_CONFIG.get('sns_topic_arn'),
         airflow_url = ALERTS_CONFIG.get('airflow_url')
     )
 
     notification.send(
         msg_subject="SUCCESS - Airflow DAG execution",
-        msg_content=self._callback_success_msg(context),
+        msg_content=notification.callback_success_msg(context),
         context=context
     )
```

### Comparing `cog-airflow-notify-sns-2.0.1/cog_airflow_notify_sns.egg-info/PKG-INFO` & `cog-airflow-notify-sns-2.0.2/cog_airflow_notify_sns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cog-airflow-notify-sns
-Version: 2.0.1
+Version: 2.0.2
 Summary: Publish Airflow notification errors to SNS Topic
 Home-page: https://github.com/cognitivo/cog.dataplatform.service.system.airflow.notification
 Author: Cognitivo.ai
 Author-email: engenharia@cognitivo.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cog-airflow-notify-sns-2.0.1/setup.py` & `cog-airflow-notify-sns-2.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 MYDIR = path.abspath(path.dirname(__file__))
 
 cmdclass = {}
 ext_modules = []
 
 setup(
     name='cog-airflow-notify-sns',  
-    version='2.0.1',
+    version='2.0.2',
     author="Cognitivo.ai",
     author_email="engenharia@cognitivo.ai",
     description="Publish Airflow notification errors to SNS Topic",
     url='https://github.com/cognitivo/cog.dataplatform.service.system.airflow.notification',
     long_description=io.open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests']),
```

