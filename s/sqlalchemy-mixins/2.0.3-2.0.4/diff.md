# Comparing `tmp/sqlalchemy_mixins-2.0.3.tar.gz` & `tmp/sqlalchemy_mixins-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_mixins-2.0.3.tar", last modified: Tue Jul  4 14:34:18 2023, max compression
+gzip compressed data, was "sqlalchemy_mixins-2.0.4.tar", last modified: Wed Jul 26 12:24:19 2023, max compression
```

## Comparing `sqlalchemy_mixins-2.0.3.tar` & `sqlalchemy_mixins-2.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:34:18.965732 sqlalchemy_mixins-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-04 14:34:18.965732 sqlalchemy_mixins-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23491 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 14:34:18.965732 sqlalchemy_mixins-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:34:18.961732 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/activerecord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/activerecord.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/eagerload.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/eagerload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/inspection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/repr.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/repr.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/serialize.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/session.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/smartquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/smartquery.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-04 14:34:08.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:34:18.965732 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-04 14:34:18.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-04 14:34:18.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:34:18.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:34:18.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-04 14:34:18.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 14:34:18.000000 sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:24:19.444843 sqlalchemy_mixins-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-26 12:24:19.444843 sqlalchemy_mixins-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23491 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:24:19.444843 sqlalchemy_mixins-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:24:19.444843 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/activerecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/activerecord.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/eagerload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/eagerload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/inspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/repr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/serialize.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15970 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/smartquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/smartquery.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-26 12:24:07.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:24:19.444843 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-26 12:24:19.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-26 12:24:19.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:24:19.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:24:19.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 12:24:19.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 12:24:19.000000 sqlalchemy_mixins-2.0.4/sqlalchemy_mixins.egg-info/top_level.txt
```

### Comparing `sqlalchemy_mixins-2.0.3/LICENSE.txt` & `sqlalchemy_mixins-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.3/PKG-INFO` & `sqlalchemy_mixins-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_mixins
-Version: 2.0.3
+Version: 2.0.4
 Summary: Active Record, Django-like queries, nested eager load and beauty __repr__ for SQLAlchemy
 Home-page: https://github.com/absent1706/sqlalchemy-mixins
 Download-URL: https://github.com/absent1706/sqlalchemy-mixins/archive/master.tar.gz
 Author: Alexander Litvinenko
 Author-email: litvinenko1706@gmail.com
 License: MIT
 Keywords: sqlalchemy,active record,activerecord,orm,django-like,django,eager load,eagerload,repr,__repr__,mysql,postgresql,pymysql,sqlite
```

### Comparing `sqlalchemy_mixins-2.0.3/README.md` & `sqlalchemy_mixins-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.3/setup.py` & `sqlalchemy_mixins-2.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def requirements():
     import os
     filename = os.path.join(os.path.dirname(__file__), 'requirements.txt')
     return [line.rstrip('\n') for line in open(filename).readlines()]
 
 setup(name='sqlalchemy_mixins',
-      version='2.0.3',
+      version='2.0.4',
       description='Active Record, Django-like queries, nested eager load '
                   'and beauty __repr__ for SQLAlchemy',
       url='https://github.com/absent1706/sqlalchemy-mixins',
       download_url='https://github.com/absent1706/sqlalchemy-mixins/archive/master.tar.gz',
       author='Alexander Litvinenko',
       author_email='litvinenko1706@gmail.com',
       license='MIT',
```

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/__init__.py` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/activerecord.py` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/activerecord.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/activerecord.pyi` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/activerecord.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/eagerload.py` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/eagerload.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/eagerload.pyi` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/eagerload.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/inspection.py` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/inspection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 from sqlalchemy import inspect
 from sqlalchemy.ext.hybrid import hybrid_property, hybrid_method
 from sqlalchemy.orm import RelationshipProperty, DeclarativeBase
 
 from .utils import classproperty
 
 
-class Base(DeclarativeBase):
-    __abstract__ = True
-
-
-class InspectionMixin(Base):
-    __abstract__ = True
+class InspectionMixin:
 
     @classproperty
     def columns(cls):
         return inspect(cls).columns.keys()
 
     @classproperty
     def primary_keys_full(cls):
```

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/inspection.pyi` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/inspection.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from typing import List, Protocol, Dict
 
 from sqlalchemy.ext.hybrid import hybrid_method
-from sqlalchemy.orm import Mapper, DeclarativeBase
+from sqlalchemy.orm import Mapper
 from sqlalchemy.orm.interfaces import MapperProperty
 
 from sqlalchemy_mixins.utils import classproperty
 
-class Base(DeclarativeBase):
-    __abstract__ = True
 
 class MappingProtocol(Protocol):
     __mapper__: Mapper
 
-class InspectionMixin(Base):
+class InspectionMixin:
 
     @classproperty
     def columns(cls) -> List[str]: ...
 
     @classproperty
     def primary_keys_full(cls: MappingProtocol) -> List[MapperProperty]: ...
```

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/repr.py` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/repr.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/serialize.py` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/serialize.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/session.py` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/session.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/smartquery.py` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/smartquery.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/smartquery.pyi` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/smartquery.pyi`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/timestamp.py` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/timestamp.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins/utils.py` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins/utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/PKG-INFO` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-mixins
-Version: 2.0.3
+Version: 2.0.4
 Summary: Active Record, Django-like queries, nested eager load and beauty __repr__ for SQLAlchemy
 Home-page: https://github.com/absent1706/sqlalchemy-mixins
 Download-URL: https://github.com/absent1706/sqlalchemy-mixins/archive/master.tar.gz
 Author: Alexander Litvinenko
 Author-email: litvinenko1706@gmail.com
 License: MIT
 Keywords: sqlalchemy,active record,activerecord,orm,django-like,django,eager load,eagerload,repr,__repr__,mysql,postgresql,pymysql,sqlite
```

### Comparing `sqlalchemy_mixins-2.0.3/sqlalchemy_mixins.egg-info/SOURCES.txt` & `sqlalchemy_mixins-2.0.4/sqlalchemy_mixins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

