# Comparing `tmp/flywheel_bids-1.2.4-py3-none-any.whl.zip` & `tmp/flywheel_bids-1.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 106036 bytes, number of entries: 54
+Zip file size: 106094 bytes, number of entries: 54
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 flywheel_bids/__init__.py
--rw-r--r--  2.0 unx    23112 b- defN 80-Jan-01 00:00 flywheel_bids/curate_bids.py
+-rw-r--r--  2.0 unx    23597 b- defN 80-Jan-01 00:00 flywheel_bids/curate_bids.py
 -rw-r--r--  2.0 unx    23741 b- defN 80-Jan-01 00:00 flywheel_bids/export_bids.py
 -rw-r--r--  2.0 unx       76 b- defN 80-Jan-01 00:00 flywheel_bids/results/__init__.py
 -rw-r--r--  2.0 unx     2361 b- defN 80-Jan-01 00:00 flywheel_bids/results/zip_htmls.py
 -rw-r--r--  2.0 unx     5147 b- defN 80-Jan-01 00:00 flywheel_bids/results/zip_intermediate.py
 -rw-r--r--  2.0 unx        5 b- defN 80-Jan-01 00:00 flywheel_bids/supporting_files/__init__.py
 -rw-r--r--  2.0 unx    10537 b- defN 80-Jan-01 00:00 flywheel_bids/supporting_files/bidsify_flywheel.py
 -rw-r--r--  2.0 unx     4353 b- defN 80-Jan-01 00:00 flywheel_bids/supporting_files/classifications.py
@@ -45,12 +45,12 @@
 -rw-r--r--  2.0 unx    44997 b- defN 80-Jan-01 00:00 flywheel_bids/templates/reproin.json
 -rw-r--r--  2.0 unx    63150 b- defN 80-Jan-01 00:00 flywheel_bids/upload_bids.py
 -rw-r--r--  2.0 unx    13998 b- defN 80-Jan-01 00:00 flywheel_bids/utils/download_run_level.py
 -rw-r--r--  2.0 unx     2026 b- defN 80-Jan-01 00:00 flywheel_bids/utils/performance.py
 -rw-r--r--  2.0 unx     1816 b- defN 80-Jan-01 00:00 flywheel_bids/utils/run_level.py
 -rw-r--r--  2.0 unx     2522 b- defN 80-Jan-01 00:00 flywheel_bids/utils/tree.py
 -rw-r--r--  2.0 unx     5898 b- defN 80-Jan-01 00:00 flywheel_bids/utils/validate.py
--rw-r--r--  2.0 unx     5627 b- defN 80-Jan-01 00:00 flywheel_bids-1.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 flywheel_bids-1.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 flywheel_bids-1.2.4.dist-info/LICENSE
-?rw-r--r--  2.0 unx     6263 b- defN 16-Jan-01 00:00 flywheel_bids-1.2.4.dist-info/RECORD
-54 files, 548116 bytes uncompressed, 95414 bytes compressed:  82.6%
+-rw-r--r--  2.0 unx     5627 b- defN 80-Jan-01 00:00 flywheel_bids-1.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 flywheel_bids-1.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 flywheel_bids-1.2.5.dist-info/LICENSE
+?rw-r--r--  2.0 unx     6263 b- defN 16-Jan-01 00:00 flywheel_bids-1.2.5.dist-info/RECORD
+54 files, 548601 bytes uncompressed, 95472 bytes compressed:  82.6%
```

## zipnote {}

```diff
@@ -144,20 +144,20 @@
 
 Filename: flywheel_bids/utils/tree.py
 Comment: 
 
 Filename: flywheel_bids/utils/validate.py
 Comment: 
 
-Filename: flywheel_bids-1.2.4.dist-info/METADATA
+Filename: flywheel_bids-1.2.5.dist-info/METADATA
 Comment: 
 
