# Comparing `tmp/STEP.py-2.2.tar.gz` & `tmp/STEP.py-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STEP.py-2.2.tar", last modified: Thu Jun  8 04:05:32 2023, max compression
+gzip compressed data, was "STEP.py-2.3.tar", last modified: Wed Jul 26 01:14:29 2023, max compression
```

## Comparing `STEP.py-2.2.tar` & `STEP.py-2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-06-08 04:05:32.420467 STEP.py-2.2/
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)     1068 2022-09-28 02:37:16.000000 STEP.py-2.2/LICENSE.txt
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)     6647 2023-06-08 04:05:32.420467 STEP.py-2.2/PKG-INFO
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)     6314 2022-09-28 02:37:16.000000 STEP.py-2.2/README.md
-drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-06-08 04:05:32.404467 STEP.py-2.2/STEP/
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)     1317 2022-04-21 05:05:19.000000 STEP.py-2.2/STEP/Cleaner.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)    39859 2023-06-08 04:00:09.000000 STEP.py-2.2/STEP/REST.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)    14931 2022-12-01 04:21:29.000000 STEP.py-2.2/STEP/SOAP.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)    11053 2022-04-21 05:05:19.000000 STEP.py-2.2/STEP/XML.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)  3190632 2022-07-29 00:09:13.000000 STEP.py-2.2/STEP/XSD.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)        0 2022-09-28 02:37:16.000000 STEP.py-2.2/STEP/__init__.py
-drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-06-08 04:05:32.411468 STEP.py-2.2/STEP.py.egg-info/
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)     6647 2023-06-08 04:05:32.000000 STEP.py-2.2/STEP.py.egg-info/PKG-INFO
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)      379 2023-06-08 04:05:32.000000 STEP.py-2.2/STEP.py.egg-info/SOURCES.txt
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)        1 2023-06-08 04:05:32.000000 STEP.py-2.2/STEP.py.egg-info/dependency_links.txt
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)      117 2023-06-08 04:05:32.000000 STEP.py-2.2/STEP.py.egg-info/requires.txt
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)        5 2023-06-08 04:05:32.000000 STEP.py-2.2/STEP.py.egg-info/top_level.txt
-drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-06-08 04:05:32.417466 STEP.py-2.2/bin/
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)      178 2022-04-21 05:05:19.000000 STEP.py-2.2/bin/excel2step.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)      287 2022-07-26 22:14:49.000000 STEP.py-2.2/bin/step.rest.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)      716 2022-07-26 22:16:51.000000 STEP.py-2.2/bin/step.soap.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)    19193 2023-03-22 04:38:13.000000 STEP.py-2.2/bin/step2uml.py
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)    16469 2022-07-19 06:08:05.000000 STEP.py-2.2/bin/uml2step.py
--rw-r--r--   0 eddo8    (197610) eddo8    (197610)       79 2023-06-08 04:05:32.421466 STEP.py-2.2/setup.cfg
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)      980 2023-06-08 03:57:40.000000 STEP.py-2.2/setup.py
-drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-06-08 04:05:32.419468 STEP.py-2.2/test/
--rwxr--r--   0 eddo8    (197610) eddo8    (197610)    10118 2022-09-01 05:43:58.000000 STEP.py-2.2/test/test_rest.py
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-07-26 01:14:29.890567 STEP.py-2.3/
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     1068 2022-09-28 02:37:16.000000 STEP.py-2.3/LICENSE.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     6647 2023-07-26 01:14:29.891567 STEP.py-2.3/PKG-INFO
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     6314 2022-09-28 02:37:16.000000 STEP.py-2.3/README.md
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-07-26 01:14:29.873567 STEP.py-2.3/STEP/
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)     1317 2022-04-21 05:05:19.000000 STEP.py-2.3/STEP/Cleaner.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    40711 2023-07-26 01:10:41.000000 STEP.py-2.3/STEP/REST.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    14931 2022-12-01 04:21:29.000000 STEP.py-2.3/STEP/SOAP.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    11053 2022-04-21 05:05:19.000000 STEP.py-2.3/STEP/XML.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)  3190632 2022-07-29 00:09:13.000000 STEP.py-2.3/STEP/XSD.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)        0 2022-09-28 02:37:16.000000 STEP.py-2.3/STEP/__init__.py
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-07-26 01:14:29.880567 STEP.py-2.3/STEP.py.egg-info/
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)     6647 2023-07-26 01:14:29.000000 STEP.py-2.3/STEP.py.egg-info/PKG-INFO
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)      379 2023-07-26 01:14:29.000000 STEP.py-2.3/STEP.py.egg-info/SOURCES.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)        1 2023-07-26 01:14:29.000000 STEP.py-2.3/STEP.py.egg-info/dependency_links.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)      117 2023-07-26 01:14:29.000000 STEP.py-2.3/STEP.py.egg-info/requires.txt
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)        5 2023-07-26 01:14:29.000000 STEP.py-2.3/STEP.py.egg-info/top_level.txt
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-07-26 01:14:29.887567 STEP.py-2.3/bin/
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      178 2022-04-21 05:05:19.000000 STEP.py-2.3/bin/excel2step.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      287 2022-07-26 22:14:49.000000 STEP.py-2.3/bin/step.rest.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      716 2022-07-26 22:16:51.000000 STEP.py-2.3/bin/step.soap.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    19193 2023-03-22 04:38:13.000000 STEP.py-2.3/bin/step2uml.py
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    16469 2022-07-19 06:08:05.000000 STEP.py-2.3/bin/uml2step.py
+-rw-r--r--   0 eddo8    (197610) eddo8    (197610)       79 2023-07-26 01:14:29.891567 STEP.py-2.3/setup.cfg
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)      980 2023-07-26 01:09:25.000000 STEP.py-2.3/setup.py
+drwxr-xr-x   0 eddo8    (197610) eddo8    (197610)        0 2023-07-26 01:14:29.889567 STEP.py-2.3/test/
+-rwxr--r--   0 eddo8    (197610) eddo8    (197610)    10118 2022-09-01 05:43:58.000000 STEP.py-2.3/test/test_rest.py
```

### Comparing `STEP.py-2.2/LICENSE.txt` & `STEP.py-2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `STEP.py-2.2/PKG-INFO` & `STEP.py-2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: STEP.py
-Version: 2.2
+Version: 2.3
 Summary: UNKNOWN
 Home-page: https://github.com/eddo888/STEP.py
 Author: David Edson
 Author-email: eddo888@tpg.com.au
 License: MIT
-Download-URL: https://github.com/eddo888/STEP.py/archive/2.2.tar.gz
+Download-URL: https://github.com/eddo888/STEP.py/archive/2.3.tar.gz
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # STEP.py
 
 python libraries to support Stibo STEP MDM APIs
```

