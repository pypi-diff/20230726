# Comparing `tmp/recorder-utils-0.1.0.tar.gz` & `tmp/recorder-utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recorder-utils-0.1.0.tar", last modified: Tue Jul 25 14:48:17 2023, max compression
+gzip compressed data, was "recorder-utils-0.2.0.tar", last modified: Tue Jul 25 22:25:53 2023, max compression
```

## Comparing `recorder-utils-0.1.0.tar` & `recorder-utils-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 onewbiek  (1000) onewbiek  (1000)        0 2023-07-25 14:48:17.743857 recorder-utils-0.1.0/
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     1668 2023-07-25 13:40:37.000000 recorder-utils-0.1.0/LICENSE
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     1917 2023-07-25 14:48:17.739857 recorder-utils-0.1.0/PKG-INFO
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     1419 2023-07-25 08:20:03.000000 recorder-utils-0.1.0/README.md
-drwxrwxr-x   0 onewbiek  (1000) onewbiek  (1000)        0 2023-07-25 14:48:17.739857 recorder-utils-0.1.0/recorder_utils/
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)      144 2023-07-03 09:55:00.000000 recorder-utils-0.1.0/recorder_utils/__init__.py
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)      610 2023-07-25 14:19:53.000000 recorder-utils-0.1.0/recorder_utils/build_offset_intervals.py
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     3996 2023-07-25 14:15:07.000000 recorder-utils-0.1.0/recorder_utils/creader_wrapper.py
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)      351 2023-07-25 14:19:30.000000 recorder-utils-0.1.0/recorder_utils/exclusions.py
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     4365 2023-07-25 14:20:23.000000 recorder-utils-0.1.0/recorder_utils/mpiio_handler.py
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     5347 2023-07-25 14:21:23.000000 recorder-utils-0.1.0/recorder_utils/posix_handler.py
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)    11669 2023-07-03 09:26:51.000000 recorder-utils-0.1.0/recorder_utils/reader.c
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     4203 2023-07-03 09:26:53.000000 recorder-utils-0.1.0/recorder_utils/reader.h
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)    10100 2023-07-03 09:26:55.000000 recorder-utils-0.1.0/recorder_utils/recorder-logger.h
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)      892 2023-07-25 14:15:42.000000 recorder-utils-0.1.0/recorder_utils/recorder2csv.py
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)    73928 2023-07-03 09:27:02.000000 recorder-utils-0.1.0/recorder_utils/uthash.h
-drwxrwxr-x   0 onewbiek  (1000) onewbiek  (1000)        0 2023-07-25 14:48:17.739857 recorder-utils-0.1.0/recorder_utils.egg-info/
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     1917 2023-07-25 14:48:17.000000 recorder-utils-0.1.0/recorder_utils.egg-info/PKG-INFO
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)      601 2023-07-25 14:48:17.000000 recorder-utils-0.1.0/recorder_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)        1 2023-07-25 14:48:17.000000 recorder-utils-0.1.0/recorder_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)       64 2023-07-25 14:48:17.000000 recorder-utils-0.1.0/recorder_utils.egg-info/entry_points.txt
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)       40 2023-07-25 14:48:17.000000 recorder-utils-0.1.0/recorder_utils.egg-info/top_level.txt
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)       38 2023-07-25 14:48:17.743857 recorder-utils-0.1.0/setup.cfg
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     1848 2023-07-25 14:24:44.000000 recorder-utils-0.1.0/setup.py
-drwxrwxr-x   0 onewbiek  (1000) onewbiek  (1000)        0 2023-07-25 14:48:17.739857 recorder-utils-0.1.0/test/
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)      240 2023-07-25 09:12:56.000000 recorder-utils-0.1.0/test/test_convert_csv.py
--rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     1353 2023-07-25 09:13:06.000000 recorder-utils-0.1.0/test/test_convert_text.py
+drwxrwxr-x   0 onewbiek  (1000) onewbiek  (1000)        0 2023-07-25 22:25:53.946472 recorder-utils-0.2.0/
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     1668 2023-07-25 13:40:37.000000 recorder-utils-0.2.0/LICENSE
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     1962 2023-07-25 22:25:53.946472 recorder-utils-0.2.0/PKG-INFO
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     1464 2023-07-25 22:03:01.000000 recorder-utils-0.2.0/README.md
+drwxrwxr-x   0 onewbiek  (1000) onewbiek  (1000)        0 2023-07-25 22:25:53.938471 recorder-utils-0.2.0/recorder_utils/
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)      144 2023-07-25 22:18:33.000000 recorder-utils-0.2.0/recorder_utils/__init__.py
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)      610 2023-07-25 14:19:53.000000 recorder-utils-0.2.0/recorder_utils/build_offset_intervals.py
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     3996 2023-07-25 14:15:07.000000 recorder-utils-0.2.0/recorder_utils/creader_wrapper.py
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)      351 2023-07-25 14:19:30.000000 recorder-utils-0.2.0/recorder_utils/exclusions.py
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     4365 2023-07-25 14:20:23.000000 recorder-utils-0.2.0/recorder_utils/mpiio_handler.py
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     5347 2023-07-25 14:21:23.000000 recorder-utils-0.2.0/recorder_utils/posix_handler.py
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)    11669 2023-07-03 09:26:51.000000 recorder-utils-0.2.0/recorder_utils/reader.c
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     4203 2023-07-03 09:26:53.000000 recorder-utils-0.2.0/recorder_utils/reader.h
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)    10100 2023-07-03 09:26:55.000000 recorder-utils-0.2.0/recorder_utils/recorder-logger.h
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)      892 2023-07-25 14:15:42.000000 recorder-utils-0.2.0/recorder_utils/recorder2csv.py
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)    73928 2023-07-03 09:27:02.000000 recorder-utils-0.2.0/recorder_utils/uthash.h
+drwxrwxr-x   0 onewbiek  (1000) onewbiek  (1000)        0 2023-07-25 22:25:53.942472 recorder-utils-0.2.0/recorder_utils.egg-info/
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     1962 2023-07-25 22:25:53.000000 recorder-utils-0.2.0/recorder_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)      638 2023-07-25 22:25:53.000000 recorder-utils-0.2.0/recorder_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)        1 2023-07-25 22:25:53.000000 recorder-utils-0.2.0/recorder_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)       66 2023-07-25 22:25:53.000000 recorder-utils-0.2.0/recorder_utils.egg-info/entry_points.txt
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)       21 2023-07-25 22:25:53.000000 recorder-utils-0.2.0/recorder_utils.egg-info/requires.txt
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)       40 2023-07-25 22:25:53.000000 recorder-utils-0.2.0/recorder_utils.egg-info/top_level.txt
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)       38 2023-07-25 22:25:53.946472 recorder-utils-0.2.0/setup.cfg
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     1923 2023-07-25 22:18:08.000000 recorder-utils-0.2.0/setup.py
+drwxrwxr-x   0 onewbiek  (1000) onewbiek  (1000)        0 2023-07-25 22:25:53.946472 recorder-utils-0.2.0/test/
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)      240 2023-07-25 09:12:56.000000 recorder-utils-0.2.0/test/test_convert_csv.py
+-rw-rw-r--   0 onewbiek  (1000) onewbiek  (1000)     1353 2023-07-25 09:13:06.000000 recorder-utils-0.2.0/test/test_convert_text.py
```

### Comparing `recorder-utils-0.1.0/LICENSE` & `recorder-utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `recorder-utils-0.1.0/PKG-INFO` & `recorder-utils-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recorder-utils
-Version: 0.1.0
+Version: 0.2.0
 Summary: Recorder utility build upon the package 'recorder-viz'
 Home-page: https://github.com/onewbiek/Recorder-utils
 Author: Onewbiek
 Author-email: yankun0213@gmail.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: License :: OSI Approved :: University of Illinois/NCSA Open Source License
 Classifier: Operating System :: OS Independent
@@ -15,20 +15,24 @@
 # Prerequisite
 
 MPI implementation such as openmpi or MPICH
 
 
 # Install
 
-Under Recorder-util directory
+Install from source
 ```
 pip install -r requirements.txt
 pip install .
 ```
 
+Or Install from pip
+```
+pip install recorder-utils
+```
 
 # Usage
 
 ```
 recorder2csv /path/to/your_trace_folder/   /path/to/output.csv/
 ```
 A csv trace file will be generated to the output file you specified
```

