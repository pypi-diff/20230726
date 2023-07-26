# Comparing `tmp/HawaData-0.8.5.tar.gz` & `tmp/HawaData-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.8.5.tar", last modified: Mon Jul 24 08:00:36 2023, max compression
+gzip compressed data, was "HawaData-0.8.6.tar", last modified: Wed Jul 26 15:08:42 2023, max compression
```

## Comparing `HawaData-0.8.5.tar` & `HawaData-0.8.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.741340 HawaData-0.8.5/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.726947 HawaData-0.8.5/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     3459 2023-07-24 08:00:36.000000 HawaData-0.8.5/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-24 08:00:36.000000 HawaData-0.8.5/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-24 08:00:36.000000 HawaData-0.8.5/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-24 08:00:36.000000 HawaData-0.8.5/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     3459 2023-07-24 08:00:36.740963 HawaData-0.8.5/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.8.5/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.727569 HawaData-0.8.5/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.8.5/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.730402 HawaData-0.8.5/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.8.5/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.8.5/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.8.5/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.8.5/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.8.5/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.732231 HawaData-0.8.5/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.8.5/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    16980 2023-07-24 08:00:29.000000 HawaData-0.8.5/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     6457 2023-07-21 07:00:47.000000 HawaData-0.8.5/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3236 2023-07-24 04:28:13.000000 HawaData-0.8.5/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2714 2023-07-24 04:07:20.000000 HawaData-0.8.5/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.736694 HawaData-0.8.5/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.8.5/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.8.5/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.8.5/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.8.5/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.8.5/hawa/data/province.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1129 2023-07-24 04:28:13.000000 HawaData-0.8.5/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1015 2023-07-19 03:28:20.000000 HawaData-0.8.5/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.739377 HawaData-0.8.5/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.8.5/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    28951 2023-07-24 04:31:22.000000 HawaData-0.8.5/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5470 2023-07-24 04:31:22.000000 HawaData-0.8.5/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-24 08:00:36.741448 HawaData-0.8.5/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.8.5/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-24 08:00:36.740111 HawaData-0.8.5/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.8.5/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-26 15:08:42.164231 HawaData-0.8.6/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-26 15:08:42.147992 HawaData-0.8.6/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3475 2023-07-26 15:08:42.000000 HawaData-0.8.6/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-26 15:08:42.000000 HawaData-0.8.6/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-26 15:08:42.000000 HawaData-0.8.6/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-26 15:08:42.000000 HawaData-0.8.6/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3475 2023-07-26 15:08:42.163817 HawaData-0.8.6/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.8.6/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-26 15:08:42.148566 HawaData-0.8.6/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.8.6/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-26 15:08:42.151608 HawaData-0.8.6/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.8.6/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.8.6/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      522 2023-07-24 09:22:05.000000 HawaData-0.8.6/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.8.6/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.8.6/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-26 15:08:42.154127 HawaData-0.8.6/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.8.6/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    17397 2023-07-24 09:26:55.000000 HawaData-0.8.6/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     6455 2023-07-26 15:07:30.000000 HawaData-0.8.6/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3236 2023-07-24 04:28:13.000000 HawaData-0.8.6/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2714 2023-07-24 04:07:20.000000 HawaData-0.8.6/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-26 15:08:42.159176 HawaData-0.8.6/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.8.6/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.8.6/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.8.6/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.8.6/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.8.6/hawa/data/province.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1129 2023-07-24 04:28:13.000000 HawaData-0.8.6/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1015 2023-07-19 03:28:20.000000 HawaData-0.8.6/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-26 15:08:42.161809 HawaData-0.8.6/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.8.6/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28951 2023-07-24 04:31:22.000000 HawaData-0.8.6/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5470 2023-07-24 04:31:22.000000 HawaData-0.8.6/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-26 15:08:42.164345 HawaData-0.8.6/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.8.6/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-26 15:08:42.162870 HawaData-0.8.6/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.8.6/test/test_query.py
```

### Comparing `HawaData-0.8.5/HawaData.egg-info/PKG-INFO` & `HawaData-0.8.6/HawaData.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.8.5
+Version: 0.8.6
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -117,7 +117,8 @@
 - 0.7.9 sort dim field
 - 0.8.0 sort dim field
 - 0.8.1 sort dim field
 - 0.8.2 add global precision
 - 0.8.3 add global precision in func
 - 0.8.4 fix extra dim/field
 - 0.8.5 load less data
