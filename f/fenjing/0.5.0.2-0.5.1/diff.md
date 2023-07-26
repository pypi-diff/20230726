# Comparing `tmp/fenjing-0.5.0.2.tar.gz` & `tmp/fenjing-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.5.0.2.tar", last modified: Wed Jul 26 19:32:16 2023, max compression
+gzip compressed data, was "fenjing-0.5.1.tar", last modified: Wed Jul 26 19:52:14 2023, max compression
```

## Comparing `fenjing-0.5.0.2.tar` & `fenjing-0.5.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:32:16.968036 fenjing-0.5.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-07-26 19:32:16.968036 fenjing-0.5.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     9413 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:32:16.968036 fenjing-0.5.0.2/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/context_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/form.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7701 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    37389 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/shell_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/submitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:32:16.968036 fenjing-0.5.0.2/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:32:16.968036 fenjing-0.5.0.2/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-07-26 19:32:16.000000 fenjing-0.5.0.2/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-26 19:32:16.000000 fenjing-0.5.0.2/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:32:16.000000 fenjing-0.5.0.2/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 19:32:16.000000 fenjing-0.5.0.2/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 19:32:16.000000 fenjing-0.5.0.2/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:32:16.968036 fenjing-0.5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:32:16.968036 fenjing-0.5.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/tests/test_cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/tests/test_full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-26 19:32:06.000000 fenjing-0.5.0.2/tests/test_payload_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:52:14.822969 fenjing-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-26 19:52:04.000000 fenjing-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-26 19:52:04.000000 fenjing-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-26 19:52:14.822969 fenjing-0.5.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9413 2023-07-26 19:52:04.000000 fenjing-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 19:52:04.000000 fenjing-0.5.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:52:14.818969 fenjing-0.5.1/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/form.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7701 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/shell_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/submitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:52:14.822969 fenjing-0.5.1/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-26 19:52:04.000000 fenjing-0.5.1/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:52:14.818969 fenjing-0.5.1/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9850 2023-07-26 19:52:14.000000 fenjing-0.5.1/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-26 19:52:14.000000 fenjing-0.5.1/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:52:14.000000 fenjing-0.5.1/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 19:52:14.000000 fenjing-0.5.1/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 19:52:14.000000 fenjing-0.5.1/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 19:52:04.000000 fenjing-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:52:14.822969 fenjing-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-26 19:52:04.000000 fenjing-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:52:14.822969 fenjing-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-26 19:52:04.000000 fenjing-0.5.1/tests/test_cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-26 19:52:04.000000 fenjing-0.5.1/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-26 19:52:04.000000 fenjing-0.5.1/tests/test_payload_gen.py
```

### Comparing `fenjing-0.5.0.2/LICENSE` & `fenjing-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/PKG-INFO` & `fenjing-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.5.0.2
+Version: 0.5.1
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.5.0.2/README.md` & `fenjing-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing/cli.py` & `fenjing-0.5.1/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing/colorize.py` & `fenjing-0.5.1/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing/config_payload.py` & `fenjing-0.5.1/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing/const.py` & `fenjing-0.5.1/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing/context_vars.py` & `fenjing-0.5.1/fenjing/context_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing/cracker.py` & `fenjing-0.5.1/fenjing/cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing/form.py` & `fenjing-0.5.1/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing/full_payload_gen.py` & `fenjing-0.5.1/fenjing/full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing/payload_gen.py` & `fenjing-0.5.1/fenjing/payload_gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1163,18 +1163,19 @@
         (LITERAL, "]"),
     ]
 
 
 @req_gen
 def gen_attribute_attrfilter(context, obj_req, attr_name):
     return [
+        (LITERAL, "("),
         obj_req,
         (LITERAL, "|attr("),
         (STRING, attr_name),
-        (LITERAL, ")"),
+        (LITERAL, "))"),
     ]
 
 
 # ---
 
 
 @req_gen
```

### Comparing `fenjing-0.5.0.2/fenjing/requester.py` & `fenjing-0.5.1/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing/scan_url.py` & `fenjing-0.5.1/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing/shell_payload.py` & `fenjing-0.5.1/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing/submitter.py` & `fenjing-0.5.1/fenjing/submitter.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing/templates/index.html` & `fenjing-0.5.1/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing/waf_func_gen.py` & `fenjing-0.5.1/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing/webui.py` & `fenjing-0.5.1/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/fenjing.egg-info/PKG-INFO` & `fenjing-0.5.1/fenjing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.5.0.2
+Version: 0.5.1
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.5.0.2/fenjing.egg-info/SOURCES.txt` & `fenjing-0.5.1/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/setup.py` & `fenjing-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/tests/test_cracker.py` & `fenjing-0.5.1/tests/test_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/tests/test_full_payload_gen.py` & `fenjing-0.5.1/tests/test_full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.5.0.2/tests/test_payload_gen.py` & `fenjing-0.5.1/tests/test_payload_gen.py`

 * *Files identical despite different names*

