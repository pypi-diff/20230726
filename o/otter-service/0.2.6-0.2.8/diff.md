# Comparing `tmp/otter_service-0.2.6.tar.gz` & `tmp/otter_service-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter_service-0.2.6.tar", last modified: Wed Jul 26 20:16:08 2023, max compression
+gzip compressed data, was "otter_service-0.2.8.tar", last modified: Wed Jul 26 21:35:09 2023, max compression
```

## Comparing `otter_service-0.2.6.tar` & `otter_service-0.2.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 20:16:08.873680 otter_service-0.2.6/
--rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.6/LICENSE
--rw-r--r--   0 sean       (501) staff       (20)     9235 2023-07-26 20:16:08.874779 otter_service-0.2.6/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)     8776 2023-07-26 18:31:30.000000 otter_service-0.2.6/README.md
--rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.6/pyproject.toml
--rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-26 20:16:08.876308 otter_service-0.2.6/setup.cfg
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 20:16:08.857794 otter_service-0.2.6/src/
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 20:16:08.866440 otter_service-0.2.6/src/otter_service/
--rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-26 20:15:09.000000 otter_service-0.2.6/src/otter_service/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)     2149 2023-07-26 15:52:24.000000 otter_service-0.2.6/src/otter_service/access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1025 2023-07-21 21:37:40.000000 otter_service-0.2.6/src/otter_service/firestore-test.py
--rw-r--r--   0 sean       (501) staff       (20)     5332 2023-07-26 19:31:25.000000 otter_service-0.2.6/src/otter_service/grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)    19654 2023-07-26 19:31:34.000000 otter_service-0.2.6/src/otter_service/otter_nb.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 20:16:08.870880 otter_service-0.2.6/src/otter_service/secrets/
--rw-r--r--   0 sean       (501) staff       (20)     1043 2023-07-26 01:06:26.000000 otter_service-0.2.6/src/otter_service/secrets/gh_key.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.6/src/otter_service/secrets/gke_key.yaml
--rw-r--r--   0 sean       (501) staff       (20)      516 2023-07-25 18:59:31.000000 otter_service-0.2.6/src/otter_service/util.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 20:16:08.869757 otter_service-0.2.6/src/otter_service.egg-info/
--rw-r--r--   0 sean       (501) staff       (20)     9235 2023-07-26 20:16:08.000000 otter_service-0.2.6/src/otter_service.egg-info/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)      610 2023-07-26 20:16:08.000000 otter_service-0.2.6/src/otter_service.egg-info/SOURCES.txt
--rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-26 20:16:08.000000 otter_service-0.2.6/src/otter_service.egg-info/dependency_links.txt
--rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-26 20:16:08.000000 otter_service-0.2.6/src/otter_service.egg-info/entry_points.txt
--rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-26 20:16:08.000000 otter_service-0.2.6/src/otter_service.egg-info/top_level.txt
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 20:16:08.873163 otter_service-0.2.6/tests/
--rw-r--r--   0 sean       (501) staff       (20)      913 2023-07-26 00:57:35.000000 otter_service-0.2.6/tests/test_access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1217 2023-07-26 00:58:54.000000 otter_service-0.2.6/tests/test_grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)     2140 2023-07-21 23:00:39.000000 otter_service-0.2.6/tests/test_otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 21:35:09.915081 otter_service-0.2.8/
+-rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.8/LICENSE
+-rw-r--r--   0 sean       (501) staff       (20)     9235 2023-07-26 21:35:09.915382 otter_service-0.2.8/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)     8776 2023-07-26 18:31:30.000000 otter_service-0.2.8/README.md
+-rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.8/pyproject.toml
+-rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-26 21:35:09.917242 otter_service-0.2.8/setup.cfg
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 21:35:09.895963 otter_service-0.2.8/src/
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 21:35:09.905963 otter_service-0.2.8/src/otter_service/
+-rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-26 21:34:48.000000 otter_service-0.2.8/src/otter_service/__init__.py
+-rw-r--r--   0 sean       (501) staff       (20)     2149 2023-07-26 15:52:24.000000 otter_service-0.2.8/src/otter_service/access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1025 2023-07-21 21:37:40.000000 otter_service-0.2.8/src/otter_service/firestore-test.py
+-rw-r--r--   0 sean       (501) staff       (20)     5320 2023-07-26 20:22:54.000000 otter_service-0.2.8/src/otter_service/grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)    19559 2023-07-26 21:23:52.000000 otter_service-0.2.8/src/otter_service/otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 21:35:09.911740 otter_service-0.2.8/src/otter_service/secrets/
+-rw-r--r--   0 sean       (501) staff       (20)     1043 2023-07-26 01:06:26.000000 otter_service-0.2.8/src/otter_service/secrets/gh_key.yaml
+-rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.8/src/otter_service/secrets/gke_key.yaml
+-rw-r--r--   0 sean       (501) staff       (20)      516 2023-07-25 18:59:31.000000 otter_service-0.2.8/src/otter_service/util.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 21:35:09.909418 otter_service-0.2.8/src/otter_service.egg-info/
+-rw-r--r--   0 sean       (501) staff       (20)     9235 2023-07-26 21:35:09.000000 otter_service-0.2.8/src/otter_service.egg-info/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)      610 2023-07-26 21:35:09.000000 otter_service-0.2.8/src/otter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-26 21:35:09.000000 otter_service-0.2.8/src/otter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-26 21:35:09.000000 otter_service-0.2.8/src/otter_service.egg-info/entry_points.txt
+-rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-26 21:35:09.000000 otter_service-0.2.8/src/otter_service.egg-info/top_level.txt
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 21:35:09.914527 otter_service-0.2.8/tests/
+-rw-r--r--   0 sean       (501) staff       (20)      913 2023-07-26 00:57:35.000000 otter_service-0.2.8/tests/test_access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1187 2023-07-26 21:32:16.000000 otter_service-0.2.8/tests/test_grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)     2140 2023-07-21 23:00:39.000000 otter_service-0.2.8/tests/test_otter_nb.py
```

### Comparing `otter_service-0.2.6/LICENSE` & `otter_service-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.6/PKG-INFO` & `otter_service-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter_service
-Version: 0.2.6
+Version: 0.2.8
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `otter_service-0.2.6/README.md` & `otter_service-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.6/setup.cfg` & `otter_service-0.2.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.6/src/otter_service/access_sops_keys.py` & `otter_service-0.2.8/src/otter_service/access_sops_keys.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.6/src/otter_service/firestore-test.py` & `otter_service-0.2.8/src/otter_service/firestore-test.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.6/src/otter_service/grade_assignment.py` & `otter_service-0.2.8/src/otter_service/grade_assignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,23 @@
     :param secrets_file: path to secrets file
     :param save_path: Where to save the archive -- for testing it is "." for normal it will /tmp
     """
     branch = "main"
     git_access_token = access_sops_keys.get(course, "github_access_token", sops_path=sops_path, secrets_file=secrets_file)
     autograder_materials_repo = access_sops_keys.get(course, "autograder_repo", sops_path=sops_path, secrets_file=secrets_file)
     materials_url = f"https://{git_access_token}:@{autograder_materials_repo}/archive/{branch}.tar.gz"
-        
+
     download_path = "/tmp/materials.tar.gz"
     if save_path is None:
         save_path = "."
         download_path = "./materials.tar.gz"
     r = requests.get(materials_url, stream=True)
     if r.status_code != 200:
         branch = "master"
-        materials_url = f"https://{git_access_token}:@{autograder_materials_repo}/archive/{branch}.tar.gz"    
+        materials_url = f"https://{git_access_token}:@{autograder_materials_repo}/archive/{branch}.tar.gz"
         r = requests.get(materials_url, stream=True)
 
     if r.status_code == 200:
         with open(download_path, 'wb') as f:
             f.write(r.raw.read())
         file = tarfile.open(download_path)
         file.extractall(save_path)
```

