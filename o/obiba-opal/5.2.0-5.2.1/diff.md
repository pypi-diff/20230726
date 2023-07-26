# Comparing `tmp/obiba_opal-5.2.0.tar.gz` & `tmp/obiba_opal-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obiba_opal-5.2.0.tar", max compression
+gzip compressed data, was "obiba_opal-5.2.1.tar", max compression
```

## Comparing `obiba_opal-5.2.0.tar` & `obiba_opal-5.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35147 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/LICENSE.txt
--rw-r--r--   0        0        0     3573 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/README.md
--rw-r--r--   0        0        0     1536 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/__init__.py
--rw-r--r--   0        0        0     6537 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/analysis.py
--rwxr-xr-x   0        0        0    14113 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/console.py
--rwxr-xr-x   0        0        0    19035 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/core.py
--rwxr-xr-x   0        0        0     7155 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/data.py
--rwxr-xr-x   0        0        0    14671 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/dictionary.py
--rw-r--r--   0        0        0    23109 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/exports.py
--rwxr-xr-x   0        0        0     4730 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/file.py
--rw-r--r--   0        0        0    47546 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/imports.py
--rw-r--r--   0        0        0    12920 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/io.py
--rw-r--r--   0        0        0    34898 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/perm.py
--rwxr-xr-x   0        0        0    11397 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/project.py
--rw-r--r--   0        0        0     1325 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/security.py
--rw-r--r--   0        0        0     4862 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/sql.py
--rwxr-xr-x   0        0        0    10891 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/subjects.py
--rw-r--r--   0        0        0    17656 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/system.py
--rw-r--r--   0        0        0    14315 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/table.py
--rw-r--r--   0        0        0      826 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/pyproject.toml
--rw-r--r--   0        0        0     4568 1970-01-01 00:00:00.000000 obiba_opal-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-07-26 06:46:32.363175 obiba_opal-5.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     3573 2023-07-26 06:46:32.363175 obiba_opal-5.2.1/README.md
+-rw-r--r--   0        0        0     1536 2023-07-26 06:46:32.363175 obiba_opal-5.2.1/obiba_opal/__init__.py
+-rw-r--r--   0        0        0     6537 2023-07-26 06:46:32.363175 obiba_opal-5.2.1/obiba_opal/analysis.py
+-rwxr-xr-x   0        0        0    14113 2023-07-26 06:46:32.363175 obiba_opal-5.2.1/obiba_opal/console.py
+-rwxr-xr-x   0        0        0    19109 2023-07-26 06:46:32.367177 obiba_opal-5.2.1/obiba_opal/core.py
+-rwxr-xr-x   0        0        0     7155 2023-07-26 06:46:32.367177 obiba_opal-5.2.1/obiba_opal/data.py
+-rwxr-xr-x   0        0        0    14671 2023-07-26 06:46:32.367177 obiba_opal-5.2.1/obiba_opal/dictionary.py
+-rw-r--r--   0        0        0    23109 2023-07-26 06:46:32.367177 obiba_opal-5.2.1/obiba_opal/exports.py
+-rwxr-xr-x   0        0        0     4730 2023-07-26 06:46:32.367177 obiba_opal-5.2.1/obiba_opal/file.py
+-rw-r--r--   0        0        0    47546 2023-07-26 06:46:32.367177 obiba_opal-5.2.1/obiba_opal/imports.py
+-rw-r--r--   0        0        0    12920 2023-07-26 06:46:32.367177 obiba_opal-5.2.1/obiba_opal/io.py
+-rw-r--r--   0        0        0    34898 2023-07-26 06:46:32.367177 obiba_opal-5.2.1/obiba_opal/perm.py
+-rwxr-xr-x   0        0        0    11385 2023-07-26 06:46:32.367177 obiba_opal-5.2.1/obiba_opal/project.py
+-rw-r--r--   0        0        0     1325 2023-07-26 06:46:32.367177 obiba_opal-5.2.1/obiba_opal/security.py
+-rw-r--r--   0        0        0     4862 2023-07-26 06:46:32.367177 obiba_opal-5.2.1/obiba_opal/sql.py
+-rwxr-xr-x   0        0        0    10891 2023-07-26 06:46:32.367177 obiba_opal-5.2.1/obiba_opal/subjects.py
+-rw-r--r--   0        0        0    17704 2023-07-26 06:46:32.367177 obiba_opal-5.2.1/obiba_opal/system.py
+-rw-r--r--   0        0        0    14315 2023-07-26 06:46:32.367177 obiba_opal-5.2.1/obiba_opal/table.py
+-rw-r--r--   0        0        0      826 2023-07-26 06:46:32.367177 obiba_opal-5.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4568 1970-01-01 00:00:00.000000 obiba_opal-5.2.1/PKG-INFO
```

### Comparing `obiba_opal-5.2.0/LICENSE.txt` & `obiba_opal-5.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/README.md` & `obiba_opal-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/obiba_opal/__init__.py` & `obiba_opal-5.2.1/obiba_opal/__init__.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/obiba_opal/analysis.py` & `obiba_opal-5.2.1/obiba_opal/analysis.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/obiba_opal/console.py` & `obiba_opal-5.2.1/obiba_opal/console.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/obiba_opal/core.py` & `obiba_opal-5.2.1/obiba_opal/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import getpass
 import json
 import os
 from requests import Session, Request, Response
 import urllib.error
 import urllib.parse
 import urllib.request
