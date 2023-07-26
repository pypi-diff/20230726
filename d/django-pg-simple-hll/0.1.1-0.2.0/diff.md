# Comparing `tmp/django_pg_simple_hll-0.1.1.tar.gz` & `tmp/django_pg_simple_hll-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pg_simple_hll-0.1.1.tar", max compression
+gzip compressed data, was "django_pg_simple_hll-0.2.0.tar", max compression
```

## Comparing `django_pg_simple_hll-0.1.1.tar` & `django_pg_simple_hll-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0     1066 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/LICENSE
--rw-r--r--   0        0        0    10927 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/django_pg_simple_hll/__init__.py
--rw-r--r--   0        0        0      688 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/django_pg_simple_hll/aggregate.py
--rw-r--r--   0        0        0      528 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/django_pg_simple_hll/migrations/0001_initial.py
--rw-r--r--   0        0        0      344 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/django_pg_simple_hll/migrations/0001_initial.reverse.sql
--rw-r--r--   0        0        0     5679 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/django_pg_simple_hll/migrations/0001_initial.sql
--rw-r--r--   0        0        0        0 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/django_pg_simple_hll/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/django_pg_simple_hll/py.typed
--rw-r--r--   0        0        0     2957 2023-05-09 16:00:29.523597 django_pg_simple_hll-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    12069 1970-01-01 00:00:00.000000 django_pg_simple_hll-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-26 13:17:51.369202 django_pg_simple_hll-0.2.0/LICENSE
+-rw-r--r--   0        0        0    13256 2023-07-26 13:17:51.369202 django_pg_simple_hll-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 13:17:51.369202 django_pg_simple_hll-0.2.0/django_pg_simple_hll/__init__.py
+-rw-r--r--   0        0        0     1482 2023-07-26 13:17:51.369202 django_pg_simple_hll-0.2.0/django_pg_simple_hll/aggregate.py
+-rw-r--r--   0        0        0      320 2023-07-26 13:17:51.369202 django_pg_simple_hll-0.2.0/django_pg_simple_hll/functions.py
+-rw-r--r--   0        0        0      284 2023-07-26 13:17:51.369202 django_pg_simple_hll-0.2.0/django_pg_simple_hll/migrations/0001_initial.py
+-rw-r--r--   0        0        0      344 2023-07-26 13:17:51.369202 django_pg_simple_hll-0.2.0/django_pg_simple_hll/migrations/0001_initial.reverse.sql
+-rw-r--r--   0        0        0     5679 2023-07-26 13:17:51.369202 django_pg_simple_hll-0.2.0/django_pg_simple_hll/migrations/0001_initial.sql
+-rw-r--r--   0        0        0      339 2023-07-26 13:17:51.369202 django_pg_simple_hll-0.2.0/django_pg_simple_hll/migrations/0002_custom_hashing.py
+-rw-r--r--   0        0        0      526 2023-07-26 13:17:51.369202 django_pg_simple_hll-0.2.0/django_pg_simple_hll/migrations/0002_custom_hashing.reverse.sql
+-rw-r--r--   0        0        0     6803 2023-07-26 13:17:51.369202 django_pg_simple_hll-0.2.0/django_pg_simple_hll/migrations/0002_custom_hashing.sql
+-rw-r--r--   0        0        0      830 2023-07-26 13:17:51.369202 django_pg_simple_hll-0.2.0/django_pg_simple_hll/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:17:51.369202 django_pg_simple_hll-0.2.0/django_pg_simple_hll/py.typed
+-rw-r--r--   0        0        0     3089 2023-07-26 13:17:51.369202 django_pg_simple_hll-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    14198 1970-01-01 00:00:00.000000 django_pg_simple_hll-0.2.0/PKG-INFO
```

### Comparing `django_pg_simple_hll-0.1.1/LICENSE` & `django_pg_simple_hll-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pg_simple_hll-0.1.1/README.md` & `django_pg_simple_hll-0.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -118,14 +118,39 @@
  {'date_of_session': datetime.date(2023, 4, 30), 'approx_unique_users': 63159},
  {'date_of_session': datetime.date(2023, 5, 1), 'approx_unique_users': 83371},
  {'date_of_session': datetime.date(2023, 5, 2), 'approx_unique_users': 96185},
  {'date_of_session': datetime.date(2023, 5, 3), 'approx_unique_users': 116565},
  {'date_of_session': datetime.date(2023, 5, 4), 'approx_unique_users': 143588}]
 ```
 
+HLL works by hashing each value it considers. For some reason, the aggregation is sometimes faster when that hashing is performed outside of the aggregation. So, it is also available in two separate steps:
+
+```python
+%%time
+list(
+    Session.objects
+        .annotate(date_of_session=TruncDate("created"))
+        .values("date_of_session")
+        .annotate(approx_unique_users=HLLCardinalityFromHash(HLLHash("user_uuid"), 9))
+        .values("approx_unique_users", "date_of_session")
+        .order_by("date_of_session")
+)
+
+CPU times: user 1.66 ms, sys: 1.23 ms, total: 2.89 ms
+Wall time: 662 ms
+
+[{'date_of_session': datetime.date(2023, 6, 2), 'approx_unique_users': 19322},
+ {'date_of_session': datetime.date(2023, 6, 3), 'approx_unique_users': 39356},
+ {'date_of_session': datetime.date(2023, 6, 4), 'approx_unique_users': 61202},
+ {'date_of_session': datetime.date(2023, 6, 5), 'approx_unique_users': 80917},
+ {'date_of_session': datetime.date(2023, 6, 6), 'approx_unique_users': 102914},
+ {'date_of_session': datetime.date(2023, 6, 7), 'approx_unique_users': 125637},
+ {'date_of_session': datetime.date(2023, 6, 8), 'approx_unique_users': 144594}]
+```
+
 The aggregation is also available in SQL for analytics:
 
 ```sql
 
 select
     date_trunc('day', created) as date_of_session,
     hll_cardinality(user_uuid, 11) as approx_unique_users