### Comparing `otter_service-0.2.6/src/otter_service/otter_nb.py` & `otter_service-0.2.8/src/otter_service/otter_nb.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import tornado.web
 import tornado.httpserver
 import tornado.ioloop
 import tornado.escape
 import tornado.options
 import tornado.gen
 from otter_service import access_sops_keys
-from otter_service.grade_assignment import grade_assignment, download_autograder_materials
+from otter_service.grade_assignment import grade_assignment
 import firebase_admin
 from firebase_admin import credentials, firestore
 import grpc
 from google.cloud.firestore_v1.client import firestore_client
 from google.cloud.firestore_v1.client import firestore_grpc_transport
 import otter_service.util as util
 
@@ -98,34 +98,40 @@
     :param course_id: the course id for this notebook
     :param assignment_id:  the assignment id for this notebook
     :return: formatted string
     """
     return f"course-v1%3A{course_id}:{os.environ['EDX_URL']}-{assignment_id}"
 
 
-async def post_grade(solutions_base_path, user_id, grade, course, section, assignment):
+async def post_grade(solutions_base_path, args):
     """
     This posts the grade to the LTI server
     :paraem solutions_base_path: where the config file is to find the assignment id
-    :param user_id: the user to post the grade for
-    :param grade: the grade as a float
-    :param course: the course this notebook is in
-    :param section: the section this notebook is in
-    :param assignment:  the assignment name for this notebook
+    :param args:
+        - userid: the user to post the grade for
+        - grade: the grade as a float
+        - course: the course this notebook is in
+        - section: the section this notebook is in
+        - assignment:  the assignment name for this notebook
     """
     body_hash = ""
     consumer_key = ""
     try:
         # post grade to EdX
         course_config = util.get_course_config(solutions_base_path)
+        course = args["course"]
+        section = args["section"]
+        assignment = args["assignment"]
+        user_id = args["userid"]
+        grade = args["grade"]
 
         course_id = course_config[course][section]["course_id"]
         assignment_id = course_config[course][section]["assignments"][assignment]
 
-        log_info_csv(user_id, course, section, assignment, f"Edx Course Config Loaded: Course Id: {course_id}, Assignment_id: {assignment_id}")
+        log_info_csv(user_id, args, f"Edx Course Config Loaded: Course Id: {course_id}, Assignment_id: {assignment_id}")
 
         sourced_id = create_sourced_id(course_id, assignment_id)
         outcomes_url = create_post_url(course_id, assignment_id)
 
         # TODO: extract this into a real library with real XML parsing
         # WARNING: You can use this only with data you trust! Beware, etc.
         post_xml = r"""