+import urllib3
 from functools import reduce
 from http import HTTPStatus
 from http.client import HTTPConnection
 
 class OpalClient:
     """
     OpalClient holds the configuration for connecting to Opal.
@@ -71,15 +72,18 @@
         :param server - Opal server address
         :param user - username
         :param password - user password
         :param no_ssl_verify - if True, the SSL certificate is not verified (not recommended)
         """
         client = cls(server)
         if client.base_url.startswith('https:'):
-            client.session.verify = False if no_ssl_verify else True
+            client.session.verify = not no_ssl_verify
+            if no_ssl_verify:
+                urllib3.disable_warnings()
+
         client.credentials(user, password)
 
         # need to know whether a OTP is needed
         try:
             client.init_otp()
         except Exception as e:
             # do the close as the exception is raised in the builder
```

### Comparing `obiba_opal-5.2.0/obiba_opal/data.py` & `obiba_opal-5.2.1/obiba_opal/data.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/obiba_opal/dictionary.py` & `obiba_opal-5.2.1/obiba_opal/dictionary.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/obiba_opal/exports.py` & `obiba_opal-5.2.1/obiba_opal/exports.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/obiba_opal/file.py` & `obiba_opal-5.2.1/obiba_opal/file.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/obiba_opal/imports.py` & `obiba_opal-5.2.1/obiba_opal/imports.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/obiba_opal/io.py` & `obiba_opal-5.2.1/obiba_opal/io.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/obiba_opal/perm.py` & `obiba_opal-5.2.1/obiba_opal/perm.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/obiba_opal/project.py` & `obiba_opal-5.2.1/obiba_opal/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 import re
 
 class ProjectService:
     """
     Project management.
     """
-    
+
     def __init__(self, client: core.OpalClient, verbose: bool = False):
         self.client = client
         self.verbose = verbose
 
     @classmethod
     def add_arguments(cls, parser):
         """
@@ -83,55 +83,55 @@
         :param name: The project name
         """
         if not name:
             raise ValueError('The project name is required.')
         request = self._make_request(fail_safe)
         response = request.get().resource(core.UriBuilder(['project', name]).build()).send()
         return response.from_json() if response.code == 200 else None
-    
+
     def delete_project(self, name: str):
         """
         Delete the project by its name.
 
         :param name: The project name
         """
         if not name:
             raise ValueError('The project name is required.')
         request = self._make_request()
         request.delete().resource(core.UriBuilder(['project', name]).build()).send()
-    
+
     def add_project(self, name: str, database: str = None, title: str = None, description: str = None, tags: list = None, export_folder: str = None):
         """
         Add a project.
 
         :param name: The project name
         :param database: The project database name. If not provided only views can be added. See get_databases() for the list of databases available for storage.
         :param title: The project title
         :param description: The project description
         :param tags: The list of project tags
         :param export_folder: The project's preferred export folder
         """
         if not name:
             raise ValueError('The project name is required.')
