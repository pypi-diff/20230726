# Comparing `tmp/otter_service-0.2.5.tar.gz` & `tmp/otter_service-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter_service-0.2.5.tar", last modified: Wed Jul 26 17:17:38 2023, max compression
+gzip compressed data, was "otter_service-0.2.6.tar", last modified: Wed Jul 26 20:16:08 2023, max compression
```

## Comparing `otter_service-0.2.5.tar` & `otter_service-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 17:17:38.128559 otter_service-0.2.5/
--rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.5/LICENSE
--rw-r--r--   0 sean       (501) staff       (20)     9491 2023-07-26 17:17:38.129479 otter_service-0.2.5/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)     9032 2023-07-26 00:15:36.000000 otter_service-0.2.5/README.md
--rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.5/pyproject.toml
--rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-26 17:17:38.131303 otter_service-0.2.5/setup.cfg
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 17:17:38.074299 otter_service-0.2.5/src/
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 17:17:38.109291 otter_service-0.2.5/src/otter_service/
--rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-26 17:16:44.000000 otter_service-0.2.5/src/otter_service/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)     2149 2023-07-26 15:52:24.000000 otter_service-0.2.5/src/otter_service/access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1025 2023-07-21 21:37:40.000000 otter_service-0.2.5/src/otter_service/firestore-test.py
--rw-r--r--   0 sean       (501) staff       (20)     5366 2023-07-26 00:52:44.000000 otter_service-0.2.5/src/otter_service/grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)    19457 2023-07-26 15:55:12.000000 otter_service-0.2.5/src/otter_service/otter_nb.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 17:17:38.120910 otter_service-0.2.5/src/otter_service/secrets/
--rw-r--r--   0 sean       (501) staff       (20)     1043 2023-07-26 01:06:26.000000 otter_service-0.2.5/src/otter_service/secrets/gh_key.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.5/src/otter_service/secrets/gke_key.yaml
--rw-r--r--   0 sean       (501) staff       (20)      516 2023-07-25 18:59:31.000000 otter_service-0.2.5/src/otter_service/util.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 17:17:38.117307 otter_service-0.2.5/src/otter_service.egg-info/
--rw-r--r--   0 sean       (501) staff       (20)     9491 2023-07-26 17:17:38.000000 otter_service-0.2.5/src/otter_service.egg-info/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)      610 2023-07-26 17:17:38.000000 otter_service-0.2.5/src/otter_service.egg-info/SOURCES.txt
--rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-26 17:17:38.000000 otter_service-0.2.5/src/otter_service.egg-info/dependency_links.txt
--rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-26 17:17:38.000000 otter_service-0.2.5/src/otter_service.egg-info/entry_points.txt
--rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-26 17:17:38.000000 otter_service-0.2.5/src/otter_service.egg-info/top_level.txt
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 17:17:38.124546 otter_service-0.2.5/tests/
--rw-r--r--   0 sean       (501) staff       (20)      913 2023-07-26 00:57:35.000000 otter_service-0.2.5/tests/test_access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1217 2023-07-26 00:58:54.000000 otter_service-0.2.5/tests/test_grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)     2140 2023-07-21 23:00:39.000000 otter_service-0.2.5/tests/test_otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 20:16:08.873680 otter_service-0.2.6/
+-rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.6/LICENSE
+-rw-r--r--   0 sean       (501) staff       (20)     9235 2023-07-26 20:16:08.874779 otter_service-0.2.6/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)     8776 2023-07-26 18:31:30.000000 otter_service-0.2.6/README.md
+-rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.6/pyproject.toml
+-rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-26 20:16:08.876308 otter_service-0.2.6/setup.cfg
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 20:16:08.857794 otter_service-0.2.6/src/
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 20:16:08.866440 otter_service-0.2.6/src/otter_service/
+-rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-26 20:15:09.000000 otter_service-0.2.6/src/otter_service/__init__.py
+-rw-r--r--   0 sean       (501) staff       (20)     2149 2023-07-26 15:52:24.000000 otter_service-0.2.6/src/otter_service/access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1025 2023-07-21 21:37:40.000000 otter_service-0.2.6/src/otter_service/firestore-test.py
+-rw-r--r--   0 sean       (501) staff       (20)     5332 2023-07-26 19:31:25.000000 otter_service-0.2.6/src/otter_service/grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)    19654 2023-07-26 19:31:34.000000 otter_service-0.2.6/src/otter_service/otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 20:16:08.870880 otter_service-0.2.6/src/otter_service/secrets/
+-rw-r--r--   0 sean       (501) staff       (20)     1043 2023-07-26 01:06:26.000000 otter_service-0.2.6/src/otter_service/secrets/gh_key.yaml
+-rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.6/src/otter_service/secrets/gke_key.yaml
+-rw-r--r--   0 sean       (501) staff       (20)      516 2023-07-25 18:59:31.000000 otter_service-0.2.6/src/otter_service/util.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 20:16:08.869757 otter_service-0.2.6/src/otter_service.egg-info/
+-rw-r--r--   0 sean       (501) staff       (20)     9235 2023-07-26 20:16:08.000000 otter_service-0.2.6/src/otter_service.egg-info/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)      610 2023-07-26 20:16:08.000000 otter_service-0.2.6/src/otter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-26 20:16:08.000000 otter_service-0.2.6/src/otter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-26 20:16:08.000000 otter_service-0.2.6/src/otter_service.egg-info/entry_points.txt
+-rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-26 20:16:08.000000 otter_service-0.2.6/src/otter_service.egg-info/top_level.txt
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 20:16:08.873163 otter_service-0.2.6/tests/
+-rw-r--r--   0 sean       (501) staff       (20)      913 2023-07-26 00:57:35.000000 otter_service-0.2.6/tests/test_access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1217 2023-07-26 00:58:54.000000 otter_service-0.2.6/tests/test_grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)     2140 2023-07-21 23:00:39.000000 otter_service-0.2.6/tests/test_otter_nb.py
```

### Comparing `otter_service-0.2.5/LICENSE` & `otter_service-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.5/PKG-INFO` & `otter_service-0.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,32 @@
-Metadata-Version: 2.1
-Name: otter_service
-Version: 0.2.5
-Summary: Grading Service for Edx 8x courses
-Home-page: https://github.com/data-8/otter-service
-Author: Vincent Su and Sean Morris
-Author-email: sean.smorris@berkeley.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # otter-nb service
 
 This repo contains a tornado flask app that accepts .ipynb files and grades them in a dockerized environment. Assuming you are running a Jupyterhub, you can ask Jupyterhub to run this otter-service as a service; you also have the option to run it in a stand alone manner. Grades are saved to a gcloud Cloud Firestore.
 
 A separate Jupyterhub extension, [otter_submit](https://github.com/data-8/otter_submit), presents a "Submit" button to the user in a notebook rendered in Jupyterhub. The button is configured to serialize and send the notebook to this otter-service as well as notify the the user of the successful submission.
 
 # FireStore/Database setup
 
 All grades are written to gcloud Cloud FireStore. During local testing with pytest, the tests remove the collection created after verifying the data was written. Local docker testing, does not delete the entries but the collection is called, otter-docker-local-test, and can be viewed and deleted by going to the gcloud console and navigating to Cloud Firebase or Cloud Firestore.
 
 # Configuration
 
 ## Notebook(ipynb metadata)
-The ipynb notebooks need to include the metadata for which assignment they are. In the case of Data 8x, there are three pieces of information that are relevant: the course id, section and lab. These are set in the metadata section of every notebook:
+The ipynb notebooks need to include the metadata for which assignment they are. In the case of Data 8x, there are three pieces of information that are relevant: the course name, section and lab. These values correspond to the course-config.json file described in the section below. These are set in the metadata section of every notebook:
 ```
 metadata:{
     "course": "8x",
     "section": "1",
-    "lab": "lab01"
+    "assignment": "lab01"
     ...
 }
 ```
 
 ## Course Configuration
-Each course needs to provide two pieces of information that is deployed in the secrets file of
+Each course needs to provide two pieces of information to whomever is handling otter-service(right now: sean.smorris@berkeley.edu) that is deployed in the secrets file of
 this application
 1) A Github access key to the private materials repo.
 
 2) The name of repository where the autograder.zip files are kept. (e.g. github.com/data-8/materials-x22-private)
 
 Finally, the private repository with the autograder.zip files needs to contain a file named: course-config.json. The file is structured like this:
 