+- 0.8.6 fix bug
```

### Comparing `HawaData-0.8.5/HawaData.egg-info/SOURCES.txt` & `HawaData-0.8.6/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.5/PKG-INFO` & `HawaData-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.8.5
+Version: 0.8.6
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -117,7 +117,8 @@
 - 0.7.9 sort dim field
 - 0.8.0 sort dim field
 - 0.8.1 sort dim field
 - 0.8.2 add global precision
 - 0.8.3 add global precision in func
 - 0.8.4 fix extra dim/field
 - 0.8.5 load less data
+- 0.8.6 fix bug
```

### Comparing `HawaData-0.8.5/README.md` & `HawaData-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.5/hawa/base/db.py` & `HawaData-0.8.6/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.5/hawa/base/init.py` & `HawaData-0.8.6/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.5/hawa/common/data.py` & `HawaData-0.8.6/hawa/common/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """通用的 report data 构造器，支持 校、区、市、省、全国级别的通用报告数据构造"""
 import json
+import time
 from collections import Counter, defaultdict
 from dataclasses import dataclass, field
 from typing import Optional, ClassVar, Any, Set
 
 import pandas as pd
 import pendulum
-from munch import Munch
 
 from hawa.base.db import DbUtil, RedisUtil
+from hawa.base.decos import log_func_time
 from hawa.base.errors import NoCasesError
 from hawa.common.query import DataQuery
 from hawa.common.utils import GradeData, CaseData, Measurement, Util
 from hawa.config import project
 
 
 class MetaCommomData(type):
@@ -80,23 +81,32 @@
     # 去年全国数据
     last_year = None
     last_year_code_scores: Optional[pd.DataFrame] = field(default_factory=pd.DataFrame)
 
     def __post_init__(self):
         # 初始化数据
         if self.is_load_all:
+            t0 = time.perf_counter()
             self.load_all_data()
+            t1 = time.perf_counter()
+            print(f"load all data cost: {t1 - t0:.2f}s")
 
             # 构建辅助工具
             self._to_build_helper()
 
+            t2 = time.perf_counter()
+            print(f"build helper cost: {t2 - t1:.2f}s")
+
             # 计算数据
             count_functions = [i for i in dir(self) if i.startswith('_to_count_')]
             for func in count_functions:
                 getattr(self, func)()
+
+            t3 = time.perf_counter()
+            print(f"count data cost: {t3 - t2:.2f}s")
         else:
             self.load_less_data()
             self._to_build_helper()
 
     def _to_init_a_meta_unit(self):
         self.meta_unit = self.query.query_unit(self.meta_unit_type, str(self.meta_unit_id))
 
@@ -142,14 +152,15 @@
         if self.cases.empty:
             raise NoCasesError(f'no cases:{self.meta_unit} {self.school_ids}')
         self.case_ids = self.cases['id'].tolist()
         self.case_project_ids = Counter(self.cases['project_id'].tolist())
         self.school_ids = self.cases['school_id'].unique().tolist()
         project.logger.debug(f'cases: {len(self.cases)}')
 
+    @log_func_time
     def _to_init_e_answers(self):
         self.answers = self.query.query_answers(case_ids=self.case_ids)
         project.logger.debug(f'answers: {len(self.answers)}')
 
     def _to_init_f_students(self):
         self.student_ids = set(self.answers['student_id'].tolist())
         student_id_list = list(self.student_ids)
@@ -171,14 +182,15 @@
             cache_data = self.codebook.to_json(orient='records', force_ascii=False)
             self.redis.conn.set(cache_key, cache_data, ex=60 * 60 * 24 * 7)
 
     def _to_build_helper(self):
         self.grade = GradeData(case_ids=self.case_ids)
         self.case = CaseData(cases=self.cases)
 
