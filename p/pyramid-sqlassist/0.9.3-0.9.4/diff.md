# Comparing `tmp/pyramid_sqlassist-0.9.3.tar.gz` & `tmp/pyramid_sqlassist-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyramid_sqlassist-0.9.3.tar", last modified: Fri Sep  1 21:45:36 2017, max compression
+gzip compressed data, was "dist/pyramid_sqlassist-0.9.4.tar", last modified: Fri Jun  8 21:29:05 2018, max compression
```

## Comparing `pyramid_sqlassist-0.9.3.tar` & `pyramid_sqlassist-0.9.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2017-09-01 21:45:36.000000 pyramid_sqlassist-0.9.3/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1431 2017-09-01 20:14:40.000000 pyramid_sqlassist-0.9.3/CHANGES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       39 2013-08-02 23:10:15.000000 pyramid_sqlassist-0.9.3/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)      536 2017-09-01 21:45:36.000000 pyramid_sqlassist-0.9.3/PKG-INFO
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2017-09-01 21:45:36.000000 pyramid_sqlassist-0.9.3/pyramid_sqlassist/
--rw-r--r--   0 jvanasco   (501) admin       (80)      220 2017-01-25 17:39:00.000000 pyramid_sqlassist-0.9.3/pyramid_sqlassist/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)    15054 2017-09-01 20:14:21.000000 pyramid_sqlassist-0.9.3/pyramid_sqlassist/interface.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     4824 2016-10-31 22:33:52.000000 pyramid_sqlassist-0.9.3/pyramid_sqlassist/objects.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     2880 2016-10-28 18:38:22.000000 pyramid_sqlassist-0.9.3/pyramid_sqlassist/tools.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2017-09-01 21:45:36.000000 pyramid_sqlassist-0.9.3/pyramid_sqlassist.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2017-09-01 21:45:35.000000 pyramid_sqlassist-0.9.3/pyramid_sqlassist.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2012-02-14 20:01:02.000000 pyramid_sqlassist-0.9.3/pyramid_sqlassist.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)      536 2017-09-01 21:45:35.000000 pyramid_sqlassist-0.9.3/pyramid_sqlassist.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       26 2017-09-01 21:45:35.000000 pyramid_sqlassist-0.9.3/pyramid_sqlassist.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      422 2017-09-01 21:45:36.000000 pyramid_sqlassist-0.9.3/pyramid_sqlassist.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       18 2017-09-01 21:45:35.000000 pyramid_sqlassist-0.9.3/pyramid_sqlassist.egg-info/top_level.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)    10215 2017-08-31 23:22:20.000000 pyramid_sqlassist-0.9.3/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)       67 2017-09-01 21:45:36.000000 pyramid_sqlassist-0.9.3/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     1250 2017-08-31 23:18:46.000000 pyramid_sqlassist-0.9.3/setup.py
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2012-02-14 19:57:53.000000 pyramid_sqlassist-0.9.3/tests.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2018-06-08 21:29:05.000000 pyramid_sqlassist-0.9.4/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1513 2018-05-02 20:48:12.000000 pyramid_sqlassist-0.9.4/CHANGES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       39 2013-08-02 23:10:15.000000 pyramid_sqlassist-0.9.4/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)      570 2018-06-08 21:29:05.000000 pyramid_sqlassist-0.9.4/PKG-INFO
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2018-06-08 21:29:05.000000 pyramid_sqlassist-0.9.4/pyramid_sqlassist/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      220 2018-05-02 19:58:43.000000 pyramid_sqlassist-0.9.4/pyramid_sqlassist/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)    15054 2017-09-01 20:14:21.000000 pyramid_sqlassist-0.9.4/pyramid_sqlassist/interface.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     5344 2018-05-02 20:52:05.000000 pyramid_sqlassist-0.9.4/pyramid_sqlassist/objects.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     2880 2016-10-28 18:38:22.000000 pyramid_sqlassist-0.9.4/pyramid_sqlassist/tools.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2018-06-08 21:29:05.000000 pyramid_sqlassist-0.9.4/pyramid_sqlassist.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2018-06-08 21:29:03.000000 pyramid_sqlassist-0.9.4/pyramid_sqlassist.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2012-02-14 20:01:02.000000 pyramid_sqlassist-0.9.4/pyramid_sqlassist.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)      570 2018-06-08 21:29:03.000000 pyramid_sqlassist-0.9.4/pyramid_sqlassist.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)       26 2018-06-08 21:29:03.000000 pyramid_sqlassist-0.9.4/pyramid_sqlassist.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      422 2018-06-08 21:29:03.000000 pyramid_sqlassist-0.9.4/pyramid_sqlassist.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       18 2018-06-08 21:29:03.000000 pyramid_sqlassist-0.9.4/pyramid_sqlassist.egg-info/top_level.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)    10215 2017-08-31 23:22:20.000000 pyramid_sqlassist-0.9.4/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)       67 2018-06-08 21:29:05.000000 pyramid_sqlassist-0.9.4/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1250 2017-08-31 23:18:46.000000 pyramid_sqlassist-0.9.4/setup.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2012-02-14 19:57:53.000000 pyramid_sqlassist-0.9.4/tests.py
```

### Comparing `pyramid_sqlassist-0.9.3/CHANGES.txt` & `pyramid_sqlassist-0.9.4/CHANGES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.9.4
+	* small optimizations for performance
+	* added `loaded_columns_as_dict()`
+
 0.9.3
 	* added setup.cfg
 	* cleaned up some formatting
 	* added `session_factory`
 	* moved version to __init__.py
 	* capitalized `_ENGINE_REGISTRY`
 	* added `is_autocommit` for tracking.