@@ -153,15 +139,14 @@
 services:
   app:
     image: otter-srv
     build:
       context: .
       dockerfile: Dockerfile-dev
       args:
-        GIT_ACCESS_TOKEN: your_access_token generated by your github account -- see below
         OTTER_SERVICE_VERSION: whatever_version you specify in otter-service/__init__.py
     env_file:
       - ../.local-env
     ports:
       - 10101:10101
     volumes:
       - /tmp/otter:/mnt/data
@@ -169,15 +154,13 @@
 
 networks:
   default:
     driver: bridge
 ```
 
 Notes:
-- GIT_ACCESS_TOKEN is generated in your GitHub account. This is used to download the materials-x22-private archive to the otter-service docker image -- if you have test files somewhere else and they are not in a private repo this is unnecessary and you would need to change the relevant lines in the Dockerfile and Dockerfile-dev files.
-
 - .local-env These are environment variables that must be set. They mirror the variables in  `deployment/cloud/deployment-config-encrypted.yaml`. You do not need to encrypt your local-env file with sops. 
 
 # Service installation in JupyterHub
 
 Instructions can be found here for running it as a service within your [jupyterhub](https://jupyterhub.readthedocs.io/en/stable/reference/services.html#launching-a-hub-managed-service)
```

### Comparing `otter_service-0.2.5/README.md` & `otter_service-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,46 @@
+Metadata-Version: 2.1
+Name: otter_service
+Version: 0.2.6
+Summary: Grading Service for Edx 8x courses
+Home-page: https://github.com/data-8/otter-service
+Author: Vincent Su and Sean Morris
+Author-email: sean.smorris@berkeley.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # otter-nb service
 
 This repo contains a tornado flask app that accepts .ipynb files and grades them in a dockerized environment. Assuming you are running a Jupyterhub, you can ask Jupyterhub to run this otter-service as a service; you also have the option to run it in a stand alone manner. Grades are saved to a gcloud Cloud Firestore.
 
 A separate Jupyterhub extension, [otter_submit](https://github.com/data-8/otter_submit), presents a "Submit" button to the user in a notebook rendered in Jupyterhub. The button is configured to serialize and send the notebook to this otter-service as well as notify the the user of the successful submission.
 
 # FireStore/Database setup
 
 All grades are written to gcloud Cloud FireStore. During local testing with pytest, the tests remove the collection created after verifying the data was written. Local docker testing, does not delete the entries but the collection is called, otter-docker-local-test, and can be viewed and deleted by going to the gcloud console and navigating to Cloud Firebase or Cloud Firestore.
 
 # Configuration
 
 ## Notebook(ipynb metadata)
-The ipynb notebooks need to include the metadata for which assignment they are. In the case of Data 8x, there are three pieces of information that are relevant: the course id, section and lab. These are set in the metadata section of every notebook:
+The ipynb notebooks need to include the metadata for which assignment they are. In the case of Data 8x, there are three pieces of information that are relevant: the course name, section and lab. These values correspond to the course-config.json file described in the section below. These are set in the metadata section of every notebook:
 ```
 metadata:{
     "course": "8x",
     "section": "1",
-    "lab": "lab01"
+    "assignment": "lab01"
     ...
 }
 ```
 
 ## Course Configuration
-Each course needs to provide two pieces of information that is deployed in the secrets file of
+Each course needs to provide two pieces of information to whomever is handling otter-service(right now: sean.smorris@berkeley.edu) that is deployed in the secrets file of
 this application
 1) A Github access key to the private materials repo.
 
 2) The name of repository where the autograder.zip files are kept. (e.g. github.com/data-8/materials-x22-private)
 
 Finally, the private repository with the autograder.zip files needs to contain a file named: course-config.json. The file is structured like this:
 
