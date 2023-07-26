# Comparing `tmp/fenjing-0.4.9.tar.gz` & `tmp/fenjing-0.4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.4.9.tar", last modified: Wed Jul 26 15:23:03 2023, max compression
+gzip compressed data, was "fenjing-0.4.9.1.tar", last modified: Wed Jul 26 15:56:24 2023, max compression
```

## Comparing `fenjing-0.4.9.tar` & `fenjing-0.4.9.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:23:03.436479 fenjing-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-26 15:22:53.000000 fenjing-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-26 15:22:53.000000 fenjing-0.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-07-26 15:23:03.436479 fenjing-0.4.9/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     9223 2023-07-26 15:22:53.000000 fenjing-0.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 15:22:53.000000 fenjing-0.4.9/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:23:03.432479 fenjing-0.4.9/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/context_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/form.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7701 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    34703 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/shell_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/submitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:23:03.436479 fenjing-0.4.9/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-26 15:22:53.000000 fenjing-0.4.9/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:23:03.436479 fenjing-0.4.9/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-07-26 15:23:03.000000 fenjing-0.4.9/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-26 15:23:03.000000 fenjing-0.4.9/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:23:03.000000 fenjing-0.4.9/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 15:23:03.000000 fenjing-0.4.9/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 15:23:03.000000 fenjing-0.4.9/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 15:22:53.000000 fenjing-0.4.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:23:03.436479 fenjing-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-26 15:22:53.000000 fenjing-0.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:23:03.436479 fenjing-0.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-26 15:22:53.000000 fenjing-0.4.9/tests/test_cracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-26 15:22:53.000000 fenjing-0.4.9/tests/test_full_payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-26 15:22:53.000000 fenjing-0.4.9/tests/test_payload_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:56:24.391519 fenjing-0.4.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-26 15:56:24.391519 fenjing-0.4.9.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9223 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:56:24.387519 fenjing-0.4.9.1/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/context_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/form.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7701 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34943 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/shell_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/submitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:56:24.387519 fenjing-0.4.9.1/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:56:24.387519 fenjing-0.4.9.1/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-26 15:56:24.000000 fenjing-0.4.9.1/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-26 15:56:24.000000 fenjing-0.4.9.1/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:56:24.000000 fenjing-0.4.9.1/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 15:56:24.000000 fenjing-0.4.9.1/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 15:56:24.000000 fenjing-0.4.9.1/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:56:24.391519 fenjing-0.4.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:56:24.387519 fenjing-0.4.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/tests/test_cracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-26 15:56:14.000000 fenjing-0.4.9.1/tests/test_payload_gen.py
```

### Comparing `fenjing-0.4.9/LICENSE` & `fenjing-0.4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/PKG-INFO` & `fenjing-0.4.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.9
+Version: 0.4.9.1
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.4.9/README.md` & `fenjing-0.4.9.1/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing/cli.py` & `fenjing-0.4.9.1/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing/colorize.py` & `fenjing-0.4.9.1/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing/config_payload.py` & `fenjing-0.4.9.1/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing/const.py` & `fenjing-0.4.9.1/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing/context_vars.py` & `fenjing-0.4.9.1/fenjing/context_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing/cracker.py` & `fenjing-0.4.9.1/fenjing/cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing/form.py` & `fenjing-0.4.9.1/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing/full_payload_gen.py` & `fenjing-0.4.9.1/fenjing/full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing/payload_gen.py` & `fenjing-0.4.9.1/fenjing/payload_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -900,29 +900,14 @@
 def gen_string_context(context: dict, value: str):
     if value not in context.values():
         return [(UNSATISFIED,)]
     v = [k for k, v in context.items() if v == value][0]
     return [(LITERAL, v)] + [(WITH_CONTEXT_VAR, v)]
 
 
-@req_gen
-def gen_string_removedunder(context: dict, value: str):
-    if not re.match("^__[A_Za-z0-9_]+__$", value):
-        return [(UNSATISFIED,)]
-    return [
-        (STRING_UNDERLINE,),
-        (LITERAL, "*"),
-        (INTEGER, 2),
-        (STRING_STRING_CONCAT,),
-        (STRING, value[2:-2]),
-        (STRING_STRING_CONCAT,),
-        (STRING_UNDERLINE,),
-        (LITERAL, "*"),
-        (INTEGER, 2),
-    ]
 
 
 @req_gen
 def gen_string_concat1(context: dict, value: str):
     return [
         (
             LITERAL,
@@ -953,14 +938,44 @@
             "({})".format(
                 "".join('"{}"'.format(c if c != '"' else '\\"') for c in value)
             ),
         )
     ]
 
 