+    @log_func_time
     def _to_count_a_final_answers(self):
         items = {k: {} for k in self.code_word_list}
         item_codes = self.query.query_item_codes(self.item_ids)
         # code-dimension/field  ~  item_id  ~ code   name
         project.logger.debug(f"{self.code_word_list=}")
         for (item_id, category), codes in item_codes.groupby(['item_id', 'category']):
             if category in self.code_word_list:
@@ -198,14 +210,15 @@
         data['grade'] = data['case_id'].apply(lambda x: x % 100)
         data['username'] = data['nickname']
         for code_word in self.code_word_list:
             data[code_word] = data.item_id.apply(lambda x: items[code_word][x])
         self.final_answers = data.drop_duplicates(subset=['case_id', 'student_id', 'item_id'])
         project.logger.debug(f'final_answers: {len(self.final_answers)}')
 
+    @log_func_time
     def _to_count_b_final_scores(self):
         self.final_scores = self.count_final_score(answers=self.final_answers)
         project.logger.debug(f'final_scores: {len(self.final_scores)}')
 
     @staticmethod
     def count_level(score, mode: str = 'f'):
         assert mode in ('f', 'r'), 'only support feedback or report'
@@ -220,22 +233,22 @@
         key = "RANK_LABEL" if mode == 'r' else 'FEEDBACK_LEVEL'
         return project.ranks[key][a]
 
     def count_final_score(self, answers: pd.DataFrame):
         records = []
         for student_id, group in answers.groupby('student_id'):
             score = group.score.mean() * 100
-            record = Munch(
-                student_id=student_id,
-                username=group['username'].tolist()[0],
-                grade=group['grade'].tolist()[0],
-                gender=group['gender'].tolist()[0],
-                score=score,
-                level=self.count_level(score),
-            )
+            record = {
+                "student_id": student_id,
+                "username": group['username'].tolist()[0],
+                "grade": group['grade'].tolist()[0],
+                "gender": group['gender'].tolist()[0],
+                "score": score,
+                "level": self.count_level(score),
+            }
             records.append(record)
         return pd.DataFrame.from_records(records)
 
     def get_last_year_miss(self, grade: int):
         key = f'{project.REDIS_PREFIX}{self.last_year_num}:data'
         data = json.loads(self.redis.conn.get(key))
         try:
```

### Comparing `HawaData-0.8.5/hawa/common/query.py` & `HawaData-0.8.6/hawa/common/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,17 +93,17 @@
         return cases
 
     def query_answers(self, case_ids: list[int], student_id: int = None):
         answer_cols = "id, student_id, item_id, case_id, answer, score, created, valid"
         if len(case_ids) == 0:
             return []
         elif len(case_ids) == 1:
-            sql = f"select {answer_cols} from answers where case_id={case_ids[0]} and valid=1;"
+            sql = f"select {answer_cols} from answers where case_id={case_ids[0]} and valid=1"
         else:
-            sql = f"select {answer_cols} from answers where case_id in {tuple(case_ids)} and valid=1;"
+            sql = f"select {answer_cols} from answers where case_id in {tuple(case_ids)} and valid=1"
         if student_id:
             sql += f" and student_id={student_id};"
         with self.db.engine_conn() as conn:
             answers = pd.read_sql(text(sql), conn).drop_duplicates(
                 subset=['case_id', 'student_id', 'item_id'])
         return answers
```

### Comparing `HawaData-0.8.5/hawa/common/utils.py` & `HawaData-0.8.6/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.5/hawa/config.py` & `HawaData-0.8.6/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.5/hawa/data/klass.py` & `HawaData-0.8.6/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.5/hawa/data/province.py` & `HawaData-0.8.6/hawa/data/province.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.5/hawa/data/school.py` & `HawaData-0.8.6/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.5/hawa/data/student.py` & `HawaData-0.8.6/hawa/data/student.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.5/hawa/paper/health.py` & `HawaData-0.8.6/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.5/hawa/paper/mht.py` & `HawaData-0.8.6/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.5/setup.py` & `HawaData-0.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.8.5/test/test_query.py` & `HawaData-0.8.6/test/test_query.py`

 * *Files identical despite different names*

