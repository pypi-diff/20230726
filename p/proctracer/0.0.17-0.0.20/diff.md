# Comparing `tmp/proctracer-0.0.17.tar.gz` & `tmp/proctracer-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proctracer-0.0.17.tar", last modified: Tue Jul 25 11:38:31 2023, max compression
+gzip compressed data, was "proctracer-0.0.20.tar", last modified: Wed Jul 26 19:54:45 2023, max compression
```

## Comparing `proctracer-0.0.17.tar` & `proctracer-0.0.20.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 11:38:31.943454 proctracer-0.0.17/
--rw-r--r--   0 root         (0) root         (0)     1498 2023-07-25 07:18:11.000000 proctracer-0.0.17/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 07:18:11.000000 proctracer-0.0.17/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 11:38:31.943454 proctracer-0.0.17/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1631 2023-07-25 07:18:11.000000 proctracer-0.0.17/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 11:38:31.939454 proctracer-0.0.17/proctracer/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-25 11:37:04.000000 proctracer-0.0.17/proctracer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 11:38:31.943454 proctracer-0.0.17/proctracer/plugins/
--rw-r--r--   0 root         (0) root         (0)      589 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3731 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/plugins/net_dev.plugin.py
--rw-r--r--   0 root         (0) root         (0)     3310 2023-07-25 11:37:39.000000 proctracer-0.0.17/proctracer/plugins/net_snmp_udp.plugin.py
--rw-r--r--   0 root         (0) root         (0)     6459 2023-07-25 11:38:03.000000 proctracer-0.0.17/proctracer/plugins/net_udpX.plugin.py
--rw-r--r--   0 root         (0) root         (0)     5625 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/plugins/pid_stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     3285 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/plugins/plugin_base.py
--rw-r--r--   0 root         (0) root         (0)     4977 2023-07-25 10:45:01.000000 proctracer-0.0.17/proctracer/plugins/plugin_proc_tracer_base.py
--rw-r--r--   0 root         (0) root         (0)     2876 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/plugins/pressure_X.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/plugins/stat.plugin.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/plugins/text_pipe.plugin.py
--rwxr-xr-x   0 root         (0) root         (0)     4706 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/proctracer.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-25 07:18:11.000000 proctracer-0.0.17/proctracer/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 11:38:31.939454 proctracer-0.0.17/proctracer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2747 2023-07-25 11:38:31.000000 proctracer-0.0.17/proctracer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      712 2023-07-25 11:38:31.000000 proctracer-0.0.17/proctracer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 11:38:31.000000 proctracer-0.0.17/proctracer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-07-25 11:38:31.000000 proctracer-0.0.17/proctracer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-25 11:38:31.000000 proctracer-0.0.17/proctracer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 11:38:31.000000 proctracer-0.0.17/proctracer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-25 11:38:31.943454 proctracer-0.0.17/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4836 2023-07-25 07:18:11.000000 proctracer-0.0.17/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 19:54:45.644325 proctracer-0.0.20/
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-07-25 07:18:11.000000 proctracer-0.0.20/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 07:18:11.000000 proctracer-0.0.20/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3521 2023-07-26 19:54:45.644325 proctracer-0.0.20/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-07-26 19:41:27.000000 proctracer-0.0.20/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 19:54:45.644325 proctracer-0.0.20/proctracer/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-26 19:54:21.000000 proctracer-0.0.20/proctracer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 19:54:45.644325 proctracer-0.0.20/proctracer/plugins/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3731 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/plugins/net_dev.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2023-07-25 11:37:39.000000 proctracer-0.0.20/proctracer/plugins/net_snmp_udp.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     6459 2023-07-25 11:38:03.000000 proctracer-0.0.20/proctracer/plugins/net_udpX.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     5625 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/plugins/pid_stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/plugins/plugin_base.py
+-rw-r--r--   0 root         (0) root         (0)     4977 2023-07-25 10:45:01.000000 proctracer-0.0.20/proctracer/plugins/plugin_proc_tracer_base.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/plugins/pressure_X.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/plugins/stat.plugin.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/plugins/text_pipe.plugin.py
+-rwxr-xr-x   0 root         (0) root         (0)     4706 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/proctracer.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-25 07:18:11.000000 proctracer-0.0.20/proctracer/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 19:54:45.644325 proctracer-0.0.20/proctracer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3521 2023-07-26 19:54:45.000000 proctracer-0.0.20/proctracer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-26 19:54:45.000000 proctracer-0.0.20/proctracer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 19:54:45.000000 proctracer-0.0.20/proctracer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-26 19:54:45.000000 proctracer-0.0.20/proctracer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-26 19:54:45.000000 proctracer-0.0.20/proctracer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-26 19:54:45.000000 proctracer-0.0.20/proctracer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-26 19:54:45.644325 proctracer-0.0.20/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4895 2023-07-26 19:20:43.000000 proctracer-0.0.20/setup.py
```

### Comparing `proctracer-0.0.17/LICENSE.md` & `proctracer-0.0.20/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.17/proctracer/plugins/__init__.py` & `proctracer-0.0.20/proctracer/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.17/proctracer/plugins/net_dev.plugin.py` & `proctracer-0.0.20/proctracer/plugins/net_dev.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.17/proctracer/plugins/net_snmp_udp.plugin.py` & `proctracer-0.0.20/proctracer/plugins/net_snmp_udp.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.17/proctracer/plugins/net_udpX.plugin.py` & `proctracer-0.0.20/proctracer/plugins/net_udpX.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.17/proctracer/plugins/pid_stat.plugin.py` & `proctracer-0.0.20/proctracer/plugins/pid_stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.17/proctracer/plugins/plugin_base.py` & `proctracer-0.0.20/proctracer/plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.17/proctracer/plugins/plugin_proc_tracer_base.py` & `proctracer-0.0.20/proctracer/plugins/plugin_proc_tracer_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.17/proctracer/plugins/pressure_X.plugin.py` & `proctracer-0.0.20/proctracer/plugins/pressure_X.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.17/proctracer/plugins/stat.plugin.py` & `proctracer-0.0.20/proctracer/plugins/stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.17/proctracer/plugins/text_pipe.plugin.py` & `proctracer-0.0.20/proctracer/plugins/text_pipe.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.17/proctracer/proctracer.py` & `proctracer-0.0.20/proctracer/proctracer.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.17/proctracer.egg-info/SOURCES.txt` & `proctracer-0.0.20/proctracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.17/setup.py` & `proctracer-0.0.20/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,27 +60,28 @@
     version=load_version(),  # + ".rc1",
 
     description='/proc Tracer',
     long_description=generate_long_description_file(),
     long_description_content_type='text/markdown',
 
     # The project's main homepage.
-    url='https://proctracer.io',
+    url='https://github.com/david-kracht/proctracer',
     project_urls={
         'Documentation': 'https://github.com/david-kracht/proctracer',
         'Source': 'https://github.com/david-kracht/proctracer.git',
         'Tracker': 'https://github.com/david-kracht/proctracer/issues',
     },
 
     # Author details
     author='David Kracht',
     author_email='dave.kracht@gmail.com',
 
     # Choose your license
     license='BSD-3',
+    license_files = ('LICENSE.md',), 
 
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8'
```