@@ -139,15 +153,14 @@
 services:
   app:
     image: otter-srv
     build:
       context: .
       dockerfile: Dockerfile-dev
       args:
-        GIT_ACCESS_TOKEN: your_access_token generated by your github account -- see below
         OTTER_SERVICE_VERSION: whatever_version you specify in otter-service/__init__.py
     env_file:
       - ../.local-env
     ports:
       - 10101:10101
     volumes:
       - /tmp/otter:/mnt/data
@@ -155,15 +168,13 @@
 
 networks:
   default:
     driver: bridge
 ```
 
 Notes:
-- GIT_ACCESS_TOKEN is generated in your GitHub account. This is used to download the materials-x22-private archive to the otter-service docker image -- if you have test files somewhere else and they are not in a private repo this is unnecessary and you would need to change the relevant lines in the Dockerfile and Dockerfile-dev files.
-
 - .local-env These are environment variables that must be set. They mirror the variables in  `deployment/cloud/deployment-config-encrypted.yaml`. You do not need to encrypt your local-env file with sops. 
 
 # Service installation in JupyterHub
 
 Instructions can be found here for running it as a service within your [jupyterhub](https://jupyterhub.readthedocs.io/en/stable/reference/services.html#launching-a-hub-managed-service)
```

### Comparing `otter_service-0.2.5/setup.cfg` & `otter_service-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.5/src/otter_service/access_sops_keys.py` & `otter_service-0.2.6/src/otter_service/access_sops_keys.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.5/src/otter_service/firestore-test.py` & `otter_service-0.2.6/src/otter_service/firestore-test.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.5/src/otter_service/grade_assignment.py` & `otter_service-0.2.6/src/otter_service/grade_assignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,28 +75,27 @@
     :param args: json containing metadata from notebook
         - course: used as key to secrets file and course config
         - section: key to course config
         - assignment: key to assignment name
     :param sops_path: [OPTIONAL] used to execute pytests
     :param secrets_file: [OPTIONAL] used to execute pytests
     :param save_path: [OPTIONAL] used to execute pytests