@@ -145,14 +170,41 @@
  2023-05-03 00:00:00+00 |              122343
  2023-05-04 00:00:00+00 |              141375
 (7 rows)
 
 Time: 2121.662 ms (00:02.122)
 ```
 
+or
+
+```sql
+
+select
+    date_trunc('day', created) as date_of_session,
+    hll_cardinality_from_hash(hll_hash(user_uuid), 11) as approx_unique_users
+from
+    testapp_session
+group by
+    date_trunc('day', created)
+order by date_of_session;
+
+    date_of_session     | approx_unique_users
+------------------------+---------------------
+ 2023-06-02 00:00:00+00 |               20013
+ 2023-06-03 00:00:00+00 |               39616
+ 2023-06-04 00:00:00+00 |               59312
+ 2023-06-05 00:00:00+00 |               81278
+ 2023-06-06 00:00:00+00 |              101880
+ 2023-06-07 00:00:00+00 |              122343
+ 2023-06-08 00:00:00+00 |              141375
+(7 rows)
+
+Time: 1810.445 ms (00:01.810)
+```
+
 ## How to use
 
 Install the package:
 
 ```sh
 pip install django-pg-simple-hll
 ```
@@ -175,162 +227,168 @@
 
 ## Should I use this?
 
 If you can use [an optimised version](https://github.com/citusdata/postgresql-hll), you should use that. It will be faster - although I haven't done any benchmarks.
 
 Use this if you can't install extensions on your database, such as on [Amazon RDS](https://aws.amazon.com/rds/).
 
+## SQL only
+
+Don't care about the Django functions, and just want to be able to run the SQL?
+The entire implementation is in a [single SQL file](django_pg_simple_hll/migrations/0002_custom_hashing.sql)
+
 ## Notes on SQL implementation
 
 This is a low-privilege implementation of [Hyperloglog](https://www.lix.polytechnique.fr/~fusy/Articles/FlFuGaMe07.pdf) approximate cardinality aggregation written in SQL and some [PL/pgSQL](https://www.postgresql.org/docs/current/plpgsql.html). Read about it [here](http://alejandro.giacometti.me/2023-03-30/hyperloglog-in-sql/),
 
 ## Notes on Performance
 
-This is not a scientific test, but here is an example of performance running on an M1 MacBook Pro, running Postgres 14 in Docker.
+This is not a scientific test, but here is an example of performance running on an M1 MacBook Pro, running Postgres 15 in Docker.
 
-For a dataset of 560k rows and 140k unique values a precision of 6 matches the speed of `COUNT(DISTINCT ...)`:
+For a dataset of 560k rows and 140k unique values a precision of 8 matches the speed of `COUNT(DISTINCT ...)`:
 
 ```sql
 
 select count(user_uuid) from testapp_session;
  count
 --------
  560000
 (1 row)
 
