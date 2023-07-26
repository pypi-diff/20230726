# Comparing `tmp/testery-1.7.0-py3-none-any.whl.zip` & `tmp/testery-1.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15923 bytes, number of entries: 11
--rw-r--r--  2.0 unx    50552 b- defN 23-Jun-21 21:37 testery.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 21:37 tests/__init__.py
--rw-r--r--  2.0 unx     2354 b- defN 23-Jun-21 21:37 tests/conftest.py
--rw-r--r--  2.0 unx     4857 b- defN 23-Jun-21 21:37 tests/test_integration.py
--rw-r--r--  2.0 unx     2797 b- defN 23-Jun-21 21:37 tests/test_unit.py
--rw-r--r--  2.0 unx     1055 b- defN 23-Jun-21 21:37 testery-1.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1264 b- defN 23-Jun-21 21:37 testery-1.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 21:37 testery-1.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 23-Jun-21 21:37 testery-1.7.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-21 21:37 testery-1.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      851 b- defN 23-Jun-21 21:37 testery-1.7.0.dist-info/RECORD
-11 files, 63896 bytes uncompressed, 14493 bytes compressed:  77.3%
+Zip file size: 15996 bytes, number of entries: 11
+-rw-r--r--  2.0 unx    51084 b- defN 23-Jul-26 20:40 testery.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-26 20:40 tests/__init__.py
+-rw-r--r--  2.0 unx     2354 b- defN 23-Jul-26 20:40 tests/conftest.py
+-rw-r--r--  2.0 unx     4857 b- defN 23-Jul-26 20:40 tests/test_integration.py
+-rw-r--r--  2.0 unx     2797 b- defN 23-Jul-26 20:40 tests/test_unit.py
+-rw-r--r--  2.0 unx     1055 b- defN 23-Jul-26 20:48 testery-1.7.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1264 b- defN 23-Jul-26 20:48 testery-1.7.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 20:48 testery-1.7.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 23-Jul-26 20:48 testery-1.7.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-26 20:48 testery-1.7.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      851 b- defN 23-Jul-26 20:48 testery-1.7.1.dist-info/RECORD
+11 files, 64428 bytes uncompressed, 14566 bytes compressed:  77.4%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: tests/test_integration.py
 Comment: 
 
 Filename: tests/test_unit.py
 Comment: 
 
-Filename: testery-1.7.0.dist-info/LICENSE
+Filename: testery-1.7.1.dist-info/LICENSE
 Comment: 
 
-Filename: testery-1.7.0.dist-info/METADATA
+Filename: testery-1.7.1.dist-info/METADATA
 Comment: 
 
-Filename: testery-1.7.0.dist-info/WHEEL
+Filename: testery-1.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: testery-1.7.0.dist-info/entry_points.txt
+Filename: testery-1.7.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: testery-1.7.0.dist-info/top_level.txt
+Filename: testery-1.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: testery-1.7.0.dist-info/RECORD
+Filename: testery-1.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## testery.py

