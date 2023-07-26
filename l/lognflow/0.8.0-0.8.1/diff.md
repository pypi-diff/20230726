# Comparing `tmp/lognflow-0.8.0.tar.gz` & `tmp/lognflow-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.8.0.tar", last modified: Tue Jul 25 12:09:07 2023, max compression
+gzip compressed data, was "lognflow-0.8.1.tar", last modified: Wed Jul 26 05:02:09 2023, max compression
```

## Comparing `lognflow-0.8.0.tar` & `lognflow-0.8.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:09:07.586255 lognflow-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-25 12:08:55.000000 lognflow-0.8.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-25 12:08:55.000000 lognflow-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-25 12:08:55.000000 lognflow-0.8.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-25 12:08:55.000000 lognflow-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-25 12:08:55.000000 lognflow-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-25 12:09:07.586255 lognflow-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-25 12:08:55.000000 lognflow-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:09:07.586255 lognflow-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 12:08:55.000000 lognflow-0.8.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:09:07.586255 lognflow-0.8.0/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-25 12:08:55.000000 lognflow-0.8.0/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64082 2023-07-25 12:08:55.000000 lognflow-0.8.0/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-07-25 12:08:55.000000 lognflow-0.8.0/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-25 12:08:55.000000 lognflow-0.8.0/lognflow/printprogress.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-25 12:08:55.000000 lognflow-0.8.0/lognflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:09:07.586255 lognflow-0.8.0/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-25 12:09:07.000000 lognflow-0.8.0/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-25 12:09:07.000000 lognflow-0.8.0/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:09:07.000000 lognflow-0.8.0/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:09:07.000000 lognflow-0.8.0/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-25 12:09:07.000000 lognflow-0.8.0/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 12:09:07.000000 lognflow-0.8.0/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-25 12:09:07.586255 lognflow-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-25 12:08:55.000000 lognflow-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:09:07.586255 lognflow-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-25 12:08:55.000000 lognflow-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-25 12:08:55.000000 lognflow-0.8.0/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-07-25 12:08:55.000000 lognflow-0.8.0/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-25 12:08:55.000000 lognflow-0.8.0/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:02:09.138044 lognflow-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-26 05:01:56.000000 lognflow-0.8.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-26 05:01:56.000000 lognflow-0.8.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-26 05:01:56.000000 lognflow-0.8.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-26 05:01:56.000000 lognflow-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-26 05:01:56.000000 lognflow-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-07-26 05:02:09.138044 lognflow-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-26 05:01:56.000000 lognflow-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:02:09.130044 lognflow-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 05:01:56.000000 lognflow-0.8.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:02:09.130044 lognflow-0.8.1/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-26 05:01:56.000000 lognflow-0.8.1/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63990 2023-07-26 05:01:56.000000 lognflow-0.8.1/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-07-26 05:01:56.000000 lognflow-0.8.1/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-26 05:01:56.000000 lognflow-0.8.1/lognflow/printprogress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-26 05:01:56.000000 lognflow-0.8.1/lognflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:02:09.134044 lognflow-0.8.1/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-07-26 05:02:09.000000 lognflow-0.8.1/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-26 05:02:09.000000 lognflow-0.8.1/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 05:02:09.000000 lognflow-0.8.1/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 05:02:08.000000 lognflow-0.8.1/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 05:02:09.000000 lognflow-0.8.1/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 05:02:09.000000 lognflow-0.8.1/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-26 05:02:09.138044 lognflow-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-26 05:01:56.000000 lognflow-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:02:09.138044 lognflow-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-26 05:01:56.000000 lognflow-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-26 05:01:56.000000 lognflow-0.8.1/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-07-26 05:01:56.000000 lognflow-0.8.1/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-26 05:01:56.000000 lognflow-0.8.1/tests/test_printprogress.py
```

### Comparing `lognflow-0.8.0/CONTRIBUTING.rst` & `lognflow-0.8.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.0/HISTORY.rst` & `lognflow-0.8.1/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -118,8 +118,12 @@
 * If variable name is splitable, we replace them with _
 
 0.8.0 (2023-07-25)
 ------------------
 * logger.save and savez are set to be identical to log_single.
 * logged.load is set to be identical to get_single.
 * utils.py is added to contain all misc functions.