-Time: 115.919 ms
+Time: 227.959 ms
 
 select count(distinct user_uuid) as unique_users from testapp_session;
  unique_users
 --------------
        140000
 (1 row)
 
-Time: 434.234 ms
+Time: 476.819 ms
 
-select hll_cardinality(user_uuid, 6) as approx_unique_users from testapp_session;
-  approx_unique_users
+ select hll_cardinality_from_hash(hll_hash(user_uuid), 8) as approx_unique_users from testapp_session;
+ approx_unique_users
 ---------------------
-              136260
+              139309
 (1 row)
 
-Time: 409.562 ms
+Time: 402.569 ms
 
-select hll_cardinality(user_uuid, 11) as approx_unique_users from testapp_session;
+select hll_cardinality_from_hash(hll_hash(user_uuid), 11) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
               141375
 (1 row)
 
-Time: 1309.422 ms (00:01.309)
+Time: 1193.696 ms (00:01.194)
 ```
 
 For a dataset of 5.6M rows and 1.4M unique values:
 
-- with a precision of 7, `hll_aggregate` runs in about 0.79x the speed of `COUNT(DISTINCT ...)`
+- with a precision of 7, `hll_aggregate` runs in about 0.81x the speed of `COUNT(DISTINCT ...)`
 - with a precision of 8, it roughly matches (0.94x)
+- with a precision of 11, it runs in about 2.4x
 
 ```sql
 select count(user_uuid) from testapp_session;
   count
 ---------
  5600000
 (1 row)
 
-Time: 6021.708 ms (00:06.022)
+Time: 3798.774 ms (00:03.799)
 
 select count(distinct user_uuid) as unique_users from testapp_session;
  unique_users
 --------------
       1400000
 (1 row)
 
-Time: 5414.085 ms (00:05.414)
+Time: 4564.531 ms (00:04.565)
 
-select hll_cardinality(user_uuid, 7) as approx_unique_users from
+select hll_cardinality_from_hash(hll_hash(user_uuid), 7) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
              1308235
 (1 row)
 
-Time: 4308.065 ms (00:04.308)
+Time: 3710.460 ms (00:03.710)
 
-select hll_cardinality(user_uuid, 8) as approx_unique_users from testapp_session;
+select hll_cardinality_from_hash(hll_hash(user_uuid), 8) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
              1407331
 (1 row)
 
-Time: 5083.205 ms (00:05.083)
+Time: 4382.913 ms (00:04.383)
 
-select hll_cardinality(user_uuid, 11) as approx_unique_users from testapp_session;
+select hll_cardinality_from_hash(hll_hash(user_uuid), 11) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
              1390983
 (1 row)
 
-Time: 12468.054 ms (00:12.468)
+Time: 11027.942 ms (00:11.028)
 ```
 
 For a dataset of 56M rows and 14M unique values:
 
-- with a precision of 8, `hll_aggregate` runs in about 0.68x the speed of `COUNT(DISTINCT ...)`
-- with a precision of 9, it runs in about 0.76x
-- with a precision of 10, it runs in about 0.87x
-- with a precision of 11, it runs in about 1.10x
+- with a precision of 8, `hll_aggregate` runs in about 0.48x the speed of `COUNT(DISTINCT ...)`
+- with a precision of 9, it runs in about 0.63x
+- with a precision of 10, it runs in about 0.73x
+- with a precision of 11, it runs in about 1.07x
 
 ```sql
 
 select count(user_uuid) from testapp_session;
   count
 ----------
  56000000
 (1 row)
 
