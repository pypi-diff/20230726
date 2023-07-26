# Comparing `tmp/mikkoo-2.2.0.tar.gz` & `tmp/mikkoo-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikkoo-2.2.0.tar", last modified: Thu Jun 22 18:48:48 2023, max compression
+gzip compressed data, was "mikkoo-2.2.1.tar", last modified: Wed Jul 26 00:25:07 2023, max compression
```

## Comparing `mikkoo-2.2.0.tar` & `mikkoo-2.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:48:47.968052 mikkoo-2.2.0/
--rw-r--r--   0 root         (0) root         (0)     1481 2023-06-22 18:48:46.000000 mikkoo-2.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    19008 2023-06-22 18:48:47.968052 mikkoo-2.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17870 2023-06-22 18:48:46.000000 mikkoo-2.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:48:47.964053 mikkoo-2.2.0/mikkoo/
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-22 18:48:46.000000 mikkoo-2.2.0/mikkoo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1996 2023-06-22 18:48:46.000000 mikkoo-2.2.0/mikkoo/controller.py
--rw-r--r--   0 root         (0) root         (0)    15839 2023-06-22 18:48:46.000000 mikkoo-2.2.0/mikkoo/mcp.py
--rw-r--r--   0 root         (0) root         (0)     3462 2023-06-22 18:48:46.000000 mikkoo-2.2.0/mikkoo/state.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-06-22 18:48:46.000000 mikkoo-2.2.0/mikkoo/stats.py
--rw-r--r--   0 root         (0) root         (0)    29898 2023-06-22 18:48:46.000000 mikkoo-2.2.0/mikkoo/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:48:47.968052 mikkoo-2.2.0/mikkoo.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19008 2023-06-22 18:48:47.000000 mikkoo-2.2.0/mikkoo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-22 18:48:47.000000 mikkoo-2.2.0/mikkoo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 18:48:47.000000 mikkoo-2.2.0/mikkoo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-22 18:48:47.000000 mikkoo-2.2.0/mikkoo.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      357 2023-06-22 18:48:47.000000 mikkoo-2.2.0/mikkoo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-22 18:48:47.000000 mikkoo-2.2.0/mikkoo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 18:48:47.000000 mikkoo-2.2.0/mikkoo.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)     2194 2023-06-22 18:48:47.968052 mikkoo-2.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       61 2023-06-22 18:48:46.000000 mikkoo-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:25:07.275823 mikkoo-2.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1481 2023-07-26 00:25:06.000000 mikkoo-2.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    19008 2023-07-26 00:25:07.275823 mikkoo-2.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17870 2023-07-26 00:25:06.000000 mikkoo-2.2.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:25:07.275823 mikkoo-2.2.1/mikkoo/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-26 00:25:06.000000 mikkoo-2.2.1/mikkoo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-07-26 00:25:06.000000 mikkoo-2.2.1/mikkoo/controller.py
+-rw-r--r--   0 root         (0) root         (0)    16019 2023-07-26 00:25:06.000000 mikkoo-2.2.1/mikkoo/mcp.py
+-rw-r--r--   0 root         (0) root         (0)     3462 2023-07-26 00:25:06.000000 mikkoo-2.2.1/mikkoo/state.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-07-26 00:25:06.000000 mikkoo-2.2.1/mikkoo/stats.py
+-rw-r--r--   0 root         (0) root         (0)    29898 2023-07-26 00:25:06.000000 mikkoo-2.2.1/mikkoo/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:25:07.275823 mikkoo-2.2.1/mikkoo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19008 2023-07-26 00:25:07.000000 mikkoo-2.2.1/mikkoo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      347 2023-07-26 00:25:07.000000 mikkoo-2.2.1/mikkoo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:25:07.000000 mikkoo-2.2.1/mikkoo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-26 00:25:07.000000 mikkoo-2.2.1/mikkoo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      357 2023-07-26 00:25:07.000000 mikkoo-2.2.1/mikkoo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-26 00:25:07.000000 mikkoo-2.2.1/mikkoo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:25:07.000000 mikkoo-2.2.1/mikkoo.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-07-26 00:25:07.275823 mikkoo-2.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-26 00:25:06.000000 mikkoo-2.2.1/setup.py
```

### Comparing `mikkoo-2.2.0/LICENSE` & `mikkoo-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mikkoo-2.2.0/PKG-INFO` & `mikkoo-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikkoo
-Version: 2.2.0
+Version: 2.2.1
 Summary: Mikkoo is a PgQ to RabbitMQ Relay
 Home-page: https://github.com/gmr/mikkoo
 Author: Gavin M. Roy
 Author-email: gavinmroy@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/gmr/mikkoo/issues
 Project-URL: Documentation, https://mikkoo.readthedocs.io
```

### Comparing `mikkoo-2.2.0/README.rst` & `mikkoo-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `mikkoo-2.2.0/mikkoo/controller.py` & `mikkoo-2.2.1/mikkoo/controller.py`

 * *Files identical despite different names*

### Comparing `mikkoo-2.2.0/mikkoo/mcp.py` & `mikkoo-2.2.1/mikkoo/mcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,19 @@
             'poll_interval', self.POLL_INTERVAL)
 
     @property
     def active_processes(self) -> typing.List[psutil.Process]:
         """Return a list of all active processes, pruning dead ones"""
         active_processes, dead_processes = [], []
         for name in self.workers.keys():
+            if not self.workers[name].process:
+                LOGGER.warning('Missing process for %s', name)
+                dead_processes.append(name)
+                continue
+
             if self.workers[name].process.pid == os.getpid():
                 continue
             try:
                 proc = psutil.Process(self.workers[name].process.pid)
             except psutil.NoSuchProcess:
                 dead_processes.append(name)
                 continue
```

### Comparing `mikkoo-2.2.0/mikkoo/state.py` & `mikkoo-2.2.1/mikkoo/state.py`

 * *Files identical despite different names*

### Comparing `mikkoo-2.2.0/mikkoo/stats.py` & `mikkoo-2.2.1/mikkoo/stats.py`

 * *Files identical despite different names*

### Comparing `mikkoo-2.2.0/mikkoo/worker.py` & `mikkoo-2.2.1/mikkoo/worker.py`

 * *Files identical despite different names*

### Comparing `mikkoo-2.2.0/mikkoo.egg-info/PKG-INFO` & `mikkoo-2.2.1/mikkoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mikkoo
-Version: 2.2.0
+Version: 2.2.1
 Summary: Mikkoo is a PgQ to RabbitMQ Relay
 Home-page: https://github.com/gmr/mikkoo
 Author: Gavin M. Roy
 Author-email: gavinmroy@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/gmr/mikkoo/issues
 Project-URL: Documentation, https://mikkoo.readthedocs.io
```

### Comparing `mikkoo-2.2.0/setup.cfg` & `mikkoo-2.2.1/setup.cfg`

 * *Files identical despite different names*