### Comparing `STEP.py-2.2/README.md` & `STEP.py-2.3/README.md`

 * *Files identical despite different names*

### Comparing `STEP.py-2.2/STEP/Cleaner.py` & `STEP.py-2.3/STEP/Cleaner.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.2/STEP/REST.py` & `STEP.py-2.3/STEP/REST.py`

 * *Files 1% similar despite different names*

```diff
@@ -1077,8 +1077,26 @@
 	#________________________________________________________________________________________________
 	@args.operation(help='release workflow task by id')
 	@args.parameter(name='id', help='the ID of workflow task')
 	def release(self, id):
 		return super().post('%s/%s/release'%(self.base,id))
 		
 	
+#====================================================================================================
+@args.command(name='attributes')
+class Attributes(STEP):
+
+	base = 'attributes'
+
+	#________________________________________________________________________________________________
+	def __init__(self, asXML=None, verbose=None, output=None, silent=True, hostname=None, username=None, context=None, workspace=None):
+		super().__init__(asXML=asXML, verbose=verbose, output=output, silent=silent, hostname=hostname, username=username, context=context, workspace=workspace)
+				
+
+	#________________________________________________________________________________________________
+	@args.operation(help='get attribute definition by id')
+	@args.parameter(name='id', help='the ID attribute')
+	def get(self, id):
+		return super().get('%s/%s'%(self.base,id))
+		
+
 if __name__ == '__main__': args.execute()
```

### Comparing `STEP.py-2.2/STEP/SOAP.py` & `STEP.py-2.3/STEP/SOAP.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.2/STEP/XML.py` & `STEP.py-2.3/STEP/XML.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.2/STEP/XSD.py` & `STEP.py-2.3/STEP/XSD.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.2/STEP.py.egg-info/PKG-INFO` & `STEP.py-2.3/STEP.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: STEP.py
-Version: 2.2
+Version: 2.3
 Summary: UNKNOWN
 Home-page: https://github.com/eddo888/STEP.py
 Author: David Edson
 Author-email: eddo888@tpg.com.au
 License: MIT
-Download-URL: https://github.com/eddo888/STEP.py/archive/2.2.tar.gz
+Download-URL: https://github.com/eddo888/STEP.py/archive/2.3.tar.gz
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # STEP.py
 
 python libraries to support Stibo STEP MDM APIs
```

### Comparing `STEP.py-2.2/bin/step.soap.py` & `STEP.py-2.3/bin/step.soap.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.2/bin/step2uml.py` & `STEP.py-2.3/bin/step2uml.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.2/bin/uml2step.py` & `STEP.py-2.3/bin/uml2step.py`

 * *Files identical despite different names*

### Comparing `STEP.py-2.2/setup.py` & `STEP.py-2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 pwd = path.abspath(path.dirname(__file__))
 with codecs.open(path.join(pwd, 'README.md'), 'r', encoding='utf8') as input:
 	long_description = input.read()
 
 name='STEP.py'
 user='eddo888'
-version='2.2'
+version='2.3'
 
 setup(
 	name=name,
 	version=version,
 	license='MIT',
 	long_description=long_description,
 	long_description_content_type="text/markdown",
```

### Comparing `STEP.py-2.2/test/test_rest.py` & `STEP.py-2.3/test/test_rest.py`

 * *Files identical despite different names*