-Time: 86902.105 ms (01:26.902)93)
+Time: 45861.085 ms (00:45.861)
 
 select count(distinct user_uuid) as unique_users from testapp_session;
  unique_users
 --------------
      14000000
 (1 row)
 
-Time: 145953.595 ms (02:25.954)
+Time: 119551.361 ms (01:59.551)
 
-select hll_cardinality(user_uuid, 8) as approx_unique_users from testapp_session;
+select hll_cardinality_from_hash(hll_hash(user_uuid), 8) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
             13469591
 (1 row)
 
-Time: 99688.330 ms (01:39.688)
+Time: 58370.988 ms (00:58.371)
 
-select hll_cardinality(user_uuid, 9) as approx_unique_users from testapp_session;
+select hll_cardinality_from_hash(hll_hash(user_uuid), 9) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
             13028181
 (1 row)
 
-Time: 111210.513 ms (01:51.211)
+Time: 75231.592 ms (01:15.232)
 
-select hll_cardinality(user_uuid, 10) as approx_unique_users from testapp_session;
+select hll_cardinality_from_hash(hll_hash(user_uuid), 10) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
             13147406
 (1 row)
 
-Time: 126465.312 ms (02:06.465)
+Time: 87497.737 ms (01:27.498)
 
-hll_cardinality(user_uuid, 11) as approx_unique_users from testapp_session;
+select hll_cardinality_from_hash(hll_hash(user_uuid), 11) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
             13363203
 (1 row)
 
-Time: 160958.580 ms (02:40.959)
+Time: 128338.223 ms (02:08.338)
 ```
 
 The real advantage though is in combination with other properties:
 
 E.g. this query runs 0.37x quicker if using `hll_aggregate` than with `COUNT(DISTINCT ...)`:
 
 ```sql
@@ -340,40 +398,40 @@
 from testapp_session
 group by
   date_trunc('day', created)
 order by
   date_of_session;
     date_of_session     | unique_users
 ------------------------+--------------
- 2023-04-28 00:00:00+00 |      2000000
- 2023-04-29 00:00:00+00 |      4000000
- 2023-04-30 00:00:00+00 |      6000000
- 2023-05-01 00:00:00+00 |      8000000
- 2023-05-02 00:00:00+00 |     10000000
- 2023-05-03 00:00:00+00 |     12000000
- 2023-05-04 00:00:00+00 |     14000000
+ 2023-06-02 00:00:00+00 |      2000000
+ 2023-06-03 00:00:00+00 |      4000000
+ 2023-06-04 00:00:00+00 |      6000000
+ 2023-06-05 00:00:00+00 |      8000000
+ 2023-06-06 00:00:00+00 |     10000000
+ 2023-06-07 00:00:00+00 |     12000000
+ 2023-06-08 00:00:00+00 |     14000000
 (7 rows)
 
-Time: 296766.361 ms (04:56.766)
+Time: 157028.067 ms (02:37.028)
 
 select
   date_trunc('day', created) as date_of_session,
-  hll_cardinality(user_uuid, 9) as unique_users
+  hll_cardinality_from_hash(hll_hash(user_uuid), 9) as unique_users
 from
   testapp_session
 group by
   date_trunc('day', created)
 order by
   date_of_session;
     date_of_session     | unique_users
 ------------------------+--------------