-    :return: grade
-    :rtype: float
+    :return: grade, solutions_base_path
+    :rtype: float, string
     """
     try:
         solutions_base_path = None
         if save_path is None:
             save_path = "/opt"
         if secrets_file is None:
             secrets_file = os.path.join(os.path.dirname(__file__), "secrets/gh_key.yaml")
         solutions_base_path = download_autograder_materials(args["course"], sops_path, secrets_file, save_path=save_path)
+
         course_config = util.get_course_config(solutions_base_path)
-        print("===========")
-        print(course_config)
-        print("----------")
+
         autograder_subpath = course_config[args["course"]][args["section"]]["subpath_to_zips"]
 
         solutions_path = f'{solutions_base_path}/{autograder_subpath}/{args["assignment"]}/autograder.zip'
 
         command = [
             'otter', 'grade',
             '-a', solutions_path,
@@ -124,14 +123,14 @@
                 raise Exception(f"Container was killed -- nothing will work: {submission}")
 
         grade = stdout.decode("utf-8").strip()
         if grade is None or grade == '':
             cmd = ' '.join(command)
             raise Exception(f"Unable to determine grade coming from otter on: {submission} using this commnad: {cmd}")
 
-        return float(grade)
+        return float(grade), solutions_base_path
     except asyncio.TimeoutError:
         raise Exception(f'Grading timed out for {submission}')
     except Exception as e:
         raise e
     finally:
         remove_notebook()
```

### Comparing `otter_service-0.2.5/src/otter_service/otter_nb.py` & `otter_service-0.2.6/src/otter_service/otter_nb.py`

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
-from otter_service.grade_assignment import grade_assignment
+from otter_service.grade_assignment import grade_assignment, download_autograder_materials
 import firebase_admin
 from firebase_admin import credentials, firestore
 import grpc
 from google.cloud.firestore_v1.client import firestore_client
 from google.cloud.firestore_v1.client import firestore_grpc_transport
 import otter_service.util as util
 
@@ -98,28 +98,29 @@
     :param course_id: the course id for this notebook
     :param assignment_id:  the assignment id for this notebook
     :return: formatted string
     """
     return f"course-v1%3A{course_id}:{os.environ['EDX_URL']}-{assignment_id}"
 
 
-async def post_grade(user_id, grade, course, section, assignment):
+async def post_grade(solutions_base_path, user_id, grade, course, section, assignment):
     """
     This posts the grade to the LTI server
+    :paraem solutions_base_path: where the config file is to find the assignment id
     :param user_id: the user to post the grade for
     :param grade: the grade as a float
     :param course: the course this notebook is in
     :param section: the section this notebook is in
     :param assignment:  the assignment name for this notebook
     """
     body_hash = ""
     consumer_key = ""
     try:
         # post grade to EdX
-        course_config = util.get_course_config()
+        course_config = util.get_course_config(solutions_base_path)
 
         course_id = course_config[course][section]["course_id"]
         assignment_id = course_config[course][section]["assignments"][assignment]
 
         log_info_csv(user_id, course, section, assignment, f"Edx Course Config Loaded: Course Id: {course_id}, Assignment_id: {assignment_id}")
 
         sourced_id = create_sourced_id(course_id, assignment_id)
@@ -322,29 +323,29 @@
         course = args["course"]
         section = args["section"]
         assignment = args["assignment"]
         name = args["name"]
         file_path = args["submission_file"]
         try:
             # Grade assignment
-            grade = await grade_assignment(file_path, args)
+            grade, solutions_base_path = await grade_assignment(file_path, args)
             log_info_csv(name, args, f"Grade: {grade}")
             # Write the grade to a Firestore
             grade_info = {
                 "userid": name,
                 "course": course,
                 "grade": grade,
                 "section": section,
                 "assignment": assignment
             }
             write_grade(grade_info)
             log_info_csv(name, args, f"Grade Written to database: {grade}")
 
             if os.getenv("POST_GRADE").lower() in ("true", '1', 't'):
