# Comparing `tmp/citsci_notebook_core_pipeline-0.0.2.tar.gz` & `tmp/citsci_notebook_core_pipeline-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citsci_notebook_core_pipeline-0.0.2.tar", last modified: Wed Jul 26 17:47:11 2023, max compression
+gzip compressed data, was "citsci_notebook_core_pipeline-0.0.3.tar", last modified: Wed Jul 26 18:17:13 2023, max compression
```

## Comparing `citsci_notebook_core_pipeline-0.0.2.tar` & `citsci_notebook_core_pipeline-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-26 17:47:11.510020 citsci_notebook_core_pipeline-0.0.2/
--rw-r--r--   0 erosas     (503) staff       (20)    16157 2023-07-24 23:31:17.000000 citsci_notebook_core_pipeline-0.0.2/LICENSE
--rw-r--r--   0 erosas     (503) staff       (20)       95 2023-07-26 17:47:11.509850 citsci_notebook_core_pipeline-0.0.2/PKG-INFO
--rw-r--r--   0 erosas     (503) staff       (20)      225 2023-07-24 21:08:04.000000 citsci_notebook_core_pipeline-0.0.2/README.md
--rw-r--r--   0 erosas     (503) staff       (20)      218 2023-07-26 17:46:43.000000 citsci_notebook_core_pipeline-0.0.2/pyproject.toml
--rw-r--r--   0 erosas     (503) staff       (20)       38 2023-07-26 17:47:11.510067 citsci_notebook_core_pipeline-0.0.2/setup.cfg
-drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-26 17:47:11.507393 citsci_notebook_core_pipeline-0.0.2/src/
-drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-26 17:47:11.508607 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline/
--rw-r--r--   0 erosas     (503) staff       (20)        0 2023-07-24 21:15:11.000000 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline/__init__.py
--rw-r--r--   0 erosas     (503) staff       (20)    11724 2023-07-26 17:36:26.000000 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline/rubin_citsci_core_pipeline.py
-drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-26 17:47:11.509644 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline.egg-info/
--rw-r--r--   0 erosas     (503) staff       (20)       95 2023-07-26 17:47:11.000000 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 erosas     (503) staff       (20)      426 2023-07-26 17:47:11.000000 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 erosas     (503) staff       (20)        1 2023-07-26 17:47:11.000000 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 erosas     (503) staff       (20)       37 2023-07-26 17:47:11.000000 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline.egg-info/requires.txt
--rw-r--r--   0 erosas     (503) staff       (20)       30 2023-07-26 17:47:11.000000 citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-26 18:17:13.620941 citsci_notebook_core_pipeline-0.0.3/
+-rw-r--r--   0 erosas     (503) staff       (20)    16157 2023-07-24 23:31:17.000000 citsci_notebook_core_pipeline-0.0.3/LICENSE
+-rw-r--r--   0 erosas     (503) staff       (20)       95 2023-07-26 18:17:13.620767 citsci_notebook_core_pipeline-0.0.3/PKG-INFO
+-rw-r--r--   0 erosas     (503) staff       (20)      225 2023-07-24 21:08:04.000000 citsci_notebook_core_pipeline-0.0.3/README.md
+-rw-r--r--   0 erosas     (503) staff       (20)      218 2023-07-26 18:16:16.000000 citsci_notebook_core_pipeline-0.0.3/pyproject.toml
+-rw-r--r--   0 erosas     (503) staff       (20)       38 2023-07-26 18:17:13.620989 citsci_notebook_core_pipeline-0.0.3/setup.cfg
+drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-26 18:17:13.618633 citsci_notebook_core_pipeline-0.0.3/src/
+drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-26 18:17:13.619826 citsci_notebook_core_pipeline-0.0.3/src/citsci_notebook_core_pipeline/
+-rw-r--r--   0 erosas     (503) staff       (20)        0 2023-07-24 21:15:11.000000 citsci_notebook_core_pipeline-0.0.3/src/citsci_notebook_core_pipeline/__init__.py
+-rw-r--r--   0 erosas     (503) staff       (20)    11728 2023-07-26 18:16:04.000000 citsci_notebook_core_pipeline-0.0.3/src/citsci_notebook_core_pipeline/rubin_citsci_core_pipeline.py
+drwxr-xr-x   0 erosas     (503) staff       (20)        0 2023-07-26 18:17:13.620597 citsci_notebook_core_pipeline-0.0.3/src/citsci_notebook_core_pipeline.egg-info/
+-rw-r--r--   0 erosas     (503) staff       (20)       95 2023-07-26 18:17:13.000000 citsci_notebook_core_pipeline-0.0.3/src/citsci_notebook_core_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 erosas     (503) staff       (20)      426 2023-07-26 18:17:13.000000 citsci_notebook_core_pipeline-0.0.3/src/citsci_notebook_core_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 erosas     (503) staff       (20)        1 2023-07-26 18:17:13.000000 citsci_notebook_core_pipeline-0.0.3/src/citsci_notebook_core_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 erosas     (503) staff       (20)       37 2023-07-26 18:17:13.000000 citsci_notebook_core_pipeline-0.0.3/src/citsci_notebook_core_pipeline.egg-info/requires.txt
+-rw-r--r--   0 erosas     (503) staff       (20)       30 2023-07-26 18:17:13.000000 citsci_notebook_core_pipeline-0.0.3/src/citsci_notebook_core_pipeline.egg-info/top_level.txt
```

### Comparing `citsci_notebook_core_pipeline-0.0.2/LICENSE` & `citsci_notebook_core_pipeline-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `citsci_notebook_core_pipeline-0.0.2/src/citsci_notebook_core_pipeline/rubin_citsci_core_pipeline.py` & `citsci_notebook_core_pipeline-0.0.3/src/citsci_notebook_core_pipeline/rubin_citsci_core_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         self.create_new_subject_set(subject_set_name)
 
         self.edc_response = self.alert_edc_of_new_citsci_data()
         
         self.process_edc_response()
         return
     
-    def get_gcp_location():
+    def get_gcp_location(self):
         return base64.b64decode("L29wdC9sc3N0L3NvZnR3YXJlL2p1cHl0ZXJsYWIvc2VjcmV0cy9idXRsZXItZ2NzLWlkZi1jcmVkcy5qc29u").decode("ascii")
             
     def process_edc_response(self):
         if(self.edc_response == None):
             self.edc_response = { "status": "error", "messages": "An error occurred while processing the data transfer process upload" }
         else:                      
             self.edc_response = json.loads(self.edc_response)
```