- 2023-04-28 00:00:00+00 |      1963972
- 2023-04-29 00:00:00+00 |      4096876
- 2023-04-30 00:00:00+00 |      5869339
- 2023-05-01 00:00:00+00 |      7412843
- 2023-05-02 00:00:00+00 |      9401010
- 2023-05-03 00:00:00+00 |     11443836
- 2023-05-04 00:00:00+00 |     13028181
+ 2023-06-02 00:00:00+00 |      1963972
+ 2023-06-03 00:00:00+00 |      4096876
+ 2023-06-04 00:00:00+00 |      5869339
+ 2023-06-05 00:00:00+00 |      7412843
+ 2023-06-06 00:00:00+00 |      9401010
+ 2023-06-07 00:00:00+00 |     11443836
+ 2023-06-08 00:00:00+00 |     13028181
 (7 rows)
 
-Time: 110217.665 ms (01:50.218)
+Time: 58778.194 ms (00:58.778)
 ```
```

### Comparing `django_pg_simple_hll-0.1.1/django_pg_simple_hll/migrations/0001_initial.sql` & `django_pg_simple_hll-0.2.0/django_pg_simple_hll/migrations/0001_initial.sql`

 * *Files identical despite different names*

### Comparing `django_pg_simple_hll-0.1.1/pyproject.toml` & `django_pg_simple_hll-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django_pg_simple_hll"
-version = "0.1.1"
+version = "0.2.0"
 description = "A low-privilege implementation of hyperloglog for django and postgres"
 authors = ["Beauhurst <opensource@beauhurst.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
   "Environment :: Web Environment",
   "Framework :: Django",
@@ -41,14 +41,15 @@
 django-stubs = "^1.16.0"
 mypy = "^1.1.1"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-django = "^4.5.2"
 ruff = "^0.0.260"
 sqlfluff = "^2.0.5"
+pytest-xdist = "^3.3.1"
 
 [tool.poetry.group.debug]
 optional = true
 
 [tool.poetry.group.debug.dependencies]
 ipdb = "^0.13.13"
 ipython = "^8.12.0"
@@ -81,18 +82,24 @@
 plugins = ["mypy_django_plugin.main"]
 
 [tool.django-stubs]
 django_settings_module = "testapp.settings"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
-addopts = "-ra --cov"
+addopts = "-ra --cov=django_pg_simple_hll -n auto"
 DJANGO_SETTINGS_MODULE = "testapp.settings"
 testpaths = ["testapp/tests.py"]
 
+[tool.coverage.run]
+branch = true
+
+[tool.coverage.report]
+show_missing = true
+
 [tool.sqlfluff.core]
 dialect = "postgres"
 
 [tool.sqlfluff.indentation]
 indented_joins = false
 indented_using_on = true
 template_blocks_indent = false
```

### Comparing `django_pg_simple_hll-0.1.1/PKG-INFO` & `django_pg_simple_hll-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pg-simple-hll
-Version: 0.1.1
+Version: 0.2.0
 Summary: A low-privilege implementation of hyperloglog for django and postgres
 License: MIT
 Author: Beauhurst
 Author-email: opensource@beauhurst.com
 Requires-Python: >=3.9,<3.12
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -14,19 +14,15 @@
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Django (>=3.2.4)
 Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
 Description-Content-Type: text/markdown
 
 # django_pg_simple_hll
 
 Postgres-only HyperLogLog cardinality aggregation for the Django ORM.
@@ -147,14 +143,39 @@
  {'date_of_session': datetime.date(2023, 4, 30), 'approx_unique_users': 63159},
  {'date_of_session': datetime.date(2023, 5, 1), 'approx_unique_users': 83371},
  {'date_of_session': datetime.date(2023, 5, 2), 'approx_unique_users': 96185},
  {'date_of_session': datetime.date(2023, 5, 3), 'approx_unique_users': 116565},
  {'date_of_session': datetime.date(2023, 5, 4), 'approx_unique_users': 143588}]
 ```
 
+HLL works by hashing each value it considers. For some reason, the aggregation is sometimes faster when that hashing is performed outside of the aggregation. So, it is also available in two separate steps:
+
+```python
+%%time
+list(
+    Session.objects
+        .annotate(date_of_session=TruncDate("created"))
+        .values("date_of_session")
+        .annotate(approx_unique_users=HLLCardinalityFromHash(HLLHash("user_uuid"), 9))
+        .values("approx_unique_users", "date_of_session")
+        .order_by("date_of_session")
+)
+
+CPU times: user 1.66 ms, sys: 1.23 ms, total: 2.89 ms
+Wall time: 662 ms
+
+[{'date_of_session': datetime.date(2023, 6, 2), 'approx_unique_users': 19322},
+ {'date_of_session': datetime.date(2023, 6, 3), 'approx_unique_users': 39356},
+ {'date_of_session': datetime.date(2023, 6, 4), 'approx_unique_users': 61202},
+ {'date_of_session': datetime.date(2023, 6, 5), 'approx_unique_users': 80917},
+ {'date_of_session': datetime.date(2023, 6, 6), 'approx_unique_users': 102914},
+ {'date_of_session': datetime.date(2023, 6, 7), 'approx_unique_users': 125637},
+ {'date_of_session': datetime.date(2023, 6, 8), 'approx_unique_users': 144594}]
+```
+
 The aggregation is also available in SQL for analytics:
 
 ```sql
 
 select
     date_trunc('day', created) as date_of_session,
     hll_cardinality(user_uuid, 11) as approx_unique_users
