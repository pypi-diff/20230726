# Comparing `tmp/pip_services4_logic-0.0.4.tar.gz` & `tmp/pip_services4_logic-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_services4_logic-0.0.4.tar", last modified: Tue Jul 25 20:00:27 2023, max compression
+gzip compressed data, was "pip_services4_logic-0.0.5.tar", last modified: Tue Jul 25 22:52:27 2023, max compression
```

## Comparing `pip_services4_logic-0.0.4.tar` & `pip_services4_logic-0.0.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 20:00:27.411907 pip_services4_logic-0.0.4/
--rw-rw-rw-   0        0        0      298 2023-07-25 19:33:15.000000 pip_services4_logic-0.0.4/CHANGELOG.md
--rw-rw-rw-   0        0        0     1076 2020-12-11 04:21:14.000000 pip_services4_logic-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       54 2020-12-11 04:21:14.000000 pip_services4_logic-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4938 2023-07-25 20:00:27.411907 pip_services4_logic-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3905 2023-07-25 10:09:02.000000 pip_services4_logic-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 20:00:27.368907 pip_services4_logic-0.0.4/pip_services4_logic/
--rw-rw-rw-   0        0        0      300 2023-07-25 09:55:38.000000 pip_services4_logic-0.0.4/pip_services4_logic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 20:00:27.392903 pip_services4_logic-0.0.4/pip_services4_logic/build/
--rw-rw-rw-   0        0        0     1898 2023-07-25 19:57:51.000000 pip_services4_logic-0.0.4/pip_services4_logic/build/DefaultLogicFactory.py
--rw-rw-rw-   0        0        0      479 2023-07-25 10:29:12.000000 pip_services4_logic-0.0.4/pip_services4_logic/build/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 20:00:27.397907 pip_services4_logic-0.0.4/pip_services4_logic/cache/
--rw-rw-rw-   0        0        0     2029 2023-07-25 10:04:42.000000 pip_services4_logic-0.0.4/pip_services4_logic/cache/CacheEntry.py
--rw-rw-rw-   0        0        0     1480 2023-07-25 10:31:16.000000 pip_services4_logic-0.0.4/pip_services4_logic/cache/DefaultCacheFactory.py
--rw-rw-rw-   0        0        0     1905 2023-07-25 10:16:58.000000 pip_services4_logic-0.0.4/pip_services4_logic/cache/ICache.py
--rw-rw-rw-   0        0        0     6046 2023-07-25 10:18:18.000000 pip_services4_logic-0.0.4/pip_services4_logic/cache/MemoryCache.py
--rw-rw-rw-   0        0        0     1843 2023-07-25 10:18:49.000000 pip_services4_logic-0.0.4/pip_services4_logic/cache/NullCache.py
--rw-rw-rw-   0        0        0      704 2023-07-25 10:04:42.000000 pip_services4_logic-0.0.4/pip_services4_logic/cache/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 20:00:27.401906 pip_services4_logic-0.0.4/pip_services4_logic/lock/
--rw-rw-rw-   0        0        0     1113 2023-07-25 10:08:26.000000 pip_services4_logic-0.0.4/pip_services4_logic/lock/DefaultLockFactory.py
--rw-rw-rw-   0        0        0     1643 2023-07-25 10:19:15.000000 pip_services4_logic-0.0.4/pip_services4_logic/lock/ILock.py
--rw-rw-rw-   0        0        0     3318 2023-07-25 10:20:25.000000 pip_services4_logic-0.0.4/pip_services4_logic/lock/Lock.py
--rw-rw-rw-   0        0        0     1847 2023-07-25 10:25:23.000000 pip_services4_logic-0.0.4/pip_services4_logic/lock/MemoryLock.py
--rw-rw-rw-   0        0        0     1724 2023-07-25 10:25:56.000000 pip_services4_logic-0.0.4/pip_services4_logic/lock/NullLock.py
--rw-rw-rw-   0        0        0      540 2023-07-25 10:04:42.000000 pip_services4_logic-0.0.4/pip_services4_logic/lock/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 20:00:27.405906 pip_services4_logic-0.0.4/pip_services4_logic/state/
--rw-rw-rw-   0        0        0     1349 2023-07-25 10:08:26.000000 pip_services4_logic-0.0.4/pip_services4_logic/state/DefaultStateStoreFactory.py
--rw-rw-rw-   0        0        0     2055 2023-07-25 10:26:28.000000 pip_services4_logic-0.0.4/pip_services4_logic/state/IStateStore.py
--rw-rw-rw-   0        0        0     4940 2023-07-25 10:27:47.000000 pip_services4_logic-0.0.4/pip_services4_logic/state/MemoryStateStore.py
--rw-rw-rw-   0        0        0     2080 2023-07-25 10:28:12.000000 pip_services4_logic-0.0.4/pip_services4_logic/state/NullStateStore.py
--rw-rw-rw-   0        0        0     1431 2023-07-25 10:04:42.000000 pip_services4_logic-0.0.4/pip_services4_logic/state/StateEntry.py
--rw-rw-rw-   0        0        0      370 2021-10-25 16:24:34.000000 pip_services4_logic-0.0.4/pip_services4_logic/state/StateValue.py
--rw-rw-rw-   0        0        0      440 2021-10-25 17:22:14.000000 pip_services4_logic-0.0.4/pip_services4_logic/state/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 20:00:27.391906 pip_services4_logic-0.0.4/pip_services4_logic.egg-info/
--rw-rw-rw-   0        0        0     4938 2023-07-25 20:00:27.000000 pip_services4_logic-0.0.4/pip_services4_logic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1453 2023-07-25 20:00:27.000000 pip_services4_logic-0.0.4/pip_services4_logic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 20:00:27.000000 pip_services4_logic-0.0.4/pip_services4_logic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-07-25 20:00:27.000000 pip_services4_logic-0.0.4/pip_services4_logic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-25 20:00:27.000000 pip_services4_logic-0.0.4/pip_services4_logic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 10:33:54.000000 pip_services4_logic-0.0.4/pip_services4_logic.egg-info/zip-safe
--rw-rw-rw-   0        0        0      180 2023-07-25 20:00:27.413907 pip_services4_logic-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1751 2023-07-25 19:58:05.000000 pip_services4_logic-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 20:00:27.364389 pip_services4_logic-0.0.4/test/
-drwxrwxrwx   0        0        0        0 2023-07-25 20:00:27.407907 pip_services4_logic-0.0.4/test/cache/
--rw-rw-rw-   0        0        0     1559 2020-12-11 04:21:14.000000 pip_services4_logic-0.0.4/test/cache/CacheFixture.py
--rw-rw-rw-   0        0        0        0 2020-12-11 04:21:14.000000 pip_services4_logic-0.0.4/test/cache/__init__.py
--rw-rw-rw-   0        0        0      852 2023-07-25 10:08:26.000000 pip_services4_logic-0.0.4/test/cache/test_MemoryCache.py
-drwxrwxrwx   0        0        0        0 2023-07-25 20:00:27.409908 pip_services4_logic-0.0.4/test/lock/
--rw-rw-rw-   0        0        0     1734 2023-07-25 10:08:26.000000 pip_services4_logic-0.0.4/test/lock/LockFixture.py
--rw-rw-rw-   0        0        0        0 2020-12-11 04:21:14.000000 pip_services4_logic-0.0.4/test/lock/__init__.py
--rw-rw-rw-   0        0        0      573 2023-07-25 10:04:42.000000 pip_services4_logic-0.0.4/test/lock/test_MemoruLock.py
-drwxrwxrwx   0        0        0        0 2023-07-25 20:00:27.411907 pip_services4_logic-0.0.4/test/state/
--rw-rw-rw-   0        0        0      904 2023-07-25 10:04:42.000000 pip_services4_logic-0.0.4/test/state/StateStoreFixture.py
--rw-rw-rw-   0        0        0       25 2021-10-25 17:22:24.000000 pip_services4_logic-0.0.4/test/state/__init__.py
--rw-rw-rw-   0        0        0      514 2023-07-25 10:04:42.000000 pip_services4_logic-0.0.4/test/state/test_MemoryStateStore.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:52:27.136080 pip_services4_logic-0.0.5/
+-rw-rw-rw-   0        0        0      298 2023-07-25 19:33:15.000000 pip_services4_logic-0.0.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1076 2020-12-11 04:21:14.000000 pip_services4_logic-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       54 2020-12-11 04:21:14.000000 pip_services4_logic-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4943 2023-07-25 22:52:27.136080 pip_services4_logic-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3910 2023-07-25 22:51:12.000000 pip_services4_logic-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 22:52:27.088924 pip_services4_logic-0.0.5/pip_services4_logic/
+-rw-rw-rw-   0        0        0      300 2023-07-25 09:55:38.000000 pip_services4_logic-0.0.5/pip_services4_logic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:52:27.105927 pip_services4_logic-0.0.5/pip_services4_logic/build/
+-rw-rw-rw-   0        0        0     1898 2023-07-25 19:57:51.000000 pip_services4_logic-0.0.5/pip_services4_logic/build/DefaultLogicFactory.py
+-rw-rw-rw-   0        0        0      479 2023-07-25 10:29:12.000000 pip_services4_logic-0.0.5/pip_services4_logic/build/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:52:27.112952 pip_services4_logic-0.0.5/pip_services4_logic/cache/
+-rw-rw-rw-   0        0        0     2029 2023-07-25 10:04:42.000000 pip_services4_logic-0.0.5/pip_services4_logic/cache/CacheEntry.py
+-rw-rw-rw-   0        0        0     1480 2023-07-25 10:31:16.000000 pip_services4_logic-0.0.5/pip_services4_logic/cache/DefaultCacheFactory.py
+-rw-rw-rw-   0        0        0     1905 2023-07-25 10:16:58.000000 pip_services4_logic-0.0.5/pip_services4_logic/cache/ICache.py
+-rw-rw-rw-   0        0        0     6046 2023-07-25 10:18:18.000000 pip_services4_logic-0.0.5/pip_services4_logic/cache/MemoryCache.py
+-rw-rw-rw-   0        0        0     1843 2023-07-25 10:18:49.000000 pip_services4_logic-0.0.5/pip_services4_logic/cache/NullCache.py
+-rw-rw-rw-   0        0        0      704 2023-07-25 10:04:42.000000 pip_services4_logic-0.0.5/pip_services4_logic/cache/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:52:27.119080 pip_services4_logic-0.0.5/pip_services4_logic/lock/
+-rw-rw-rw-   0        0        0     1118 2023-07-25 22:51:12.000000 pip_services4_logic-0.0.5/pip_services4_logic/lock/DefaultLockFactory.py
+-rw-rw-rw-   0        0        0     1643 2023-07-25 10:19:15.000000 pip_services4_logic-0.0.5/pip_services4_logic/lock/ILock.py
+-rw-rw-rw-   0        0        0     3318 2023-07-25 10:20:25.000000 pip_services4_logic-0.0.5/pip_services4_logic/lock/Lock.py
+-rw-rw-rw-   0        0        0     1847 2023-07-25 10:25:23.000000 pip_services4_logic-0.0.5/pip_services4_logic/lock/MemoryLock.py
+-rw-rw-rw-   0        0        0     1724 2023-07-25 10:25:56.000000 pip_services4_logic-0.0.5/pip_services4_logic/lock/NullLock.py
+-rw-rw-rw-   0        0        0      540 2023-07-25 10:04:42.000000 pip_services4_logic-0.0.5/pip_services4_logic/lock/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:52:27.126080 pip_services4_logic-0.0.5/pip_services4_logic/state/
+-rw-rw-rw-   0        0        0     1354 2023-07-25 22:51:12.000000 pip_services4_logic-0.0.5/pip_services4_logic/state/DefaultStateStoreFactory.py
+-rw-rw-rw-   0        0        0     2055 2023-07-25 10:26:28.000000 pip_services4_logic-0.0.5/pip_services4_logic/state/IStateStore.py
+-rw-rw-rw-   0        0        0     4940 2023-07-25 10:27:47.000000 pip_services4_logic-0.0.5/pip_services4_logic/state/MemoryStateStore.py
+-rw-rw-rw-   0        0        0     2080 2023-07-25 10:28:12.000000 pip_services4_logic-0.0.5/pip_services4_logic/state/NullStateStore.py
+-rw-rw-rw-   0        0        0     1431 2023-07-25 10:04:42.000000 pip_services4_logic-0.0.5/pip_services4_logic/state/StateEntry.py
+-rw-rw-rw-   0        0        0      370 2021-10-25 16:24:34.000000 pip_services4_logic-0.0.5/pip_services4_logic/state/StateValue.py
+-rw-rw-rw-   0        0        0      440 2021-10-25 17:22:14.000000 pip_services4_logic-0.0.5/pip_services4_logic/state/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:52:27.104928 pip_services4_logic-0.0.5/pip_services4_logic.egg-info/
+-rw-rw-rw-   0        0        0     4943 2023-07-25 22:52:27.000000 pip_services4_logic-0.0.5/pip_services4_logic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1453 2023-07-25 22:52:27.000000 pip_services4_logic-0.0.5/pip_services4_logic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 22:52:27.000000 pip_services4_logic-0.0.5/pip_services4_logic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-25 22:52:27.000000 pip_services4_logic-0.0.5/pip_services4_logic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-25 22:52:27.000000 pip_services4_logic-0.0.5/pip_services4_logic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 22:52:27.000000 pip_services4_logic-0.0.5/pip_services4_logic.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      180 2023-07-25 22:52:27.142079 pip_services4_logic-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1719 2023-07-25 22:52:19.000000 pip_services4_logic-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:52:27.082926 pip_services4_logic-0.0.5/test/
+drwxrwxrwx   0        0        0        0 2023-07-25 22:52:27.129081 pip_services4_logic-0.0.5/test/cache/
+-rw-rw-rw-   0        0        0     1559 2020-12-11 04:21:14.000000 pip_services4_logic-0.0.5/test/cache/CacheFixture.py
+-rw-rw-rw-   0        0        0        0 2020-12-11 04:21:14.000000 pip_services4_logic-0.0.5/test/cache/__init__.py
+-rw-rw-rw-   0        0        0      852 2023-07-25 10:08:26.000000 pip_services4_logic-0.0.5/test/cache/test_MemoryCache.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:52:27.132079 pip_services4_logic-0.0.5/test/lock/
+-rw-rw-rw-   0        0        0     1734 2023-07-25 10:08:26.000000 pip_services4_logic-0.0.5/test/lock/LockFixture.py
+-rw-rw-rw-   0        0        0        0 2020-12-11 04:21:14.000000 pip_services4_logic-0.0.5/test/lock/__init__.py
+-rw-rw-rw-   0        0        0      573 2023-07-25 10:04:42.000000 pip_services4_logic-0.0.5/test/lock/test_MemoruLock.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:52:27.135079 pip_services4_logic-0.0.5/test/state/
+-rw-rw-rw-   0        0        0      904 2023-07-25 10:04:42.000000 pip_services4_logic-0.0.5/test/state/StateStoreFixture.py
+-rw-rw-rw-   0        0        0       25 2021-10-25 17:22:24.000000 pip_services4_logic-0.0.5/test/state/__init__.py
+-rw-rw-rw-   0        0        0      514 2023-07-25 10:04:42.000000 pip_services4_logic-0.0.5/test/state/test_MemoryStateStore.py
```

### Comparing `pip_services4_logic-0.0.4/LICENSE` & `pip_services4_logic-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/PKG-INFO` & `pip_services4_logic-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_services4_logic
-Version: 0.0.4
+Version: 0.0.5
 Summary: Component definitions for Pip.Services in Python
 Home-page: https://github.com/pip-services4/pip-services4-python/pip-services4-logic-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -95,15 +95,15 @@
 ```
 
 If you need to create components using their locators (descriptors) implement 
 component factories similar to the example below.
 
 ```python
 from pip_services3_commons.refer import Descriptor
