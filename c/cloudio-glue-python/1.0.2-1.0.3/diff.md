# Comparing `tmp/cloudio-glue-python-1.0.2.tar.gz` & `tmp/cloudio-glue-python-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudio-glue-python-1.0.2.tar", last modified: Mon Jul 25 09:01:41 2022, max compression
+gzip compressed data, was "cloudio-glue-python-1.0.3.tar", last modified: Wed Jul 26 09:28:43 2023, max compression
```

## Comparing `cloudio-glue-python-1.0.2.tar` & `cloudio-glue-python-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-07-25 09:01:41.024586 cloudio-glue-python-1.0.2/
--rw-rw-rw-   0        0        0     1136 2021-03-24 07:03:12.000000 cloudio-glue-python-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     5850 2022-07-25 09:01:41.023609 cloudio-glue-python-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4557 2022-07-25 08:58:08.000000 cloudio-glue-python-1.0.2/README.md
--rw-rw-rw-   0        0        0       93 2022-07-25 06:20:23.000000 cloudio-glue-python-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-07-25 09:01:41.024586 cloudio-glue-python-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     7998 2022-07-25 08:58:08.000000 cloudio-glue-python-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-25 09:01:41.009559 cloudio-glue-python-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2022-07-25 09:01:41.013664 cloudio-glue-python-1.0.2/src/cloudio/
--rw-rw-rw-   0        0        0      304 2022-07-25 06:20:32.000000 cloudio-glue-python-1.0.2/src/cloudio/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-25 09:01:41.019561 cloudio-glue-python-1.0.2/src/cloudio/glue/
--rw-rw-rw-   0        0        0      679 2022-07-25 06:20:32.000000 cloudio-glue-python-1.0.2/src/cloudio/glue/__init__.py
--rw-rw-rw-   0        0        0     3626 2022-07-25 06:20:23.000000 cloudio-glue-python-1.0.2/src/cloudio/glue/cloudio_attribute.py
--rw-rw-rw-   0        0        0    20216 2022-07-25 08:58:08.000000 cloudio-glue-python-1.0.2/src/cloudio/glue/model_to_cloud_connector.py
--rw-rw-rw-   0        0        0      212 2022-07-25 08:58:08.000000 cloudio-glue-python-1.0.2/src/cloudio/glue/version.py
-drwxrwxrwx   0        0        0        0 2022-07-25 09:01:41.023609 cloudio-glue-python-1.0.2/src/cloudio_glue_python.egg-info/
--rw-rw-rw-   0        0        0     5850 2022-07-25 09:01:40.000000 cloudio-glue-python-1.0.2/src/cloudio_glue_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2022-07-25 09:01:41.000000 cloudio-glue-python-1.0.2/src/cloudio_glue_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-25 09:01:40.000000 cloudio-glue-python-1.0.2/src/cloudio_glue_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2022-07-25 09:01:40.000000 cloudio-glue-python-1.0.2/src/cloudio_glue_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-07-25 09:01:40.000000 cloudio-glue-python-1.0.2/src/cloudio_glue_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 09:28:43.041570 cloudio-glue-python-1.0.3/
+-rw-rw-rw-   0        0        0     1136 2021-03-24 07:03:12.000000 cloudio-glue-python-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5850 2023-07-26 09:28:43.040571 cloudio-glue-python-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4557 2022-07-25 08:58:08.000000 cloudio-glue-python-1.0.3/README.md
+-rw-rw-rw-   0        0        0       93 2022-07-25 06:20:23.000000 cloudio-glue-python-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 09:28:43.041870 cloudio-glue-python-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     7998 2022-07-25 08:58:08.000000 cloudio-glue-python-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:28:43.025567 cloudio-glue-python-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 09:28:43.029569 cloudio-glue-python-1.0.3/src/cloudio/
+-rw-rw-rw-   0        0        0      304 2022-07-25 06:20:32.000000 cloudio-glue-python-1.0.3/src/cloudio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:28:43.036568 cloudio-glue-python-1.0.3/src/cloudio/glue/
+-rw-rw-rw-   0        0        0      679 2022-07-25 06:20:32.000000 cloudio-glue-python-1.0.3/src/cloudio/glue/__init__.py
+-rw-rw-rw-   0        0        0     3804 2023-07-26 09:19:09.000000 cloudio-glue-python-1.0.3/src/cloudio/glue/cloudio_attribute.py
+-rw-rw-rw-   0        0        0    20216 2022-07-25 08:58:08.000000 cloudio-glue-python-1.0.3/src/cloudio/glue/model_to_cloud_connector.py
+-rw-rw-rw-   0        0        0      228 2023-07-26 09:19:10.000000 cloudio-glue-python-1.0.3/src/cloudio/glue/version.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:28:43.039567 cloudio-glue-python-1.0.3/src/cloudio_glue_python.egg-info/
+-rw-rw-rw-   0        0        0     5850 2023-07-26 09:28:43.000000 cloudio-glue-python-1.0.3/src/cloudio_glue_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-07-26 09:28:43.000000 cloudio-glue-python-1.0.3/src/cloudio_glue_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 09:28:43.000000 cloudio-glue-python-1.0.3/src/cloudio_glue_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-26 09:28:43.000000 cloudio-glue-python-1.0.3/src/cloudio_glue_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 09:28:43.000000 cloudio-glue-python-1.0.3/src/cloudio_glue_python.egg-info/top_level.txt
```

### Comparing `cloudio-glue-python-1.0.2/LICENSE` & `cloudio-glue-python-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudio-glue-python-1.0.2/PKG-INFO` & `cloudio-glue-python-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudio-glue-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: cloud.iO endpoint glue
 Home-page: https://cloudio.hevs.ch
 Author: HES-SO Valais, School of Engineering, Sion
 Author-email: thomas.sterren@hevs.ch
 License: MIT
 Project-URL: Bug Tracker, https://github.com/boozo-unlimited/cloudio-glue-python/issues
 Project-URL: Source Code, https://github.com/boozo-unlimited/cloudio-glue-python