@@ -174,14 +195,41 @@
  2023-05-03 00:00:00+00 |              122343
  2023-05-04 00:00:00+00 |              141375
 (7 rows)
 
 Time: 2121.662 ms (00:02.122)
 ```
 
+or
+
+```sql
+
+select
+    date_trunc('day', created) as date_of_session,
+    hll_cardinality_from_hash(hll_hash(user_uuid), 11) as approx_unique_users
+from
+    testapp_session
+group by
+    date_trunc('day', created)
+order by date_of_session;
+
+    date_of_session     | approx_unique_users
+------------------------+---------------------
+ 2023-06-02 00:00:00+00 |               20013
+ 2023-06-03 00:00:00+00 |               39616
+ 2023-06-04 00:00:00+00 |               59312
+ 2023-06-05 00:00:00+00 |               81278
+ 2023-06-06 00:00:00+00 |              101880
+ 2023-06-07 00:00:00+00 |              122343
+ 2023-06-08 00:00:00+00 |              141375
+(7 rows)
+
+Time: 1810.445 ms (00:01.810)
+```
+
 ## How to use
 
 Install the package:
 
 ```sh
 pip install django-pg-simple-hll
 ```
@@ -204,162 +252,168 @@
 
 ## Should I use this?
 
 If you can use [an optimised version](https://github.com/citusdata/postgresql-hll), you should use that. It will be faster - although I haven't done any benchmarks.
 
 Use this if you can't install extensions on your database, such as on [Amazon RDS](https://aws.amazon.com/rds/).
 
+## SQL only
+
+Don't care about the Django functions, and just want to be able to run the SQL?
+The entire implementation is in a [single SQL file](django_pg_simple_hll/migrations/0002_custom_hashing.sql)
+
 ## Notes on SQL implementation
 
 This is a low-privilege implementation of [Hyperloglog](https://www.lix.polytechnique.fr/~fusy/Articles/FlFuGaMe07.pdf) approximate cardinality aggregation written in SQL and some [PL/pgSQL](https://www.postgresql.org/docs/current/plpgsql.html). Read about it [here](http://alejandro.giacometti.me/2023-03-30/hyperloglog-in-sql/),
 
 ## Notes on Performance
 
-This is not a scientific test, but here is an example of performance running on an M1 MacBook Pro, running Postgres 14 in Docker.
+This is not a scientific test, but here is an example of performance running on an M1 MacBook Pro, running Postgres 15 in Docker.
 
-For a dataset of 560k rows and 140k unique values a precision of 6 matches the speed of `COUNT(DISTINCT ...)`:
+For a dataset of 560k rows and 140k unique values a precision of 8 matches the speed of `COUNT(DISTINCT ...)`:
 
 ```sql
 
 select count(user_uuid) from testapp_session;
  count
 --------
  560000
 (1 row)
 