-        
+
         # create project
         project = {'name': name}
         if database:
             project['database'] = database
         if title:
             project['title'] = title
         else:
             project['title'] = name
         if description:
             project['description'] = description
         if tags:
             project['tags'] = tags
         if export_folder:
             project['exportFolder'] = export_folder
-        
+
         request = self._make_request()
         request.accept_json().content_type_json()
         request.post().resource(core.UriBuilder(['projects']).build()).content(json.dumps(project)).send()
 
     def get_databases(self, usage: str = 'storage') -> list:
         """
         Get the databases available.
@@ -274,13 +274,13 @@
         job_resource = re.sub(r'http.*\/ws', r'', location)
         request = client.new_request()
         request.fail_on_error().accept_json()
         if args.verbose:
             request.verbose()
         response = request.get().resource(job_resource).send()
         # format response
-        res = response.content
+        res = response.content.decode('utf-8')
         if args.json:
             res = response.pretty_json()
 
         # output to stdout
         print(res)
```

### Comparing `obiba_opal-5.2.0/obiba_opal/security.py` & `obiba_opal-5.2.1/obiba_opal/security.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/obiba_opal/sql.py` & `obiba_opal-5.2.1/obiba_opal/sql.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/obiba_opal/subjects.py` & `obiba_opal-5.2.1/obiba_opal/subjects.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/obiba_opal/system.py` & `obiba_opal-5.2.1/obiba_opal/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                 request.verbose()
 
             # send request
             request.get().resource(cls.do_ws(args))
             response = request.send()
 
             # format response
-            res = response.content
+            res = response.content.decode('utf-8')
 
             if args.json:
                 res = response.pretty_json()
 
             # output to stdout
             print(res)
         finally:
@@ -152,15 +152,15 @@
                 response = request.get().resource('/plugin/' + args.status + '/service').send()
             elif args.start:
                 response = request.put().resource('/plugin/' + args.start + '/service').send()
             elif args.stop:
                 response = request.delete().resource('/plugin/' + args.stop + '/service').send()
 
             # format response
-            res = response.content
+            res = response.content.decode('utf-8')
             if args.json:
                 res = response.pretty_json()
 
             # output to stdout
             print(res)
         finally:
             client.close()
@@ -446,15 +446,15 @@
             if method in ['POST', 'PUT']:
               request = service.make_request_with_content_type(args.method, args.content_type, args.accept, args.headers)
             else:
               request = service.make_request(args.method, args.accept, args.headers)
 
             # format response
             response = service.send_request(args.ws, request)
-            res = response.content
+            res = response.content.decode('utf-8')
 
             if args.json:
                 res = response.pretty_json()
             elif args.method in ['OPTIONS']:
                 res = response.headers['Allow']
 
             # output to stdout
```

### Comparing `obiba_opal-5.2.0/obiba_opal/table.py` & `obiba_opal-5.2.1/obiba_opal/table.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.2.0/pyproject.toml` & `obiba_opal-5.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "obiba-opal"
-version = "5.2.0"
+version = "5.2.1"
 description = "OBiBa/Opal python client."
 authors = ["Yannick Marcon <yannick.marcon@obiba.org>"]
 maintainers = ["Yannick Marcon <yannick.marcon@obiba.org>"]
 license = "GPL-v3"
 readme = "README.md"
 packages = [{include = "obiba_opal"}]
 homepage = "https://www.obiba.org"
```

### Comparing `obiba_opal-5.2.0/PKG-INFO` & `obiba_opal-5.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obiba-opal
-Version: 5.2.0
+Version: 5.2.1
 Summary: OBiBa/Opal python client.
 Home-page: https://www.obiba.org
 License: GPL-v3
 Author: Yannick Marcon
 Author-email: yannick.marcon@obiba.org
 Maintainer: Yannick Marcon
 Maintainer-email: yannick.marcon@obiba.org
```