```

### Comparing `pyramid_sqlassist-0.9.3/PKG-INFO` & `pyramid_sqlassist-0.9.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: pyramid_sqlassist
-Version: 0.9.3
+Version: 0.9.4
 Summary: Efficiently manage multiple SqlAlchemy connections for Pyramid
 Home-page: https://github.com/jvanasco/pyramid_sqlassist
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT
+Description-Content-Type: UNKNOWN
 Description: sqlassist
         =========
         
 Keywords: web pyramid sqlalchemy
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Pyramid
```

### Comparing `pyramid_sqlassist-0.9.3/pyramid_sqlassist/interface.py` & `pyramid_sqlassist-0.9.4/pyramid_sqlassist/interface.py`

 * *Files identical despite different names*

### Comparing `pyramid_sqlassist-0.9.3/pyramid_sqlassist/objects.py` & `pyramid_sqlassist-0.9.4/pyramid_sqlassist/objects.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,107 +1,131 @@
 import logging
 log = logging.getLogger(__name__)
 
 
 import sqlalchemy
-import sqlalchemy.orm as sqlalchemy_orm
+import sqlalchemy.sql
+from sqlalchemy.orm import class_mapper as sa_class_mapper
 
+# this is used a bit
+func_lower = sqlalchemy.sql.func.lower
 
 # ==============================================================================
 
 
 class CoreObject(object):
     __table_pkey__ = None
 
 
 class UtilityObject(CoreObject):
 
     def get__by__id(self, dbSession, id, id_column='id'):
         """gets an item by an id column named 'id'.  id column can be overriden"""
-        if not hasattr(self.__class__, id_column) and hasattr(self, '__table_pkey__'):
+        _cls = self.__class__
+        if not hasattr(_cls, id_column) and hasattr(self, '__table_pkey__'):
             id_column = self.__table_pkey__
-        id_col = getattr(self.__class__, id_column)
+        id_col = getattr(_cls, id_column)
         if isinstance(id, (list, tuple)):
-            return dbSession.query(self.__class__).filter(id_col.in_(id)).all()
+            return dbSession.query(_cls).filter(id_col.in_(id)).all()
         else:
             id_dict = {id_column: id}
-            return dbSession.query(self.__class__).filter_by(**id_dict).first()
+            return dbSession.query(_cls).filter_by(**id_dict).first()
 
     def get__by__column__lower(self, dbSession, column, search, allow_many=False):
         """gets items from the database based on a lowercase version of the column.
         useful for situations where you have a function index on a table
         (such as indexing on the lower version of an email addresses)"""