-Time: 115.919 ms
+Time: 227.959 ms
 
 select count(distinct user_uuid) as unique_users from testapp_session;
  unique_users
 --------------
        140000
 (1 row)
 
-Time: 434.234 ms
+Time: 476.819 ms
 
-select hll_cardinality(user_uuid, 6) as approx_unique_users from testapp_session;
-  approx_unique_users
+ select hll_cardinality_from_hash(hll_hash(user_uuid), 8) as approx_unique_users from testapp_session;
+ approx_unique_users
 ---------------------
-              136260
+              139309
 (1 row)
 
-Time: 409.562 ms
+Time: 402.569 ms
 
-select hll_cardinality(user_uuid, 11) as approx_unique_users from testapp_session;
+select hll_cardinality_from_hash(hll_hash(user_uuid), 11) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
               141375
 (1 row)
 
-Time: 1309.422 ms (00:01.309)
+Time: 1193.696 ms (00:01.194)
 ```
 
 For a dataset of 5.6M rows and 1.4M unique values:
 
-- with a precision of 7, `hll_aggregate` runs in about 0.79x the speed of `COUNT(DISTINCT ...)`
+- with a precision of 7, `hll_aggregate` runs in about 0.81x the speed of `COUNT(DISTINCT ...)`
 - with a precision of 8, it roughly matches (0.94x)
+- with a precision of 11, it runs in about 2.4x
 
 ```sql
 select count(user_uuid) from testapp_session;
   count
 ---------
  5600000
 (1 row)
 
-Time: 6021.708 ms (00:06.022)
+Time: 3798.774 ms (00:03.799)
 
 select count(distinct user_uuid) as unique_users from testapp_session;
  unique_users
 --------------
       1400000
 (1 row)
 
-Time: 5414.085 ms (00:05.414)
+Time: 4564.531 ms (00:04.565)
 
-select hll_cardinality(user_uuid, 7) as approx_unique_users from
+select hll_cardinality_from_hash(hll_hash(user_uuid), 7) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
              1308235
 (1 row)
 
-Time: 4308.065 ms (00:04.308)
+Time: 3710.460 ms (00:03.710)
 
-select hll_cardinality(user_uuid, 8) as approx_unique_users from testapp_session;
+select hll_cardinality_from_hash(hll_hash(user_uuid), 8) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
              1407331
 (1 row)
 
-Time: 5083.205 ms (00:05.083)
+Time: 4382.913 ms (00:04.383)
 
-select hll_cardinality(user_uuid, 11) as approx_unique_users from testapp_session;
+select hll_cardinality_from_hash(hll_hash(user_uuid), 11) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
              1390983
 (1 row)
 
-Time: 12468.054 ms (00:12.468)
+Time: 11027.942 ms (00:11.028)
 ```
 
 For a dataset of 56M rows and 14M unique values:
 
-- with a precision of 8, `hll_aggregate` runs in about 0.68x the speed of `COUNT(DISTINCT ...)`
-- with a precision of 9, it runs in about 0.76x
-- with a precision of 10, it runs in about 0.87x
-- with a precision of 11, it runs in about 1.10x
+- with a precision of 8, `hll_aggregate` runs in about 0.48x the speed of `COUNT(DISTINCT ...)`
+- with a precision of 9, it runs in about 0.63x
+- with a precision of 10, it runs in about 0.73x
+- with a precision of 11, it runs in about 1.07x
 
 ```sql
 
 select count(user_uuid) from testapp_session;
   count
 ----------
  56000000
 (1 row)
 
-Time: 86902.105 ms (01:26.902)93)
+Time: 45861.085 ms (00:45.861)
 
 select count(distinct user_uuid) as unique_users from testapp_session;
  unique_users
 --------------
      14000000
 (1 row)
 
-Time: 145953.595 ms (02:25.954)
+Time: 119551.361 ms (01:59.551)
 
