# Comparing `tmp/python-univer-1.4.6.tar.gz` & `tmp/python-univer-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-univer-1.4.6.tar", last modified: Sun Jul 23 20:31:15 2023, max compression
+gzip compressed data, was "python-univer-1.4.7.tar", last modified: Tue Jul 25 23:51:25 2023, max compression
```

## Comparing `python-univer-1.4.6.tar` & `python-univer-1.4.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-23 20:31:15.706666 python-univer-1.4.6/
--rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.6/LICENSE
--rw-r--r--   0 user      (1000) user      (1001)     1233 2023-07-23 20:31:15.706666 python-univer-1.4.6/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1001)      706 2023-07-18 16:09:38.000000 python-univer-1.4.6/README.md
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-23 20:31:15.666666 python-univer-1.4.6/python_univer.egg-info/
--rw-r--r--   0 user      (1000) user      (1001)     1233 2023-07-23 20:31:15.000000 python-univer-1.4.6/python_univer.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1001)      732 2023-07-23 20:31:15.000000 python-univer-1.4.6/python_univer.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1001)        1 2023-07-23 20:31:15.000000 python-univer-1.4.6/python_univer.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1001)       18 2023-07-23 20:31:15.000000 python-univer-1.4.6/python_univer.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1001)       10 2023-07-23 20:31:15.000000 python-univer-1.4.6/python_univer.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1001)       38 2023-07-23 20:31:15.706666 python-univer-1.4.6/setup.cfg
--rw-r--r--   0 user      (1000) user      (1001)      891 2023-07-23 20:29:56.000000 python-univer-1.4.6/setup.py
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-23 20:31:15.673333 python-univer-1.4.6/univer_db/
--rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/__init__.py
--rw-r--r--   0 user      (1000) user      (1001)      472 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/config.py
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-23 20:31:15.703333 python-univer-1.4.6/univer_db/models/
--rw-r--r--   0 user      (1000) user      (1001)      225 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/models/__init__.py
--rw-r--r--   0 user      (1000) user      (1001)     9234 2023-07-23 10:05:33.000000 python-univer-1.4.6/univer_db/models/base.py
--rw-r--r--   0 user      (1000) user      (1001)     8231 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/models/dormitories.py
--rw-r--r--   0 user      (1000) user      (1001)     1873 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/models/geo.py
--rw-r--r--   0 user      (1000) user      (1001)      951 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/models/grades.py
--rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/models/groups.py
--rw-r--r--   0 user      (1000) user      (1001)    35329 2023-07-23 11:18:08.000000 python-univer-1.4.6/univer_db/models/models.py
--rw-r--r--   0 user      (1000) user      (1001)     9202 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/models/orders.py
--rw-r--r--   0 user      (1000) user      (1001)    25488 2023-07-23 20:29:29.000000 python-univer-1.4.6/univer_db/models/roles.py
--rw-r--r--   0 user      (1000) user      (1001)     4182 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/models/schedule.py
--rw-r--r--   0 user      (1000) user      (1001)     3558 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/models/sheets.py
--rw-r--r--   0 user      (1000) user      (1001)     5047 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/models/structures.py
--rw-r--r--   0 user      (1000) user      (1001)      769 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/orm.py
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-23 20:31:15.706666 python-univer-1.4.6/univer_db/tests/
--rw-r--r--   0 user      (1000) user      (1001)      264 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/tests/__init__.py
--rw-r--r--   0 user      (1000) user      (1001)      569 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/tests/geo.py
--rw-r--r--   0 user      (1000) user      (1001)     2635 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/tests/models.py
--rw-r--r--   0 user      (1000) user      (1001)     1136 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/tests/roles.py
--rw-r--r--   0 user      (1000) user      (1001)      624 2023-07-18 16:09:38.000000 python-univer-1.4.6/univer_db/tests/structures.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-25 23:51:25.849998 python-univer-1.4.7/
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.7/LICENSE
+-rw-r--r--   0 user      (1000) user      (1001)     1233 2023-07-25 23:51:25.849998 python-univer-1.4.7/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1001)      706 2023-07-18 16:09:38.000000 python-univer-1.4.7/README.md
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-25 23:51:25.846664 python-univer-1.4.7/python_univer.egg-info/
+-rw-r--r--   0 user      (1000) user      (1001)     1233 2023-07-25 23:51:25.000000 python-univer-1.4.7/python_univer.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1001)      732 2023-07-25 23:51:25.000000 python-univer-1.4.7/python_univer.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1001)        1 2023-07-25 23:51:25.000000 python-univer-1.4.7/python_univer.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1001)       18 2023-07-25 23:51:25.000000 python-univer-1.4.7/python_univer.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1001)       10 2023-07-25 23:51:25.000000 python-univer-1.4.7/python_univer.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1001)       38 2023-07-25 23:51:25.849998 python-univer-1.4.7/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1001)      891 2023-07-25 23:51:12.000000 python-univer-1.4.7/setup.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-25 23:51:25.849998 python-univer-1.4.7/univer_db/
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/__init__.py
+-rw-r--r--   0 user      (1000) user      (1001)      472 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/config.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-25 23:51:25.849998 python-univer-1.4.7/univer_db/models/
+-rw-r--r--   0 user      (1000) user      (1001)      225 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/models/__init__.py
+-rw-r--r--   0 user      (1000) user      (1001)     9276 2023-07-25 23:49:51.000000 python-univer-1.4.7/univer_db/models/base.py
+-rw-r--r--   0 user      (1000) user      (1001)     8231 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/models/dormitories.py
+-rw-r--r--   0 user      (1000) user      (1001)     1888 2023-07-25 23:43:54.000000 python-univer-1.4.7/univer_db/models/geo.py
+-rw-r--r--   0 user      (1000) user      (1001)      951 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/models/grades.py
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/models/groups.py
+-rw-r--r--   0 user      (1000) user      (1001)    35417 2023-07-25 23:50:41.000000 python-univer-1.4.7/univer_db/models/models.py
+-rw-r--r--   0 user      (1000) user      (1001)     9229 2023-07-25 23:49:39.000000 python-univer-1.4.7/univer_db/models/orders.py
+-rw-r--r--   0 user      (1000) user      (1001)    25491 2023-07-25 23:48:54.000000 python-univer-1.4.7/univer_db/models/roles.py
+-rw-r--r--   0 user      (1000) user      (1001)     4194 2023-07-25 23:48:54.000000 python-univer-1.4.7/univer_db/models/schedule.py
+-rw-r--r--   0 user      (1000) user      (1001)     3573 2023-07-25 23:48:09.000000 python-univer-1.4.7/univer_db/models/sheets.py
+-rw-r--r--   0 user      (1000) user      (1001)     5071 2023-07-25 23:46:52.000000 python-univer-1.4.7/univer_db/models/structures.py
+-rw-r--r--   0 user      (1000) user      (1001)      769 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/orm.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-07-25 23:51:25.849998 python-univer-1.4.7/univer_db/tests/
+-rw-r--r--   0 user      (1000) user      (1001)      264 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/tests/__init__.py
+-rw-r--r--   0 user      (1000) user      (1001)      569 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/tests/geo.py
+-rw-r--r--   0 user      (1000) user      (1001)     2635 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/tests/models.py
+-rw-r--r--   0 user      (1000) user      (1001)     1136 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/tests/roles.py
+-rw-r--r--   0 user      (1000) user      (1001)      624 2023-07-18 16:09:38.000000 python-univer-1.4.7/univer_db/tests/structures.py
```

### Comparing `python-univer-1.4.6/PKG-INFO` & `python-univer-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-univer
-Version: 1.4.6
+Version: 1.4.7
 Summary: Данная библиотека содержить SqlAlchemy ORM для системы Univer
 Home-page: https://github.com/yessenovuniversity/python_univer
 Author: Nauryzbek Aitbayev
 Author-email: nauryzbek.aitbayev@yu.edu.kz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-univer-1.4.6/README.md` & `python-univer-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.6/python_univer.egg-info/PKG-INFO` & `python-univer-1.4.7/python_univer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-univer
