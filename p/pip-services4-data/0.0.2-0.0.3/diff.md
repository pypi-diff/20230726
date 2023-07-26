# Comparing `tmp/pip_services4_data-0.0.2.tar.gz` & `tmp/pip_services4_data-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_services4_data-0.0.2.tar", last modified: Wed Jul 26 00:16:01 2023, max compression
+gzip compressed data, was "pip_services4_data-0.0.3.tar", last modified: Wed Jul 26 00:20:07 2023, max compression
```

## Comparing `pip_services4_data-0.0.2.tar` & `pip_services4_data-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 00:16:01.311191 pip_services4_data-0.0.2/
--rw-rw-rw-   0        0        0      297 2023-07-25 23:10:37.000000 pip_services4_data-0.0.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1076 2020-12-11 04:36:42.000000 pip_services4_data-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       54 2020-12-11 04:36:42.000000 pip_services4_data-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2490 2023-07-26 00:16:01.311191 pip_services4_data-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1574 2023-07-25 23:11:05.000000 pip_services4_data-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 00:16:01.310190 pip_services4_data-0.0.2/pip_services4_data.egg-info/
--rw-rw-rw-   0        0        0     2490 2023-07-26 00:16:01.000000 pip_services4_data-0.0.2/pip_services4_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-07-26 00:16:01.000000 pip_services4_data-0.0.2/pip_services4_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 00:16:01.000000 pip_services4_data-0.0.2/pip_services4_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-26 00:16:01.000000 pip_services4_data-0.0.2/pip_services4_data.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 00:16:01.000000 pip_services4_data-0.0.2/pip_services4_data.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 23:38:18.000000 pip_services4_data-0.0.2/pip_services4_data.egg-info/zip-safe
--rw-rw-rw-   0        0        0      180 2023-07-26 00:16:01.313192 pip_services4_data-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1587 2023-07-26 00:15:45.000000 pip_services4_data-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:20:07.122811 pip_services4_data-0.0.3/
+-rw-rw-rw-   0        0        0      297 2023-07-25 23:10:37.000000 pip_services4_data-0.0.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1076 2020-12-11 04:36:42.000000 pip_services4_data-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       54 2020-12-11 04:36:42.000000 pip_services4_data-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2490 2023-07-26 00:20:07.122811 pip_services4_data-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1574 2023-07-25 23:11:05.000000 pip_services4_data-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 00:20:07.034418 pip_services4_data-0.0.3/pip_services4_data/
+-rw-rw-rw-   0        0        0       38 2023-07-26 00:19:54.000000 pip_services4_data-0.0.3/pip_services4_data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:20:07.070751 pip_services4_data-0.0.3/pip_services4_data/data/
+-rw-rw-rw-   0        0        0      753 2022-02-25 23:15:06.000000 pip_services4_data-0.0.3/pip_services4_data/data/IChangeable.py
+-rw-rw-rw-   0        0        0      673 2021-05-26 21:22:12.000000 pip_services4_data-0.0.3/pip_services4_data/data/IIdentifiable.py
+-rw-rw-rw-   0        0        0      548 2021-05-03 14:36:30.000000 pip_services4_data-0.0.3/pip_services4_data/data/INamed.py
+-rw-rw-rw-   0        0        0      914 2021-05-03 14:36:46.000000 pip_services4_data-0.0.3/pip_services4_data/data/IStringIdentifiable.py
+-rw-rw-rw-   0        0        0     1059 2021-09-12 21:28:16.000000 pip_services4_data-0.0.3/pip_services4_data/data/ITrackable.py
+-rw-rw-rw-   0        0        0     1212 2021-05-03 23:04:18.000000 pip_services4_data-0.0.3/pip_services4_data/data/IVersioned.py
+-rw-rw-rw-   0        0        0     5306 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/data/MultiString.py
+-rw-rw-rw-   0        0        0      981 2023-07-25 23:33:08.000000 pip_services4_data-0.0.3/pip_services4_data/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:20:07.072745 pip_services4_data-0.0.3/pip_services4_data/keys/
+-rw-rw-rw-   0        0        0     1414 2021-09-12 21:24:00.000000 pip_services4_data-0.0.3/pip_services4_data/keys/IdGenerator.py
+-rw-rw-rw-   0        0        0       75 2023-07-25 23:18:49.000000 pip_services4_data-0.0.3/pip_services4_data/keys/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:20:07.075741 pip_services4_data-0.0.3/pip_services4_data/process/
+-rw-rw-rw-   0        0        0     5545 2021-05-03 15:37:12.000000 pip_services4_data-0.0.3/pip_services4_data/process/TagsProcessor.py
+-rw-rw-rw-   0        0        0       73 2023-07-25 23:20:35.000000 pip_services4_data-0.0.3/pip_services4_data/process/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:20:07.084743 pip_services4_data-0.0.3/pip_services4_data/query/
+-rw-rw-rw-   0        0        0     2298 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/query/DataPage.py
+-rw-rw-rw-   0        0        0     2150 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/query/FilterParams.py
+-rw-rw-rw-   0        0        0     4744 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/query/PagingParams.py
+-rw-rw-rw-   0        0        0     5644 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/query/ProjectionParams.py
+-rw-rw-rw-   0        0        0     1032 2021-05-03 14:48:22.000000 pip_services4_data-0.0.3/pip_services4_data/query/SortField.py
+-rw-rw-rw-   0        0        0     1026 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/query/SortParams.py
+-rw-rw-rw-   0        0        0     1936 2021-09-12 21:23:02.000000 pip_services4_data-0.0.3/pip_services4_data/query/TokenizedDataPage.py
+-rw-rw-rw-   0        0        0     3650 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/query/TokenizedPagingParams.py
+-rw-rw-rw-   0        0        0      529 2023-07-25 23:21:06.000000 pip_services4_data-0.0.3/pip_services4_data/query/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:20:07.094743 pip_services4_data-0.0.3/pip_services4_data/random/
+-rw-rw-rw-   0        0        0      910 2022-02-16 12:27:10.000000 pip_services4_data-0.0.3/pip_services4_data/random/RandomArray.py
+-rw-rw-rw-   0        0        0     1596 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/random/RandomBoolean.py
+-rw-rw-rw-   0        0        0     3490 2022-02-16 12:27:10.000000 pip_services4_data-0.0.3/pip_services4_data/random/RandomDateTime.py
+-rw-rw-rw-   0        0        0     1481 2022-02-16 12:27:10.000000 pip_services4_data-0.0.3/pip_services4_data/random/RandomDouble.py
+-rw-rw-rw-   0        0        0     1461 2022-02-16 12:27:10.000000 pip_services4_data-0.0.3/pip_services4_data/random/RandomFloat.py
+-rw-rw-rw-   0        0        0     2635 2022-02-16 12:27:10.000000 pip_services4_data-0.0.3/pip_services4_data/random/RandomInteger.py
+-rw-rw-rw-   0        0        0     3090 2022-02-16 12:27:10.000000 pip_services4_data-0.0.3/pip_services4_data/random/RandomString.py
+-rw-rw-rw-   0        0        0    13157 2022-02-16 12:27:10.000000 pip_services4_data-0.0.3/pip_services4_data/random/RandomText.py
+-rw-rw-rw-   0        0        0      956 2022-02-16 12:27:10.000000 pip_services4_data-0.0.3/pip_services4_data/random/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:20:07.121810 pip_services4_data-0.0.3/pip_services4_data/validate/
+-rw-rw-rw-   0        0        0     1864 2021-09-12 21:54:30.000000 pip_services4_data-0.0.3/pip_services4_data/validate/AndRule.py
+-rw-rw-rw-   0        0        0     3320 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/validate/ArraySchema.py
+-rw-rw-rw-   0        0        0     2473 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/validate/AtLeastOneExistsRule.py
+-rw-rw-rw-   0        0        0     2174 2021-09-12 21:46:50.000000 pip_services4_data-0.0.3/pip_services4_data/validate/ExcludedRule.py
+-rw-rw-rw-   0        0        0      742 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/validate/FilterParamsSchema.py
+-rw-rw-rw-   0        0        0     1245 2021-09-12 21:54:14.000000 pip_services4_data-0.0.3/pip_services4_data/validate/IValidationRule.py
+-rw-rw-rw-   0        0        0     2173 2021-09-12 21:46:50.000000 pip_services4_data-0.0.3/pip_services4_data/validate/IncludedRule.py
+-rw-rw-rw-   0        0        0     4084 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/validate/MapSchema.py
+-rw-rw-rw-   0        0        0     2068 2021-09-12 21:46:50.000000 pip_services4_data-0.0.3/pip_services4_data/validate/NotRule.py
+-rw-rw-rw-   0        0        0     5508 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/validate/ObjectComparator.py
+-rw-rw-rw-   0        0        0     6917 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/validate/ObjectSchema.py
+-rw-rw-rw-   0        0        0     2852 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/validate/OnlyOneExistRule.py
+-rw-rw-rw-   0        0        0     2103 2021-09-12 21:53:08.000000 pip_services4_data-0.0.3/pip_services4_data/validate/OrRule.py
+-rw-rw-rw-   0        0        0      911 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/validate/PagingParamsSchema.py
+-rw-rw-rw-   0        0        0      415 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/validate/ProjectionParamsSchema.py
+-rw-rw-rw-   0        0        0     2850 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/validate/PropertiesComparisonRule.py
+-rw-rw-rw-   0        0        0     2733 2021-09-12 21:53:08.000000 pip_services4_data-0.0.3/pip_services4_data/validate/PropertySchema.py
+-rw-rw-rw-   0        0        0     8112 2023-07-25 23:37:41.000000 pip_services4_data-0.0.3/pip_services4_data/validate/Schema.py
+-rw-rw-rw-   0        0        0     3824 2023-07-25 23:37:49.000000 pip_services4_data-0.0.3/pip_services4_data/validate/ValidationException.py
+-rw-rw-rw-   0        0        0     2907 2023-07-25 23:28:45.000000 pip_services4_data-0.0.3/pip_services4_data/validate/ValidationResult.py
+-rw-rw-rw-   0        0        0      663 2021-04-30 15:49:00.000000 pip_services4_data-0.0.3/pip_services4_data/validate/ValidationResultType.py
+-rw-rw-rw-   0        0        0     2352 2021-09-12 21:53:08.000000 pip_services4_data-0.0.3/pip_services4_data/validate/ValueComparisonRule.py
+-rw-rw-rw-   0        0        0     1941 2023-07-25 23:29:50.000000 pip_services4_data-0.0.3/pip_services4_data/validate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:20:07.060414 pip_services4_data-0.0.3/pip_services4_data.egg-info/
+-rw-rw-rw-   0        0        0     2490 2023-07-26 00:20:06.000000 pip_services4_data-0.0.3/pip_services4_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2619 2023-07-26 00:20:06.000000 pip_services4_data-0.0.3/pip_services4_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 00:20:06.000000 pip_services4_data-0.0.3/pip_services4_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-26 00:20:06.000000 pip_services4_data-0.0.3/pip_services4_data.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-26 00:20:06.000000 pip_services4_data-0.0.3/pip_services4_data.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 23:38:18.000000 pip_services4_data-0.0.3/pip_services4_data.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      180 2023-07-26 00:20:07.124810 pip_services4_data-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1587 2023-07-26 00:20:01.000000 pip_services4_data-0.0.3/setup.py
```

### Comparing `pip_services4_data-0.0.2/LICENSE` & `pip_services4_data-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_services4_data-0.0.2/PKG-INFO` & `pip_services4_data-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_services4_data
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data processing and persistence components for Pip.Services in Python
 Home-page: http://github.com/pip-services3-python/pip-services4-data-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_data-0.0.2/README.md` & `pip_services4_data-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pip_services4_data-0.0.2/pip_services4_data.egg-info/PKG-INFO` & `pip_services4_data-0.0.3/pip_services4_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-services4-data
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data processing and persistence components for Pip.Services in Python
 Home-page: http://github.com/pip-services3-python/pip-services4-data-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_data-0.0.2/setup.py` & `pip_services4_data-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 try:
     readme = open('readme.md').read()
 except:
     readme = __doc__
 
 setup(
     name='pip_services4_data',
-    version='0.0.2',
+    version='0.0.3',
     url='http://github.com/pip-services3-python/pip-services4-data-python',
     license='MIT',
     author='Conceptual Vision Consulting LLC',
     author_email='seroukhov@gmail.com',
     description='Data processing and persistence components for Pip.Services in Python',
     long_description=readme,
     long_description_content_type="text/markdown",
```