-Filename: flywheel_bids-1.2.4.dist-info/WHEEL
+Filename: flywheel_bids-1.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: flywheel_bids-1.2.4.dist-info/LICENSE
+Filename: flywheel_bids-1.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: flywheel_bids-1.2.4.dist-info/RECORD
+Filename: flywheel_bids-1.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flywheel_bids/curate_bids.py

```diff
@@ -193,44 +193,53 @@
     def __init__(self):
         self.containers = 0  # counts project, sessions and acquisitions
         self.sessions = 0
         self.acquisitions = 0
         self.files = 0
 
 
-def save_project_sidecar(project, project_node):
+def save_project_sidecar(project, project_node, save_sidecar_as_metadata):
     """Save "dataset_description.json" sidecar file
 
-    Remove info that was just put on the project_node and attach it as a file
+    Remove info that was just put on the project_node and attach it as a json file
     on the project if it does not yet exist.
 
     Args:
         project (Project container)
         project_node (TreeNode) a "context" representation of the project
+        save_sidecar_as_metadata (bool): if true, save sidecar data as metadata also
     """
 
     SIDECAR_NAME = "dataset_description.json"
     proj_sidecars = [file for file in project.files if file.name == SIDECAR_NAME]
 
     if len(proj_sidecars) > 1:
         logger.debug("ERROR: multiple '%s' files exist", SIDECAR_NAME)
     elif len(proj_sidecars) == 1:
         logger.info("'%s' file already exists", SIDECAR_NAME)
     else:  # create and attach file to project
         logger.info("'%s' file does not exist, creating it...", SIDECAR_NAME)
-        json_data = project_node.data["info"]["BIDS"]
-        template_val = json_data.pop("template")
-        rule_id_val = json_data.pop("rule_id")
-        json_str = json.dumps(json_data, indent=4)
-        file_spec = flywheel.FileSpec(SIDECAR_NAME, json_str, "text/plain")
-        project.upload_file(file_spec)
-        project_node.data["info"]["BIDS"] = {
-            "template": template_val,
-            "rule_id": rule_id_val,
-        }
+        if "info" in project_node:
+            if "BIDS" in project_node.data["info"]:
+                json_data = project_node.data["info"]["BIDS"]
+                if "template" in json_data:
+                    del json_data["template"]
+                if "rule_id" in json_data:
+                    del json_data["rule_id"]
+                json_str = json.dumps(json_data, indent=4)
+                file_spec = flywheel.FileSpec(SIDECAR_NAME, json_str, "text/plain")
+                project.upload_file(file_spec)
+
+                if not save_sidecar_as_metadata:  # remove BIDS namespace
+                    del project_node.data["info"]["BIDS"]
+                # else: that BIDS info will be updated in project metadata
+            else:
+                logger.debug("ERROR: no BIDS information exists")
+        else:
+            logger.debug("ERROR: no project.info exists")
 
 
 def curate_bids(
     fw,
     project_id,
     subject_id="",
     session_id="",
@@ -288,16 +297,15 @@
         project_node,
         count,
         reset=reset,
         dont_recurate_project=dont_recurate_project,
         dry_run=dry_run,
     )
 
-    if not save_sidecar_as_metadata:  # then (default) save project metadata as sidecar
-        save_project_sidecar(project, project_node)
+    save_project_sidecar(project, project_node, save_sidecar_as_metadata)
 
     if session_id:
         logger.info("Getting single session ID=%s", session_id)
         session = fw.get_session(session_id)
         subject_id = session.subject.id
 
     if subject_id:
```