```

### Comparing `cloudio-glue-python-1.0.2/README.md` & `cloudio-glue-python-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cloudio-glue-python-1.0.2/setup.py` & `cloudio-glue-python-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `cloudio-glue-python-1.0.2/src/cloudio/glue/__init__.py` & `cloudio-glue-python-1.0.3/src/cloudio/glue/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudio-glue-python-1.0.2/src/cloudio/glue/cloudio_attribute.py` & `cloudio-glue-python-1.0.3/src/cloudio/glue/cloudio_attribute.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,19 @@
         """
         try:
             # Try if fget method is another descriptor
             return self._fget.__get__(obj, the_type)()
         except TypeError:
             pass
 
-        return self._fget.__get__(obj)
+        try:
+            return self._fget.__get__(obj)
+        except TypeError:
+            # Call real fget method
+            return self._fget(obj)  # Called for example when having ABC meta derived property
 
     def __set__(self, obj, value):
         """Assigns value to decorated attribute.
 
         :param obj: The composite instance containing the attribute
         :param value: The value to assign to the attribute
         :return: Value returned by the setter method.
```

### Comparing `cloudio-glue-python-1.0.2/src/cloudio/glue/model_to_cloud_connector.py` & `cloudio-glue-python-1.0.3/src/cloudio/glue/model_to_cloud_connector.py`

 * *Files identical despite different names*

### Comparing `cloudio-glue-python-1.0.2/src/cloudio_glue_python.egg-info/PKG-INFO` & `cloudio-glue-python-1.0.3/src/cloudio_glue_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudio-glue-python
-Version: 1.0.2
+Version: 1.0.3
 Summary: cloud.iO endpoint glue
 Home-page: https://cloudio.hevs.ch
 Author: HES-SO Valais, School of Engineering, Sion
 Author-email: thomas.sterren@hevs.ch
 License: MIT
 Project-URL: Bug Tracker, https://github.com/boozo-unlimited/cloudio-glue-python/issues
 Project-URL: Source Code, https://github.com/boozo-unlimited/cloudio-glue-python
```