-* replace_all added to utils
+* replace_all added to utils
+
+0.8.1 (2023-07-26)
+------------------
+* a bug fixed in log_var
```

### Comparing `lognflow-0.8.0/LICENSE` & `lognflow-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.0/PKG-INFO` & `lognflow-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.8.0
+Version: 0.8.1
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -212,7 +212,11 @@
 
 0.8.0 (2023-07-25)
 ------------------
 * logger.save and savez are set to be identical to log_single.
 * logged.load is set to be identical to get_single.
 * utils.py is added to contain all misc functions.
 * replace_all added to utils
+
+0.8.1 (2023-07-26)
+------------------
+* a bug fixed in log_var
```

### Comparing `lognflow-0.8.0/README.rst` & `lognflow-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.0/docs/Makefile` & `lognflow-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.0/docs/conf.py` & `lognflow-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.0/docs/installation.rst` & `lognflow-0.8.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.0/docs/make.bat` & `lognflow-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.0/lognflow/lognflow.py` & `lognflow-0.8.1/lognflow/lognflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -553,28 +553,25 @@
                     path like name such as myscript/myvar.
         """
         param_dir, param_name = self._prepare_param_dir(parameter_name)
         
         _var = self._vars_dict[parameter_name]
         _var_data_array = _var.data_array[_var.time_array > 0]
         _var_time_array = _var.time_array[_var.time_array > 0]
-        if((_var.save_as == 'npz')):# | (_var.save_as == 'npy')):
+        if((_var.save_as == 'npz') | (_var.save_as == 'npy')):
             fpath = param_dir / f'{param_name}_{_var.file_start_time}.npz'
             np.savez(fpath,
                 time_array = _var_time_array,
                 data_array = _var_data_array)
-        else:#if(_var.save_as == 'txt'):
+        else:
             fpath = param_dir / f'{param_name}_time_{_var.file_start_time}.txt'
             np.savetxt(fpath, _var_time_array)
             fpath = param_dir / f'{param_name}_data_{_var.file_start_time}.txt'
             np.savetxt(fpath, _var_data_array)
-        try:
-            return fpath
-        except:
-            print('here')
+        return fpath
     
     def get_var(self, parameter_name: str) -> tuple:
         """ Get the buffered numpy arrays
             If you need the buffered variable back.
             :param parameter_name: str
                 examples: myvar or myscript/myvar
                     parameter_name can be just a name e.g. myvar, or could be a
@@ -1438,15 +1435,16 @@
         ims = []
         for img in stack:    
             im = ax.imshow(img, animated=True)
             plt.xticks([]),plt.yticks([])
             ims.append([im])
         ani = animation.ArtistAnimation(\
             fig, ims, interval = interval, blit = blit,
-            repeat_delay = repeat_delay)    
+            repeat_delay = repeat_delay)
+
         ani.save(fpath, dpi = dpi, 
                  writer = animation.PillowWriter(fps=int(1000/interval)))
         return fpath
 
     def replace_time_with_index(self, var_name):
         """ index in file names
             lognflow uses time stamps to make new log files for a variable.
```

### Comparing `lognflow-0.8.0/lognflow/logviewer.py` & `lognflow-0.8.1/lognflow/logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.0/lognflow/printprogress.py` & `lognflow-0.8.1/lognflow/printprogress.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.0/lognflow/utils.py` & `lognflow-0.8.1/lognflow/utils.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.0/lognflow.egg-info/PKG-INFO` & `lognflow-0.8.1/lognflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.8.0
+Version: 0.8.1
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -212,7 +212,11 @@
 
 0.8.0 (2023-07-25)
 ------------------
 * logger.save and savez are set to be identical to log_single.
 * logged.load is set to be identical to get_single.
 * utils.py is added to contain all misc functions.
 * replace_all added to utils
+
+0.8.1 (2023-07-26)
+------------------
+* a bug fixed in log_var
```

### Comparing `lognflow-0.8.0/lognflow.egg-info/SOURCES.txt` & `lognflow-0.8.1/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.0/setup.py` & `lognflow-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.8.0'
+__version__ = '0.8.1'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.8.0/tests/test_lognflow.py` & `lognflow-0.8.1/tests/test_lognflow.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.0/tests/test_logviewer.py` & `lognflow-0.8.1/tests/test_logviewer.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.8.0/tests/test_printprogress.py` & `lognflow-0.8.1/tests/test_printprogress.py`

 * *Files identical despite different names*

