# Comparing `tmp/otter_service-0.2.4.tar.gz` & `tmp/otter_service-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter_service-0.2.4.tar", last modified: Fri Jul 21 22:48:36 2023, max compression
+gzip compressed data, was "otter_service-0.2.5.tar", last modified: Wed Jul 26 17:17:38 2023, max compression
```

## Comparing `otter_service-0.2.4.tar` & `otter_service-0.2.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 22:48:36.668910 otter_service-0.2.4/
--rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.4/LICENSE
--rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 22:48:36.669122 otter_service-0.2.4/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)     7704 2023-07-21 17:54:42.000000 otter_service-0.2.4/README.md
--rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.4/pyproject.toml
--rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-21 22:48:36.670053 otter_service-0.2.4/setup.cfg
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 22:48:36.653994 otter_service-0.2.4/src/
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 22:48:36.660045 otter_service-0.2.4/src/otter_service/
--rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-21 22:47:47.000000 otter_service-0.2.4/src/otter_service/__init__.py
--rw-r--r--   0 sean       (501) staff       (20)     1722 2023-07-21 17:51:59.000000 otter_service-0.2.4/src/otter_service/access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1025 2023-07-21 21:37:40.000000 otter_service-0.2.4/src/otter_service/firestore-test.py
--rw-r--r--   0 sean       (501) staff       (20)     5059 2023-07-21 21:13:17.000000 otter_service-0.2.4/src/otter_service/grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)    19655 2023-07-21 22:47:47.000000 otter_service-0.2.4/src/otter_service/otter_nb.py
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 22:48:36.663850 otter_service-0.2.4/src/otter_service/secrets/
--rw-r--r--   0 sean       (501) staff       (20)      983 2023-07-21 17:51:59.000000 otter_service-0.2.4/src/otter_service/secrets/gh_key.yaml
--rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.4/src/otter_service/secrets/gke_key.yaml
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 22:48:36.662629 otter_service-0.2.4/src/otter_service.egg-info/
--rw-r--r--   0 sean       (501) staff       (20)     8163 2023-07-21 22:48:36.000000 otter_service-0.2.4/src/otter_service.egg-info/PKG-INFO
--rw-r--r--   0 sean       (501) staff       (20)      584 2023-07-21 22:48:36.000000 otter_service-0.2.4/src/otter_service.egg-info/SOURCES.txt
--rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-21 22:48:36.000000 otter_service-0.2.4/src/otter_service.egg-info/dependency_links.txt
--rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-21 22:48:36.000000 otter_service-0.2.4/src/otter_service.egg-info/entry_points.txt
--rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-21 22:48:36.000000 otter_service-0.2.4/src/otter_service.egg-info/top_level.txt
-drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-21 22:48:36.668444 otter_service-0.2.4/tests/
--rw-r--r--   0 sean       (501) staff       (20)      895 2022-06-18 01:43:56.000000 otter_service-0.2.4/tests/test_access_sops_keys.py
--rw-r--r--   0 sean       (501) staff       (20)     1416 2023-07-21 17:51:59.000000 otter_service-0.2.4/tests/test_grade_assignment.py
--rw-r--r--   0 sean       (501) staff       (20)     2140 2023-07-21 22:47:47.000000 otter_service-0.2.4/tests/test_otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 17:17:38.128559 otter_service-0.2.5/
+-rw-r--r--   0 sean       (501) staff       (20)     1498 2021-10-24 00:07:22.000000 otter_service-0.2.5/LICENSE
+-rw-r--r--   0 sean       (501) staff       (20)     9491 2023-07-26 17:17:38.129479 otter_service-0.2.5/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)     9032 2023-07-26 00:15:36.000000 otter_service-0.2.5/README.md
+-rw-r--r--   0 sean       (501) staff       (20)      103 2023-07-20 15:40:45.000000 otter_service-0.2.5/pyproject.toml
+-rw-r--r--   0 sean       (501) staff       (20)      786 2023-07-26 17:17:38.131303 otter_service-0.2.5/setup.cfg
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 17:17:38.074299 otter_service-0.2.5/src/
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 17:17:38.109291 otter_service-0.2.5/src/otter_service/
+-rw-r--r--   0 sean       (501) staff       (20)       22 2023-07-26 17:16:44.000000 otter_service-0.2.5/src/otter_service/__init__.py
+-rw-r--r--   0 sean       (501) staff       (20)     2149 2023-07-26 15:52:24.000000 otter_service-0.2.5/src/otter_service/access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1025 2023-07-21 21:37:40.000000 otter_service-0.2.5/src/otter_service/firestore-test.py
+-rw-r--r--   0 sean       (501) staff       (20)     5366 2023-07-26 00:52:44.000000 otter_service-0.2.5/src/otter_service/grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)    19457 2023-07-26 15:55:12.000000 otter_service-0.2.5/src/otter_service/otter_nb.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 17:17:38.120910 otter_service-0.2.5/src/otter_service/secrets/
+-rw-r--r--   0 sean       (501) staff       (20)     1043 2023-07-26 01:06:26.000000 otter_service-0.2.5/src/otter_service/secrets/gh_key.yaml
+-rw-r--r--   0 sean       (501) staff       (20)     1229 2022-06-11 00:39:08.000000 otter_service-0.2.5/src/otter_service/secrets/gke_key.yaml
+-rw-r--r--   0 sean       (501) staff       (20)      516 2023-07-25 18:59:31.000000 otter_service-0.2.5/src/otter_service/util.py
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 17:17:38.117307 otter_service-0.2.5/src/otter_service.egg-info/
+-rw-r--r--   0 sean       (501) staff       (20)     9491 2023-07-26 17:17:38.000000 otter_service-0.2.5/src/otter_service.egg-info/PKG-INFO
+-rw-r--r--   0 sean       (501) staff       (20)      610 2023-07-26 17:17:38.000000 otter_service-0.2.5/src/otter_service.egg-info/SOURCES.txt
+-rw-r--r--   0 sean       (501) staff       (20)        1 2023-07-26 17:17:38.000000 otter_service-0.2.5/src/otter_service.egg-info/dependency_links.txt
+-rw-r--r--   0 sean       (501) staff       (20)       62 2023-07-26 17:17:38.000000 otter_service-0.2.5/src/otter_service.egg-info/entry_points.txt
+-rw-r--r--   0 sean       (501) staff       (20)       14 2023-07-26 17:17:38.000000 otter_service-0.2.5/src/otter_service.egg-info/top_level.txt
+drwxr-xr-x   0 sean       (501) staff       (20)        0 2023-07-26 17:17:38.124546 otter_service-0.2.5/tests/
+-rw-r--r--   0 sean       (501) staff       (20)      913 2023-07-26 00:57:35.000000 otter_service-0.2.5/tests/test_access_sops_keys.py
+-rw-r--r--   0 sean       (501) staff       (20)     1217 2023-07-26 00:58:54.000000 otter_service-0.2.5/tests/test_grade_assignment.py
+-rw-r--r--   0 sean       (501) staff       (20)     2140 2023-07-21 23:00:39.000000 otter_service-0.2.5/tests/test_otter_nb.py
```

### Comparing `otter_service-0.2.4/LICENSE` & `otter_service-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.4/PKG-INFO` & `otter_service-0.2.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: otter_service
-Version: 0.2.4
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
@@ -31,16 +17,56 @@
     "course": "8x",
     "section": "1",
     "lab": "lab01"
     ...
 }
 ```
 
-## Course config path
-Please see the repository `data-8/materials-x22-private`. The repository houses a config file, 8x_course_config_edge.json and 8x_course_config.json. The system relies on this file specified in the environment variable, `COURSE_CONFIG_PATH`, to know which lab is associated with which assignment id in EdX. If you are not posting grades to an LTI server, than you do not need to worry about this.
+## Course Configuration
+Each course needs to provide two pieces of information that is deployed in the secrets file of
+this application
+1) A Github access key to the private materials repo.
+
+2) The name of repository where the autograder.zip files are kept. (e.g. github.com/data-8/materials-x22-private)
+
+Finally, the private repository with the autograder.zip files needs to contain a file named: course-config.json. The file is structured like this:
+
+(1) course name which matches the course name in every notebooks metadata<br>
+(2) section which matches the section in every notebooks metadata - if only one section put '1'<br>
+(3) Edx course id<br>
+(4) subpath to each autograder.zip in private autograder.zip repo<br>
+(5) each EDX assignment name and assignment Id -- the assignment name must match the notebook metadata
+
+```
+{
+  "8x" : { //(1)
+    "1": { //(2)
+      "course_id": "BerkeleyX+Data8.1x+3T2022", //(3)
+      "subpath_to_zips": "materials/x22/lab/1", //(4)
+      "assignments": {  //(5)
+        "lab01": "6333e19d6b4d46f88df671ba50f616d8",
+        "lab02": "fbf6740d45094b9b977111d218969273",
+        "lab03": "0c8f28bdc48d4231843f62b512d73638",
+        "lab04": "8db69daf14cf4751a088106be912c0cd",
+        "lab05": "4cb9e3491c284cd5ae29bb48219ee15b"
+      }
+    },
+    "2":{
+      "course_id": "BerkeleyX+Data8.2x+3T2022",
+      "subpath_to_zips": "materials/x22/lab/2",
+      "assignments": {
+        "lab01": "7abc0025c10f4b8ab123dbc88d34faaf",
+        ...
+```
+Here is an example of the folder structure in the materials-x22-private repo. 
+![Alt text](image.png)
+
+Note how the folder structure is mirrored in the course-config.json.
+
+If you are not posting grades to an LTI server, than you do not need to worry about this.
 
 
 ## Test files
 This gets tricky. The notebooks and the corresponding test files used by this service are of course connected. The files `Dockerfile` and `Dockerfile-dev` (used for local testing) download the current set of test files from the repository, `materials-x22-private`, for the `materials-x22` notebooks. If you bring in different notebooks, you would need to change the two dockerfiles to bring in the corresponding tests. 
 
 We assume a specific path to the test files. If you mirror the path found in the `materials-x22-private` repository, all will work well. If you change the path, then you must change the `solutions-path` variable in `grade_assignment.py`.
```

### Comparing `otter_service-0.2.4/setup.cfg` & `otter_service-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.4/src/otter_service/access_sops_keys.py` & `otter_service-0.2.5/src/otter_service/access_sops_keys.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,62 @@
 import os
 import subprocess
 import yaml
 
 
-def get(key_name, sops_path=None, secrets_file=None) -> str:
+def get(course_key, key_name, sops_path=None, secrets_file=None) -> str:
     """
     This method first tries to decrypt sops file and then tries the
     environment. it will return an Exception if the key is not found
 
+    :param course_key: the course to find in Google Secrets Manager
     :param key_name: the name of the key to retrieve from the Secrets or the environment
     :param secrets_file: the name of the secrets file associated with the key
     :return: the secret
     """
     try:
-        secret = get_via_env(key_name)
+        secret = get_via_env(course_key, key_name)
         if secret is None:
-            secret = get_via_sops(key_name, sops_path=sops_path, secrets_file=secrets_file)
+            secret = get_via_sops(course_key, key_name, sops_path=sops_path, secrets_file=secrets_file)
         return secret
     except Exception as ex:
         raise Exception(f"Key not decrypted: {key_name}; please configure: Error: {ex}") from ex
 
 
-def get_via_sops(key, sops_path=None, secrets_file=None):
+def get_via_sops(course_key, key, sops_path=None, secrets_file=None):
     """
     This function attempts to use sops to decrpyt the secrets/{secrets_file}
 
-    :param key: the key to find in Google Secrets Manager
+    :param course_key: the course to find in Google Secrets Manager
+    :param key: the key to find in the course in Google Secrets Manager
     :param sops_path: [OPTIONAL] used to execute pytests
     :param secrets_file: [OPTIONAL] used to execute pytests
     :return: the value of the key or None
     """
     try:
         if sops_path is None:
             sops_path = "/root/go/bin/sops"
 
         secrets_file = secrets_file
 
         sops_output = subprocess.check_output([sops_path, "-d", secrets_file], stderr=subprocess.STDOUT)
         dct = yaml.safe_load(sops_output)
-        return dct[key]
+        if course_key is None:
+            return dct[key]
+        return dct[course_key][key]
     except Exception as ex:
         raise ex
 
 
-def get_via_env(key):
+def get_via_env(course_key, key):
     """
     This checks the environment for the key.
 
+    :param course_key: the course to find in Google Secrets Manager
     :param key: the key to find in the environment
     :return: the value of the key or None
     """
     if key in os.environ:
-        return os.environ[key]
+        if course_key is None:
+            return os.environ[key]
+        return os.environ[course_key][key]
     return None
```

### Comparing `otter_service-0.2.4/src/otter_service/firestore-test.py` & `otter_service-0.2.5/src/otter_service/firestore-test.py`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.4/src/otter_service/grade_assignment.py` & `otter_service-0.2.5/src/otter_service/grade_assignment.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,99 +2,108 @@
 import async_timeout
 import requests
 import tarfile
 import os
 import glob
 from otter_service import access_sops_keys
 import shutil
+import otter_service.util as util
 
 
-def download_autograder_materials(url, save_path=None):
+def download_autograder_materials(course, sops_path, secrets_file, save_path=None):
     """
-    This function downloads the appropriate archive of autograder materials be used for testing
+    This function downloads the appropriate archive of autograder materials be used for testing. The archive
+    must be on the main branch(but it will also try the master branch if main fails)
 
-    :param url: the url to the archive of materials
+    :param course: key to git access token in secrets file
+    :param sops_path: path to sops executable
+    :param secrets_file: path to secrets file
     :param save_path: Where to save the archive -- for testing it is "." for normal it will /tmp
     """
+    branch = "main"
+    git_access_token = access_sops_keys.get(course, "github_access_token", sops_path=sops_path, secrets_file=secrets_file)
+    autograder_materials_repo = access_sops_keys.get(course, "autograder_repo", sops_path=sops_path, secrets_file=secrets_file)
+    materials_url = f"https://{git_access_token}:@{autograder_materials_repo}/archive/{branch}.tar.gz"
+        
     download_path = "/tmp/materials.tar.gz"
     if save_path is None:
         save_path = "."
         download_path = "./materials.tar.gz"
-    r = requests.get(url, stream=True)
+    r = requests.get(materials_url, stream=True)
+    if r.status_code != 200:
+        branch = "master"
+        materials_url = f"https://{git_access_token}:@{autograder_materials_repo}/archive/{branch}.tar.gz"    
+        r = requests.get(materials_url, stream=True)
 
     if r.status_code == 200:
         with open(download_path, 'wb') as f:
             f.write(r.raw.read())
         file = tarfile.open(download_path)
         file.extractall(save_path)
         file.close()
-        url_parts = url.split("/")
+        url_parts = materials_url.split("/")
         branch = url_parts[-1].split(".")[0]
-        file_name = os.environ["AUTOGRADER_REPO"]
+        file_name = autograder_materials_repo.split("/")[-1]
         extracted_path = f"{save_path}/{file_name}-{branch}"
         storage_path = f"{save_path}/{file_name}"
         if os.path.isdir(storage_path):
             shutil.rmtree(storage_path)
         os.rename(extracted_path, storage_path)
         os.remove(download_path)
     else:
-        raise Exception(f"Unable to access: {url}")
+        raise Exception(f"Unable to access: {autograder_materials_repo}")
     return storage_path
 
 
 def remove_notebook():
     files = glob.glob('/tmp/*')
     for f in files:
         if not os.path.isdir(f):
             try:
                 os.remove(f)
             except Exception:
                 pass
 
 
-async def grade_assignment(submission, sec='3', assignment='lab01', solutions_path=None, sops_path=None, secrets_file=None, save_path=None):
+async def grade_assignment(submission,
+                           args,
+                           sops_path=None, secrets_file=None, save_path=None):
     """
     This function spins up a docker instance using otter, grades the submission
     and returns the grade
 
     :param submission: the path to the file you want to grade
-    :param sec: the course section; it is used to determine the path to the solution file
-    :param assignment: the name of the assignment; it is used to determine the path to the solution file
-    :param solutions_path: [OPTIONAL] used to execute pytests
+    :param args: json containing metadata from notebook
+        - course: used as key to secrets file and course config
+        - section: key to course config
+        - assignment: key to assignment name
     :param sops_path: [OPTIONAL] used to execute pytests
     :param secrets_file: [OPTIONAL] used to execute pytests
     :param save_path: [OPTIONAL] used to execute pytests
     :return: grade
     :rtype: float
     """
     try:
         solutions_base_path = None
         if save_path is None:
             save_path = "/opt"
         if secrets_file is None:
             secrets_file = os.path.join(os.path.dirname(__file__), "secrets/gh_key.yaml")
-        git_access_token = access_sops_keys.get("github_access_token", sops_path=sops_path, secrets_file=secrets_file)
-        materials_url = os.environ["AUTOGRADER_MATERIALS_URL"]
-        materials_url = f"https://{git_access_token}:@{materials_url}"
-        autograder_materials_subpath = os.environ["AUTOGRADER_MATERIALS_SUBPATH"]
-        solutions_base_path = download_autograder_materials(materials_url, save_path=save_path)
-        assign_type = "lab"
-        if "hw" in assignment:
-            assign_type = "hw"
-        if solutions_path is None:
-            solutions_path = '{solutions_base_path}/{autograder_materials_subpath}/{assign_type}/{sec}/{assignment}/autograder.zip'
-        zip_path = solutions_path.format(solutions_base_path=solutions_base_path,
-                                         autograder_materials_subpath=autograder_materials_subpath,
-                                         assign_type=assign_type,
-                                         sec=sec,
-                                         assignment=assignment)
+        solutions_base_path = download_autograder_materials(args["course"], sops_path, secrets_file, save_path=save_path)
+        course_config = util.get_course_config(solutions_base_path)
+        print("===========")
+        print(course_config)
+        print("----------")
+        autograder_subpath = course_config[args["course"]][args["section"]]["subpath_to_zips"]
+
+        solutions_path = f'{solutions_base_path}/{autograder_subpath}/{args["assignment"]}/autograder.zip'
 
         command = [
             'otter', 'grade',
-            '-a', zip_path,
+            '-a', solutions_path,
             '-p', submission
         ]
         process = await asyncio.create_subprocess_exec(
             *command,
             stdin=asyncio.subprocess.PIPE,
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE
```

### Comparing `otter_service-0.2.4/src/otter_service/otter_nb.py` & `otter_service-0.2.5/src/otter_service/otter_nb.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from otter_service import access_sops_keys
 from otter_service.grade_assignment import grade_assignment
 import firebase_admin
 from firebase_admin import credentials, firestore
 import grpc
 from google.cloud.firestore_v1.client import firestore_client
 from google.cloud.firestore_v1.client import firestore_grpc_transport
+import otter_service.util as util
+
 
 PREFIX = os.environ.get('JUPYTERHUB_SERVICE_PREFIX', '/services/otter_grade/')
 
 # Use the application default credentials
 cred = credentials.ApplicationDefault()
 firebase_admin.initialize_app(cred, {
     'projectId': os.environ.get("GCP_PROJECT_ID"),
@@ -109,21 +111,15 @@
     :param section: the section this notebook is in
     :param assignment:  the assignment name for this notebook
     """
     body_hash = ""
     consumer_key = ""
     try:
         # post grade to EdX
-        with open(f'{os.environ["COURSE_CONFIG_PATH"]}', 'r', encoding="utf8") as filename:
-            # Course DEPENDENT configuration file
-            # Should contain page for hitting the gradebook (outcomes_url)
-            # as well as resource IDs for assignments
-            # e.g. sourcedid['3']['lab02'] = c09d043b662b4b4b96fceacb1f4aa1c9
-            # Make sure that it's placed in the working directory of the service (pwdx <PID>)
-            course_config = json.load(filename)
+        course_config = util.get_course_config()
 
         course_id = course_config[course][section]["course_id"]
         assignment_id = course_config[course][section]["assignments"][assignment]
 
         log_info_csv(user_id, course, section, assignment, f"Edx Course Config Loaded: Course Id: {course_id}, Assignment_id: {assignment_id}")
 
         sourced_id = create_sourced_id(course_id, assignment_id)
@@ -154,16 +150,16 @@
                 </result>
               </resultRecord>
             </replaceResultRequest>
           </imsx_POXBody>
         </imsx_POXEnvelopeRequest>
         """
         secrets_file = os.path.join(os.path.dirname(__file__), "secrets/gke_key.yaml")
-        consumer_key = access_sops_keys.get("LTI_CONSUMER_KEY", secrets_file=secrets_file)
-        consumer_secret = access_sops_keys.get("LTI_CONSUMER_SECRET", secrets_file=secrets_file)
+        consumer_key = access_sops_keys.get(None, "LTI_CONSUMER_KEY", secrets_file=secrets_file)
+        consumer_secret = access_sops_keys.get(None, "LTI_CONSUMER_SECRET", secrets_file=secrets_file)
 
         sourced_id = f"{sourced_id}:{user_id}"
         post_data = post_xml.format(grade=float(grade), sourcedid=sourced_id)
 
         # Yes, we do have to use sha1 :(
         body_hash_sha = sha1()
         body_hash_sha.update(post_data.encode('utf-8'))
@@ -231,123 +227,131 @@
         self.write("This is a post only page. You probably shouldn't be here!")
         user = self.get_current_user()
         self.write(json.dumps(user))
         self.finish()
 
     # @authenticated
     async def post(self):
-        notebook = None
-        section = None
-        assignment = None
         user = {}
-        course = "not-set-yet"
+        metadata = {
+            "course": "not-set-yet",
+            "section": None,
+            "assignment": None
+        }
+        notebook = None
         timestamp = get_timestamp()
         using_test_user = False
         try:
             # Accept notebook submissions, saves, then grades them
             user = self.get_current_user()
-            log_info_csv("PRINT USER OBJ", course, section, assignment, str(user))
+            log_info_csv("PRINT USER OBJ", metadata, str(user))
             if user is None:
                 url_referer = self.request.headers.get("Referer")
                 if url_referer is None:
                     user = {"name": os.getenv("TEST_USER")}
                 else:
                     user = {"name": url_referer.split("/")[4]}
                 using_test_user = True
             req_data = tornado.escape.json_decode(self.request.body)
             # in the future, assignment should be metadata in notebook
             if 'nb' in req_data:
                 notebook = req_data['nb']
 
+            if "course" in notebook['metadata']:
+                metadata["course"] = notebook['metadata']['course']
+
             if "section" in notebook['metadata']:
-                section = notebook['metadata']['section']
+                metadata["section"] = notebook['metadata']['section']
 
             if "assignment" in notebook['metadata']:
-                assignment = notebook['metadata']['assignment']
+                metadata["assignment"] = notebook['metadata']['assignment']
             elif "lab" in notebook['metadata']:
-                assignment = notebook['metadata']['lab']
+                metadata["assignment"] = notebook['metadata']['lab']
+            
+            if metadata["course"] is None or \
+                metadata["section"] is None or \
+                    metadata["assignment"] is None:
+                err_msg = "Notebook does not have required metadata: course, section, and assignment"
+                raise GradeSubmissionException(err_msg)
 
-            if "course" in notebook['metadata']:
-                course = notebook['metadata']['course']
-
-            if notebook is None or section is None or assignment is None:
-                raise GradeSubmissionException("Notebook does not have required metadata or maybe no notebook in post")
-
-            log_info_csv(user["name"], course, section, assignment, f"User logged in -  Using Referrer: {using_test_user}")
+            log_info_csv(user["name"], metadata, f"User logged in -  Using Referrer: {using_test_user}")
             # save notebook submission with user id and time stamp - this will be deleted
             sub_timestamp = timestamp.replace(" ", "-").replace(",", "-").replace(":", "-")
-            submission_file = f"/tmp/{user['name']}_{section}_{assignment}_{sub_timestamp}.ipynb"
+            submission_file = f"/tmp/{user['name']}_{metadata['course']}_{metadata['section']}_{metadata['assignment']}_{sub_timestamp}.ipynb"
             with open(submission_file, 'w', encoding="utf8") as outfile:
                 json.dump(notebook, outfile)
-            save_submission(user['name'], course, section, assignment, notebook)
-            log_info_csv(user["name"], course, section, assignment, "user submission saved to logs")
+            save_submission(user['name'], metadata, notebook)
+            log_info_csv(user["name"], metadata, "user submission saved to logs")
 
-            args = {}
-            args["course"] = course
-            args["section"] = section
-            args["assignments"] = assignment
-            args["name"] = user["name"]
-            args["submission_file"] = submission_file
-            args["timestamp"] = str(timestamp)
+            metadata["name"] = user["name"]
+            metadata["submission_file"] = submission_file
+            metadata["timestamp"] = str(timestamp)
 
-            tornado.ioloop.IOLoop.current().spawn_callback(self._grade_and_post, args)
+            tornado.ioloop.IOLoop.current().spawn_callback(self._grade_and_post, metadata)
 
             # Let user know their submission was received
             self.write("Your submission is being graded and will be posted to the gradebook once it is finished running!")
             self.finish()
         except GradeSubmissionException as grade_submission_exception:
             if notebook is None:
-                section = "No notebook was in the request body"
-                assignment = "No notebook was in the request body"
+                metadata["section"] = "No notebook was in the request body"
+                metadata["assignment"] = "No notebook was in the request body"
             else:
-                if section is None:
-                    section = "Section: problem getting section - not in notebook?"
-                if assignment is None:
-                    assignment = "Assignment: problem getting assignment - not in notebook?"
+                if metadata["section"] is None:
+                    metadata["section"] = "Section: problem getting section - not in notebook?"
+                if metadata["assignment"] is None:
+                    metadata["assignment"] = "Assignment: problem getting assignment - not in notebook?"
 
-            log_error_csv(user['name'], course, section, assignment, str(grade_submission_exception))
+            log_error_csv(user['name'], metadata, str(grade_submission_exception))
         except Exception as ex:  # pylint: disable=broad-except
-            log_error_csv(user, course, section, assignment, str(ex))
+            log_error_csv(user, metadata, str(ex))
 
     async def _grade_and_post(self, args):
         """
         This is called by spawn_callback method on the IOLoop to move the actual grading and
         posting of the grade out of the main thread.
 
-        :param args course, section, assignments, name, submission_file, timestamp coming from post method above
+        :param args
+            - course
+            - section
+            - assignment
+            - autograder_subpath
+            - name
+            - submission_file
+            - timestamp
         """
         course = args["course"]
         section = args["section"]
-        assignment = args["assignments"]
+        assignment = args["assignment"]
         name = args["name"]
         file_path = args["submission_file"]
         try:
             # Grade assignment
-            grade = await grade_assignment(file_path, section, assignment)
-            log_info_csv(name, course, section, assignment, f"Grade: {grade}")
+            grade = await grade_assignment(file_path, args)
+            log_info_csv(name, args, f"Grade: {grade}")
             # Write the grade to a Firestore
             grade_info = {
                 "userid": name,
                 "course": course,
                 "grade": grade,
                 "section": section,
                 "assignment": assignment
             }
             write_grade(grade_info)
-            log_info_csv(name, course, section, assignment, f"Grade Written to database: {grade}")
+            log_info_csv(name, args, f"Grade Written to database: {grade}")
 
             if os.getenv("POST_GRADE").lower() in ("true", '1', 't'):
                 await post_grade(name, grade, course, section, assignment)
             else:
-                log_info_csv(name, course, section, assignment, f"Grade NOT posted to EdX on purpose: {grade}")
+                log_info_csv(name, args, f"Grade NOT posted to EdX on purpose: {grade}")
                 raise GradePostException("NOT POSTING Grades on purpose; see deployment-config-encrypted.yaml -- POST_GRADE")
         except GradePostException as gp:
-            log_error_csv(name, course, section, assignment, str(gp))
+            log_error_csv(name, args, str(gp))
         except Exception as ex:
-            log_error_csv(name, course, section, assignment, str(ex))
+            log_error_csv(name, args, str(ex))
         finally:
             if os.path.exists(file_path):
                 os.remove(file_path)
 
 
 def get_timestamp():
     """
@@ -355,68 +359,70 @@
     """
     date_format = "%Y-%m-%d %H:%M:%S,%f"
     date = datetime.now(tz=pytz.utc)
     date = date.astimezone(timezone('US/Pacific'))
     return date.strftime(date_format)[:-3]
 
 
-def write_logs(username, course, section, assignment, msg, trace, type, collection):
+def write_logs(username, data, msg, trace, type, collection):
     if os.getenv("VERBOSE_LOGGING") == "True" or type == "error":
         try:
             db = firestore.client()
             # this redirects FireStore to local emulator when local testing!
             if os.getenv("ENVIRONMENT") == "otter-docker-local-test":
                 channel = grpc.insecure_channel("host.docker.internal:8080")
                 transport = firestore_grpc_transport.FirestoreGrpcTransport(channel=channel)
                 db._firestore_api_internal = firestore_client.FirestoreClient(transport=transport)
             data = {
                 'user': username,
-                'course': course,
-                'section': section,
-                'assignment': assignment,
+                'course': data["course"],
+                'section': data["section"],
+                'assignment': data["assignment"],
                 'message': msg,
                 'trace': trace,
                 'type': type,
                 'timestamp': get_timestamp()
             }
             return db.collection(collection).add(data)
         except Exception as err:
             raise Exception(f"Error inserting {type} log into Google FireStore: {data}") from err
 
 
-def log_info_csv(username, course, section, assignment, msg):
+def log_info_csv(username, data, msg):
     """
     This logs information in the chain of events -- user logs in and submits,
     graded, posted to Edx
 
     :param username: the username
-    :param course: the course
-    :param section: the section
-    :param assignment: the assignment
+    :param data: json struct of data
+        - course: the course
+        - section: the section
+        - assignment: the assignment
     :param msg: optional message to logs
     """
     try:
-        write_logs(username, course, section, assignment, msg, None, "info", f'{os.environ.get("ENVIRONMENT")}-logs')
+        write_logs(username, data, msg, None, "info", f'{os.environ.get("ENVIRONMENT")}-logs')
     except Exception as e:
         raise e
 
 
-def log_error_csv(username, course, section, assignment, msg):
+def log_error_csv(username, data, msg):
     """
     This logs the errors occurring when posting assignments
 
     :param timestamp: when the error occurred
     :param username: the username
-    :param course: the course
-    :param section: the section
-    :param assignment: the assignment
+    :param data: json struct of data
+        - course: the course
+        - section: the section
+        - assignment: the assignment
     :param msg: optional message to logs
     """
     try:
-        write_logs(username, course, section, assignment, msg, str(traceback.format_exc()), "error", f'{os.environ.get("ENVIRONMENT")}-logs')
+        write_logs(username, data, msg, str(traceback.format_exc()), "error", f'{os.environ.get("ENVIRONMENT")}-logs')
     except Exception as e:
         raise e
 
 
 def log_tornado_issues(msg, type):
     """
     This logs the errors associated with tornado
@@ -434,30 +440,32 @@
             'timestamp': get_timestamp()
         }
         return db.collection(f'{os.environ.get("ENVIRONMENT")}-tornado-logs').add(data)
     except Exception as err:
         raise Exception(f"Error inserting {type} log into Google FireStore: {data}") from err
 
 
-def save_submission(username, course, section, assignment, notebook):
+def save_submission(username, data, notebook):
     """
     This logs the errors associated with tornado
 
-    :param msg: message about error
+    :param username: username
+    :param data: json struct of data
+        - course: the course
+        - section: the section
+        - assignment: the assignment
+        - autograder_materials_repo: the repo containing the autograder.zip
+        - autograder_subpath: the path in the repo to autograder.zip
+    :notebook: the cells in the notebook!
     """
     try:
         db = firestore.client()
-        data = {
-            'user': username,
-            'course': course,
-            'section': section,
-            'assignment': assignment,
-            'notebook': notebook,
-            'timestamp': get_timestamp()
-        }
+        data['user'] = username
+        data['notebook'] = notebook
+        data['timestamp'] = get_timestamp()
         return db.collection(f'{os.environ.get("ENVIRONMENT")}-submissions').add(data)
     except Exception as err:
         raise Exception(f"Error inserting {type} log into Google FireStore: {data}") from err
 
 
 def sig_handler(server, sig, frame):
     io_loop = tornado.ioloop.IOLoop.instance()
```

### Comparing `otter_service-0.2.4/src/otter_service/secrets/gke_key.yaml` & `otter_service-0.2.5/src/otter_service/secrets/gke_key.yaml`

 * *Files identical despite different names*

### Comparing `otter_service-0.2.4/src/otter_service.egg-info/PKG-INFO` & `otter_service-0.2.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: otter-service
-Version: 0.2.4
+Name: otter_service
+Version: 0.2.5
 Summary: Grading Service for Edx 8x courses
 Home-page: https://github.com/data-8/otter-service
 Author: Vincent Su and Sean Morris
 Author-email: sean.smorris@berkeley.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,16 +31,56 @@
     "course": "8x",
     "section": "1",
     "lab": "lab01"
     ...
 }
 ```
 
-## Course config path
-Please see the repository `data-8/materials-x22-private`. The repository houses a config file, 8x_course_config_edge.json and 8x_course_config.json. The system relies on this file specified in the environment variable, `COURSE_CONFIG_PATH`, to know which lab is associated with which assignment id in EdX. If you are not posting grades to an LTI server, than you do not need to worry about this.
+## Course Configuration
+Each course needs to provide two pieces of information that is deployed in the secrets file of
+this application
+1) A Github access key to the private materials repo.
+
+2) The name of repository where the autograder.zip files are kept. (e.g. github.com/data-8/materials-x22-private)
+
+Finally, the private repository with the autograder.zip files needs to contain a file named: course-config.json. The file is structured like this:
+
+(1) course name which matches the course name in every notebooks metadata<br>
+(2) section which matches the section in every notebooks metadata - if only one section put '1'<br>
+(3) Edx course id<br>
+(4) subpath to each autograder.zip in private autograder.zip repo<br>
+(5) each EDX assignment name and assignment Id -- the assignment name must match the notebook metadata
+
+```
+{
+  "8x" : { //(1)
+    "1": { //(2)
+      "course_id": "BerkeleyX+Data8.1x+3T2022", //(3)
+      "subpath_to_zips": "materials/x22/lab/1", //(4)
+      "assignments": {  //(5)
+        "lab01": "6333e19d6b4d46f88df671ba50f616d8",
+        "lab02": "fbf6740d45094b9b977111d218969273",
+        "lab03": "0c8f28bdc48d4231843f62b512d73638",
+        "lab04": "8db69daf14cf4751a088106be912c0cd",
+        "lab05": "4cb9e3491c284cd5ae29bb48219ee15b"
+      }
+    },
+    "2":{
+      "course_id": "BerkeleyX+Data8.2x+3T2022",
+      "subpath_to_zips": "materials/x22/lab/2",
+      "assignments": {
+        "lab01": "7abc0025c10f4b8ab123dbc88d34faaf",
+        ...
+```
+Here is an example of the folder structure in the materials-x22-private repo. 
+![Alt text](image.png)
+
+Note how the folder structure is mirrored in the course-config.json.
+
+If you are not posting grades to an LTI server, than you do not need to worry about this.
 
 
 ## Test files
 This gets tricky. The notebooks and the corresponding test files used by this service are of course connected. The files `Dockerfile` and `Dockerfile-dev` (used for local testing) download the current set of test files from the repository, `materials-x22-private`, for the `materials-x22` notebooks. If you bring in different notebooks, you would need to change the two dockerfiles to bring in the corresponding tests. 
 
 We assume a specific path to the test files. If you mirror the path found in the `materials-x22-private` repository, all will work well. If you change the path, then you must change the `solutions-path` variable in `grade_assignment.py`.
```

### Comparing `otter_service-0.2.4/src/otter_service.egg-info/SOURCES.txt` & `otter_service-0.2.5/src/otter_service.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.cfg
 src/otter_service/__init__.py
 src/otter_service/access_sops_keys.py
 src/otter_service/firestore-test.py
 src/otter_service/grade_assignment.py
 src/otter_service/otter_nb.py
+src/otter_service/util.py
 src/otter_service.egg-info/PKG-INFO
 src/otter_service.egg-info/SOURCES.txt
 src/otter_service.egg-info/dependency_links.txt
 src/otter_service.egg-info/entry_points.txt
 src/otter_service.egg-info/top_level.txt
 src/otter_service/secrets/gh_key.yaml
 src/otter_service/secrets/gke_key.yaml
```

### Comparing `otter_service-0.2.4/tests/test_access_sops_keys.py` & `otter_service-0.2.5/tests/test_access_sops_keys.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,25 @@
     if 'LTI_CONSUMER_KEY' in os.environ:
         del os.environ['LTI_CONSUMER_KEY']
 
 
 def test_get_sops():
     secrets_path = os.path.join(os.path.dirname(__file__), "test_files/test_key.yaml")
     sops_path = "sops"
-    key = ask.get_via_sops("LTI_CONSUMER_KEY", sops_path=sops_path, secrets_file=secrets_path)
+    key = ask.get_via_sops(None, "LTI_CONSUMER_KEY", sops_path=sops_path, secrets_file=secrets_path)
     assert "test_lti_key" in key
 
 
 def test_get_via_env(setup):
-    key = ask.get_via_env("LTI_CONSUMER_KEY")
+    key = ask.get_via_env(None, "LTI_CONSUMER_KEY")
     assert "TEST_ENV_KEY" in key
 
 
 def test_get(setup):
-    key = ask.get("LTI_CONSUMER_KEY")
+    key = ask.get(None, "LTI_CONSUMER_KEY")
     assert "TEST_ENV_KEY" in key
     del os.environ['LTI_CONSUMER_KEY']
     try:
         key = ask.get("LTI_CONSUMER_KEY")  # this should raise Exception
         assert False
     except Exception:
         assert True
```

### Comparing `otter_service-0.2.4/tests/test_grade_assignment.py` & `otter_service-0.2.5/tests/test_grade_assignment.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,25 +13,26 @@
     if os.path.isdir("./materials-x22-private"):
         shutil.rmtree("./materials-x22-private")
 
 
 def test_download_autograder_materials(configure):
     key_test = "tests/test_files/gh_key.yaml"
     sops_path = "sops"
-    git_access_token = ask.get_via_sops("github_access_token", sops_path=sops_path, secrets_file=key_test)
-    materials_url = f"https://{git_access_token}:@github.com/data-8/materials-x22-private/archive/main.tar.gz"
-    ga.download_autograder_materials(materials_url)
+    ga.download_autograder_materials("8x", sops_path, key_test)
     assert os.path.isdir("./materials-x22-private")
 
 
 @pytest.mark.asyncio
 async def test_grade_assignment(configure):
-    solutions_path = 'tests/test_files/autograder.zip'
     secrets_file = os.path.join(os.path.dirname(__file__), "test_files/gh_key.yaml")
+    args = {
+        "course": "8x",
+        "section": "1",
+        "assignment": "lab01",
+        "autograder_materials_repo": "github.com/data-8/materials-x22-private"
+    }
     grade = await ga.grade_assignment("tests/test_files/lab01.ipynb",
-                                      "1",
-                                      "lab01",
-                                      solutions_path=solutions_path,
+                                      args,
                                       sops_path="sops",
                                       secrets_file=secrets_file,
                                       save_path=".")
     assert 1.0 == grade
```

### Comparing `otter_service-0.2.4/tests/test_otter_nb.py` & `otter_service-0.2.5/tests/test_otter_nb.py`

 * *Files identical despite different names*