-select hll_cardinality(user_uuid, 8) as approx_unique_users from testapp_session;
+select hll_cardinality_from_hash(hll_hash(user_uuid), 8) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
             13469591
 (1 row)
 
-Time: 99688.330 ms (01:39.688)
+Time: 58370.988 ms (00:58.371)
 
-select hll_cardinality(user_uuid, 9) as approx_unique_users from testapp_session;
+select hll_cardinality_from_hash(hll_hash(user_uuid), 9) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
             13028181
 (1 row)
 
-Time: 111210.513 ms (01:51.211)
+Time: 75231.592 ms (01:15.232)
 
-select hll_cardinality(user_uuid, 10) as approx_unique_users from testapp_session;
+select hll_cardinality_from_hash(hll_hash(user_uuid), 10) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
             13147406
 (1 row)
 
-Time: 126465.312 ms (02:06.465)
+Time: 87497.737 ms (01:27.498)
 
-hll_cardinality(user_uuid, 11) as approx_unique_users from testapp_session;
+select hll_cardinality_from_hash(hll_hash(user_uuid), 11) as approx_unique_users from testapp_session;
  approx_unique_users
 ---------------------
             13363203
 (1 row)
 
-Time: 160958.580 ms (02:40.959)
+Time: 128338.223 ms (02:08.338)
 ```
 
 The real advantage though is in combination with other properties:
 
 E.g. this query runs 0.37x quicker if using `hll_aggregate` than with `COUNT(DISTINCT ...)`:
 
 ```sql
@@ -369,41 +423,41 @@
 from testapp_session
 group by
   date_trunc('day', created)
 order by
   date_of_session;
     date_of_session     | unique_users
 ------------------------+--------------
- 2023-04-28 00:00:00+00 |      2000000
- 2023-04-29 00:00:00+00 |      4000000
- 2023-04-30 00:00:00+00 |      6000000
- 2023-05-01 00:00:00+00 |      8000000
- 2023-05-02 00:00:00+00 |     10000000
- 2023-05-03 00:00:00+00 |     12000000
- 2023-05-04 00:00:00+00 |     14000000
+ 2023-06-02 00:00:00+00 |      2000000
+ 2023-06-03 00:00:00+00 |      4000000
+ 2023-06-04 00:00:00+00 |      6000000
+ 2023-06-05 00:00:00+00 |      8000000
+ 2023-06-06 00:00:00+00 |     10000000
+ 2023-06-07 00:00:00+00 |     12000000
+ 2023-06-08 00:00:00+00 |     14000000
 (7 rows)
 
-Time: 296766.361 ms (04:56.766)
+Time: 157028.067 ms (02:37.028)
 
 select
   date_trunc('day', created) as date_of_session,
-  hll_cardinality(user_uuid, 9) as unique_users
+  hll_cardinality_from_hash(hll_hash(user_uuid), 9) as unique_users
 from
   testapp_session
 group by
   date_trunc('day', created)
 order by
   date_of_session;
     date_of_session     | unique_users
 ------------------------+--------------
- 2023-04-28 00:00:00+00 |      1963972
- 2023-04-29 00:00:00+00 |      4096876
- 2023-04-30 00:00:00+00 |      5869339
- 2023-05-01 00:00:00+00 |      7412843
- 2023-05-02 00:00:00+00 |      9401010
- 2023-05-03 00:00:00+00 |     11443836
- 2023-05-04 00:00:00+00 |     13028181
+ 2023-06-02 00:00:00+00 |      1963972
+ 2023-06-03 00:00:00+00 |      4096876
+ 2023-06-04 00:00:00+00 |      5869339
+ 2023-06-05 00:00:00+00 |      7412843
+ 2023-06-06 00:00:00+00 |      9401010
+ 2023-06-07 00:00:00+00 |     11443836
+ 2023-06-08 00:00:00+00 |     13028181
 (7 rows)
 
-Time: 110217.665 ms (01:50.218)
+Time: 58778.194 ms (00:58.778)
 ```
```