-                await post_grade(name, grade, course, section, assignment)
+                await post_grade(solutions_base_path, name, grade, course, section, assignment)
             else:
                 log_info_csv(name, args, f"Grade NOT posted to EdX on purpose: {grade}")
                 raise GradePostException("NOT POSTING Grades on purpose; see deployment-config-encrypted.yaml -- POST_GRADE")
         except GradePostException as gp:
             log_error_csv(name, args, str(gp))
         except Exception as ex:
             log_error_csv(name, args, str(ex))
```

### Comparing `otter_service-0.2.5/src/otter_service/secrets/gh_key.yaml` & `otter_service-0.2.6/src/otter_service/secrets/gh_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.5/src/otter_service/secrets/gke_key.yaml` & `otter_service-0.2.6/src/otter_service/secrets/gke_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.5/src/otter_service/util.py` & `otter_service-0.2.6/src/otter_service/util.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.5/src/otter_service.egg-info/PKG-INFO` & `otter_service-0.2.6/src/otter_service.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-service
-Version: 0.2.5
+Version: 0.2.6
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,26 +21,26 @@
 # FireStore/Database setup
 
 All grades are written to gcloud Cloud FireStore. During local testing with pytest, the tests remove the collection created after verifying the data was written. Local docker testing, does not delete the entries but the collection is called, otter-docker-local-test, and can be viewed and deleted by going to the gcloud console and navigating to Cloud Firebase or Cloud Firestore.
 
 # Configuration
 
 ## Notebook(ipynb metadata)
-The ipynb notebooks need to include the metadata for which assignment they are. In the case of Data 8x, there are three pieces of information that are relevant: the course id, section and lab. These are set in the metadata section of every notebook:
+The ipynb notebooks need to include the metadata for which assignment they are. In the case of Data 8x, there are three pieces of information that are relevant: the course name, section and lab. These values correspond to the course-config.json file described in the section below. These are set in the metadata section of every notebook:
 ```
 metadata:{
     "course": "8x",
     "section": "1",
-    "lab": "lab01"
+    "assignment": "lab01"
     ...
 }
 ```
 
 ## Course Configuration
-Each course needs to provide two pieces of information that is deployed in the secrets file of
+Each course needs to provide two pieces of information to whomever is handling otter-service(right now: sean.smorris@berkeley.edu) that is deployed in the secrets file of
 this application
 1) A Github access key to the private materials repo.
 
 2) The name of repository where the autograder.zip files are kept. (e.g. github.com/data-8/materials-x22-private)
 
 Finally, the private repository with the autograder.zip files needs to contain a file named: course-config.json. The file is structured like this:
 
@@ -153,15 +153,14 @@
 services:
   app:
     image: otter-srv
     build:
       context: .
       dockerfile: Dockerfile-dev
       args:
-        GIT_ACCESS_TOKEN: your_access_token generated by your github account -- see below
         OTTER_SERVICE_VERSION: whatever_version you specify in otter-service/__init__.py
     env_file:
       - ../.local-env
     ports:
       - 10101:10101
     volumes:
       - /tmp/otter:/mnt/data
@@ -169,15 +168,13 @@
 
 networks:
   default:
     driver: bridge
 ```
 
 Notes:
-- GIT_ACCESS_TOKEN is generated in your GitHub account. This is used to download the materials-x22-private archive to the otter-service docker image -- if you have test files somewhere else and they are not in a private repo this is unnecessary and you would need to change the relevant lines in the Dockerfile and Dockerfile-dev files.
-
 - .local-env These are environment variables that must be set. They mirror the variables in  `deployment/cloud/deployment-config-encrypted.yaml`. You do not need to encrypt your local-env file with sops. 
 
 # Service installation in JupyterHub
 
 Instructions can be found here for running it as a service within your [jupyterhub](https://jupyterhub.readthedocs.io/en/stable/reference/services.html#launching-a-hub-managed-service)
```

### Comparing `otter_service-0.2.5/src/otter_service.egg-info/SOURCES.txt` & `otter_service-0.2.6/src/otter_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.5/tests/test_access_sops_keys.py` & `otter_service-0.2.6/tests/test_access_sops_keys.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.5/tests/test_grade_assignment.py` & `otter_service-0.2.6/tests/test_grade_assignment.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.5/tests/test_otter_nb.py` & `otter_service-0.2.6/tests/test_otter_nb.py`

 * *Files identical despite different names*

