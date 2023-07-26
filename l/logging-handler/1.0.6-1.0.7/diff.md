# Comparing `tmp/logging_handler-1.0.6.tar.gz` & `tmp/logging_handler-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logging_handler-1.0.6.tar", last modified: Fri Apr 21 21:34:08 2023, max compression
+gzip compressed data, was "logging_handler-1.0.7.tar", last modified: Wed Jul 26 20:43:15 2023, max compression
```

## Comparing `logging_handler-1.0.6.tar` & `logging_handler-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-04-21 21:34:08.686852 logging_handler-1.0.6/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1069 2023-01-27 21:59:39.000000 logging_handler-1.0.6/LICENSE
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4004 2023-04-21 21:34:08.683519 logging_handler-1.0.6/PKG-INFO
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3278 2023-01-27 21:59:39.000000 logging_handler-1.0.6/README.md
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      804 2023-04-21 21:33:30.000000 logging_handler-1.0.6/pyproject.toml
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       38 2023-04-21 21:34:08.686852 logging_handler-1.0.6/setup.cfg
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-04-21 21:34:08.683519 logging_handler-1.0.6/src/
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-04-21 21:34:08.683519 logging_handler-1.0.6/src/logging_handler/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4632 2023-04-21 21:33:22.000000 logging_handler-1.0.6/src/logging_handler/__init__.py
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-04-21 21:34:08.683519 logging_handler-1.0.6/src/logging_handler.egg-info/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4004 2023-04-21 21:34:08.000000 logging_handler-1.0.6/src/logging_handler.egg-info/PKG-INFO
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      236 2023-04-21 21:34:08.000000 logging_handler-1.0.6/src/logging_handler.egg-info/SOURCES.txt
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)        1 2023-04-21 21:34:08.000000 logging_handler-1.0.6/src/logging_handler.egg-info/dependency_links.txt
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       16 2023-04-21 21:34:08.000000 logging_handler-1.0.6/src/logging_handler.egg-info/top_level.txt
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-07-26 20:43:15.896707 logging_handler-1.0.7/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1069 2023-07-19 07:12:34.000000 logging_handler-1.0.7/LICENSE
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4004 2023-07-26 20:43:15.896707 logging_handler-1.0.7/PKG-INFO
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3278 2023-07-19 07:12:34.000000 logging_handler-1.0.7/README.md
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      804 2023-07-26 02:40:01.000000 logging_handler-1.0.7/pyproject.toml
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       38 2023-07-26 20:43:15.896707 logging_handler-1.0.7/setup.cfg
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-07-26 20:43:15.896707 logging_handler-1.0.7/src/
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-07-26 20:43:15.896707 logging_handler-1.0.7/src/logging_handler/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4698 2023-07-26 02:40:06.000000 logging_handler-1.0.7/src/logging_handler/__init__.py
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-07-26 20:43:15.896707 logging_handler-1.0.7/src/logging_handler.egg-info/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4004 2023-07-26 20:43:15.000000 logging_handler-1.0.7/src/logging_handler.egg-info/PKG-INFO
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      236 2023-07-26 20:43:15.000000 logging_handler-1.0.7/src/logging_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)        1 2023-07-26 20:43:15.000000 logging_handler-1.0.7/src/logging_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       16 2023-07-26 20:43:15.000000 logging_handler-1.0.7/src/logging_handler.egg-info/top_level.txt
```

### Comparing `logging_handler-1.0.6/LICENSE` & `logging_handler-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `logging_handler-1.0.6/PKG-INFO` & `logging_handler-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logging_handler
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python Library to quickly create logging handlers
 Author-email: Thomas Dunteman <git@learningtopi.com>
 Project-URL: Homepage, https://www.learningtopi.com/python-modules-applications/python_logging_handler/
 Project-URL: Bug Tracker, https://github.com/LearningToPi/logging_handler/issues
 Project-URL: Source Code, https://github.com/LearningToPi/logging_handler
 Keywords: logging,syslog
 Classifier: Topic :: System :: Logging
```