```diff
@@ -28,15 +28,14 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.params.insert(0, click.Option(('--token',), required=True, help='Your Testery API token.'))
         self.params.insert(0, click.Option(('--testery-dev',), is_flag=True, default=False, hidden=True))
 
 
 def get_api_url(is_dev):
-
     if is_dev:
         return 'https://api.dev.testery.io/api'
     return 'https://api.testery.io/api'
 
 
 def report_test_run(test_run, output):
     if output == "teamcity":
@@ -290,14 +289,20 @@
     print(environment_request)
 
     headers['Authorization'] = "Bearer " + token
     response = requests.post(api_url + '/environments',
                                       headers=headers,
                                       json=environment_request)
 
+    if not response.ok:
+        if response.status_code == 401:
+            raise Exception('Unauthorized. Please check your API token.')
+        else:
+            raise Exception(f'Request Failed - Response Status Code: {response.status_code}')
+
     print(response.json())
 
 @click.command('create-schedule')
 @click.option('--testery-dev', is_flag=True, default=False, hidden=True)
 @click.option('--token', required=True, help='Your Testery API token.')
 @click.option('--git-ref', default=None, help='The git commit hash of the tests you want to run. Defaults to latest.')
 @click.option('--git-branch', default=None, help='The git branch whose latest commit you want to run.')
@@ -448,14 +453,20 @@
     """
 
     # Look up environment id by key.
     headers['Authorization'] = "Bearer " + token
     api_url = get_api_url(testery_dev)
     environments_response = requests.get(api_url + '/environments', headers=headers)
 
+    if not environments_response.ok:
+        if environments_response.status_code == 401:
+            raise Exception('Unauthorized. Please check your API token.')
+        else:
+            raise Exception(f'Request Failed - Response Status Code: {environments_response.status_code}')
+
     environments = environments_response.json()
 
     for environment in environments:
         if environment['key'] == key:
             print('DELETE %s/environments/%s' % (api_url, environment['id']))
             response = requests.delete(api_url + '/environments/' + str(environment['id']),headers=headers)
             print(response)
```

## Comparing `testery-1.7.0.dist-info/LICENSE` & `testery-1.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `testery-1.7.0.dist-info/METADATA` & `testery-1.7.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testery
-Version: 1.7.0
+Version: 1.7.1
 Summary: Testery CLI
 Home-page: https://github.com/testery/testery-cli
 Author: Testery
 Author-email: chris.harbert@testery.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `testery-1.7.0.dist-info/RECORD` & `testery-1.7.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-testery.py,sha256=Rip01NC2Ln7d1pcvcJ9KYw_3ld5ooiZC-uZ-bRRZ7mI,50552
+testery.py,sha256=_mi0-TMdXUdZV_P9CPbwHRNeahFr7MjfEHh1-H8cDjY,51084
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/conftest.py,sha256=AfQWy8n3D0jiQx2zlUCPa4s8MtoL-_x4IA2PEB61N0s,2354
 tests/test_integration.py,sha256=OuTRk7nJz11ks6Z21GcMND5xEt-Q9hKWboiP-uR6hok,4857
 tests/test_unit.py,sha256=0W33Gq-L6JxjAfeIGcOvqrA4Enl4HTvMRgvW4FAGMpg,2797
-testery-1.7.0.dist-info/LICENSE,sha256=4rsos8RTe2mQ-45ObCk7hPTRRvvHEwWATKlJzsGUTzM,1055
-testery-1.7.0.dist-info/METADATA,sha256=VyaRrz06qbFMAVCsnOEHy8tH3rsRvm9dXAFRdwV0eV8,1264
-testery-1.7.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-testery-1.7.0.dist-info/entry_points.txt,sha256=xTvd-fyvG6xBEMNwgnh6wKZTJAZjmlvEhfy9Zx_CW3A,60
-testery-1.7.0.dist-info/top_level.txt,sha256=E6h8DoEMFLwOQSYaj2ZC-fLqF86Ll00a-eKiZjjKlbk,14
-testery-1.7.0.dist-info/RECORD,,
+testery-1.7.1.dist-info/LICENSE,sha256=4rsos8RTe2mQ-45ObCk7hPTRRvvHEwWATKlJzsGUTzM,1055
+testery-1.7.1.dist-info/METADATA,sha256=26qSF3dyHKJmDpcH3TmBY3L_fHrscW0S_V8tzGyef6s,1264
+testery-1.7.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+testery-1.7.1.dist-info/entry_points.txt,sha256=xTvd-fyvG6xBEMNwgnh6wKZTJAZjmlvEhfy9Zx_CW3A,60
+testery-1.7.1.dist-info/top_level.txt,sha256=E6h8DoEMFLwOQSYaj2ZC-fLqF86Ll00a-eKiZjjKlbk,14
+testery-1.7.1.dist-info/RECORD,,
```