-from pip_services4_logic.build import Factory
+from pip_services4_components.build import Factory
 
 
 class MyFactory(Factory):
     my_component_descriptor = Descriptor("myservice", "mycomponent", "default", "*", "1.0")
 
     def __init__(self):
         super(MyFactory, self).__init__()
```

### Comparing `pip_services4_logic-0.0.4/README.md` & `pip_services4_logic-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 ```
 
 If you need to create components using their locators (descriptors) implement 
 component factories similar to the example below.
 
 ```python
 from pip_services3_commons.refer import Descriptor
-from pip_services4_logic.build import Factory
+from pip_services4_components.build import Factory
 
 
 class MyFactory(Factory):
     my_component_descriptor = Descriptor("myservice", "mycomponent", "default", "*", "1.0")
 
     def __init__(self):
         super(MyFactory, self).__init__()
```

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/build/DefaultLogicFactory.py` & `pip_services4_logic-0.0.5/pip_services4_logic/build/DefaultLogicFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/cache/CacheEntry.py` & `pip_services4_logic-0.0.5/pip_services4_logic/cache/CacheEntry.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/cache/DefaultCacheFactory.py` & `pip_services4_logic-0.0.5/pip_services4_logic/cache/DefaultCacheFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/cache/ICache.py` & `pip_services4_logic-0.0.5/pip_services4_logic/cache/ICache.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/cache/MemoryCache.py` & `pip_services4_logic-0.0.5/pip_services4_logic/cache/MemoryCache.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/cache/NullCache.py` & `pip_services4_logic-0.0.5/pip_services4_logic/cache/NullCache.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/cache/__init__.py` & `pip_services4_logic-0.0.5/pip_services4_logic/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/lock/DefaultLockFactory.py` & `pip_services4_logic-0.0.5/pip_services4_logic/lock/DefaultLockFactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from pip_services4_components.refer import Descriptor
 
-from pip_services4_logic.build import Factory
+from pip_services4_components.build import Factory
 from .MemoryLock import MemoryLock
 from .NullLock import NullLock
 
 
 class DefaultLockFactory(Factory):
     """
     Creates :class:`ILock <pip_services4_logic.lock.ILock.ILock>` components by their descriptors.
```

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/lock/ILock.py` & `pip_services4_logic-0.0.5/pip_services4_logic/lock/ILock.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/lock/Lock.py` & `pip_services4_logic-0.0.5/pip_services4_logic/lock/Lock.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/lock/MemoryLock.py` & `pip_services4_logic-0.0.5/pip_services4_logic/lock/MemoryLock.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/lock/NullLock.py` & `pip_services4_logic-0.0.5/pip_services4_logic/lock/NullLock.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/lock/__init__.py` & `pip_services4_logic-0.0.5/pip_services4_logic/lock/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/state/DefaultStateStoreFactory.py` & `pip_services4_logic-0.0.5/pip_services4_logic/state/DefaultStateStoreFactory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from pip_services4_components.refer import Descriptor
 
