# Comparing `tmp/mdk-5.7.2.tar.gz` & `tmp/mdk-5.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdk-5.7.2.tar", last modified: Fri Jul 21 17:56:37 2023, max compression
+gzip compressed data, was "mdk-5.7.3.tar", last modified: Tue Jul 25 23:20:51 2023, max compression
```

## Comparing `mdk-5.7.2.tar` & `mdk-5.7.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 austin    (3007) ldap-eng  (2001)        0 2023-07-21 17:56:35.177949 mdk-5.7.2/
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)     1068 2023-07-21 16:55:29.000000 mdk-5.7.2/LICENSE
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)     1430 2023-07-21 17:56:35.177949 mdk-5.7.2/PKG-INFO
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)      921 2023-07-21 16:55:29.000000 mdk-5.7.2/README.md
-drwxrwxr-x   0 austin    (3007) ldap-eng  (2001)        0 2023-07-21 17:56:35.173949 mdk-5.7.2/mdk/
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        0 2023-07-21 16:55:29.000000 mdk-5.7.2/mdk/__init__.py
--rwxrwxr-x   0 austin    (3007) ldap-eng  (2001)     3620 2023-07-21 16:55:29.000000 mdk-5.7.2/mdk/main.py
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)    16978 2023-07-21 17:49:24.000000 mdk-5.7.2/mdk/utils.py
-drwxrwxr-x   0 austin    (3007) ldap-eng  (2001)        0 2023-07-21 17:56:35.177949 mdk-5.7.2/mdk.egg-info/
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)     1430 2023-07-21 17:56:31.000000 mdk-5.7.2/mdk.egg-info/PKG-INFO
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)      241 2023-07-21 17:56:34.000000 mdk-5.7.2/mdk.egg-info/SOURCES.txt
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        1 2023-07-21 17:56:34.000000 mdk-5.7.2/mdk.egg-info/dependency_links.txt
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)       38 2023-07-21 17:56:34.000000 mdk-5.7.2/mdk.egg-info/entry_points.txt
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        9 2023-07-21 17:56:34.000000 mdk-5.7.2/mdk.egg-info/requires.txt
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        4 2023-07-21 17:56:34.000000 mdk-5.7.2/mdk.egg-info/top_level.txt
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)       67 2023-07-21 17:56:35.177949 mdk-5.7.2/setup.cfg
--rw-rw-r--   0 austin    (3007) ldap-eng  (2001)      985 2023-07-21 16:55:29.000000 mdk-5.7.2/setup.py
+drwxrwxr-x   0 austin    (3007) ldap-eng  (2001)        0 2023-07-25 23:20:51.628290 mdk-5.7.3/
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)     1068 2023-07-21 16:55:29.000000 mdk-5.7.3/LICENSE
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)     1430 2023-07-25 23:20:51.628290 mdk-5.7.3/PKG-INFO
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)      921 2023-07-21 16:55:29.000000 mdk-5.7.3/README.md
+drwxrwxr-x   0 austin    (3007) ldap-eng  (2001)        0 2023-07-25 23:20:51.628290 mdk-5.7.3/mdk/
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        0 2023-07-21 16:55:29.000000 mdk-5.7.3/mdk/__init__.py
+-rwxrwxr-x   0 austin    (3007) ldap-eng  (2001)     3620 2023-07-21 16:55:29.000000 mdk-5.7.3/mdk/main.py
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)    16978 2023-07-25 23:19:57.000000 mdk-5.7.3/mdk/utils.py
+drwxrwxr-x   0 austin    (3007) ldap-eng  (2001)        0 2023-07-25 23:20:51.628290 mdk-5.7.3/mdk.egg-info/
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)     1430 2023-07-25 23:20:51.000000 mdk-5.7.3/mdk.egg-info/PKG-INFO
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)      241 2023-07-25 23:20:51.000000 mdk-5.7.3/mdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        1 2023-07-25 23:20:51.000000 mdk-5.7.3/mdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)       38 2023-07-25 23:20:51.000000 mdk-5.7.3/mdk.egg-info/entry_points.txt
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        9 2023-07-25 23:20:51.000000 mdk-5.7.3/mdk.egg-info/requires.txt
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)        4 2023-07-25 23:20:51.000000 mdk-5.7.3/mdk.egg-info/top_level.txt
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)       67 2023-07-25 23:20:51.628290 mdk-5.7.3/setup.cfg
+-rw-rw-r--   0 austin    (3007) ldap-eng  (2001)      985 2023-07-21 16:55:29.000000 mdk-5.7.3/setup.py
```

### Comparing `mdk-5.7.2/LICENSE` & `mdk-5.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mdk-5.7.2/PKG-INFO` & `mdk-5.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdk
-Version: 5.7.2
+Version: 5.7.3
 Summary: a docker-compose helper
 Home-page: https://matician.com/
 Author: Michael Darr
 Author-email: mdarr@matician.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `mdk-5.7.2/README.md` & `mdk-5.7.3/README.md`

 * *Files identical despite different names*

### Comparing `mdk-5.7.2/mdk/main.py` & `mdk-5.7.3/mdk/main.py`

 * *Files identical despite different names*

### Comparing `mdk-5.7.2/mdk/utils.py` & `mdk-5.7.3/mdk/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -75,27 +75,27 @@
     def __init__(self):
         self.conf_version = ()
         self.conf_root = None
         self.conf_paths = []
         self.conf_data = []
         self._inspect = None
 
-        # find global user conf
-        self.conf_paths.append(Path.home()/CONFIG_EXTENSION_USER_PATH)
-
         # find nearest config file & sibling ext conf (add "_" to cwd b/c cwd().parents doesn't include cwd)
         for dir_path in (Path().cwd()/"_").parents:
             if (dir_path/CONFIG_FILENAME).is_file():
                 self.conf_root = dir_path
                 self.conf_paths.append(dir_path/CONFIG_FILENAME)
                 self.conf_paths.append(dir_path/CONFIG_EXTENSION_FILENAME)
                 break
         else:
             Log.fatal(f'{CONFIG_FILENAME} found in neither this directory nor any of its parents.')
 
+        # find global user conf
+        self.conf_paths.append(Path.home()/CONFIG_EXTENSION_USER_PATH)
+
         # load our configuration as a list of dicts, later configs override earlier ones
         self.conf_data = [json.load(open(path)) for path in self.conf_paths if path.is_file()]
 
         # ensure that we are new enough to properly parse this config
         conf_version = self.conf("mdk-version", str)
         if conf_version:
             try:
```

### Comparing `mdk-5.7.2/mdk.egg-info/PKG-INFO` & `mdk-5.7.3/mdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdk
-Version: 5.7.2
+Version: 5.7.3
 Summary: a docker-compose helper
 Home-page: https://matician.com/
 Author: Michael Darr
 Author-email: mdarr@matician.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `mdk-5.7.2/setup.py` & `mdk-5.7.3/setup.py`

 * *Files identical despite different names*