### Comparing `logging_handler-1.0.6/README.md` & `logging_handler-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `logging_handler-1.0.6/pyproject.toml` & `logging_handler-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "logging_handler"
-version = "1.0.6"
+version = "1.0.7"
 description = "Python Library to quickly create logging handlers"
 authors = [{name = "Thomas Dunteman", email= "git@learningtopi.com"}]
 keywords = ["logging", "syslog"]
 readme = "README.md"
 requires-python =">=3.6"
 classifiers = [
     "Topic :: System :: Logging",
```

### Comparing `logging_handler-1.0.6/src/logging_handler/__init__.py` & `logging_handler-1.0.7/src/logging_handler/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,86 +24,87 @@
 '''
 import logging
 import logging.handlers
 from glob import glob
 from datetime import datetime, timedelta
 import pathlib
 import os
-from functools import singledispatch
 
-__VERSION__ = (1, 0, 2)
+__VERSION__ = (1, 0, 7)
 
-DEBUG = logging.DEBUG
-INFO = logging.INFO
-WARNING = logging.WARNING
-ERROR = logging.ERROR
-CRITICAL = logging.CRITICAL
-
-_log_level_name = {
-    'DEBUG': DEBUG,
-    "INFO": INFO,
-    "WARNING": WARNING,
-    "ERROR": ERROR,
-    "CRITICAL": CRITICAL
-}
+DEFAULT_LEVEL = logging.WARNING
 
-_supported_log_levels = [DEBUG, INFO, WARNING, ERROR, CRITICAL]
+DEBUG = 'DEBUG'
+INFO = 'INFO'
+WARNING = 'WARNING'
+ERROR = 'ERROR'
+CRITICAL = 'CRITICAL'
+
+_log_level_number = {
+    'DEBUG': logging.DEBUG,
+    "INFO": logging.INFO,
+    "WARNING": logging.WARNING,
+    "ERROR": logging.ERROR,
+    "CRITICAL": logging.CRITICAL
+}
 
 
 def create_logger(console_level=WARNING, log_file='', file_level=WARNING, name='', file_mode='a', console=True,
-                  syslog=False, syslog_script_name='', log_file_vars=[], log_file_retention_days=0, propagate=False):
+                  syslog=False, syslog_script_name='', log_file_vars=None, log_file_retention_days=0, propagate=False):
     """ Creates a logger and returns the handle.
-        Log file vars should be sent as a dict -> {"var": "{date}", "set": "%Y-%m-%d-%Y-%M"}
+        Log file vars should be sent as a list of dict -> [{"var": "{date}", "set": "%Y-%m-%d-%Y-%M"}]
 
         Supported log file vars:
             {date} - will be replaced with the current date using the provided strftime format
     
      """
     logger = logging.getLogger(name)
     logger.handlers.clear() # Clear all existing handlers before creating new ones!
     logger.setLevel(logging.DEBUG)
     logger.propagate = propagate
     formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 
     # Console
     if console:
         console_handler = logging.StreamHandler()
-        console_handler.setLevel(_log_level_name.get(console_level.upper(), logging.INFO) if not isinstance(console_level, int) else console_level)
+        console_handler.setLevel(console_level if isinstance(console_level, int) else _log_level_number.get(str(console_level).upper(), DEFAULT_LEVEL))
         console_handler.setFormatter(formatter)
         logger.addHandler(console_handler)
 
     # syslog
     if syslog:
         syslog_formatter = logging.Formatter(syslog_script_name + '[%(process)d]: %(levelname)s: %(message)s')
         syslog_handler = logging.handlers.SysLogHandler(address='/dev/log')
-        syslog_handler.setLevel(_log_level_name.get(file_level.upper(), logging.WARNING) if not isinstance(file_level, int) else file_level)
+        syslog_handler.setLevel(file_level if isinstance(file_level, int) else _log_level_number.get(str(file_level).upper(), DEFAULT_LEVEL))
         syslog_handler.setFormatter(syslog_formatter)
         logger.addHandler(syslog_handler)
 
     # file
     if log_file != '':
         # replace variables in the log file name
-        for var in log_file_vars:
-            if type(var) == dict and 'var' in var and 'set' in var and var['var'] == "{date}":
-                log_file = log_file.replace(var['var'], datetime.now().strftime(var['set']))
+        if log_file_vars is not None:
+            for var in log_file_vars:
+                if isinstance(var, dict) and 'var' in var and 'set' in var and var['var'] == "{date}":
+                    log_file = log_file.replace(var['var'], datetime.now().strftime(var['set']))
         file_handler = logging.FileHandler(log_file, mode=file_mode, encoding='utf-8', delay=False)
-        file_handler.setLevel(_log_level_name.get(file_level.upper(), logging.WARNING) if not isinstance(file_level, int) else file_level)
+        file_handler.setLevel(file_level if isinstance(file_level, int) else _log_level_number.get(str(file_level).upper(), DEFAULT_LEVEL))
         file_handler.setFormatter(formatter)
         logger.addHandler(file_handler)
 
         # manage retention
         if log_file_retention_days > 0:
             # replace variables with a *
             log_file_search_name = log_file
-            for var in log_file_vars:
-                log_file_search_name.replace(var['var'], '*')
+            if log_file_vars is not None:
+                for var in log_file_vars:
+                    log_file_search_name.replace(var['var'], '*')
             old_log_files = glob(log_file_search_name)
             for old_log_file in old_log_files:
                 # check the age and delete if needed
                 fname = pathlib.Path(old_log_file)
                 mtime = datetime.fromtimestamp(fname.stat().st_mtime)
                 if mtime < datetime.now() - timedelta(days=log_file_retention_days):
                     logger.info('Deleting old log file %s.  Modified time %s, retention set to %i days.', old_log_file, mtime, log_file_retention_days)
                     os.remove(old_log_file)
 
     # return the logger
-    return logger
+    return logger
```

### Comparing `logging_handler-1.0.6/src/logging_handler.egg-info/PKG-INFO` & `logging_handler-1.0.7/src/logging_handler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logging-handler
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python Library to quickly create logging handlers
 Author-email: Thomas Dunteman <git@learningtopi.com>
 Project-URL: Homepage, https://www.learningtopi.com/python-modules-applications/python_logging_handler/
 Project-URL: Bug Tracker, https://github.com/LearningToPi/logging_handler/issues
 Project-URL: Source Code, https://github.com/LearningToPi/logging_handler
 Keywords: logging,syslog
 Classifier: Topic :: System :: Logging
```

