# Comparing `tmp/clearconf-0.3.5.tar.gz` & `tmp/clearconf-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clearconf-0.3.5.tar", max compression
+gzip compressed data, was "clearconf-0.3.6.tar", max compression
```

## Comparing `clearconf-0.3.5.tar` & `clearconf-0.3.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2786 2023-07-19 06:41:06.394975 clearconf-0.3.5/README.md
--rw-r--r--   0        0        0       37 2023-07-19 06:41:06.394975 clearconf-0.3.5/clearconf/__init__.py
--rw-r--r--   0        0        0     1745 2023-07-19 06:41:06.394975 clearconf-0.3.5/clearconf/assets/example_conf.py
--rw-r--r--   0        0        0      968 2023-07-19 06:41:06.394975 clearconf-0.3.5/clearconf/assets/init.py
--rw-r--r--   0        0        0      213 2023-07-19 06:41:06.394975 clearconf-0.3.5/clearconf/assets/stub_conf.py
--rw-r--r--   0        0        0     7491 2023-07-25 11:08:48.171745 clearconf-0.3.5/clearconf/base_config.py
--rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.5/clearconf/cli/__init__.py
--rw-r--r--   0        0        0      930 2023-07-19 06:41:06.394975 clearconf-0.3.5/clearconf/cli/defaults.py
--rw-r--r--   0        0        0     1729 2023-07-19 06:41:06.394975 clearconf-0.3.5/clearconf/cli/main.py
--rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.5/clearconf/utils/__init__.py
--rw-r--r--   0        0        0      746 2023-07-19 06:41:06.394975 clearconf-0.3.5/clearconf/utils/conf.py
--rw-r--r--   0        0        0      917 2023-07-19 06:41:06.394975 clearconf-0.3.5/clearconf/utils/file.py
--rw-r--r--   0        0        0      509 2023-07-19 06:41:06.394975 clearconf-0.3.5/clearconf/utils/stdout.py
--rw-r--r--   0        0        0      728 2023-07-25 11:06:51.882551 clearconf-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     3529 1970-01-01 00:00:00.000000 clearconf-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     2786 2023-07-19 06:41:06.394975 clearconf-0.3.6/README.md
+-rw-r--r--   0        0        0       37 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/__init__.py
+-rw-r--r--   0        0        0     1745 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/assets/example_conf.py
+-rw-r--r--   0        0        0      968 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/assets/init.py
+-rw-r--r--   0        0        0      213 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/assets/stub_conf.py
+-rw-r--r--   0        0        0     7569 2023-07-26 13:03:32.560181 clearconf-0.3.6/clearconf/base_config.py
+-rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/cli/__init__.py
+-rw-r--r--   0        0        0      930 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/cli/defaults.py
+-rw-r--r--   0        0        0     1729 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/cli/main.py
+-rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/utils/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/utils/conf.py
+-rw-r--r--   0        0        0      917 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/utils/file.py
+-rw-r--r--   0        0        0      509 2023-07-19 06:41:06.394975 clearconf-0.3.6/clearconf/utils/stdout.py
+-rw-r--r--   0        0        0      729 2023-07-26 13:04:13.980596 clearconf-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3530 1970-01-01 00:00:00.000000 clearconf-0.3.6/PKG-INFO
```

### Comparing `clearconf-0.3.5/README.md` & `clearconf-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.5/clearconf/assets/example_conf.py` & `clearconf-0.3.6/clearconf/assets/example_conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.5/clearconf/assets/init.py` & `clearconf-0.3.6/clearconf/assets/init.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.5/clearconf/base_config.py` & `clearconf-0.3.6/clearconf/base_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,20 @@
                     if type(attr).__name__ == 'function':
                         if attr.__name__ == '<lambda>':
                             funcString = str(inspect.getsourcelines(attr)[0])
                             res[k] = funcString.strip("['\\n']").split(" = ")[1]
                         else:
                             res[k] = f'function : {attr.__name__}'
                     elif attr.__module__.split('.')[0] == '__main__' or 'config' in attr.__module__:
-                        if len(attr.mro()) >= 5: # when a config class is subclassed to use it directly
-                            subclass_name = [a for a in [a.__name__ for a in attr.mro()] if a not in [k, f'{k}_Mod', 'BaseConfig']][0]
-                            k = f'{k}({subclass_name})'
+                        subclass_names = [a for a in [a.__name__ for a in attr.mro()] 
+                                     if a not in [k, f'{k}_mod', 'BaseConfig', 'object']]
+                        
+                        if len(subclass_names) > 0: # when a config class is subclassed to use it directly
+                            k = f'{k}({subclass_names[0]})'
+
                         res[k] = attr.to_dict()
                     else:
                         # End up here if attr is not a class defined inside module.
                         if type(attr).__name__ == 'type':  # it is a class
                             name = f'{attr.__module__}.{attr.__name__}'
                         else: # it is an object
                             if attr.__str__ is not object.__str__:
```

### Comparing `clearconf-0.3.5/clearconf/cli/defaults.py` & `clearconf-0.3.6/clearconf/cli/defaults.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.5/clearconf/cli/main.py` & `clearconf-0.3.6/clearconf/cli/main.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.5/clearconf/utils/conf.py` & `clearconf-0.3.6/clearconf/utils/conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.5/clearconf/utils/file.py` & `clearconf-0.3.6/clearconf/utils/file.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.5/pyproject.toml` & `clearconf-0.3.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "clearconf"
-version = "0.3.5"
+version = "0.3.6"
 description = "ClearConf is a library created to support easy and manageble python configuration. It consists in a CLI tool to manage the configuration directory, and in a python class (BaseConfig) which adds additional functionalities to a configuration class."
-authors = ["andrearosasco <andrearosasco.ar@gmail.com>"]
+authors = ["Andrea Rosasco <andrearosasco.ar@gmail.com>"]
 homepage = "https://github.com/andrearosasco/clearconf"
 repository = "https://github.com/andrearosasco/clearconf"
 readme = "README.md"
 
 
 [tool.poetry.scripts]
 cconf = "clearconf.cli.main:main"
```

### Comparing `clearconf-0.3.5/PKG-INFO` & `clearconf-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: clearconf
-Version: 0.3.5
+Version: 0.3.6
 Summary: ClearConf is a library created to support easy and manageble python configuration. It consists in a CLI tool to manage the configuration directory, and in a python class (BaseConfig) which adds additional functionalities to a configuration class.
 Home-page: https://github.com/andrearosasco/clearconf
-Author: andrearosasco
+Author: Andrea Rosasco
 Author-email: andrearosasco.ar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