-Version: 1.4.6
+Version: 1.4.7
 Summary: Данная библиотека содержить SqlAlchemy ORM для системы Univer
 Home-page: https://github.com/yessenovuniversity/python_univer
 Author: Nauryzbek Aitbayev
 Author-email: nauryzbek.aitbayev@yu.edu.kz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-univer-1.4.6/python_univer.egg-info/SOURCES.txt` & `python-univer-1.4.7/python_univer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.6/setup.py` & `python-univer-1.4.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="python-univer",
-    version="1.4.6",
+    version="1.4.7",
     author="Nauryzbek Aitbayev",
     author_email="nauryzbek.aitbayev@yu.edu.kz",
     description="Данная библиотека содержить SqlAlchemy ORM для системы Univer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yessenovuniversity/python_univer",
     packages=setuptools.find_packages(),
```

### Comparing `python-univer-1.4.6/univer_db/models/base.py` & `python-univer-1.4.7/univer_db/models/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlalchemy import Column, Integer, String, Float, Boolean, ForeignKey, Date, DateTime
+from sqlalchemy import Column, Integer, String, Float, Boolean, ForeignKey, Date, DateTime, Unicode
 from sqlalchemy.orm import relationship
 
 from univer_db.orm import get_base
 
 
 Base = get_base()
 