-from pip_services4_logic.build import Factory
+from pip_services4_components.build import Factory
 from .MemoryStateStore import MemoryStateStore
 from .NullStateStore import NullStateStore
 
 
 class DefaultStateStoreFactory(Factory):
     """
     Creates :class:`IStateStore <pip_services4_logic.state.IStateStore.IStateStore>` components by their descriptors.
```

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/state/IStateStore.py` & `pip_services4_logic-0.0.5/pip_services4_logic/state/IStateStore.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/state/MemoryStateStore.py` & `pip_services4_logic-0.0.5/pip_services4_logic/state/MemoryStateStore.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/state/NullStateStore.py` & `pip_services4_logic-0.0.5/pip_services4_logic/state/NullStateStore.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic/state/StateEntry.py` & `pip_services4_logic-0.0.5/pip_services4_logic/state/StateEntry.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic.egg-info/PKG-INFO` & `pip_services4_logic-0.0.5/pip_services4_logic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-services4-logic
-Version: 0.0.4
+Version: 0.0.5
 Summary: Component definitions for Pip.Services in Python
 Home-page: https://github.com/pip-services4/pip-services4-python/pip-services4-logic-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -95,15 +95,15 @@
 ```
 
 If you need to create components using their locators (descriptors) implement 
 component factories similar to the example below.
 
 ```python
 from pip_services3_commons.refer import Descriptor
-from pip_services4_logic.build import Factory
+from pip_services4_components.build import Factory
 
 
 class MyFactory(Factory):
     my_component_descriptor = Descriptor("myservice", "mycomponent", "default", "*", "1.0")
 
     def __init__(self):
         super(MyFactory, self).__init__()
```

### Comparing `pip_services4_logic-0.0.4/pip_services4_logic.egg-info/SOURCES.txt` & `pip_services4_logic-0.0.5/pip_services4_logic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/setup.py` & `pip_services4_logic-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,28 +19,27 @@
 try:
     readme = open('README.md').read()
 except:
     readme = __doc__
 
 setup(
     name='pip_services4_logic',
-    version='0.0.4',
+    version='0.0.5',
     url='https://github.com/pip-services4/pip-services4-python/pip-services4-logic-python',
     license='MIT',
     description='Component definitions for Pip.Services in Python',
     author='Conceptual Vision Consulting LLC',
     author_email='seroukhov@gmail.com',
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['config', 'data', 'test']),
     include_package_data=True,
     zip_safe=True,
     platforms='any',
     install_requires=[
-        'PyYAML >= 6.0, < 7.0',
         'pip_services4_commons >= 0.0.1, < 1.0',
         'pip_services4_components >= 0.0.2, < 1.0',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

### Comparing `pip_services4_logic-0.0.4/test/cache/CacheFixture.py` & `pip_services4_logic-0.0.5/test/cache/CacheFixture.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/test/cache/test_MemoryCache.py` & `pip_services4_logic-0.0.5/test/cache/test_MemoryCache.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/test/lock/LockFixture.py` & `pip_services4_logic-0.0.5/test/lock/LockFixture.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/test/lock/test_MemoruLock.py` & `pip_services4_logic-0.0.5/test/lock/test_MemoruLock.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/test/state/StateStoreFixture.py` & `pip_services4_logic-0.0.5/test/state/StateStoreFixture.py`

 * *Files identical despite different names*

### Comparing `pip_services4_logic-0.0.4/test/state/test_MemoryStateStore.py` & `pip_services4_logic-0.0.5/test/state/test_MemoryStateStore.py`

 * *Files identical despite different names*