+
+@req_gen
+def gen_string_chars(context: dict, value: str):
+    ans: List[Any] = [(LITERAL, "("), (CHAR, value[0])]
+    for c in value[1:]:
+        ans.append((STRING_STRING_CONCAT,))
+        ans.append((CHAR, c))
+    ans.append(
+        (LITERAL, ")"),
+    )
+    return ans
+
+
+
+@req_gen
+def gen_string_removedunder(context: dict, value: str):
+    if not re.match("^__[A_Za-z0-9_]+__$", value):
+        return [(UNSATISFIED,)]
+    return [
+        (STRING_UNDERLINE,),
+        (LITERAL, "*"),
+        (INTEGER, 2),
+        (STRING_STRING_CONCAT,),
+        (STRING, value[2:-2]),
+        (STRING_STRING_CONCAT,),
+        (STRING_UNDERLINE,),
+        (LITERAL, "*"),
+        (INTEGER, 2),
+    ]
+
 @req_gen
 def gen_string_dictjoin(context: dict, value: str):
     if not re.match("^[a-zA-Z_]+$", value):
         return [(UNSATISFIED,)]
     return [(LITERAL, "(dict({}=x)|join)".format(value))]
 
 
@@ -1000,25 +1015,14 @@
         return [(UNSATISFIED,)]
 
     return [
         (LITERAL, "(dict({})|join)".format(",".join(f"{part}=x" for part in value)))
     ]
 
 
-@req_gen
-def gen_string_chars(context: dict, value: str):
-    ans: List[Any] = [(LITERAL, "("), (CHAR, value[0])]
-    for c in value[1:]:
-        ans.append((STRING_STRING_CONCAT,))
-        ans.append((CHAR, c))
-    ans.append(
-        (LITERAL, ")"),
-    )
-    return ans
-
 
 @req_gen
 def gen_string_formatpercent(context: dict, value: str):
     # (('%c'*n)%(97,98,99))
     req = []
     req.append((LITERAL, "(("))
     req.append((STRING_MANY_PERCENT_LOWER_C, len(value)))
@@ -1263,14 +1267,25 @@
         (LITERAL, "namespace"),
         (ATTRIBUTE, "__init__"),
         (ATTRIBUTE, "__globals__"),
         (ITEM, "__builtins__"),
         (ITEM, "eval")
     )]
 
+@req_gen
+def gen_eval_func_g(context):
+    return [(
+        CHAINED_ATTRIBUTE_ITEM,
+        (LITERAL, "g"),
+        (ATTRIBUTE, "pop"),
+        (ATTRIBUTE, "__globals__"),
+        (ITEM, "__builtins__"),
+        (ITEM, "eval")
+    )]
+
 # ---
 
 
 @req_gen
 def gen_eval_normal(context, code):
     return [
         (LITERAL, "("),
```

### Comparing `fenjing-0.4.9/fenjing/requester.py` & `fenjing-0.4.9.1/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing/scan_url.py` & `fenjing-0.4.9.1/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing/shell_payload.py` & `fenjing-0.4.9.1/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing/submitter.py` & `fenjing-0.4.9.1/fenjing/submitter.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing/templates/index.html` & `fenjing-0.4.9.1/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing/waf_func_gen.py` & `fenjing-0.4.9.1/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing/webui.py` & `fenjing-0.4.9.1/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/fenjing.egg-info/PKG-INFO` & `fenjing-0.4.9.1/fenjing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.4.9
+Version: 0.4.9.1
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.4.9/fenjing.egg-info/SOURCES.txt` & `fenjing-0.4.9.1/fenjing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/setup.py` & `fenjing-0.4.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/tests/test_cracker.py` & `fenjing-0.4.9.1/tests/test_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/tests/test_full_payload_gen.py` & `fenjing-0.4.9.1/tests/test_full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.4.9/tests/test_payload_gen.py` & `fenjing-0.4.9.1/tests/test_payload_gen.py`

 * *Files identical despite different names*