-        items = dbSession.query(self.__class__)\
-            .filter(sqlalchemy.sql.func.lower(getattr(self.__class__, column)) == search.lower(),
+        _cls = self.__class__
+        items = dbSession.query(_cls)\
+            .filter(func_lower(getattr(_cls, column)) == search.lower(),
                     )\
             .all()
         if items:
             if not allow_many:
                 if len(items) > 1:
                     raise ValueError("get__by__column__lower should return 1 and only 1 item")
                 elif len(items) == 1:
                     return items[0]
             else:
                 return items
         return None
 
     def get__by__column__similar(self, dbSession, column, seed, prefix_only=True):
         """seaches for a name column entry with the submitted seed prefix"""
-        query = dbSession.query(self.__class__)
+        _cls = self.__class__
+        query = dbSession.query(_cls)
         if prefix_only:
-            query = query.filter(sqlalchemy.sql.func.lower(getattr(self.__class__, column)).startswith(seed.lower()),
+            query = query.filter(func_lower(getattr(_cls, column)).startswith(seed.lower()),
                                  )
         else:
-            query = query.filter(sqlalchemy.sql.func.lower(getattr(self.__class__, column)).contains(seed.lower()),
+            query = query.filter(func_lower(getattr(_cls, column)).contains(seed.lower()),
                                  )
         results = query\
-            .order_by(getattr(self.__class__, column).asc())\
+            .order_by(getattr(_cls, column).asc())\
             .all()
         return results
 
     def get__by__column__exact_then_ilike(self, dbSession, column, seed):
         """ seaches for an exact, then case-insensitive version of the name column"""
-        item = dbSession.query(self.__class__).filter(getattr(self.__class__, column) == seed).first()
+        _cls = self.__class__
+        item = dbSession.query(_cls).filter(getattr(_cls, column) == seed).first()
         if not item:
-            item = dbSession.query(self.__class__).filter(getattr(self.__class__, column).ilike(seed)).first()
+            item = dbSession.query(_cls).filter(getattr(_cls, column).ilike(seed)).first()
         return item
 
     def get__range(self, dbSession, start=0, limit=None, sort_direction='asc', order_col=None, order_case_sensitive=True, filters=[], debug_query=False):
         """gets a range of items"""
+        _cls = self.__class__
         if not order_col:
             order_col = 'id'
-        query = dbSession.query(self.__class__)
+        query = dbSession.query(_cls)
         for filter in filters:
             query = query.filter(filter)
         for col in order_col.split(','):
             # declared columns do not have self.__class__.c
             # reflected columns did in earlier sqlalchemy
-            col = getattr(self.__class__, col)
+            col = getattr(_cls, col)
             if sort_direction == 'asc':
                 if order_case_sensitive:
                     query = query.order_by(col.asc())
                 else:
-                    query = query.order_by(sqlalchemy.sql.func.lower(col).asc())
+                    query = query.order_by(func_lower(col).asc())
             elif sort_direction == 'desc':
                 if order_case_sensitive:
                     query = query.order_by(col.desc())
                 else:
-                    query = query.order_by(sqlalchemy.sql.func.lower(col).desc())
+                    query = query.order_by(func_lower(col).desc())
             else:
                 raise ValueError('invalid sort direction')
         query = query.offset(start).limit(limit)
         results = query.all()
         if __debug__ and debug_query:
             log.debug("get__range")
             log.debug(query)
             log.debug(results)
         return results
 
     def columns_as_dict(self):
-        return dict((col.name, getattr(self, col.name)) for col in sqlalchemy_orm.class_mapper(self.__class__).mapped_table.c)
+        """
+        Beware: this function will trigger a load of attributes if they have not been loaded yet.
+        """
+        return dict((col.name, getattr(self, col.name))
+                    for col
+                    in sa_class_mapper(self.__class__).mapped_table.c
+                    )
+
+    def loaded_columns_as_dict(self):
+        """
+        This function will only return the loaded columns as a dict.
+        """
+        _dict = self.__dict__
+        return {col.name: _dict[col.name]
+                for col in sa_class_mapper(self.__class__).mapped_table.c
+                if col.name in _dict
+                }
 
 
 class ReflectedTable(UtilityObject):
     """Base class for database objects that are mapped to tables by reflection.
        Have your various model classes inherit from this class.
        If class.__tablename__ is defined, it will reflect that table.
        If class.__primarykey__ is defined, it will set that as the primary key.
```

### Comparing `pyramid_sqlassist-0.9.3/pyramid_sqlassist/tools.py` & `pyramid_sqlassist-0.9.4/pyramid_sqlassist/tools.py`

 * *Files identical despite different names*

### Comparing `pyramid_sqlassist-0.9.3/README.md` & `pyramid_sqlassist-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pyramid_sqlassist-0.9.3/setup.py` & `pyramid_sqlassist-0.9.4/setup.py`

 * *Files identical despite different names*

