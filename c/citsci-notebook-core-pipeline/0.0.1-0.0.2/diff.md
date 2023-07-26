# Comparing `tmp/citsci_notebook_core_pipeline-0.0.1.tar.gz` & `tmp/citsci_notebook_core_pipeline-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citsci_notebook_core_pipeline-0.0.1.tar", last modified: Tue Jul 25 22:34:09 2023, max compression
+gzip compressed data, was "citsci_notebook_core_pipeline-0.0.2.tar", last modified: Wed Jul 26 17:47:11 2023, max compression
```

## Comparing `citsci_notebook_core_pipeline-0.0.1.tar` & `citsci_notebook_core_pipeline-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-25 22:34:09.554911 citsci_notebook_core_pipeline-0.0.1/
--rw-r--r--   0 erosas     (503) staff       (20)    16157 2023-07-24 23:31:17.000000 citsci_notebook_core_pipeline-0.0.1/LICENSE
--rw-r--r--   0 erosas     (503) staff       (20)       95 2023-07-25 22:34:09.554736 citsci_notebook_core_pipeline-0.0.1/PKG-INFO
--rw-r--r--   0 erosas     (503) staff       (20)      225 2023-07-24 21:08:04.000000 citsci_notebook_core_pipeline-0.0.1/README.md
--rw-r--r--   0 erosas     (503) staff       (20)      218 2023-07-25 22:31:44.000000 citsci_notebook_core_pipeline-0.0.1/pyproject.toml
--rw-r--r--   0 erosas     (503) staff       (20)       38 2023-07-25 22:34:09.554960 citsci_notebook_core_pipeline-0.0.1/setup.cfg
-drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-25 22:34:09.551427 citsci_notebook_core_pipeline-0.0.1/src/
-drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-25 22:34:09.552782 citsci_notebook_core_pipeline-0.0.1/src/citsci_notebook_core_pipeline/
--rw-r--r--   0 erosas     (503) staff       (20)        0 2023-07-24 21:15:11.000000 citsci_notebook_core_pipeline-0.0.1/src/citsci_notebook_core_pipeline/__init__.py
--rw-r--r--   0 erosas     (503) staff       (20)    11551 2023-07-25 22:31:29.000000 citsci_notebook_core_pipeline-0.0.1/src/citsci_notebook_core_pipeline/rubin_citsci_core_pipeline.py
-drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-25 22:34:09.554525 citsci_notebook_core_pipeline-0.0.1/src/citsci_notebook_core_pipeline.egg-info/
--rw-r--r--   0 erosas     (503) staff       (20)       95 2023-07-25 22:34:09.000000 citsci_notebook_core_pipeline-0.0.1/src/citsci_notebook_core_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 erosas     (503) staff       (20)      426 2023-07-25 22:34:09.000000 citsci_notebook_core_pipeline-0.0.1/src/citsci_notebook_core_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 erosas     (503) staff       (20)        1 2023-07-25 22:34:09.000000 citsci_notebook_core_pipeline-0.0.1/src/citsci_notebook_core_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 erosas     (503) staff       (20)       37 2023-07-25 22:34:09.000000 citsci_notebook_core_pipeline-0.0.1/src/citsci_notebook_core_pipeline.egg-info/requires.txt
--rw-r--r--   0 erosas     (503) staff       (20)       30 2023-07-25 22:34:09.000000 citsci_notebook_core_pipeline-0.0.1/src/citsci_notebook_core_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-26 17:47:11.510020 citsci_notebook_core_pipeline-0.0.2/
+-rw-r--r--   0 erosas     (503) staff       (20)    16157 2023-07-24 23:31:17.000000 citsci_notebook_core_pipeline-0.0.2/LICENSE
+-rw-r--r--   0 erosas     (503) staff       (20)       95 2023-07-26 17:47:11.509850 citsci_notebook_core_pipeline-0.0.2/PKG-INFO
+-rw-r--r--   0 erosas     (503) staff       (20)      225 2023-07-24 21:08:04.000000 citsci_notebook_core_pipeline-0.0.2/README.md
+-rw-r--r--   0 erosas     (503) staff       (20)      218 2023-07-26 17:46:43.000000 citsci_notebook_core_pipeline-0.0.2/pyproject.toml
+-rw-r--r--   0 erosas     (503) staff       (20)       38 2023-07-26 17:47:11.510067 citsci_notebook_core_pipeline-0.0.2/setup.cfg
+drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-26 17:47:11.507393 citsci_notebook_core_pipeline-0.0.2/src/
+drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-26 17:47:11.508607 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline/
+-rw-r--r--   0 erosas     (503) staff       (20)        0 2023-07-24 21:15:11.000000 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline/__init__.py
+-rw-r--r--   0 erosas     (503) staff       (20)    11724 2023-07-26 17:36:26.000000 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline/rubin_citsci_core_pipeline.py
+drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-26 17:47:11.509644 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline.egg-info/
+-rw-r--r--   0 erosas     (503) staff       (20)       95 2023-07-26 17:47:11.000000 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 erosas     (503) staff       (20)      426 2023-07-26 17:47:11.000000 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 erosas     (503) staff       (20)        1 2023-07-26 17:47:11.000000 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 erosas     (503) staff       (20)       37 2023-07-26 17:47:11.000000 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline.egg-info/requires.txt
+-rw-r--r--   0 erosas     (503) staff       (20)       30 2023-07-26 17:47:11.000000 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline.egg-info/top_level.txt
```

### Comparing `citsci_notebook_core_pipeline-0.0.1/LICENSE` & `citsci_notebook_core_pipeline-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `citsci_notebook_core_pipeline-0.0.1/src/citsci_notebook_core_pipeline/rubin_citsci_core_pipeline.py` & `citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline/rubin_citsci_core_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 # version 4 of the License, or (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # Creative Commons NC-ND License for more details.
 
-import csv, uuid, os, shutil, json, logging, urllib.request
+import csv, uuid, os, shutil, json, logging, urllib.request, base64
 from datetime import datetime, timezone, timedelta
 from IPython.display import display
 import google.cloud.storage as storage
 import panoptes_client
 from panoptes_client import Project, SubjectSet, Classification
 
 class CitSciPipeline:
     
     def __init__(self):
-        os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = "/opt/lsst/software/jupyterlab/butler-secret/butler-gcs-idf-creds.json"
+        os.environ[base64.b64decode("R09PR0xFX0FQUExJQ0FUSU9OX0NSRURFTlRJQUxT").decode("ascii")] = self.get_gcp_location()
         self.vendor_batch_id = 0
         self.project_id = -1
         self.guid = ""
         self.manifest_url = ""
         self.edc_response = ""
         self.step = 0
         self.email = ""
@@ -144,14 +144,17 @@
         self.upload_cutouts(zip_path)
         self.create_new_subject_set(subject_set_name)
 
         self.edc_response = self.alert_edc_of_new_citsci_data()
         
         self.process_edc_response()
         return
+    
+    def get_gcp_location():
+        return base64.b64decode("L29wdC9sc3N0L3NvZnR3YXJlL2p1cHl0ZXJsYWIvc2VjcmV0cy9idXRsZXItZ2NzLWlkZi1jcmVkcy5qc29u").decode("ascii")
             
     def process_edc_response(self):
         if(self.edc_response == None):
             self.edc_response = { "status": "error", "messages": "An error occurred while processing the data transfer process upload" }
         else:                      
             self.edc_response = json.loads(self.edc_response)
         if self.edc_response["status"] == "success":
```