@@ -15,22 +15,22 @@
 
     __tablename__ = 'univer_payment_forms'
 
     # Идентификатор
     id = Column('payment_form_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('payment_form_name_ru', String(100))
-    name_kz = Column('payment_form_name_kz', String(100))
-    name_en = Column('payment_form_name_en', String(100))
+    name_ru = Column('payment_form_name_ru', Unicode(100))
+    name_kz = Column('payment_form_name_kz', Unicode(100))
+    name_en = Column('payment_form_name_en', Unicode(100))
 
     # Краткое наименование
-    short_name_ru = Column('payment_form_short_name_ru', String(100))
-    short_name_kz = Column('payment_form_short_name_kz', String(100))
-    short_name_en = Column('payment_form_short_name_en', String(100))
+    short_name_ru = Column('payment_form_short_name_ru', Unicode(100))
+    short_name_kz = Column('payment_form_short_name_kz', Unicode(100))
+    short_name_en = Column('payment_form_short_name_en', Unicode(100))
 
     # Статус
     status = Column(Integer)
 
     def __repr__(self):
         return '<PaymentForm {} (id={} status={})>'.format(self, self.id, self.status)
 
@@ -49,17 +49,17 @@
     # Идентификатор
     id = Column('stage_id', Integer, primary_key=True)
 
     # Статус
     status = Column(Integer)
 
     # Наименование
-    name_kz = Column('stage_name_kz', String(200))
-    name_ru = Column('stage_name_ru', String(200))
-    name_en = Column('stage_name_en', String(200))
+    name_kz = Column('stage_name_kz', Unicode(200))
+    name_ru = Column('stage_name_ru', Unicode(200))
+    name_en = Column('stage_name_en', Unicode(200))
 
     def __repr__(self):
         return "<Stage {} (id={} status={})>".format(self, self.id, self.status)
 
     def __str__(self):
         return self.name_ru
 
@@ -75,17 +75,17 @@
     # Идентификатор
     id = Column('education_form_id', Integer, primary_key=True)
 
     # Статус
     status = Column(Integer)
 
     # Наименование
-    name_kz = Column('education_form_name_kz', String(200))
-    name_ru = Column('education_form_name_ru', String(200))
-    name_en = Column('education_form_name_en', String(200))
+    name_kz = Column('education_form_name_kz', Unicode(200))
+    name_ru = Column('education_form_name_ru', Unicode(200))
+    name_en = Column('education_form_name_en', Unicode(200))
 
     def __repr__(self):
         return "<EducationForm {} (id={} status={})>".format(self, self.id, self.status)
 
     def __str__(self):
         return self.name_ru
 
@@ -98,17 +98,17 @@
 
     __tablename__ = 'univer_edu_levels'
 
     # Идентификатор
     id = Column('edu_level_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('edu_level_name_ru', String(100))
-    name_kz = Column('edu_level_name_kz', String(100))
-    name_en = Column('edu_level_name_en', String(100))
+    name_ru = Column('edu_level_name_ru', Unicode(100))
+    name_kz = Column('edu_level_name_kz', Unicode(100))
+    name_en = Column('edu_level_name_en', Unicode(100))
 
     # Статус
     status = Column(Integer)
 
     def __repr__(self):
         return '<EduLevel {} (id={} status={})'.format(self, self.id, self.status)
 
@@ -122,17 +122,17 @@
     """
     __tablename__ = 'univer_enrollment_type'
 
     # Идентификатор
     id = Column('enrollment_type_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('enrollment_type_name_ru', String(100))
-    name_kz = Column('enrollment_type_name_kz', String(100))
-    name_en = Column('enrollment_type_name_en', String(100))
+    name_ru = Column('enrollment_type_name_ru', Unicode(100))
+    name_kz = Column('enrollment_type_name_kz', Unicode(100))
+    name_en = Column('enrollment_type_name_en', Unicode(100))
 
     # Статус
     status = Column(Integer)
 
     def __repr__(self):
         return '<EnrollmentType {} (id={} status={})>'.format(self, self.id, self.status)
 
@@ -166,22 +166,22 @@
     """
     __tablename__ = 'univer_citizenship_1c'
 
     # Идентификатор
     id = Column('citizenship_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('citizenship_name_ru', String(500))
-    name_kz = Column('citizenship_name_kz', String(500))
-    name_en = Column('citizenship_name_en', String(500))
+    name_ru = Column('citizenship_name_ru', Unicode(500))
+    name_kz = Column('citizenship_name_kz', Unicode(500))
+    name_en = Column('citizenship_name_en', Unicode(500))
 
     # Короткое наименование
-    short_name_ru = Column('citizenship_short_name_ru', String(500))
-    short_name_kz = Column('citizenship_short_name_kz', String(500))
-    short_name_en = Column('citizenship_short_name_en', String(500))
+    short_name_ru = Column('citizenship_short_name_ru', Unicode(500))
+    short_name_kz = Column('citizenship_short_name_kz', Unicode(500))
+    short_name_en = Column('citizenship_short_name_en', Unicode(500))
 
     # ISO-коды
     code = Column('citizenship_code', Integer)
     code2 = Column('citizenship_code2', String(250))
     code3 = Column('citizenship_code3', String(250))
 
     # Статус
@@ -203,22 +203,22 @@
     # Идентификатор
     id = Column('nationality_id', Integer, primary_key=True)
 
     # Статус
     status = Column(Integer)
 
     # Наименование
-    name_ru = Column('nationality_name_ru', String(100))
-    name_kz = Column('nationality_name_kz', String(100))
-    name_en = Column('nationality_name_en', String(100))
+    name_ru = Column('nationality_name_ru', Unicode(100))
+    name_kz = Column('nationality_name_kz', Unicode(100))
+    name_en = Column('nationality_name_en', Unicode(100))
 
     # Короткое наименование
-    short_name_ru = Column('nationality_short_name_ru', String(20))
-    short_name_kz = Column('nationality_short_name_kz', String(20))
-    short_name_en = Column('nationality_short_name_en', String(20))
+    short_name_ru = Column('nationality_short_name_ru', Unicode(20))
+    short_name_kz = Column('nationality_short_name_kz', Unicode(20))
+    short_name_en = Column('nationality_short_name_en', Unicode(20))
 
     def __repr__(self):
         return '<Nationality {} (id={} status={})>'.format(self, self.id, self.status)
 
     def __str__(self):
         return self.name_ru
 
@@ -288,17 +288,17 @@
     """
     __tablename__ = 'univer_family_status_1c'
 
     # Идентификатор
     id = Column('family_status_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('family_status_name_ru', String(500))
-    name_kz = Column('family_status_name_kz', String(500))
-    name_en = Column('family_status_name_en', String(500))
+    name_ru = Column('family_status_name_ru', Unicode(500))
+    name_kz = Column('family_status_name_kz', Unicode(500))
+    name_en = Column('family_status_name_en', Unicode(500))
 
     # Статус
     status = Column(Integer)
 
     def __repr__(self):
         return '<FamilyStatus {} (id={} status={})>'.format(self, self.id, self.status)
```

### Comparing `python-univer-1.4.6/univer_db/models/dormitories.py` & `python-univer-1.4.7/univer_db/models/dormitories.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.6/univer_db/models/geo.py` & `python-univer-1.4.7/univer_db/models/geo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlalchemy import Column, Integer, String, ForeignKey
+from sqlalchemy import Column, Integer, String, ForeignKey, Unicode
 from sqlalchemy.orm import relationship
 
 from univer_db.orm import get_base
 
 
 Base = get_base()
 
@@ -13,17 +13,17 @@
     """
     __tablename__ = 'abiturient_reg_ats_types'
 
     # Идентификатор
     id = Column(Integer, primary_key=True)
 
     # Наименование
-    value_ru = Column(String(100))
-    value_kz = Column(String(100))
-    value_en = Column(String(100))
+    value_ru = Column(Unicode(100))
+    value_kz = Column(Unicode(100))
+    value_en = Column(Unicode(100))
 
     # Код
     code = Column(Integer)
 
     # Актуальный
     actual = Column(Integer)
 
@@ -51,17 +51,17 @@
     parents = Column(String(100))
 
     # Тип
     type_id = Column('d_ats_type_id', ForeignKey('abiturient_reg_ats_types.id'))
     type = relationship('AbiturientRegAtsType')
 
     # Наименование
-    name_ru = Column('name_rus', String(240))
-    name_kz = Column('name_kaz', String(240))
-    name_en = Column('name_eng', String(240))
+    name_ru = Column('name_rus', Unicode(240))
+    name_kz = Column('name_kaz', Unicode(240))
+    name_en = Column('name_eng', Unicode(240))
 
     # RCO
     rco = Column(String(20))
 
     # КАТО
     cato = Column(String(20))
```

### Comparing `python-univer-1.4.6/univer_db/models/grades.py` & `python-univer-1.4.7/univer_db/models/grades.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.6/univer_db/models/models.py` & `python-univer-1.4.7/univer_db/models/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlalchemy import Column, Integer, String, Float, Boolean, ForeignKey, Date, DateTime
+from sqlalchemy import Column, Integer, String, Float, Boolean, ForeignKey, Date, DateTime, Unicode
 from sqlalchemy.orm import relationship, validates
 
 from univer_db.orm import get_base
 
 
 Base = get_base()
 
@@ -17,33 +17,33 @@
 
     id = Column('speciality_id', Integer, primary_key=True)
     status = Column(Integer)
     faculty_id = Column(ForeignKey('univer_faculty.faculty_id'))
     faculty = relationship('Faculty')
     stage_id = Column(ForeignKey('univer_stage.stage_id'))
     stage = relationship('Stage')
-    name_kz = Column('speciality_name_kz', String(200))
-    name_ru = Column('speciality_name_ru', String(200))
-    name_en = Column('speciality_name_en', String(200))
+    name_kz = Column('speciality_name_kz', Unicode(200))
+    name_ru = Column('speciality_name_ru', Unicode(200))
+    name_en = Column('speciality_name_en', Unicode(200))
     code = Column('speciality_okpd', String(10))
-    requirements_kz = Column('speciality_requirements_kz', String)
-    requirements_ru = Column('speciality_requirements_ru', String)
-    requirements_en = Column('speciality_requirements_en', String)
-    description_kz = Column('speciality_discription_kz', String)
-    description_ru = Column('speciality_discription_ru', String)
-    description_en = Column('speciality_discription_en', String)
-    further_study_kz = Column('speciality_access_further_study_kz', String)
-    further_study_ru = Column('speciality_access_further_study_ru', String)
-    further_study_en = Column('speciality_access_further_study_en', String)
-    prof_status_kz = Column('speciality_prof_status_kz', String)
-    prof_status_ru = Column('speciality_prof_status_ru', String)
-    prof_status_en = Column('speciality_prof_status_en', String)
-    result_ru = Column(String)
-    result_kz = Column(String)
-    result_en = Column(String)
+    requirements_kz = Column('speciality_requirements_kz', Unicode)
+    requirements_ru = Column('speciality_requirements_ru', Unicode)
+    requirements_en = Column('speciality_requirements_en', Unicode)
+    description_kz = Column('speciality_discription_kz', Unicode)
+    description_ru = Column('speciality_discription_ru', Unicode)
+    description_en = Column('speciality_discription_en', Unicode)
+    further_study_kz = Column('speciality_access_further_study_kz', Unicode)
+    further_study_ru = Column('speciality_access_further_study_ru', Unicode)
+    further_study_en = Column('speciality_access_further_study_en', Unicode)
+    prof_status_kz = Column('speciality_prof_status_kz', Unicode)
+    prof_status_ru = Column('speciality_prof_status_ru', Unicode)
+    prof_status_en = Column('speciality_prof_status_en', Unicode)
+    result_ru = Column(Unicode)
+    result_kz = Column(Unicode)
+    result_en = Column(Unicode)
     type = Column(Integer)
 
     def __repr__(self):
         return "<Speciality {}>".format(self)
 
     def __str__(self):
         return "{} - {}".format(self.code, self.name_ru)
@@ -83,22 +83,22 @@
     # 0 - Обязательная дисциплина
     # 1 - Элективная дисциплина
     # 2 - Практика
     # 3 - Спец. дисциплина
     type = Column('subject_type', Integer)
 
     # Наименование
-    name_kz = Column('subject_name_kz', String(500))
-    name_ru = Column('subject_name_ru', String(500))
-    name_en = Column('subject_name_en', String(500))
+    name_kz = Column('subject_name_kz', Unicode(500))
+    name_ru = Column('subject_name_ru', Unicode(500))
+    name_en = Column('subject_name_en', Unicode(500))
 
     # Описание
-    description_kz = Column('subject_description_kz', String)
-    description_ru = Column('subject_description_ru', String)
-    description_en = Column('subject_description_en', String)
+    description_kz = Column('subject_description_kz', Unicode)
+    description_ru = Column('subject_description_ru', Unicode)
+    description_en = Column('subject_description_en', Unicode)
 
     # Статус
     status = Column(Integer)
 
     def __repr__(self):
         return f'<Subject {self} (id={self.id} status={self.status} type={self.type})>'
 
@@ -112,17 +112,17 @@
     """
     __tablename__ = 'univer_educ_type'
 
     # Идентификатор
     id = Column('educ_type_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('educ_type_name_ru', String(100))
-    name_kz = Column('educ_type_name_kz', String(100))
-    name_en = Column('educ_type_name_en', String(100))
+    name_ru = Column('educ_type_name_ru', Unicode(100))
+    name_kz = Column('educ_type_name_kz', Unicode(100))
+    name_en = Column('educ_type_name_en', Unicode(100))
 
     def __repr__(self):
         return '<EducType {}>'.format(self.name_ru)
 
     def __str__(self):
         return self.name_ru
 
@@ -133,17 +133,17 @@
     """
     __tablename__ = 'univer_lang_division'
 
     # Идентификатор
     id = Column('lang_division_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('lang_division_name_ru', String(100))
-    name_kz = Column('lang_division_name_kz', String(100))
-    name_en = Column('lang_division_name_en', String(100))
+    name_ru = Column('lang_division_name_ru', Unicode(100))
+    name_kz = Column('lang_division_name_kz', Unicode(100))
+    name_en = Column('lang_division_name_en', Unicode(100))
 
     # Статус
     status = Column(Integer)
 
     def __repr__(self):
         return '<LangDivision {} (id={}, status={})>'.format(self, self.id, self.status)
 
@@ -154,17 +154,17 @@
 class DocumentIdentity(Base):
     """
     Тип документа
     """
     __tablename__ = 'univer_document_identity'
 
     id = Column('document_identity_type', Integer, primary_key=True)
-    name_ru = Column('document_name_ru', String(100))
-    name_kz = Column('document_name_kz', String(100))
-    name_en = Column('document_name_en', String(100))
+    name_ru = Column('document_name_ru', Unicode(100))
+    name_kz = Column('document_name_kz', Unicode(100))
+    name_en = Column('document_name_en', Unicode(100))
 
     def __repr__(self):
         return '<DocumentIdentity {} (id={})'.format(self, self.id)
 
     def __str__(self):
         return self.name_ru
 
@@ -174,17 +174,17 @@
     Модель "Учебное заведение"
     Статус: Выполняется
     """
 
     __tablename__ = 'univer_edu_institutions'
 
     id = Column('edu_institution_id', Integer, primary_key=True)
-    name_kz = Column('edu_institution_name_kz', String)
-    name_ru = Column('edu_institution_name_ru', String)
-    name_en = Column('edu_institution_name_en', String)
+    name_kz = Column('edu_institution_name_kz', Unicode)
+    name_ru = Column('edu_institution_name_ru', Unicode)
+    name_en = Column('edu_institution_name_en', Unicode)
 
     def __repr__(self):
         return '<Institution {} (id={})>'.format(self, self.id)
 
     def __str__(self):
         return self.name_ru
 
@@ -195,17 +195,17 @@
     """
     __tablename__ = 'univer_graduate_doctypes'
 
     # Идентификатор
     id = Column('graduate_doctype_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('graduate_doctype_name_ru', String)
-    name_kz = Column('graduate_doctype_name_kz', String)
-    name_en = Column('graduate_doctype_name_en', String)
+    name_ru = Column('graduate_doctype_name_ru', Unicode)
+    name_kz = Column('graduate_doctype_name_kz', Unicode)
+    name_en = Column('graduate_doctype_name_en', Unicode)
 
     def __repr__(self):
         return '<GraduateDocType {} (id={})>'.format(self, self.id)
 
     def __str__(self):
         return self.name_ru
 
@@ -220,15 +220,15 @@
     # Идентификатор
     id = Column('graduate_info_id', Integer, primary_key=True)
 
     # Дата выдачи
     date = Column('graduate_info_date', DateTime)
 
     # Наименование учебного заведения
-    institution_name = Column('graduate_info_institution_name', String)
+    institution_name = Column('graduate_info_institution_name', Unicode)
 
     # Тип учебного заведения
     institution_type_id = Column(
         'edu_institution_type_id', ForeignKey('univer_edu_institution_types.edu_institution_type_id')
     )
     institution_type = relationship('InstitutionType')
 
@@ -264,17 +264,17 @@
     """
     __tablename__ = 'univer_edu_institution_types'
 
     # Идентификатор
     id = Column('edu_institution_type_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('edu_institution_type_name_ru', String(100))
-    name_kz = Column('edu_institution_type_name_kz', String(100))
-    name_en = Column('edu_institution_type_name_en', String(100))
+    name_ru = Column('edu_institution_type_name_ru', Unicode(100))
+    name_kz = Column('edu_institution_type_name_kz', Unicode(100))
+    name_en = Column('edu_institution_type_name_en', Unicode(100))
 
     # Статус
     status = Column('status', Integer)
 
     def __repr__(self):
         return '<InstitutionType {} (id={} status={})>'.format(self, self.id, self.status)
 
@@ -414,17 +414,17 @@
     """
     __tablename__ = 'univer_cycles'
 
     # Идентификатор
     id = Column('cycle_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('cycle_name_ru', String)
-    name_kz = Column('cycle_name_kz', String)
-    name_en = Column('cycle_name_en', String)
+    name_ru = Column('cycle_name_ru', Unicode)
+    name_kz = Column('cycle_name_kz', Unicode)
+    name_en = Column('cycle_name_en', Unicode)
 
     def __repr__(self):
         return '<Cycle {}>'.format(self)
 
     def __str__(self):
         return self.name_ru
 
@@ -438,20 +438,20 @@
     # Идентификатор
     id = Column('cycle_component_id', Integer, primary_key=True)
 
     # Статус
     status = Column(Integer)
 
     # Наименование
-    name_ru = Column('cycle_component_name_ru', String)
-    name_kz = Column('cycle_component_name_kz', String)
-    name_en = Column('cycle_component_name_en', String)
-    short_name_ru = Column('cycle_component_short_name_ru', String)
-    short_name_kz = Column('cycle_component_short_name_kz', String)
-    short_name_en = Column('cycle_component_short_name_en', String)
+    name_ru = Column('cycle_component_name_ru', Unicode)
+    name_kz = Column('cycle_component_name_kz', Unicode)
+    name_en = Column('cycle_component_name_en', Unicode)
+    short_name_ru = Column('cycle_component_short_name_ru', Unicode)
+    short_name_kz = Column('cycle_component_short_name_kz', Unicode)
+    short_name_en = Column('cycle_component_short_name_en', Unicode)
 
     def __repr__(self):
         return f'<CycleComponent {self} (id={self.id} status={self.status})>'
 
     def __str__(self):
         return self.name_ru
 
@@ -503,22 +503,22 @@
     """
     __tablename__ = 'univer_educ_lang'
 
     # Идентификатор
     id = Column('educ_lang_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('educ_lang_name_ru', String)
-    name_kz = Column('educ_lang_name_kz', String)
-    name_en = Column('educ_lang_name_en', String)
+    name_ru = Column('educ_lang_name_ru', Unicode)
+    name_kz = Column('educ_lang_name_kz', Unicode)
+    name_en = Column('educ_lang_name_en', Unicode)
 
     # Короткое наименование
-    short_name_ru = Column('educ_lang_short_name_ru', String)
-    short_name_kz = Column('educ_lang_short_name_kz', String)
-    short_name_en = Column('educ_lang_short_name_en', String)
+    short_name_ru = Column('educ_lang_short_name_ru', Unicode)
+    short_name_kz = Column('educ_lang_short_name_kz', Unicode)
+    short_name_en = Column('educ_lang_short_name_en', Unicode)
 
     # Статус
     status = Column(Integer)
 
     def __repr__(self):
         return '<EducLang {}>'.format(self)
 
@@ -630,22 +630,22 @@
     """
     __tablename__ = 'univer_control'
 
     # Идентификатор
     id = Column('control_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('control_name_ru', String(100))
-    name_kz = Column('control_name_kz', String(100))
-    name_en = Column('control_name_en', String(100))
+    name_ru = Column('control_name_ru', Unicode(100))
+    name_kz = Column('control_name_kz', Unicode(100))
+    name_en = Column('control_name_en', Unicode(100))
 
     # Короткое наименование
-    short_name_ru = Column('control_short_name_ru', String)
-    short_name_kz = Column('control_short_name_kz', String)
-    short_name_en = Column('control_short_name_en', String)
+    short_name_ru = Column('control_short_name_ru', Unicode)
+    short_name_kz = Column('control_short_name_kz', Unicode)
+    short_name_en = Column('control_short_name_en', Unicode)
 
     # Максимальная оценка
     max_ball = Column('control_max_ball', Integer)
 
     # Статус
     status = Column(Integer)
 
@@ -668,17 +668,17 @@
 
     __tablename__ = 'univer_controll_type'
 
     # Идентификатор
     id = Column('controll_type_id', Integer, primary_key=True)
 
     # Наименование
-    name_kz = Column('controll_type_name_kz', String(100))
-    name_ru = Column('controll_type_name_ru', String(100))
-    name_en = Column('controll_type_name_en', String(100))
+    name_kz = Column('controll_type_name_kz', Unicode(100))
+    name_ru = Column('controll_type_name_ru', Unicode(100))
+    name_en = Column('controll_type_name_en', Unicode(100))
 
     def __repr__(self):
         return '<ControllType {}>'.format(self)
 
     def __str__(self):
         return self.name_ru
 
@@ -740,22 +740,22 @@
     # Максимальное значение
     max_val = Column('mark_type_maxval', Integer)
 
     # GPA
     gpa = Column('mark_type_gpa', Float)
 
     # Наименование
-    name_ru = Column('mark_text_ru', String(50))
-    name_kz = Column('mark_text_kz', String(50))
-    name_en = Column('mark_text_en', String(50))
+    name_ru = Column('mark_text_ru', Unicode(50))
+    name_kz = Column('mark_text_kz', Unicode(50))
+    name_en = Column('mark_text_en', Unicode(50))
 
     # Короткое наименование
-    short_name_ru = Column('mark_text_short_ru', String(10))
-    short_name_kz = Column('mark_text_short_kz', String(10))
-    short_name_en = Column('mark_text_short_en', String(10))
+    short_name_ru = Column('mark_text_short_ru', Unicode(10))
+    short_name_kz = Column('mark_text_short_kz', Unicode(10))
+    short_name_en = Column('mark_text_short_en', Unicode(10))
 
     # Статус
     # Возможные значения:
     # - 1 (Активный)
     # - 2 (Архивный)
     status = Column('mark_status', Integer)
 
@@ -1111,17 +1111,17 @@
         return value
 
     # Регион
     region_id = Column(ForeignKey('univer_region.region_id'))
     region = relationship('Region')
 
     # Наименование
-    name_ru = Column('district_name_ru', String())
-    name_kz = Column('district_name_kz', String())
-    name_en = Column('district_name_en', String())
+    name_ru = Column('district_name_ru', Unicode())
+    name_kz = Column('district_name_kz', Unicode())
+    name_en = Column('district_name_en', Unicode())
 
     # Код района
     code = Column('district_code', Integer)
 
     # Текущий район
     current = Column('current_district', Integer)
 
@@ -1155,16 +1155,16 @@
     educ_plan_id = Column(ForeignKey('univer_educ_plan.educ_plan_id'))
     educ_plan = relationship('EducPlan')
 
     # Семестр позиции учебного плана
     educ_plan_pos_semester = Column('educ_plan_pos_semestr', Integer)
 
     # Наименование
-    name_ru = Column('pos_group_name_ru', String)
-    name_kz = Column('pos_group_name_kz', String)
-    name_en = Column('pos_group_name_en', String)
+    name_ru = Column('pos_group_name_ru', Unicode)
+    name_kz = Column('pos_group_name_kz', Unicode)
+    name_en = Column('pos_group_name_en', Unicode)
 
     def __repr__(self):
         return f'<EducPlanPosGroup {self} (id={self.id} educ_plan_id={self.educ_plan_id})>'
 
     def __str__(self):
         return self.name_ru
```

### Comparing `python-univer-1.4.6/univer_db/models/orders.py` & `python-univer-1.4.7/univer_db/models/orders.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlalchemy import Column, Integer, String, Float, Boolean, ForeignKey, Date, DateTime
+from sqlalchemy import Column, Integer, String, Float, Boolean, ForeignKey, Date, DateTime, Unicode
 from sqlalchemy.orm import relationship, validates
 
 from univer_db.orm import get_base
 
 
 Base = get_base()
 
@@ -119,17 +119,17 @@
         - 1 (Активный)
         - 2 (Архивный)
         """
         assert value in [1, 2]
         return value
 
     # Наименование
-    name_ru = Column('order_type_name_ru', String(300))
-    name_kz = Column('order_type_name_kz', String(300))
-    name_en = Column('order_type_name_en', String(300))
+    name_ru = Column('order_type_name_ru', Unicode(300))
+    name_kz = Column('order_type_name_kz', Unicode(300))
+    name_en = Column('order_type_name_en', Unicode(300))
 
     # Неизвестное поле
     template = Column('order_type_template', String(150))
 
     # Неизвестное поле
     need_signed = Column('order_type_need_signed', Integer)
 
@@ -155,27 +155,27 @@
     """
     __tablename__ = 'univer_order_action'
 
     # Идентификатор
     id = Column('order_action_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('order_action_name_ru', String(500))
-    name_kz = Column('order_action_name_kz', String(500))
-    name_en = Column('order_action_name_en', String(500))
+    name_ru = Column('order_action_name_ru', Unicode(500))
+    name_kz = Column('order_action_name_kz', Unicode(500))
+    name_en = Column('order_action_name_en', Unicode(500))
 
     # Короткое наименование
-    short_name_ru = Column('order_action_short_name_ru', String(200))
-    short_name_kz = Column('order_action_short_name_kz', String(200))
-    short_name_en = Column('order_action_short_name_en', String(200))
+    short_name_ru = Column('order_action_short_name_ru', Unicode(200))
+    short_name_kz = Column('order_action_short_name_kz', Unicode(200))
+    short_name_en = Column('order_action_short_name_en', Unicode(200))
 
     # ???
-    value_ru = Column('order_action_value_ru', String(250))
-    value_kz = Column('order_action_value_kz', String(250))
-    value_en = Column('order_action_value_en', String(250))
+    value_ru = Column('order_action_value_ru', Unicode(250))
+    value_kz = Column('order_action_value_kz', Unicode(250))
+    value_en = Column('order_action_value_en', Unicode(250))
 
     # Тип приказа
     order_type_id = Column(ForeignKey('univer_order_type.order_type_id'))
     order_type = relationship('OrderType')
 
     # Статус
     status = Column(Integer)
@@ -218,17 +218,17 @@
     """
     __tablename__ = 'univer_order_reason_link'
 
     # Идентификатор
     id = Column('order_reason_link_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('order_reason_link_text_ru', String)
-    name_kz = Column('order_reason_link_text_kz', String)
-    name_en = Column('order_reason_link_text_en', String)
+    name_ru = Column('order_reason_link_text_ru', Unicode)
+    name_kz = Column('order_reason_link_text_kz', Unicode)
+    name_en = Column('order_reason_link_text_en', Unicode)
 
     # Статус
     # Возможные значения:
     # - 1 (Активный)
     # - 2 (Архивный)
     status = Column(Integer)
 
@@ -255,17 +255,17 @@
     """
     __tablename__ = 'univer_order_reasons'
 
     # Идентификатор
     id = Column('order_reason_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('order_reason_name_ru', String(500))
-    name_kz = Column('order_reason_name_kz', String(500))
-    name_en = Column('order_reason_name_en', String(500))
+    name_ru = Column('order_reason_name_ru', Unicode(500))
+    name_kz = Column('order_reason_name_kz', Unicode(500))
+    name_en = Column('order_reason_name_en', Unicode(500))
 
     # Статус студента
     edu_status_id = Column('student_edu_status_id', ForeignKey(
         'univer_student_edu_statuses.student_edu_status_id'))
     edu_status = relationship('EduStatus')
 
     # Статус
```

### Comparing `python-univer-1.4.6/univer_db/models/roles.py` & `python-univer-1.4.7/univer_db/models/roles.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,17 +373,17 @@
     """
     __tablename__ = 'univer_parent_types'
 
     # Идентификатор
     id = Column('parent_type_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column(String(200))
-    name_kz = Column(String(200))
-    name_en = Column(String(200))
+    name_ru = Column(Unicode(200))
+    name_kz = Column(Unicode(200))
+    name_en = Column(Unicode(200))
 
     # Пол
     # 0 - Мужчина, 1 - Женщина
     sex = Column(Integer)
 
     # Статус
     # 1 - Активный
```

### Comparing `python-univer-1.4.6/univer_db/models/schedule.py` & `python-univer-1.4.7/univer_db/models/schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlalchemy import Column, Integer, String, Float, Boolean, ForeignKey, Date, DateTime, Time
+from sqlalchemy import Column, Integer, String, Float, Boolean, ForeignKey, Date, DateTime, Time, Unicode
 from sqlalchemy.orm import relationship
 
 from univer_db.orm import get_base
 
 
 Base = get_base()
 
@@ -13,21 +13,21 @@
     """
     __tablename__ = 'univer_schedule_time_type'
 
     # Идентификтор
     id = Column('schedule_time_type_id', Integer, primary_key=True)
 
     # Наименование (на казахском)
-    name_kz = Column('schedule_time_type_name_kz', String)
+    name_kz = Column('schedule_time_type_name_kz', Unicode)
 
     # Наименование (на русском)
-    name_ru = Column('schedule_time_type_name_ru', String)
+    name_ru = Column('schedule_time_type_name_ru', Unicode)
 
     # Наименование (на английском)
-    name_en = Column('schedule_time_type_name_en', String)
+    name_en = Column('schedule_time_type_name_en', Unicode)
 
     def __repr__(self):
         return '<ScheduleTimeType {}>'.format(self)
 
     def __str__(self):
         return str(self.id)
```

### Comparing `python-univer-1.4.6/univer_db/models/sheets.py` & `python-univer-1.4.7/univer_db/models/sheets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlalchemy import Column, Integer, String, Float, Boolean, ForeignKey, Date, DateTime, REAL
+from sqlalchemy import Column, Integer, String, Float, Boolean, ForeignKey, Date, DateTime, REAL, Unicode
 from sqlalchemy.orm import relationship
 
 from univer_db.orm import get_base
 
 
 Base = get_base()
 
@@ -53,22 +53,22 @@
     """
     __tablename__ = 'univer_sheet_type'
 
     # Идентификатор
     id = Column('sheet_type_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('sheet_type_name_ru', String(200))
-    name_kz = Column('sheet_type_name_kz', String(200))
-    name_en = Column('sheet_type_name_en', String(200))
+    name_ru = Column('sheet_type_name_ru', Unicode(200))
+    name_kz = Column('sheet_type_name_kz', Unicode(200))
+    name_en = Column('sheet_type_name_en', Unicode(200))
 
     # Короткое наименование
-    short_name_ru = Column('sheet_type_short_name_ru', String)
-    short_name_kz = Column('sheet_type_short_name_kz', String)
-    short_name_en = Column('sheet_type_short_name_en', String)
+    short_name_ru = Column('sheet_type_short_name_ru', Unicode)
+    short_name_kz = Column('sheet_type_short_name_kz', Unicode)
+    short_name_en = Column('sheet_type_short_name_en', Unicode)
 
     # Статус
     status = Column(Integer)
 
     def __repr__(self):
         return '<SheetType {} (id={} status={})>'.format(self, self.id, self.status)
```

### Comparing `python-univer-1.4.6/univer_db/models/structures.py` & `python-univer-1.4.7/univer_db/models/structures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlalchemy import Column, Integer, String, Float, Boolean, ForeignKey, Date, DateTime
+from sqlalchemy import Column, Integer, String, Float, Boolean, ForeignKey, Date, DateTime, Unicode
 from sqlalchemy.orm import relationship
 
 from univer_db.orm import get_base
 
 
 Base = get_base()
 
@@ -14,17 +14,17 @@
 
     __tablename__ = 'univer_structure_division_1c'
 
     # Идентификатор
     id = Column('structure_division_id', Integer, primary_key=True)
 
     # Наименование
-    name_kz = Column('structure_division_name_kz', String(500))
-    name_ru = Column('structure_division_name_ru', String(500))
-    name_en = Column('structure_division_name_en', String(500))
+    name_kz = Column('structure_division_name_kz', Unicode(500))
+    name_ru = Column('structure_division_name_ru', Unicode(500))
+    name_en = Column('structure_division_name_en', Unicode(500))
 
     # Родительское подразделение
     parent_id = Column('structure_division_ext', ForeignKey(
         'univer_structure_division_1c.structure_division_id'))
     parent = relationship('StructureDivision',
                           remote_side='StructureDivision.id')
 
@@ -44,17 +44,17 @@
     """
     __tablename__ = 'univer_type_personal_1c'
 
     # Идентификатор
     id = Column('type_personal_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('type_personal_name_ru', String(100))
-    name_kz = Column('type_personal_name_kz', String(100))
-    name_en = Column('type_personal_name_en', String(100))
+    name_ru = Column('type_personal_name_ru', Unicode(100))
+    name_kz = Column('type_personal_name_kz', Unicode(100))
+    name_en = Column('type_personal_name_en', Unicode(100))
 
     # Статус
     status = Column(Integer)
 
     def __repr__(self):
         return '<PersonnelType {} (id={} status={})'.format(self, self.id, self.status)
 
@@ -109,17 +109,17 @@
     Модель "Факультет"
     """
 
     __tablename__ = 'univer_faculty'
 
     id = Column('faculty_id', Integer, primary_key=True)
     status = Column(Integer)
-    name_kz = Column('faculty_name_kz', String(200))
-    name_ru = Column('faculty_name_ru', String(200))
-    name_en = Column('faculty_name_en', String(200))
+    name_kz = Column('faculty_name_kz', Unicode(200))
+    name_ru = Column('faculty_name_ru', Unicode(200))
+    name_en = Column('faculty_name_en', Unicode(200))
 
     def __repr__(self):
         return "<Faculty {}>".format(self)
 
     def __str__(self):
         return self.name_ru
 
@@ -131,17 +131,17 @@
 
     __tablename__ = 'univer_chair'
 
     id = Column('chair_id', Integer, primary_key=True)
     faculty_id = Column(ForeignKey('univer_faculty.faculty_id'))
     faculty = relationship('Faculty')
     status = Column(Integer)
-    name_kz = Column('chair_name_kz', String(200))
-    name_ru = Column('chair_name_ru', String(200))
-    name_en = Column('chair_name_en', String(200))
+    name_kz = Column('chair_name_kz', Unicode(200))
+    name_ru = Column('chair_name_ru', Unicode(200))
+    name_en = Column('chair_name_en', Unicode(200))
     structure_division_id = Column(ForeignKey(
         'univer_structure_division_1c.structure_division_id'))
     structure_division = relationship('StructureDivision')
 
     def __repr__(self):
         return '<Chair {}>'.format(self)
 
@@ -155,17 +155,17 @@
     """
     __tablename__ = 'univer_personal_position_1c'
 
     # Идентификатор
     id = Column('personal_position_id', Integer, primary_key=True)
 
     # Наименование
-    name_ru = Column('personal_position_name_ru', String(500))
-    name_kz = Column('personal_position_name_kz', String(500))
-    name_en = Column('personal_position_name_en', String(500))
+    name_ru = Column('personal_position_name_ru', Unicode(500))
+    name_kz = Column('personal_position_name_kz', Unicode(500))
+    name_en = Column('personal_position_name_en', Unicode(500))
 
     # Статус
     status = Column(Integer)
 
     def __repr__(self):
         return '<PersonnelPosition {}>'.format(self)
```

### Comparing `python-univer-1.4.6/univer_db/orm.py` & `python-univer-1.4.7/univer_db/orm.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.6/univer_db/tests/geo.py` & `python-univer-1.4.7/univer_db/tests/geo.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.6/univer_db/tests/models.py` & `python-univer-1.4.7/univer_db/tests/models.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.6/univer_db/tests/roles.py` & `python-univer-1.4.7/univer_db/tests/roles.py`

 * *Files identical despite different names*

### Comparing `python-univer-1.4.6/univer_db/tests/structures.py` & `python-univer-1.4.7/univer_db/tests/structures.py`

 * *Files identical despite different names*

