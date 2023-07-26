# Comparing `tmp/datature-1.1.0.tar.gz` & `tmp/datature-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Puppeteer/Puppeteer/pypi/puppeteer/dist/.tmp-67kkp98n/datature-1.1.0.tar", last modified: Tue Jun  6 07:05:53 2023, max compression
+gzip compressed data, was "/home/runner/work/Puppeteer/Puppeteer/pypi/puppeteer/dist/.tmp-9uj1awqt/datature-1.1.1.tar", last modified: Wed Jul 26 05:15:23 2023, max compression
```

## Comparing `datature-1.1.0.tar` & `datature-1.1.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-06-06 07:05:39.000000 datature-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-06 07:05:39.000000 datature-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-06 07:05:53.000000 datature-1.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-06 07:05:39.000000 datature-1.1.0/datature/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/datature/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-06-06 07:05:39.000000 datature-1.1.0/datature/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-06 07:05:39.000000 datature-1.1.0/datature/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-06-06 07:05:39.000000 datature-1.1.0/datature/cli/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-06 07:05:39.000000 datature-1.1.0/datature/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-06 07:05:39.000000 datature-1.1.0/datature/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/datature/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-06 07:05:39.000000 datature-1.1.0/datature/http/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-06 07:05:39.000000 datature-1.1.0/datature/http/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-06 07:05:39.000000 datature-1.1.0/datature/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-06 07:05:39.000000 datature-1.1.0/datature/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-06 07:05:39.000000 datature-1.1.0/datature/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-06 07:05:39.000000 datature-1.1.0/datature/processor/base_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-06 07:05:39.000000 datature-1.1.0/datature/processor/dicom_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-06-06 07:05:39.000000 datature-1.1.0/datature/processor/nii_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature/rest/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/asset/__int__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/asset/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/asset/upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    14873 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-06 07:05:39.000000 datature-1.1.0/datature/rest/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/datature/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-06 07:05:39.000000 datature-1.1.0/datature/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/datature.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-06 07:05:53.000000 datature-1.1.0/datature.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-06 07:05:53.000000 datature-1.1.0/datature.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 07:05:53.000000 datature-1.1.0/datature.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 07:05:53.000000 datature-1.1.0/datature.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-06 07:05:53.000000 datature-1.1.0/datature.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-06 07:05:53.000000 datature-1.1.0/datature.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-06 07:05:39.000000 datature-1.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-06 07:05:39.000000 datature-1.1.0/docs/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-06 07:05:39.000000 datature-1.1.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 07:05:53.000000 datature-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-06 07:05:39.000000 datature-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/test/fixture/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/test/fixture/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/test/fixture/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/test/fixture/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-06 07:05:39.000000 datature-1.1.0/test/fixture/data/error_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-06 07:05:39.000000 datature-1.1.0/test/fixture/data/operation_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-06 07:05:39.000000 datature-1.1.0/test/fixture/data/upload_session_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-06 07:05:39.000000 datature-1.1.0/test/fixture/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/test/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/test/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-06 07:05:39.000000 datature-1.1.0/test/http/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-06 07:05:39.000000 datature-1.1.0/test/http/test_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:53.000000 datature-1.1.0/test/rest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_asset_upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-06 07:05:39.000000 datature-1.1.0/test/rest/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-06 07:05:39.000000 datature-1.1.0/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-06 07:05:39.000000 datature-1.1.0/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-07-26 05:15:08.000000 datature-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 05:15:08.000000 datature-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-26 05:15:23.000000 datature-1.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/datature/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 05:15:08.000000 datature-1.1.1/datature/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/datature/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:08.000000 datature-1.1.1/datature/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-07-26 05:15:08.000000 datature-1.1.1/datature/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-26 05:15:08.000000 datature-1.1.1/datature/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-07-26 05:15:08.000000 datature-1.1.1/datature/cli/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-26 05:15:08.000000 datature-1.1.1/datature/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-26 05:15:08.000000 datature-1.1.1/datature/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/datature/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:08.000000 datature-1.1.1/datature/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-26 05:15:08.000000 datature-1.1.1/datature/http/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-26 05:15:08.000000 datature-1.1.1/datature/http/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-26 05:15:08.000000 datature-1.1.1/datature/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-26 05:15:08.000000 datature-1.1.1/datature/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/datature/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-26 05:15:08.000000 datature-1.1.1/datature/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-26 05:15:08.000000 datature-1.1.1/datature/processor/base_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-26 05:15:08.000000 datature-1.1.1/datature/processor/dicom_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-26 05:15:08.000000 datature-1.1.1/datature/processor/nii_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/datature/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-26 05:15:08.000000 datature-1.1.1/datature/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15290 2023-07-26 05:15:08.000000 datature-1.1.1/datature/rest/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-07-26 05:15:08.000000 datature-1.1.1/datature/rest/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/datature/rest/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:08.000000 datature-1.1.1/datature/rest/asset/__int__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-07-26 05:15:08.000000 datature-1.1.1/datature/rest/asset/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-07-26 05:15:08.000000 datature-1.1.1/datature/rest/asset/upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-07-26 05:15:08.000000 datature-1.1.1/datature/rest/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-26 05:15:08.000000 datature-1.1.1/datature/rest/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-07-26 05:15:08.000000 datature-1.1.1/datature/rest/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-26 05:15:08.000000 datature-1.1.1/datature/rest/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-26 05:15:08.000000 datature-1.1.1/datature/rest/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-07-26 05:15:08.000000 datature-1.1.1/datature/rest/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-26 05:15:08.000000 datature-1.1.1/datature/rest/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/datature/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:08.000000 datature-1.1.1/datature/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-26 05:15:08.000000 datature-1.1.1/datature/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/datature.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-26 05:15:23.000000 datature-1.1.1/datature.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-26 05:15:23.000000 datature-1.1.1/datature.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 05:15:23.000000 datature-1.1.1/datature.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-26 05:15:23.000000 datature-1.1.1/datature.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-26 05:15:23.000000 datature-1.1.1/datature.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-26 05:15:23.000000 datature-1.1.1/datature.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-26 05:15:08.000000 datature-1.1.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-26 05:15:08.000000 datature-1.1.1/docs/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-26 05:15:08.000000 datature-1.1.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 05:15:23.000000 datature-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-26 05:15:08.000000 datature-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:08.000000 datature-1.1.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/test/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:08.000000 datature-1.1.1/test/fixture/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/test/fixture/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:08.000000 datature-1.1.1/test/fixture/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-26 05:15:08.000000 datature-1.1.1/test/fixture/data/error_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-26 05:15:08.000000 datature-1.1.1/test/fixture/data/operation_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-26 05:15:08.000000 datature-1.1.1/test/fixture/data/upload_session_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-26 05:15:08.000000 datature-1.1.1/test/fixture/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/test/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:08.000000 datature-1.1.1/test/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-26 05:15:08.000000 datature-1.1.1/test/http/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-26 05:15:08.000000 datature-1.1.1/test/http/test_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:23.000000 datature-1.1.1/test/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:15:08.000000 datature-1.1.1/test/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-26 05:15:08.000000 datature-1.1.1/test/rest/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-26 05:15:08.000000 datature-1.1.1/test/rest/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-26 05:15:08.000000 datature-1.1.1/test/rest/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-07-26 05:15:08.000000 datature-1.1.1/test/rest/test_asset_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-26 05:15:08.000000 datature-1.1.1/test/rest/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-26 05:15:08.000000 datature-1.1.1/test/rest/test_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-26 05:15:08.000000 datature-1.1.1/test/rest/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-26 05:15:08.000000 datature-1.1.1/test/rest/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-26 05:15:08.000000 datature-1.1.1/test/rest/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-26 05:15:08.000000 datature-1.1.1/test/rest/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-26 05:15:08.000000 datature-1.1.1/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-26 05:15:08.000000 datature-1.1.1/test/test_logger.py
```

### Comparing `datature-1.1.0/LICENSE` & `datature-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/PKG-INFO` & `datature-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datature
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python bindings for the Datature API
 Author: Raighne Weng
 Author-email: raighne@datature.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `datature-1.1.0/datature/__init__.py` & `datature-1.1.1/datature/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   init module, include global configuration
 '''
 
 # Global Configuration
 API_BASE_URL = "https://api.datature.io/v1"
-SDK_VERSION = "1.1.0"
+SDK_VERSION = "1.1.1"
 
 # Constant environment
 OPERATION_LOOPING_TIMES = 20
 ASSET_UPLOAD_BATCH_SIZE = 5000
 SHOW_PROGRESS = False
 OPERATION_LOOPING_DELAY_SECONDS = 5
 HTTP_TIMEOUT_SECONDS = 120
```