## Comparing `flywheel_bids-1.2.4.dist-info/METADATA` & `flywheel_bids-1.2.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flywheel-bids
-Version: 1.2.4
+Version: 1.2.5
 Summary: Flywheel BIDS Client
 Home-page: https://gitlab.com/flywheel-io/public/bids-client
 License: MIT
 Keywords: Flywheel,flywheel,BIDS,SDK
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
```

## Comparing `flywheel_bids-1.2.4.dist-info/LICENSE` & `flywheel_bids-1.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `flywheel_bids-1.2.4.dist-info/RECORD` & `flywheel_bids-1.2.5.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 flywheel_bids/__init__.py,sha256=Y4xogqvLXa5sAUBRzU_qrcOE145CqsQhbeTjpwPmX1E,5
-flywheel_bids/curate_bids.py,sha256=4mySzrV43am7bz88Fd36XBQPCzFc2YCAXK_JOhDmHC0,23112
+flywheel_bids/curate_bids.py,sha256=JMXXGc4x5HIUhT_KUoejc-kT-fK5SRbhap-Xf7bOIfI,23597
 flywheel_bids/export_bids.py,sha256=Oa4eQ6Flu61m2DrfaAtnMmUuqpjkjn7W6fnbHHMLPiY,23741
 flywheel_bids/results/__init__.py,sha256=enUMUGNyNRTT1jGvzqiPUAO0b7akF5ybOwmdvELPIbU,76
 flywheel_bids/results/zip_htmls.py,sha256=LcntrHonTlUerhwxZ1SlG--5JMHeIvh1d0dvd2tOUfY,2361
 flywheel_bids/results/zip_intermediate.py,sha256=DZmSBnkj_YdpRKfZC13MimwjGjwclWDXF06uv3uMS9c,5147
 flywheel_bids/supporting_files/__init__.py,sha256=Y4xogqvLXa5sAUBRzU_qrcOE145CqsQhbeTjpwPmX1E,5
 flywheel_bids/supporting_files/bidsify_flywheel.py,sha256=_JAy7mZOM5BrMl-TMvSs7gnr-lrkfCzI33yo8EvMoH4,10537
 flywheel_bids/supporting_files/classifications.py,sha256=uisUcFW-36Zq4uXFnd-sI1Q93E9E6zgeBqipeF0AdtA,4353
@@ -44,11 +44,11 @@
 flywheel_bids/templates/reproin.json,sha256=j9FxrVe3k6wqF4Kgice7FPnMDzdoDnVhkVD3FV0ylgU,44997
 flywheel_bids/upload_bids.py,sha256=Z8NkWpmTtOYGJkXx2gCWvvmkJ51X8DPnMIpIjgnodQ0,63150
 flywheel_bids/utils/download_run_level.py,sha256=NssyGcOzVURfagXgzryQHLA9YZFA3PzwI7EyuQUyVLU,13998
 flywheel_bids/utils/performance.py,sha256=rcC3DyvpdJO1k18vyFlK93OhazPctBwABb6qA4kNEMo,2026
 flywheel_bids/utils/run_level.py,sha256=FL_ChyzCECoUS7HrdRjWCEnE6e78wIA5ePKjQ4PiT2c,1816
 flywheel_bids/utils/tree.py,sha256=6bfQmkp1iqwk9RrIXxrMHMldwe9ALbvL81RA5NIqXn0,2522
 flywheel_bids/utils/validate.py,sha256=noMFXBD7_k8wioxhSIiw7JNzExiyPcS3DyBbpWUiaww,5898
-flywheel_bids-1.2.4.dist-info/METADATA,sha256=TVc2uOBEcDVC0ygoI7aN2uOWtz1lEicrS4MGyZ2NsAo,5627
-flywheel_bids-1.2.4.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-flywheel_bids-1.2.4.dist-info/LICENSE,sha256=dqr2l_pCmH5B2MnrF0BMMugS_MmWV4bPLqF9aHWn4Tk,1066
-flywheel_bids-1.2.4.dist-info/RECORD,,
+flywheel_bids-1.2.5.dist-info/METADATA,sha256=tLgTer049kFKNlsPV25NV6lA31vfCB0ipGmjPE26loc,5627
+flywheel_bids-1.2.5.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+flywheel_bids-1.2.5.dist-info/LICENSE,sha256=dqr2l_pCmH5B2MnrF0BMMugS_MmWV4bPLqF9aHWn4Tk,1066
+flywheel_bids-1.2.5.dist-info/RECORD,,
```

