# Comparing `tmp/clearconf-0.3.6.tar.gz` & `tmp/clearconf-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clearconf-0.3.6.tar", max compression
+gzip compressed data, was "clearconf-0.3.7.tar", max compression
```

## Comparing `clearconf-0.3.6.tar` & `clearconf-0.3.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2786 2023-07-19 06:41:06.394975 clearconf-0.3.6/README.md
--rw-r--r--   0        0        0       37 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/__init__.py
--rw-r--r--   0        0        0     1745 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/assets/example_conf.py
--rw-r--r--   0        0        0      968 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/assets/init.py
--rw-r--r--   0        0        0      213 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/assets/stub_conf.py
--rw-r--r--   0        0        0     7569 2023-07-26 13:03:32.560181 clearconf-0.3.6/clearconf/base_config.py
--rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/cli/__init__.py
--rw-r--r--   0        0        0      930 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/cli/defaults.py
--rw-r--r--   0        0        0     1729 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/cli/main.py
--rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/utils/__init__.py
--rw-r--r--   0        0        0      746 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/utils/conf.py
--rw-r--r--   0        0        0      917 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/utils/file.py
--rw-r--r--   0        0        0      509 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/utils/stdout.py
--rw-r--r--   0        0        0      729 2023-07-26 13:04:13.980596 clearconf-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     3530 1970-01-01 00:00:00.000000 clearconf-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     2786 2023-07-19 06:41:06.394975 clearconf-0.3.7/README.md
+-rw-r--r--   0        0        0       37 2023-07-19 06:41:06.394975 clearconf-0.3.7/clearconf/__init__.py
+-rw-r--r--   0        0        0     1745 2023-07-19 06:41:06.394975 clearconf-0.3.7/clearconf/assets/example_conf.py
+-rw-r--r--   0        0        0      968 2023-07-19 06:41:06.394975 clearconf-0.3.7/clearconf/assets/init.py
+-rw-r--r--   0        0        0      213 2023-07-19 06:41:06.394975 clearconf-0.3.7/clearconf/assets/stub_conf.py
+-rw-r--r--   0        0        0     7682 2023-07-26 16:57:04.301719 clearconf-0.3.7/clearconf/base_config.py
+-rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.7/clearconf/cli/__init__.py
+-rw-r--r--   0        0        0      930 2023-07-19 06:41:06.394975 clearconf-0.3.7/clearconf/cli/defaults.py
+-rw-r--r--   0        0        0     1729 2023-07-19 06:41:06.394975 clearconf-0.3.7/clearconf/cli/main.py
+-rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.7/clearconf/utils/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-19 06:41:06.394975 clearconf-0.3.7/clearconf/utils/conf.py
+-rw-r--r--   0        0        0      917 2023-07-19 06:41:06.394975 clearconf-0.3.7/clearconf/utils/file.py
+-rw-r--r--   0        0        0      509 2023-07-19 06:41:06.394975 clearconf-0.3.7/clearconf/utils/stdout.py
+-rw-r--r--   0        0        0      729 2023-07-26 16:57:10.773784 clearconf-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     3530 1970-01-01 00:00:00.000000 clearconf-0.3.7/PKG-INFO
```

### Comparing `clearconf-0.3.6/README.md` & `clearconf-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.6/clearconf/assets/example_conf.py` & `clearconf-0.3.7/clearconf/assets/example_conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.6/clearconf/assets/init.py` & `clearconf-0.3.7/clearconf/assets/init.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.6/clearconf/base_config.py` & `clearconf-0.3.7/clearconf/base_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,18 +35,19 @@
                 key =  target.mro()[2].__name__
             if len(target.mro()) >= 5:
                 key = f'{key}({target.mro()[3].__name__})'
             output = {key: res}
 
         target_attr = set(dir(target))
         # This removes variables from superclasses
-        for i in range(3, len(target.__mro__) - 1):
+        for attr in [a for a in target.mro() 
+                     if a.__name__ not in [target.__name__, f'{target.__name__}_mod', target.__name__[:-4], 'BaseConfig', 'Config', 'object']]:
             # The allows inheritance between configs but I guess there are better solutions
-            if 'configs' not in target.__mro__[i].__module__:
-                target_attr = target_attr - set(dir(target.__mro__[i]))
+            if 'configs' not in attr.__module__:
+                target_attr = target_attr - set(dir(attr))
 
         for k in target_attr:
             if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict', 'get_cfg']:
                 attr = getattr(target, k)
 
                 # If it's a module get inside
                 if hasattr(attr, '__module__'):
```

### Comparing `clearconf-0.3.6/clearconf/cli/defaults.py` & `clearconf-0.3.7/clearconf/cli/defaults.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.6/clearconf/cli/main.py` & `clearconf-0.3.7/clearconf/cli/main.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.6/clearconf/utils/conf.py` & `clearconf-0.3.7/clearconf/utils/conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.6/clearconf/utils/file.py` & `clearconf-0.3.7/clearconf/utils/file.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.6/pyproject.toml` & `clearconf-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clearconf"
-version = "0.3.6"
+version = "0.3.7"
 description = "ClearConf is a library created to support easy and manageble python configuration. It consists in a CLI tool to manage the configuration directory, and in a python class (BaseConfig) which adds additional functionalities to a configuration class."
 authors = ["Andrea Rosasco <andrearosasco.ar@gmail.com>"]
 homepage = "https://github.com/andrearosasco/clearconf"
 repository = "https://github.com/andrearosasco/clearconf"
 readme = "README.md"
```

### Comparing `clearconf-0.3.6/PKG-INFO` & `clearconf-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clearconf
-Version: 0.3.6
+Version: 0.3.7
 Summary: ClearConf is a library created to support easy and manageble python configuration. It consists in a CLI tool to manage the configuration directory, and in a python class (BaseConfig) which adds additional functionalities to a configuration class.
 Home-page: https://github.com/andrearosasco/clearconf
 Author: Andrea Rosasco
 Author-email: andrearosasco.ar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