### Comparing `datature-1.1.0/datature/cli/commands.py` & `datature-1.1.1/datature/cli/commands.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/datature/cli/config.py` & `datature-1.1.1/datature/cli/config.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/datature/cli/functions.py` & `datature-1.1.1/datature/cli/functions.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/datature/cli/main.py` & `datature-1.1.1/datature/cli/main.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/datature/error.py` & `datature-1.1.1/datature/error.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/datature/http/requester.py` & `datature-1.1.1/datature/http/requester.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/datature/http/resource.py` & `datature-1.1.1/datature/http/resource.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/datature/logger.py` & `datature-1.1.1/datature/logger.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/datature/messages.py` & `datature-1.1.1/datature/messages.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/datature/processor/__init__.py` & `datature-1.1.1/datature/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/datature/processor/base_processor.py` & `datature-1.1.1/datature/processor/base_processor.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/datature/processor/dicom_processor.py` & `datature-1.1.1/datature/processor/dicom_processor.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/datature/processor/nii_processor.py` & `datature-1.1.1/datature/processor/nii_processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,24 @@
 @Author  :   Raighne.Weng
 @Version :   1.1.0
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Nii Processor
 '''
 
+import shutil
 import tempfile
 from typing import List
 from pathlib import Path
 from os import makedirs, path
 
 import cv2
 import numpy as np
 import nibabel as nib
+import matplotlib.image as mpImage
 from datature import error
 from datature.processor.base_processor import BaseProcessor
 
 
 # pylint: disable=R0914,E1101
 class NiiProcessor(BaseProcessor):
     """Nii processor class"""
@@ -68,54 +70,62 @@
         # Get image pixel
         scan_headers = scan.header
         pix_dim = scan_headers['pixdim'][1:4]
 
         # Calculate new image dimensions from aspect ratio
         new_scan_dims = np.multiply(scan_array.shape, pix_dim)
         new_scan_dims = (round(new_scan_dims[0]), round(new_scan_dims[1]),
-                     round(new_scan_dims[2]))
+                         round(new_scan_dims[2]))
 
         # if client provide the orientation
         if orientation and orientation in ["x", "y", "z"]:
             output_file_path = f"{video_output}/{file_name}-{orientation}.mp4"
 
-            self.__write_video(scan_array, orientation, output_file_path, new_scan_dims)
+            self.__write_video(scan_array, new_scan_dims, orientation,
+                               output_file_path)
 
             return [output_file_path]
 
         # if not then save all orientations
         output_file_paths = []
         for orientation in ["x", "y", "z"]:
             output_file_path = f"{video_output}/{file_name}-{orientation}.mp4"
 
-            self.__write_video(scan_array, orientation, output_file_path, new_scan_dims)
+            self.__write_video(scan_array, new_scan_dims, orientation,
+                               output_file_path)
 
             output_file_paths.append(output_file_path)
-
         return output_file_paths
 
-    def __write_video(self, scan_array, orientation, saved_path, scan_dims):
+    def __write_video(self, scan_array, scan_dims, orientation, saved_path):
         """Write video to file
 
         :param scan_array: The NIfTI scan array data.
+        :param scan_dims: The image dimensions of the file.
         :param axis: The orientation of the pics.
         :param saved_path: The saved file path.
-        :param scan_dims: The image dimensions of the file.
         """
         axis = {'x': 0, 'y': 1, 'z': 2}[orientation]
-        size = {'x': [scan_dims[2],scan_dims[1]],
-                'y': [scan_dims[2],scan_dims[0]],
-                'z': [scan_dims[1],scan_dims[0]]
+        size = {'x': [scan_dims[2], scan_dims[1]],
+                'y': [scan_dims[2], scan_dims[0]],
+                'z': [scan_dims[1], scan_dims[0]]
                 }[orientation]
 
         four_cc = cv2.VideoWriter_fourcc(*"mp4v")
-        video_writer = cv2.VideoWriter(saved_path, four_cc, 30.0, size)
+        video_writer = cv2.VideoWriter(
+            saved_path, four_cc, 30.0, size)
+
+        cache_path = tempfile.mkdtemp()
 
         for i in range(scan_array.shape[axis]):
             # Get slice along the correct axis and resize
             slice_axis = scan_array.take(i, axis=axis)
-            image = cv2.resize(slice_axis, size)
 
-            # Convert to RGB and write to video file
-            new_image = cv2.cvtColor(np.uint8(image), cv2.COLOR_GRAY2RGB)
+            # Convert to Grayscale and write to video file
+            mpImage.imsave(
+                f'{cache_path}/{orientation}-{str(i)}.png', slice_axis, cmap='gray')
+            new_image = cv2.imread(f'{cache_path}/{orientation}-{str(i)}.png')
+
+            new_image = cv2.resize(new_image, size)
             video_writer.write(new_image)
+        shutil.rmtree(cache_path)
         video_writer.release()
```

### Comparing `datature-1.1.0/datature/rest/__init__.py` & `datature-1.1.1/datature/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/datature/rest/annotation.py` & `datature-1.1.1/datature/rest/annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     def list(cls, asset_id: str) -> dict:
         """Lists all annotations of a specific asset.
 
         :param asset_id: The ID of the asset.
         :return: A list of dictionaries containing annotation metadata with the following structure:
 
                 .. code-block:: json
-                        [
+
+                         [
                             {
                                 "id": "annot_8188782f-a86b-4961-9e2a-697509085460",
                                 "object": "annotation",
                                 "bound_type": "rectangle",
                                 "bound": [
                                     [
                                         0.596875,
@@ -75,14 +76,15 @@
     def create(cls, annotation: AnnotationMetadata) -> dict:
         """Creates an annotation.
 
         :param annotation: The metadata of the annotation.
         :return: A dictionary containing the annotation metadata with the following structure:
 
                 .. code-block:: json
+
                          {
                             "id": "annot_8188782f-a86b-4961-9e2a-697509085460",
                             "object": "annotation",
                             "bound_type": "rectangle",
                             "bound": [
                                 [
                                     0.596875,
@@ -136,14 +138,15 @@
     def retrieve(cls, annotation_id: str) -> dict:
         """Retrieves a specific annotation using the annotation ID.
 
         :param annotation_id: The ID of the annotation.
         :return: A dictionary containing the specific annotation metadata with the following structure:
 
                 .. code-block:: json
+
                         {
                             "id": "annot_8188782f-a86b-4961-9e2a-697509085460",
                             "object": "annotation",
                             "bound_type": "rectangle",
                             "bound": [
                                 [
                                     0.596875,
@@ -181,14 +184,15 @@
     def delete(cls, annotation_id: str) -> dict:
         """Deletes a specific annotation from the project.
 
         :param annotation_id: The ID of the annotation.
         :return: A dictionary containing the deleted annotation ID and the deletion status with the following structure:
 
                 .. code-block:: json
+
                         {
                             "id": "annot_8188782f-a86b-4961-9e2a-697509085460",
                             "deleted": true
                         }
 
         :example:
                 .. code-block:: python
@@ -209,14 +213,15 @@
 
         :param annotation_format: The annotation format for bounding boxes or polygons as a string.
         :param export_options: A dictionary containing other export options.
         :param background: Signal to complete the annotation export process in the background. Defaults to False.
         :return: A dictionary containing the operation metadata of the annotation export with the following structure:
 
                 .. code-block:: json
+
                         {
                             "id": "op_508fc5d1-e908-486d-9e7b-1dca99b80024",
                             "object": "operation",
                             "op_link": "users/api|affaf/proje-1dca99b80024",
                             "status": {
                                 "overview": "Queued",
                                 "message": "Operation queued",
@@ -275,14 +280,15 @@
     def retrieve_exported_file(cls, op_id: str) -> dict:
         """Retrieves the download link of the exported annotations.
 
         :param op_id: The operation ID of the annotation export.
         :return: A dictionary with the download metadata of the annotation export with the following structure:
 
                 .. code-block:: json
+
                     {
                         "op_id": "op_cf8c538a-bcb5-49a9-82cf-fb0d13b49bb1",
                         "op_link": "users/afb0d13b49bb1",
                         "status": "Finished",
                         "download": {
                             "method": "GET",
                             "url": "https://storage.googleape7ab37588a6ce2f692351757f5967",
@@ -311,14 +317,15 @@
 
         :param annotation_format: The annotation format for bounding boxes or polygons as a string.
         :param file_path: The file path or folder containing the annotation metadata to be uploaded. The file contents should match the annotation format specified.
         :param background: Signal to complete the annotation upload process in the background. Defaults to False.
         :return: A dictionary containing the operation metadata of the annotation upload with the following structure:
 
                 .. code-block:: json
+
                         {
                             "id": "op_508fc5d1-e908-486d-9e7b-1dca99b80024",
                             "object": "operation",
                             "op_link": "users/api|affaf/proje-1dca99b80024",
                             "status": {
                                 "overview": "Queued",
                                 "message": "Operation queued",
```

### Comparing `datature-1.1.0/datature/rest/artifact.py` & `datature-1.1.1/datature/rest/artifact.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     @classmethod
     def list(cls) -> dict:
         """Lists all artifacts in the project.
 
         :return: A list of dictionaries containing the artifact metadata with the following structure:
 
                 .. code-block:: json
+
                         [
                             {
                                 "id": "artifact_63bd140e67b42dc9f431ffe2",
                                 "object": "artifact",
                                 "is_training": false,
                                 "step": 3000,
                                 "flow_title": "Blood Cell Detector",
@@ -70,14 +71,15 @@
     def retrieve(cls, artifact_id: str) -> dict:
         """Retrieves a specific artifact using the artifact ID.
 
         :param artifact_id: The ID of the artifact as a string.
         :return: A dictionary containing the specific artifact metadata with the following structure:
 
                 .. code-block:: json
+
                             {
                                 "id": "artifact_63bd140e67b42dc9f431ffe2",
                                 "object": "artifact",
                                 "is_training": false,
                                 "step": 3000,
                                 "flow_title": "Blood Cell Detector",
                                 "run_id": "run_63bd08d8cdf700575fa4dd01",
@@ -115,14 +117,15 @@
     def list_exported(cls, artifact_id: str) -> dict:
         """Lists all exported models of a specific artifact.
 
         :param artifact_id: The ID of the artifact as a string.
         :return: A list of dictionaries with the exported model metadata with the following structure:
 
                 .. code-block:: json
+
                         [
                             {
                                 "id": "model_d15aba68872b045e27ac3db06a401da3",
                                 "object": "model",
                                 "status": "Finished",
                                 "format": "tensorflow",
                                 "create_date": 1673336054173,
@@ -153,27 +156,28 @@
 
         :param artifact_id: The ID of the artifact as a string.
         :param model_format: The export format of the model.
 
         :return: A dictionary containing the operation metadata of the model export with the following structure:
 
                 .. code-block:: json
+
                             {
                                 "id": "model_d15aba68872b045e27ac3db06a401da3",
                                 "object": "model",
                                 "status": "Running",
                                 "format": "tensorflow",
                                 "create_date": 1673336054173,
                             }
 
         :example:
                 .. code-block:: python
 
                         import datature
 
                         datature.secret_key = "5aa41e8ba........"
-                        datature.Artifact.create_model(
+                        datature.Artifact.export_model(
                             "artifact_63bd140e67b42dc9f431ffe2", "tensorflow")
         """
         return cls.request("POST",
                            f"/artifact/{artifact_id}/export",
                            request_body={"format": model_format})
```

### Comparing `datature-1.1.0/datature/rest/asset/asset.py` & `datature-1.1.1/datature/rest/asset/asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     def list(cls, pagination: Pagination = None) -> dict:
         """Retrieves a list of all assets in the project.
 
         :param pagination: A dictionary containing the limit of the number of assets to be returned in each page (defaults to 10), and the page cursor for page selection (defaults to the first page).
         :return: A dictionary of asset metadata with the following structure:
 
                 .. code-block:: json
+
                         {
                             "prev_page": "YjYzYmJkM2FjN2UxOTA4ZmU0ZjE0Yjk5Mg",
                             "next_page": "ZjYzYmJkM2FjN2UxOTA4ZmU0ZjE0YjlhMw",
                             "data": [
                                 {
                                     "id": "asset_6aea3395-9a72-4bb5-9ee0-19248c903c56",
                                     "object": "asset",
@@ -82,14 +83,15 @@
     def retrieve(cls, asset_id_or_name: str) -> dict:
         """Retrieves a specific asset using the asset ID or file name.
 
         :param asset_id_or_name: The ID or file name of the asset as a string.
         :return: A dictionary containing the metadata of one asset with the following structure:
 
                 .. code-block:: json
+
                         {
                             "id": "asset_6aea3395-9a72-4bb5-9ee0-19248c903c56",
                             "object": "asset",
                             "filename": "17.jpg",
                             "project": "proj_cd067221d5a6e4007ccbb4afb5966535",
                             "create_date": 1673253803928,
                             "metadata": {
@@ -129,14 +131,15 @@
         """Updates the metadata of a specific asset.
 
         :param asset_id_or_name: The ID or file name of the asset as a string.
         :param asset_meta: The new metadata of the asset to be updated.
         :return: A dictionary of the updated asset metadata with the following structure:
 
                 .. code-block:: json
+
                         {
                             "id": "asset_6aea3395-9a72-4bb5-9ee0-19248c903c56",
                             "object": "asset",
                             "filename": "17.jpg",
                             "project": "proj_cd067221d5a6e4007ccbb4afb5966535",
                             "create_date": 1673253803928,
                             "metadata": {
@@ -189,14 +192,15 @@
     def delete(cls, asset_id_or_name: str) -> dict:
         """Deletes a specific asset from the project.
 
         :param asset_id_or_name: The ID or file name of the asset as a string.
         :return: A dictionary containing the deleted asset ID and the deletion status with the following structure.
 
                 .. code-block:: json
+
                         {
                             "id": "asset_6aea3395-9a72-4bb5-9ee0-19248c903c56",
                             "deleted": true
                         }
         :example:
 
                 .. code-block:: python
@@ -225,15 +229,15 @@
                         import datature
 
                         datature.secret_key = "5aa41e8ba........"
 
                         files = os.listdir("Your assets folder")
 
                         batch_size = 5000
-                        num_batches = len(files)
+                        num_batches = len(files) // batch_size
 
                         # split to batches, each batch includes 5000 assets
                         batches = [files[i*batch_size:
                                     (i+1) * batch_size] for i in range(num_batches)]
 
                         if len(files) % batch_size != 0:
                             batches.append(files[num_batches * batch_size:])
@@ -254,14 +258,15 @@
     def group(cls, group: str = None) -> dict:
         """Retrieve asset statistics categorized by asset group and asset status.
 
         :param group: A comma-separated string of name(s) of asset group(s).
         :return: A list of dictionaries of the categorized asset statistics with the following structure:
 
                 .. code-block:: json
+
                         [
                             {
                                 "cohort": "main",
                                 "statistic": {
                                     "assetTotal": 446,
                                     "assetAnnotated": 13,
                                     "assetReviewed": 0,
```

### Comparing `datature-1.1.0/datature/rest/asset/upload_session.py` & `datature-1.1.1/datature/rest/asset/upload_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -200,22 +200,14 @@
                         "size": size,
                         "crc32c": crc32,
                         "mime": mime_kind.mime
                     }
                 elif mime_kind.mime == "video/mp4":
                     cap = cv2.VideoCapture(file_path)
                     frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
-                    four_c_c = int(cap.get(cv2.CAP_PROP_FOURCC))
-                    codec = chr(four_c_c
-                                & 0xff) + chr((four_c_c >> 8) & 0xff) + chr(
-                                    (four_c_c >> 16)
-                                    & 0xff) + chr((four_c_c >> 24) & 0xff)
-                    if not (codec.startswith('avc1')
-                            or codec.startswith('mp4v')):
-                        raise error.Error("UnSupported asset file")
 
                     asset_metadata = {
                         "filename": filename,
                         "size": size,
                         "crc32c": crc32,
                         "mime": mime_kind.mime,
                         "frames": frames,
```

### Comparing `datature-1.1.0/datature/rest/deploy.py` & `datature-1.1.1/datature/rest/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     @classmethod
     def list(cls) -> dict:
         """Lists all deployments in a project.
 
         :return: A list of dictionaries containing deployment metadata with the following structure:
 
                 .. code-block:: json
+
                         [
                             {
                                 "id": "deploy_30922d5e-b2f6-43dc-b7b4-e29e2c30fb45",
                                 "object": "deploy",
                                 "project_id": "proj_cd067221d5a6e4007ccbb4afb5966535",
                                 "model_id": "model_5cbcf0fb9f692621f9cfc1ea8f1d68c7",
                                 "scaling": {
@@ -64,14 +65,15 @@
     def retrieve(cls, deploy_id: str) -> dict:
         """Retrieves a specific deployment using the deployment ID.
 
         :param deploy_id: The ID of the deployment as a string.
         :return: A dictionary containing the specific deployment metadata with the following structure:
 
                 .. code-block:: json
+
                             {
                                 "id": "deploy_30922d5e-b2f6-43dc-b7b4-e29e2c30fb45",
                                 "object": "deploy",
                                 "project_id": "proj_cd067221d5a6e4007ccbb4afb5966535",
                                 "model_id": "model_5cbcf0fb9f692621f9cfc1ea8f1d68c7",
                                 "scaling": {
                                     "mode": "fixed",
@@ -102,14 +104,15 @@
     def delete(cls, deploy_id: str) -> dict:
         """Deletes a specific deployment from the project.
 
         :param deploy_id: The id of the deployment.
         :return: A dictionary containing the deleted deployment ID and the deletion status with the following structure:
 
                 .. code-block:: json
+
                             {
                                 "id": "deploy_30922d5e-b2f6-43dc-b7b4-e29e2c30fb45",
                                 "deleted": true
                             }
 
         :example:
                 .. code-block:: python
@@ -125,14 +128,15 @@
     def create(cls, deployment: DeploymentMetadata) -> dict:
         """Creates a deployment for a specific model using the model ID.
 
         :param deployment: The configuration metadata of the deployment.
         :return: A dictionary containing the created deployment metadata with the following structure:
 
                 .. code-block:: json
+
                         {
                             "id": "op_508fc5d1-e908-486d-9e7b-1dca99b80024",
                             "object": "operation",
                             "op_link": "users/api|affaf/proje-1dca99b80024",
                             "status": {
                                 "overview": "Queued",
                                 "message": "Operation queued",
```

### Comparing `datature-1.1.0/datature/rest/operation.py` & `datature-1.1.1/datature/rest/operation.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     def retrieve(cls, op_link: str) -> dict:
         """Retrieves an executed operation status using the operation link.
 
         :param op_link: The link of the operation as a string.
         :return: A dictionary containing the operation metadata with the following structure.
 
                 .. code-block:: json
+
                         {
                             "id": "op_508fc5d1-e908-486d-9e7b-1dca99b80024",
                             "object": "operation",
                             "op_link": "users/api|affaf/proje-1dca99b80024",
                             "status": {
                                 "overview": "Queued",
                                 "message": "Operation queued",
```

### Comparing `datature-1.1.0/datature/rest/project.py` & `datature-1.1.1/datature/rest/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     @classmethod
     def retrieve(cls) -> dict:
         """Retrieves project information.
 
         :return: A dictionary containing the project metadata with the following structure:
 
                 .. code-block:: json
+
                         {
                             "id": "proj_cd067221d5a6e4007ccbb4afb5966535",
                             "object": "project",
                             "owner": "user_6323fea23e292439f31c58cd",
                             "name": "New Test Name",
                             "type": "classification",
                             "create_date": 1673253800069,
@@ -71,14 +72,15 @@
     def modify(cls, project: ProjectMetadata) -> dict:
         """Updates the project name.
 
         :param project: The new metadata of the project to be updated.
         :return: A dictionary containing the project metadata and the updated project name with the following structure:
 
                 .. code-block:: json
+
                         {
                             "id": "proj_cd067221d5a6e4007ccbb4afb5966535",
                             "object": "project",
                             "owner": "user_6323fea23e292439f31c58cd",
                             "name": "New Test Name",
                             "type": "classification",
                             "create_date": 1673253800069,
@@ -116,14 +118,15 @@
     @classmethod
     def quota(cls) -> dict:
         """Retrieves the project quota showing the limits based on the tier the project account is on and the current usage.
 
         :return: A dictionary containing the project quota metadata with the following structure:
 
                 .. code-block:: json
+
                         {
                             "limit": {
                                 "collaborator": 3,
                                 "image": 60000,
                                 "compute": 20000,
                                 "artifact": 50,
                                 "artifact_export": 50,
@@ -156,14 +159,15 @@
     @classmethod
     def insight(cls) -> dict:
         """Retrieves project insight and metrics of the completed training runs.
 
         :return: A dictionary containing the project insight metadata with the following structure:
 
                 .. code-block:: json
+
                         [
                             {
                                 "flow_title": "Blood Cell Detector",
                                 "run_id": "run_63eb212ff0f856bf95085095",
                                 "step": 600,
                                 "create_date": 1676354685212,
                                 "metric": {
@@ -205,14 +209,15 @@
     @classmethod
     def users(cls) -> dict:
         """Retrieves all users in the project. This includes Project Owners, Collaborators and Datature Experts.
 
         :return: A list of dictionaries containing the project user metadata with the following structure:
 
                 .. code-block:: json
+
                         [
                             {
                                 "id": "user_6323fea23e292439f31c58cd",
                                 "object": "user",
                                 "access_type": "owner",
                                 "email": "xxx@datature.io",
                                 "nickname": "xxx",
```

### Comparing `datature-1.1.0/datature/rest/run.py` & `datature-1.1.1/datature/rest/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     @classmethod
     def list(cls) -> dict:
         """Lists all training runs regardless of status.
 
         :return: A list of dictionaries containing the training run metadata with the following structure:
 
                 .. code-block:: json
+
                         [
                             {
                                 "id": "run_63eb212ff0f856bf95085095",
                                 "object": "run",
                                 "project_id": "proj_cd067221d5a6e4007ccbb4afb5966535",
                                 "flow_id": "flow_63bbd3bf8a78eb906f417396",
                                 "status": {
@@ -87,14 +88,15 @@
     def retrieve(cls, run_id: str) -> dict:
         """Retrieves a specific training run using the run ID.
 
         :param run_id: The ID of the training run.
         :return: A dictionary containing the specific training run metadata with the following structure:
 
                 .. code-block:: json
+
                             {
                                 "id": "run_63eb212ff0f856bf95085095",
                                 "object": "run",
                                 "project_id": "proj_cd067221d5a6e4007ccbb4afb5966535",
                                 "flow_id": "flow_63bbd3bf8a78eb906f417396",
                                 "status": {
                                     "conditions": [
@@ -148,14 +150,15 @@
     def kill(cls, run_id: str) -> dict:
         """Kills a specific training run using the run ID.
 
         :param run_id: The ID of the training run.
         :return: A dictionary containing the killed training metadata with the following structure:
 
                 .. code-block:: json
+
                             {
                                 "id": "run_63eb212ff0f856bf95085095",
                                 "object": "run",
                                 "project_id": "proj_cd067221d5a6e4007ccbb4afb5966535",
                                 "flow_id": "flow_63bbd3bf8a78eb906f417396",
                                 "status": {
                                     "conditions": [
@@ -212,14 +215,15 @@
         """Starts a new training run from a specific workflow using the flow ID.
 
         :param flow_id: The ID of the workflow.
         :param setup: The metadata of the training.
         :return: A dictionary containing the newly-initialized training run metadata with the following structure:
 
                 .. code-block:: json
+
                             {
                                 "id": "run_63eb212ff0f856bf95085095",
                                 "object": "run",
                                 "project_id": "proj_cd067221d5a6e4007ccbb4afb5966535",
                                 "flow_id": "flow_63bbd3bf8a78eb906f417396",
                                 "status": {
                                     "conditions": [
@@ -316,14 +320,15 @@
     def log(cls, log_id: str) -> dict:
         """Retrieves a specific training log using the log ID.
 
         :param log_id: The ID of the training log.
         :return: A dictionary with the specific training log metadata with the following structure:
 
                 .. code-block:: json
+
                         {
                             "id": "log_63eb212ff0f856bf95085095",
                             "object": "log",
                             "event": [
                                 {
                                     "ev": "memoryUsage",
                                     "pl": {},
```

### Comparing `datature-1.1.0/datature/rest/tag.py` & `datature-1.1.1/datature/rest/tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     @classmethod
     def list(cls) -> dict:
         """Lists all tags in the project.
 
         :return: A list of dictionaries containing tag metadata with the following structure:
 
                 .. code-block:: json
+
                         [
                             {
                                 "index": 0,
                                 "name": "tagName1"
                             }
                         ]
 
@@ -48,14 +49,15 @@
     def create(cls, name: str) -> dict:
         """Creates a new tag. The indices of new tags created will begin from the last existing tag index.
 
         :param name: The name of the new tag.
         :return: An updated list of dictionaries containing tag metadata with the following structure:
 
                 .. code-block:: json
+
                         [
                             {
                                 "index": 0,
                                 "name": "tagName1"
                             }, {
                                 "index": 1,
                                 "name": "tagName2"
@@ -77,14 +79,15 @@
         """Updates the name of a specific tag using the tag index.
 
         :param index: The index of the tag to update.
         :param name: The new name of the tag.
         :return: An updated list of dictionaries containing tag metadata with the following structure:
 
                 .. code-block:: json
+
                         [
                             {
                                 "index": 0,
                                 "name": "tagName1"
                             }, {
                                 "index": 1,
                                 "name": "tagName3"
@@ -105,14 +108,15 @@
     def delete(cls, index: int) -> dict:
         """Deletes a specific tag using the tag index. The tag indices of other tags will be left unchanged. The indices of new tags created will begin from the last existing tag index.
 
         :param index: The index of the tag.
         :return: A dictionary containing the deletion status of the tag with the following structure:
 
                 .. code-block:: json
+
                         {
                             "deleted": true
                         }
 
         :example:
                 .. code-block:: python
```

### Comparing `datature-1.1.0/datature/rest/types.py` & `datature-1.1.1/datature/rest/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     num_of_instances: int = 1
 
 
 @dataclass
 class Accelerator:
     """The hardware accelerator to be used for the training.
 
-    :param name: The name of the GPU to be used for the training (GPU_T4, GPU_V100, GPU_P100, GPU_K80).
+    :param name: The name of the GPU to be used for the training (GPU_T4, GPU_V100, GPU_P100, GPU_K80, GPU_A100_40GB, GPU_A100_80GB).
     :param count: The number of GPUs to be used for the training. More GPUs will use up more compute minutes. Defaults to 1.
     """
 
     name: str
     count: int = 1
```

### Comparing `datature-1.1.0/datature/rest/workflow.py` & `datature-1.1.1/datature/rest/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     @classmethod
     def list(cls) -> dict:
         """Lists all workflows in the project.
 
         :return: A list of dictionaries containing the workflow metadata with the following structure:
 
                 .. code-block:: json
+
                             [
                                 {
                                     "id": "flow_639309be08b4488a914b8802",
                                     "object": "workflow",
                                     "title": "My very awesome workflow",
                                     "state": "",
                                     "project_id": "proj_b705a30ae26671657f1fd51eb2d4739d",
@@ -53,14 +54,15 @@
     def retrieve(cls, flow_id: str) -> dict:
         """Retrieves a specific workflow using the flow ID.
 
         :param flow_id: The ID of the workflow.
         :return: A dictionary containing the specific workflow metadata with the following structure:
 
                 .. code-block:: json
+
                                 {
                                     "id": "flow_639309be08b4488a914b8802",
                                     "object": "workflow",
                                     "title": "My very awesome workflow",
                                     "state": "",
                                     "project_id": "proj_b705a30ae26671657f1fd51eb2d4739d",
                                     "last_updated": 1670581881299
@@ -81,14 +83,15 @@
         """Updates title of a specific workflow using the flow ID.
 
         :param flow_id: The ID of the workflow.
         :param flow: The new metadata of the workflow to be updated.
         :return: A dictionary containing the updated workflow metadata with the following structure:
 
                 .. code-block:: json
+
                                 {
                                     "id": "flow_639309be08b4488a914b8802",
                                     "object": "workflow",
                                     "title": "My awesome workflow",
                                     "state": "",
                                     "project_id": "proj_b705a30ae26671657f1fd51eb2d4739d",
                                     "last_updated": 1670581881299
@@ -109,14 +112,15 @@
     def delete(cls, flow_id: str) -> dict:
         """Deletes a specific workflow using the flow ID.
 
         :param flow_id: The ID of the workflow
         :return: A dictionary containing the deleted workflow ID and deletion status with the following structure:
 
                 .. code-block:: json
+
                                 {
                                     "id": "flow_639309be08b4488a914b8802",
                                     "deleted":true
                                 }
 
         :example:
                 .. code-block:: python
```

### Comparing `datature-1.1.0/datature/utils/utils.py` & `datature-1.1.1/datature/utils/utils.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/datature.egg-info/PKG-INFO` & `datature-1.1.1/datature.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datature
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python bindings for the Datature API
 Author: Raighne Weng
 Author-email: raighne@datature.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `datature-1.1.0/datature.egg-info/SOURCES.txt` & `datature-1.1.1/datature.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/docs/source/conf.py` & `datature-1.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/docs/upload.py` & `datature-1.1.1/docs/upload.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/readme.md` & `datature-1.1.1/readme.md`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/setup.py` & `datature-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     long_description=long_description,
     description="Python bindings for the Datature API",
     packages=setuptools.find_namespace_packages(),
     python_requires=">=3.7",
     install_requires=[
         "requests", "google-crc32c", "pyhumps", "pyyaml", "inquirer", "halo",
         "filetype", "opencv-python", "alive-progress", "pydicom", "nibabel",
-        "pillow"
+        "matplotlib"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License"
     ],
     extras_require={
         'docs': ["sphinx", "sphinx-rtd-theme", "sphinx_markdown_builder"]
```

### Comparing `datature-1.1.0/test/fixture/data/error_fixture.py` & `datature-1.1.1/test/fixture/data/error_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/fixture/data/operation_fixture.py` & `datature-1.1.1/test/fixture/data/operation_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/fixture/data/upload_session_fixture.py` & `datature-1.1.1/test/fixture/data/upload_session_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/fixture/mock.py` & `datature-1.1.1/test/fixture/mock.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/http/test_requester.py` & `datature-1.1.1/test/http/test_requester.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/http/test_resource.py` & `datature-1.1.1/test/http/test_resource.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/rest/test_annotation.py` & `datature-1.1.1/test/rest/test_annotation.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/rest/test_artifact.py` & `datature-1.1.1/test/rest/test_artifact.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/rest/test_asset.py` & `datature-1.1.1/test/rest/test_asset.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/rest/test_asset_upload_session.py` & `datature-1.1.1/test/rest/test_asset_upload_session.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/rest/test_deploy.py` & `datature-1.1.1/test/rest/test_deploy.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/rest/test_operation.py` & `datature-1.1.1/test/rest/test_operation.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/rest/test_project.py` & `datature-1.1.1/test/rest/test_project.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/rest/test_run.py` & `datature-1.1.1/test/rest/test_run.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/rest/test_tag.py` & `datature-1.1.1/test/rest/test_tag.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/rest/test_workflow.py` & `datature-1.1.1/test/rest/test_workflow.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/test_error.py` & `datature-1.1.1/test/test_error.py`

 * *Files identical despite different names*

### Comparing `datature-1.1.0/test/test_logger.py` & `datature-1.1.1/test/test_logger.py`

 * *Files identical despite different names*