### Comparing `recorder-utils-0.1.0/README.md` & `recorder-utils-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # Prerequisite
 
 MPI implementation such as openmpi or MPICH
 
 
 # Install
 
-Under Recorder-util directory
+Install from source
 ```
 pip install -r requirements.txt
 pip install .
 ```
 
+Or Install from pip
+```
+pip install recorder-utils
+```
 
 # Usage
 
 ```
 recorder2csv /path/to/your_trace_folder/   /path/to/output.csv/
 ```
 A csv trace file will be generated to the output file you specified
```

### Comparing `recorder-utils-0.1.0/recorder_utils/build_offset_intervals.py` & `recorder-utils-0.2.0/recorder_utils/build_offset_intervals.py`

 * *Files identical despite different names*

### Comparing `recorder-utils-0.1.0/recorder_utils/creader_wrapper.py` & `recorder-utils-0.2.0/recorder_utils/creader_wrapper.py`

 * *Files identical despite different names*

### Comparing `recorder-utils-0.1.0/recorder_utils/mpiio_handler.py` & `recorder-utils-0.2.0/recorder_utils/mpiio_handler.py`

 * *Files identical despite different names*

### Comparing `recorder-utils-0.1.0/recorder_utils/posix_handler.py` & `recorder-utils-0.2.0/recorder_utils/posix_handler.py`

 * *Files identical despite different names*

### Comparing `recorder-utils-0.1.0/recorder_utils/reader.c` & `recorder-utils-0.2.0/recorder_utils/reader.c`

 * *Files identical despite different names*

### Comparing `recorder-utils-0.1.0/recorder_utils/reader.h` & `recorder-utils-0.2.0/recorder_utils/reader.h`

 * *Files identical despite different names*

### Comparing `recorder-utils-0.1.0/recorder_utils/recorder-logger.h` & `recorder-utils-0.2.0/recorder_utils/recorder-logger.h`

 * *Files identical despite different names*

### Comparing `recorder-utils-0.1.0/recorder_utils/recorder2csv.py` & `recorder-utils-0.2.0/recorder_utils/recorder2csv.py`

 * *Files identical despite different names*

### Comparing `recorder-utils-0.1.0/recorder_utils/uthash.h` & `recorder-utils-0.2.0/recorder_utils/uthash.h`

 * *Files identical despite different names*

### Comparing `recorder-utils-0.1.0/recorder_utils.egg-info/PKG-INFO` & `recorder-utils-0.2.0/recorder_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recorder-utils
-Version: 0.1.0
+Version: 0.2.0
 Summary: Recorder utility build upon the package 'recorder-viz'
 Home-page: https://github.com/onewbiek/Recorder-utils
 Author: Onewbiek
 Author-email: yankun0213@gmail.com
 Classifier: Programming Language :: Python :: 2.7
 Classifier: License :: OSI Approved :: University of Illinois/NCSA Open Source License
 Classifier: Operating System :: OS Independent