@@ -197,15 +203,15 @@
         response_tree = etree.fromstring(resp_text.encode('utf-8'))
 
         # XML and its namespaces. UBOOF!
         status = response_tree.find('.//{http://www.imsglobal.org/services/ltiv1p1/xsd/imsoms_v1p0}imsx_statusInfo')
         code_major = status.find('{http://www.imsglobal.org/services/ltiv1p1/xsd/imsoms_v1p0}imsx_codeMajor').text
         desc = status.find('{http://www.imsglobal.org/services/ltiv1p1/xsd/imsoms_v1p0}imsx_description').text
 
-        log_info_csv(user_id, course, section, assignment, f"Posted to Edx: code: {code_major}, desc: {desc}")
+        log_info_csv(user_id, args, f"Posted to Edx: code: {code_major}, desc: {desc}")
 
         if code_major != 'success':
             raise GradePostException(desc)
 
     except GradePostException as grade_post_exception:
         raise grade_post_exception
     except Exception as ex:
@@ -261,17 +267,15 @@
                 metadata["course"] = notebook['metadata']['course']
 
             if "section" in notebook['metadata']:
                 metadata["section"] = notebook['metadata']['section']
 
             if "assignment" in notebook['metadata']:
                 metadata["assignment"] = notebook['metadata']['assignment']
-            elif "lab" in notebook['metadata']:
-                metadata["assignment"] = notebook['metadata']['lab']
-            
+
             if metadata["course"] is None or \
                 metadata["section"] is None or \
                     metadata["assignment"] is None:
                 err_msg = "Notebook does not have required metadata: course, section, and assignment"
                 raise GradeSubmissionException(err_msg)
 
             log_info_csv(user["name"], metadata, f"User logged in -  Using Referrer: {using_test_user}")
@@ -337,15 +341,15 @@
                 "section": section,
                 "assignment": assignment
             }
             write_grade(grade_info)
             log_info_csv(name, args, f"Grade Written to database: {grade}")
 
             if os.getenv("POST_GRADE").lower() in ("true", '1', 't'):
-                await post_grade(solutions_base_path, name, grade, course, section, assignment)
+                await post_grade(solutions_base_path, grade_info)
             else:
                 log_info_csv(name, args, f"Grade NOT posted to EdX on purpose: {grade}")
                 raise GradePostException("NOT POSTING Grades on purpose; see deployment-config-encrypted.yaml -- POST_GRADE")
         except GradePostException as gp:
             log_error_csv(name, args, str(gp))
         except Exception as ex:
             log_error_csv(name, args, str(ex))
```

### Comparing `otter_service-0.2.6/src/otter_service/secrets/gh_key.yaml` & `otter_service-0.2.8/src/otter_service/secrets/gh_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.6/src/otter_service/secrets/gke_key.yaml` & `otter_service-0.2.8/src/otter_service/secrets/gke_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.6/src/otter_service/util.py` & `otter_service-0.2.8/src/otter_service/util.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.6/src/otter_service.egg-info/PKG-INFO` & `otter_service-0.2.8/src/otter_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-service
-Version: 0.2.6
+Version: 0.2.8
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `otter_service-0.2.6/src/otter_service.egg-info/SOURCES.txt` & `otter_service-0.2.8/src/otter_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.6/tests/test_access_sops_keys.py` & `otter_service-0.2.8/tests/test_access_sops_keys.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.6/tests/test_grade_assignment.py` & `otter_service-0.2.8/tests/test_grade_assignment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-import otter_service.access_sops_keys as ask
 import otter_service.grade_assignment as ga
 import os
 import shutil
 
 
 @pytest.fixture()
 def configure():
@@ -26,13 +25,13 @@
     secrets_file = os.path.join(os.path.dirname(__file__), "test_files/gh_key.yaml")
     args = {
         "course": "8x",
         "section": "1",
         "assignment": "lab01",
         "autograder_materials_repo": "github.com/data-8/materials-x22-private"
     }
-    grade = await ga.grade_assignment("tests/test_files/lab01.ipynb",
-                                      args,
-                                      sops_path="sops",
-                                      secrets_file=secrets_file,
-                                      save_path=".")
+    grade, _ = await ga.grade_assignment("tests/test_files/lab01.ipynb",
+                                         args,
+                                         sops_path="sops",
+                                         secrets_file=secrets_file,
+                                         save_path=".")
     assert 1.0 == grade
```

### Comparing `otter_service-0.2.6/tests/test_otter_nb.py` & `otter_service-0.2.8/tests/test_otter_nb.py`

 * *Files identical despite different names*

