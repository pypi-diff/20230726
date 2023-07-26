# Comparing `tmp/distanceclosure-0.4.1.macosx-10.9-x86_64.tar.gz` & `tmp/distanceclosure-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distanceclosure-0.4.1.macosx-10.9-x86_64.tar", last modified: Wed Jun 22 14:34:15 2022, max compression
+gzip compressed data, was "distanceclosure-0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `distanceclosure-0.4.1.macosx-10.9-x86_64.tar` & `distanceclosure-0.5.tar`

### file list

```diff
@@ -1,48 +1,9 @@
-drwxr-xr-x   0 rionbr     (501) staff       (20)        0 2022-06-22 14:34:15.465424 ./
-drwxr-xr-x   0 rionbr     (501) staff       (20)        0 2022-06-22 14:34:15.465525 ./opt/
-drwxr-xr-x   0 rionbr     (501) staff       (20)        0 2022-06-22 14:34:15.465631 ./opt/anaconda3/
-drwxr-xr-x   0 rionbr     (501) staff       (20)        0 2022-06-22 14:34:15.465741 ./opt/anaconda3/lib/
-drwxr-xr-x   0 rionbr     (501) staff       (20)        0 2022-06-22 14:34:15.465847 ./opt/anaconda3/lib/python3.9/
-drwxr-xr-x   0 rionbr     (501) staff       (20)        0 2022-06-22 14:34:15.532838 ./opt/anaconda3/lib/python3.9/site-packages/
-drwxr-xr-x   0 rionbr     (501) staff       (20)        0 2022-06-22 14:34:15.506069 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/
--rw-r--r--   0 rionbr     (501) staff       (20)      426 2022-06-22 14:30:30.000000 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/__init__.py
-drwxr-xr-x   0 rionbr     (501) staff       (20)        0 2022-06-22 14:34:15.517094 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/__pycache__/
--rw-r--r--   0 rionbr     (501) staff       (20)      609 2022-06-22 14:34:15.507337 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rionbr     (501) staff       (20)     7465 2022-06-22 14:34:15.516789 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/__pycache__/closure.cpython-39.pyc
--rw-r--r--   0 rionbr     (501) staff       (20)     4453 2022-06-22 14:34:15.506317 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/__pycache__/dijkstra.cpython-39.pyc
--rw-r--r--   0 rionbr     (501) staff       (20)     7295 2022-06-22 14:34:15.508758 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/__pycache__/distance.cpython-39.pyc
--rw-r--r--   0 rionbr     (501) staff       (20)     5991 2022-06-22 14:34:15.514646 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 rionbr     (501) staff       (20)     7708 2022-06-22 14:30:30.000000 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/closure.py
-drwxr-xr-x   0 rionbr     (501) staff       (20)        0 2022-06-22 14:34:15.506747 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/cython/
--rw-r--r--   0 rionbr     (501) staff       (20)        0 2022-06-22 14:30:30.000000 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/cython/__init__.py
-drwxr-xr-x   0 rionbr     (501) staff       (20)        0 2022-06-22 14:34:15.507058 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/cython/__pycache__/
--rw-r--r--   0 rionbr     (501) staff       (20)      168 2022-06-22 14:34:15.506833 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/cython/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rionbr     (501) staff       (20)   286162 2022-06-22 14:34:14.000000 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/cython/dijkstra.c
--rwxr-xr-x   0 rionbr     (501) staff       (20)    82848 2022-06-22 14:34:15.000000 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/cython/dijkstra.cpython-39-darwin.so
-drwxr-xr-x   0 rionbr     (501) staff       (20)        0 2022-06-22 14:34:15.487001 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/cython/libpqueue/
--rwxr-xr-x   0 rionbr     (501) staff       (20)     6948 2022-06-22 14:30:30.000000 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/cython/libpqueue/pqueue.c
--rw-r--r--   0 rionbr     (501) staff       (20)     3717 2022-06-22 14:30:30.000000 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/cython/pqueue.pxd
--rw-r--r--   0 rionbr     (501) staff       (20)     4891 2022-06-22 14:30:30.000000 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/dijkstra.py
--rw-r--r--   0 rionbr     (501) staff       (20)     7951 2022-06-22 14:30:30.000000 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/distance.py
--rw-r--r--   0 rionbr     (501) staff       (20)     4970 2022-06-22 14:30:30.000000 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/utils.py
-drwxr-xr-x   0 rionbr     (501) staff       (20)        0 2022-06-22 14:34:15.547041 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure-0.4.1-py3.9.egg-info/
--rw-r--r--   0 rionbr     (501) staff       (20)      775 2022-06-22 14:34:14.160418 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure-0.4.1-py3.9.egg-info/PKG-INFO
--rw-r--r--   0 rionbr     (501) staff       (20)      685 2022-06-22 14:34:14.206914 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure-0.4.1-py3.9.egg-info/SOURCES.txt
--rw-r--r--   0 rionbr     (501) staff       (20)        1 2022-06-22 14:34:14.160734 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure-0.4.1-py3.9.egg-info/dependency_links.txt
--rw-r--r--   0 rionbr     (501) staff       (20)        1 2017-04-06 15:42:45.000000 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure-0.4.1-py3.9.egg-info/not-zip-safe
--rw-r--r--   0 rionbr     (501) staff       (20)       35 2022-06-22 14:34:14.178635 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure-0.4.1-py3.9.egg-info/requires.txt
--rw-r--r--   0 rionbr     (501) staff       (20)       22 2022-06-22 14:34:14.179498 ./opt/anaconda3/lib/python3.9/site-packages/distanceclosure-0.4.1-py3.9.egg-info/top_level.txt
-drwxr-xr-x   0 rionbr     (501) staff       (20)        0 2022-06-22 14:34:15.517680 ./opt/anaconda3/lib/python3.9/site-packages/tests/
--rw-r--r--   0 rionbr     (501) staff       (20)        0 2022-06-22 14:30:30.000000 ./opt/anaconda3/lib/python3.9/site-packages/tests/__init__.py
-drwxr-xr-x   0 rionbr     (501) staff       (20)        0 2022-06-22 14:34:15.529749 ./opt/anaconda3/lib/python3.9/site-packages/tests/__pycache__/
--rw-r--r--   0 rionbr     (501) staff       (20)      151 2022-06-22 14:34:15.521253 ./opt/anaconda3/lib/python3.9/site-packages/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rionbr     (501) staff       (20)     2605 2022-06-22 14:34:15.527056 ./opt/anaconda3/lib/python3.9/site-packages/tests/__pycache__/test_closure.cpython-39.pyc
--rw-r--r--   0 rionbr     (501) staff       (20)     2324 2022-06-22 14:34:15.520820 ./opt/anaconda3/lib/python3.9/site-packages/tests/__pycache__/test_dijkstra.cpython-39.pyc
--rw-r--r--   0 rionbr     (501) staff       (20)     1787 2022-06-22 14:34:15.522009 ./opt/anaconda3/lib/python3.9/site-packages/tests/__pycache__/test_dijkstra_time.cpython-39.pyc
--rw-r--r--   0 rionbr     (501) staff       (20)     6534 2022-06-22 14:34:15.519549 ./opt/anaconda3/lib/python3.9/site-packages/tests/__pycache__/test_distance.cpython-39.pyc
--rw-r--r--   0 rionbr     (501) staff       (20)     2060 2022-06-22 14:34:15.517774 ./opt/anaconda3/lib/python3.9/site-packages/tests/__pycache__/test_utils.cpython-39.pyc
--rw-r--r--   0 rionbr     (501) staff       (20)     2512 2022-06-22 14:30:30.000000 ./opt/anaconda3/lib/python3.9/site-packages/tests/test_closure.py
--rw-r--r--   0 rionbr     (501) staff       (20)     2207 2022-06-22 14:30:30.000000 ./opt/anaconda3/lib/python3.9/site-packages/tests/test_dijkstra.py
--rw-r--r--   0 rionbr     (501) staff       (20)     1618 2022-06-22 14:30:30.000000 ./opt/anaconda3/lib/python3.9/site-packages/tests/test_dijkstra_time.py
--rw-r--r--   0 rionbr     (501) staff       (20)     5829 2022-06-22 14:30:30.000000 ./opt/anaconda3/lib/python3.9/site-packages/tests/test_distance.py
--rw-r--r--   0 rionbr     (501) staff       (20)     1510 2022-06-22 14:30:30.000000 ./opt/anaconda3/lib/python3.9/site-packages/tests/test_utils.py
+-rw-r--r--   0        0        0     3785 2023-07-26 16:06:17.119368 distanceclosure-0.5/README.md
+-rw-r--r--   0        0        0      516 2023-07-26 07:45:06.993449 distanceclosure-0.5/distanceclosure/__init__.py
+-rw-r--r--   0        0        0     5447 2023-07-26 06:47:10.248183 distanceclosure-0.5/distanceclosure/backbone.py
+-rw-r--r--   0        0        0     7708 2023-07-26 06:47:10.248183 distanceclosure-0.5/distanceclosure/closure.py
+-rw-r--r--   0        0        0     4891 2023-07-26 06:47:10.256183 distanceclosure-0.5/distanceclosure/dijkstra.py
+-rw-r--r--   0        0        0     7951 2023-07-26 06:47:10.256183 distanceclosure-0.5/distanceclosure/distance.py
+-rw-r--r--   0        0        0     4970 2023-07-26 06:47:10.256183 distanceclosure-0.5/distanceclosure/utils.py
+-rw-r--r--   0        0        0      733 2023-07-26 16:39:36.435836 distanceclosure-0.5/pyproject.toml
+-rw-r--r--   0        0        0     4424 1970-01-01 00:00:00.000000 distanceclosure-0.5/PKG-INFO
```

### Comparing `./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/closure.py` & `distanceclosure-0.5/distanceclosure/closure.py`

 * *Files identical despite different names*

### Comparing `./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/dijkstra.py` & `distanceclosure-0.5/distanceclosure/dijkstra.py`

 * *Files identical despite different names*

### Comparing `./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/distance.py` & `distanceclosure-0.5/distanceclosure/distance.py`

 * *Files identical despite different names*

### Comparing `./opt/anaconda3/lib/python3.9/site-packages/distanceclosure/utils.py` & `distanceclosure-0.5/distanceclosure/utils.py`

 * *Files identical despite different names*