@@ -15,20 +15,24 @@
 # Prerequisite
 
 MPI implementation such as openmpi or MPICH
 
 
 # Install
 
-Under Recorder-util directory
+Install from source
 ```
 pip install -r requirements.txt
 pip install .
 ```
 
+Or Install from pip
+```
+pip install recorder-utils
+```
 
 # Usage
 
 ```
 recorder2csv /path/to/your_trace_folder/   /path/to/output.csv/
 ```
 A csv trace file will be generated to the output file you specified
```

### Comparing `recorder-utils-0.1.0/recorder_utils.egg-info/SOURCES.txt` & `recorder-utils-0.2.0/recorder_utils.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -12,10 +12,11 @@
 recorder_utils/recorder-logger.h
 recorder_utils/recorder2csv.py
 recorder_utils/uthash.h
 recorder_utils.egg-info/PKG-INFO
 recorder_utils.egg-info/SOURCES.txt
 recorder_utils.egg-info/dependency_links.txt
 recorder_utils.egg-info/entry_points.txt
+recorder_utils.egg-info/requires.txt
 recorder_utils.egg-info/top_level.txt
 test/test_convert_csv.py
 test/test_convert_text.py
```

### Comparing `recorder-utils-0.1.0/setup.py` & `recorder-utils-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,30 +20,34 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="recorder-utils",
-    version="0.1.0",
+    version="0.2.0",
     author="Onewbiek",
     author_email="yankun0213@gmail.com",
     description="Recorder utility build upon the package \'recorder-viz\'",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/onewbiek/Recorder-utils",
     packages=['recorder_utils'],                  # package for import: after installaion, import recorder_utils
     package_data = {'recorder_utils': ['*.h']},   # *.h by default will not be copied, we use this to ship it.
+    install_requires=[
+        "mpi4py==3.1.4",
+        "pandas",
+    ],
     classifiers=[
         "Programming Language :: Python :: 2.7",
         "License :: OSI Approved :: University of Illinois/NCSA Open Source License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=2.7',
     entry_points={
         "console_scripts": [
-            "recorder2csv=recorder2csv.recorder2csv:main"
+            "recorder2csv=recorder_utils.recorder2csv:main"
         ]
     },
     ext_modules=[c_reader_module],
     cmdclass={'build_ext': my_build_ext},
 )
```

### Comparing `recorder-utils-0.1.0/test/test_convert_text.py` & `recorder-utils-0.2.0/test/test_convert_text.py`

 * *Files identical despite different names*

