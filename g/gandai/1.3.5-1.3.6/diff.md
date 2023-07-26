# Comparing `tmp/gandai-1.3.5.tar.gz` & `tmp/gandai-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.3.5.tar", last modified: Tue Jul 25 20:42:44 2023, max compression
+gzip compressed data, was "gandai-1.3.6.tar", last modified: Wed Jul 26 17:55:47 2023, max compression
```

## Comparing `gandai-1.3.5.tar` & `gandai-1.3.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:42:44.405139 gandai-1.3.5/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.3.5/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-25 20:42:44.404998 gandai-1.3.5/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:42:44.397438 gandai-1.3.5/gandai/
--rw-r--r--   0 parker     (501) staff       (20)       46 2023-07-17 18:25:43.000000 gandai-1.3.5/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:42:44.402803 gandai-1.3.5/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      264 2023-07-17 18:43:09.000000 gandai-1.3.5/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.3.5/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4120 2023-07-25 17:01:01.000000 gandai-1.3.5/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-19 22:26:35.000000 gandai-1.3.5/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.3.5/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2023-07-17 18:43:09.000000 gandai-1.3.5/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3757 2023-07-25 19:02:34.000000 gandai-1.3.5/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.3.5/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1373 2023-07-23 18:54:58.000000 gandai-1.3.5/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4285 2023-07-25 16:56:41.000000 gandai-1.3.5/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6151 2023-07-17 18:43:10.000000 gandai-1.3.5/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    31858 2023-07-25 20:16:58.000000 gandai-1.3.5/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2221 2023-07-17 18:43:09.000000 gandai-1.3.5/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.3.5/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    15985 2023-07-23 23:17:10.000000 gandai-1.3.5/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2368 2023-07-25 17:01:00.000000 gandai-1.3.5/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1759 2023-07-25 20:25:00.000000 gandai-1.3.5/gandai/auth.py
--rw-r--r--   0 parker     (501) staff       (20)     1200 2023-07-17 18:25:43.000000 gandai-1.3.5/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1631 2023-07-25 19:02:05.000000 gandai-1.3.5/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)      402 2023-07-23 18:54:56.000000 gandai-1.3.5/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)     3030 2023-07-23 20:20:45.000000 gandai-1.3.5/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:42:44.403641 gandai-1.3.5/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.3.5/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:42:44.404151 gandai-1.3.5/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.3.5/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.3.5/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.3.5/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.3.5/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.3.5/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:42:44.404772 gandai-1.3.5/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.3.5/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3061 2023-07-17 18:25:43.000000 gandai-1.3.5/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     2683 2023-07-17 18:25:43.000000 gandai-1.3.5/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    20866 2023-07-25 20:16:56.000000 gandai-1.3.5/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1069 2023-07-25 20:41:48.000000 gandai-1.3.5/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)    10783 2023-07-23 23:17:02.000000 gandai-1.3.5/gandai/sources.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-25 20:42:44.398217 gandai-1.3.5/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-25 20:42:44.000000 gandai-1.3.5/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1275 2023-07-25 20:42:44.000000 gandai-1.3.5/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-25 20:42:44.000000 gandai-1.3.5/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-07-25 20:42:44.000000 gandai-1.3.5/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      383 2023-07-25 20:42:13.000000 gandai-1.3.5/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-25 20:42:44.405170 gandai-1.3.5/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.3.5/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-26 17:55:47.838841 gandai-1.3.6/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.3.6/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-26 17:55:47.838725 gandai-1.3.6/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-26 17:55:47.833822 gandai-1.3.6/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)       46 2023-07-17 18:25:43.000000 gandai-1.3.6/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-26 17:55:47.836801 gandai-1.3.6/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      264 2023-07-17 18:43:09.000000 gandai-1.3.6/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.3.6/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4120 2023-07-25 17:01:01.000000 gandai-1.3.6/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-26 14:50:18.000000 gandai-1.3.6/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.3.6/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2023-07-17 18:43:09.000000 gandai-1.3.6/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3757 2023-07-25 19:02:34.000000 gandai-1.3.6/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.3.6/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1373 2023-07-23 18:54:58.000000 gandai-1.3.6/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4285 2023-07-26 14:50:18.000000 gandai-1.3.6/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6151 2023-07-17 18:43:10.000000 gandai-1.3.6/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    31858 2023-07-26 14:50:18.000000 gandai-1.3.6/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2221 2023-07-26 13:45:26.000000 gandai-1.3.6/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.3.6/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    17500 2023-07-26 17:54:47.000000 gandai-1.3.6/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2368 2023-07-25 17:01:00.000000 gandai-1.3.6/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1759 2023-07-25 20:25:00.000000 gandai-1.3.6/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1200 2023-07-17 18:25:43.000000 gandai-1.3.6/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1631 2023-07-25 19:02:05.000000 gandai-1.3.6/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)      402 2023-07-23 18:54:56.000000 gandai-1.3.6/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)     3030 2023-07-25 23:46:20.000000 gandai-1.3.6/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-26 17:55:47.837502 gandai-1.3.6/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.3.6/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-26 17:55:47.837978 gandai-1.3.6/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.3.6/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.3.6/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.3.6/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.3.6/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.3.6/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-26 17:55:47.838549 gandai-1.3.6/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.3.6/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3061 2023-07-17 18:25:43.000000 gandai-1.3.6/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     2683 2023-07-17 18:25:43.000000 gandai-1.3.6/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    20866 2023-07-26 14:03:27.000000 gandai-1.3.6/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1069 2023-07-25 20:41:48.000000 gandai-1.3.6/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)    11623 2023-07-26 17:54:47.000000 gandai-1.3.6/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-07-26 17:55:47.834247 gandai-1.3.6/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      214 2023-07-26 17:55:47.000000 gandai-1.3.6/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1275 2023-07-26 17:55:47.000000 gandai-1.3.6/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-07-26 17:55:47.000000 gandai-1.3.6/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-07-26 17:55:47.000000 gandai-1.3.6/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      383 2023-07-26 17:55:31.000000 gandai-1.3.6/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-07-26 17:55:47.838871 gandai-1.3.6/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.3.6/setup.py
```

### Comparing `gandai-1.3.5/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.3.6/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.3.6/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.3.6/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xa787b564 (Mon Jul 17 18:25:43 2023 UTC)
-files sz: 1822
+moddate:  0x9c2fc064 (Tue Jul 25 20:25:00 2023 UTC)
+files sz: 1759
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a036d
@@ -68,83 +68,83 @@
     10          82 LOAD_CONST               0 (0)
                 84 LOAD_CONST               6 (('access_secret_version',))
                 86 IMPORT_NAME             13 (gandai.secrets)
                 88 IMPORT_FROM             14 (access_secret_version)
                 90 STORE_NAME              14 (access_secret_version)
                 92 POP_TOP
    
-    17          94 BUILD_MAP                0
+    14          94 BUILD_MAP                0
                 96 STORE_NAME              15 (ds)
    
-    18          98 PUSH_NULL
+    15          98 PUSH_NULL
                100 LOAD_NAME               12 (Client)
    
-    19         102 PUSH_NULL
+    16         102 PUSH_NULL
                104 LOAD_NAME               14 (access_secret_version)
                106 LOAD_CONST               7 ('TWILIO_APP')
                108 PRECALL                  1
                112 CALL                     1
                122 PUSH_NULL
                124 LOAD_NAME               14 (access_secret_version)
                126 LOAD_CONST               8 ('TWILIO_TOKEN')
                128 PRECALL                  1
                132 CALL                     1
    
-    18         142 PRECALL                  2
+    15         142 PRECALL                  2
                146 CALL                     2
                156 STORE_NAME              16 (twilio_client)
    
-    23         158 LOAD_NAME                4 (dataclass)
+    20         158 LOAD_NAME                4 (dataclass)
    
-    24         160 PUSH_NULL
+    21         160 PUSH_NULL
                162 LOAD_BUILD_CLASS
-               164 LOAD_CONST               9 (<code object Auth, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 23>)
+               164 LOAD_CONST               9 (<code object Auth, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 20>)
                166 MAKE_FUNCTION            0
                168 LOAD_CONST              10 ('Auth')
                170 PRECALL                  2
                174 CALL                     2
    
-    23         184 PRECALL                  0
+    20         184 PRECALL                  0
                188 CALL                     0
    
-    24         198 STORE_NAME              17 (Auth)
+    21         198 STORE_NAME              17 (Auth)
    
-    40         200 LOAD_CONST              11 ('auth')
+    37         200 LOAD_CONST              11 ('auth')
                202 LOAD_NAME               17 (Auth)
                204 LOAD_CONST              12 ('return')
                206 LOAD_CONST               1 (None)
                208 BUILD_TUPLE              4
-               210 LOAD_CONST              13 (<code object _send_code, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 40>)
+               210 LOAD_CONST              13 (<code object _send_code, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 37>)
                212 MAKE_FUNCTION            4 (annotations)
                214 STORE_NAME              18 (_send_code)
    
-    49         216 LOAD_CONST              14 ('phone')
+    46         216 LOAD_CONST              14 ('phone')
                218 LOAD_NAME               19 (str)
                220 LOAD_CONST              12 ('return')
                222 LOAD_CONST               1 (None)
                224 BUILD_TUPLE              4
-               226 LOAD_CONST              15 (<code object send_code, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 49>)
+               226 LOAD_CONST              15 (<code object send_code, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 46>)
                228 MAKE_FUNCTION            4 (annotations)
                230 STORE_NAME              20 (send_code)
    
-    57         232 LOAD_CONST              16 ('code')
+    54         232 LOAD_CONST              16 ('code')
                234 LOAD_NAME               19 (str)
                236 LOAD_CONST              12 ('return')
                238 LOAD_NAME               17 (Auth)
                240 BUILD_TUPLE              4
-               242 LOAD_CONST              17 (<code object authenticate, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 57>)
+               242 LOAD_CONST              17 (<code object authenticate, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 54>)
                244 MAKE_FUNCTION            4 (annotations)
                246 STORE_NAME              21 (authenticate)
    
-    70         248 LOAD_CONST              18 ('token')
+    67         248 LOAD_CONST              18 ('token')
                250 LOAD_NAME               19 (str)
                252 LOAD_CONST              12 ('return')
                254 LOAD_NAME               22 (bool)
                256 BUILD_TUPLE              4
-               258 LOAD_CONST              19 (<code object validate, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 70>)
+               258 LOAD_CONST              19 (<code object validate, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 67>)
                260 MAKE_FUNCTION            4 (annotations)
                262 STORE_NAME              23 (validate)
                264 LOAD_CONST               1 (None)
                266 RETURN_VALUE
    consts
       0
       None
@@ -162,68 +162,68 @@
          flags     : 0
          code
             0x970065005a0164005a025500020065036401ac02a6010000ab01000000
             00000000005a046505650664033c0000006505650664043c000000650565
             0664053c000000020065036401ac02a6010000ab0100000000000000005a
             076508650664063c000000020065036401ac02a6010000ab010000000000
             0000005a096505650664073c000000640884005a0a64095300
-          23           0 RESUME                   0
+          20           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Auth')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          25          12 PUSH_NULL
+          22          12 PUSH_NULL
                       14 LOAD_NAME                3 (field)
                       16 LOAD_CONST               1 (False)
                       18 KW_NAMES                 2
                       20 PRECALL                  1
                       24 CALL                     1
                       34 STORE_NAME               4 (key)
                       36 LOAD_NAME                5 (str)
                       38 LOAD_NAME                6 (__annotations__)
                       40 LOAD_CONST               3 ('key')
                       42 STORE_SUBSCR
          
-          26          46 LOAD_NAME                5 (str)
+          23          46 LOAD_NAME                5 (str)
                       48 LOAD_NAME                6 (__annotations__)
                       50 LOAD_CONST               4 ('phone')
                       52 STORE_SUBSCR
          
-          27          56 LOAD_NAME                5 (str)
+          24          56 LOAD_NAME                5 (str)
                       58 LOAD_NAME                6 (__annotations__)
                       60 LOAD_CONST               5 ('code')
                       62 STORE_SUBSCR
          
-          28          66 PUSH_NULL
+          25          66 PUSH_NULL
                       68 LOAD_NAME                3 (field)
                       70 LOAD_CONST               1 (False)
                       72 KW_NAMES                 2
                       74 PRECALL                  1
                       78 CALL                     1
                       88 STORE_NAME               7 (expires)
                       90 LOAD_NAME                8 (int)
                       92 LOAD_NAME                6 (__annotations__)
                       94 LOAD_CONST               6 ('expires')
                       96 STORE_SUBSCR
          
-          29         100 PUSH_NULL
+          26         100 PUSH_NULL
                      102 LOAD_NAME                3 (field)
                      104 LOAD_CONST               1 (False)
                      106 KW_NAMES                 2
                      108 PRECALL                  1
                      112 CALL                     1
                      122 STORE_NAME               9 (token)
                      124 LOAD_NAME                5 (str)
                      126 LOAD_NAME                6 (__annotations__)
                      128 LOAD_CONST               7 ('token')
                      130 STORE_SUBSCR
          
-          31         134 LOAD_CONST               8 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 31>)
+          28         134 LOAD_CONST               8 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 28>)
                      136 MAKE_FUNCTION            0
                      138 STORE_NAME              10 (__post_init__)
                      140 LOAD_CONST               9 (None)
                      142 RETURN_VALUE
          consts
             'Auth'
             False
@@ -249,71 +249,71 @@
                   00000000007c017a0000007c005f06000000000000000064047c006a0300
                   000000000000009b0064057c006a0600000000000000009b009d047c005f
                   0700000000000000007411000000000000000000007c006a070000000000
                   000000a0090000000000000000000000000000000000000000a6000000ab
                   000000000000000000a6010000ab010000000000000000a00a0000000000
                   000000000000000000000000000000a6000000ab0000000000000000007c
                   005f0b000000000000000064005300
-                31           0 RESUME                   0
+                28           0 RESUME                   0
                
-                32           2 LOAD_GLOBAL              1 (NULL + len)
+                29           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_GLOBAL              3 (NULL + str)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (code)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 PRECALL                  1
                             56 CALL                     1
                             66 LOAD_CONST               1 (6)
                             68 COMPARE_OP               2 (==)
                             74 POP_JUMP_FORWARD_IF_TRUE     2 (to 80)
                             76 LOAD_ASSERTION_ERROR
                             78 RAISE_VARARGS            1
                
-                33     >>   80 LOAD_GLOBAL              1 (NULL + len)
+                30     >>   80 LOAD_GLOBAL              1 (NULL + len)
                             92 LOAD_GLOBAL              3 (NULL + str)
                            104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                3 (phone)
                            116 PRECALL                  1
                            120 CALL                     1
                            130 PRECALL                  1
                            134 CALL                     1
                            144 LOAD_CONST               2 (10)
                            146 COMPARE_OP               2 (==)
                            152 POP_JUMP_FORWARD_IF_TRUE     2 (to 158)
                            154 LOAD_ASSERTION_ERROR
                            156 RAISE_VARARGS            1
                
-                34     >>  158 LOAD_CONST               3 (604800)
+                31     >>  158 LOAD_CONST               3 (604800)
                            160 STORE_FAST               1 (SEVEN_DAYS)
                
-                35         162 LOAD_GLOBAL              9 (NULL + int)
+                32         162 LOAD_GLOBAL              9 (NULL + int)
                            174 LOAD_GLOBAL             11 (NULL + time)
                            186 PRECALL                  0
                            190 CALL                     0
                            200 PRECALL                  1
                            204 CALL                     1
                            214 LOAD_FAST                1 (SEVEN_DAYS)
                            216 BINARY_OP                0 (+)
                            220 LOAD_FAST                0 (self)
                            222 STORE_ATTR               6 (expires)
                
-                36         232 LOAD_CONST               4 ('auth/')
+                33         232 LOAD_CONST               4 ('auth/')
                            234 LOAD_FAST                0 (self)
                            236 LOAD_ATTR                3 (phone)
                            246 FORMAT_VALUE             0
                            248 LOAD_CONST               5 ('/')
                            250 LOAD_FAST                0 (self)
                            252 LOAD_ATTR                6 (expires)
                            262 FORMAT_VALUE             0
                            264 BUILD_STRING             4
                            266 LOAD_FAST                0 (self)
                            268 STORE_ATTR               7 (key)
                
-                37         278 LOAD_GLOBAL             17 (NULL + md5)
+                34         278 LOAD_GLOBAL             17 (NULL + md5)
                            290 LOAD_FAST                0 (self)
                            292 LOAD_ATTR                7 (key)
                            302 LOAD_METHOD              9 (encode)
                            324 PRECALL                  0
                            328 CALL                     0
                            338 PRECALL                  1
                            342 CALL                     1
@@ -333,24 +333,24 @@
                   '/'
                names      ('len', 'str', 'code', 'phone', 'int', 'time', 'expires', 'key', 'md5', 'encode', 'hexdigest', 'token')
                varnames   ('self', 'SEVEN_DAYS')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
                name       '__post_init__'
-               firstlineno 31
+               firstlineno 28
                lnotab 0x02014e014e01040146012e01
             None
          names      ('__name__', '__module__', '__qualname__', 'field', 'key', 'str', '__annotations__', 'expires', 'int', 'token', '__post_init__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
          name       'Auth'
-         firstlineno 23
+         firstlineno 20
          lnotab 0x0c0222010a010a0122012202
       'Auth'
       'auth'
       'return'
       code
          argcount  : 1
          nlocals   : 2
@@ -359,40 +359,40 @@
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007c006a03000000000000000074
             09000000000000000000006401a6010000ab0100000000000000007c006a
             0500000000000000009b0064029d02ac03a6030000ab0300000000000000
             007d01740d0000000000000000000064047c006a0300000000000000009b
             009d02a6010000ab010000000000000000010064005300
-          40           0 RESUME                   0
+          37           0 RESUME                   0
          
-          41           2 LOAD_GLOBAL              0 (twilio_client)
+          38           2 LOAD_GLOBAL              0 (twilio_client)
                       14 LOAD_ATTR                1 (messages)
                       24 LOAD_METHOD              2 (create)
          
-          42          46 LOAD_FAST                0 (auth)
+          39          46 LOAD_FAST                0 (auth)
                       48 LOAD_ATTR                3 (phone)
          
-          43          58 LOAD_GLOBAL              9 (NULL + access_secret_version)
+          40          58 LOAD_GLOBAL              9 (NULL + access_secret_version)
                       70 LOAD_CONST               1 ('TWILIO_NUMBER')
                       72 PRECALL                  1
                       76 CALL                     1
          
-          44          86 LOAD_FAST                0 (auth)
+          41          86 LOAD_FAST                0 (auth)
                       88 LOAD_ATTR                5 (code)
                       98 FORMAT_VALUE             0
                      100 LOAD_CONST               2 (' is your TargetSelect authentication code.')
                      102 BUILD_STRING             2
          
-          41         104 KW_NAMES                 3
+          38         104 KW_NAMES                 3
                      106 PRECALL                  3
                      110 CALL                     3
                      120 STORE_FAST               1 (message)
          
-          46         122 LOAD_GLOBAL             13 (NULL + print)
+          43         122 LOAD_GLOBAL             13 (NULL + print)
                      134 LOAD_CONST               4 ('Login Sent to ')
                      136 LOAD_FAST                0 (auth)
                      138 LOAD_ATTR                3 (phone)
                      148 FORMAT_VALUE             0
                      150 BUILD_STRING             2
                      152 PRECALL                  1
                      156 CALL                     1
@@ -407,15 +407,15 @@
             'Login Sent to '
          names      ('twilio_client', 'messages', 'create', 'phone', 'access_secret_version', 'code', 'print')
          varnames   ('auth', 'message')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
          name       '_send_code'
-         firstlineno 40
+         firstlineno 37
          lnotab 0x02012c010c011c0112fd1205
       'phone'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -423,45 +423,45 @@
             0x97007401000000000000000000007403000000000000000000006a0200
             0000000000000064016402a6020000ab020000000000000000a6010000ab
             0100000000000000007d017407000000000000000000007c007c01ac03a6
             020000ab0200000000000000007d027409000000000000000000007c02a6
             010000ab010000000000000000740a000000000000000000007c026a0600
             000000000000003c000000740f000000000000000000007c02a6010000ab
             010000000000000000010064005300
-          49           0 RESUME                   0
+          46           0 RESUME                   0
          
-          51           2 LOAD_GLOBAL              1 (NULL + str)
+          48           2 LOAD_GLOBAL              1 (NULL + str)
                       14 LOAD_GLOBAL              3 (NULL + random)
                       26 LOAD_ATTR                2 (randint)
                       36 LOAD_CONST               1 (100000)
                       38 LOAD_CONST               2 (999999)
                       40 PRECALL                  2
                       44 CALL                     2
                       54 PRECALL                  1
                       58 CALL                     1
                       68 STORE_FAST               1 (auth_code)
          
-          52          70 LOAD_GLOBAL              7 (NULL + Auth)
+          49          70 LOAD_GLOBAL              7 (NULL + Auth)
                       82 LOAD_FAST                0 (phone)
                       84 LOAD_FAST                1 (auth_code)
                       86 KW_NAMES                 3
                       88 PRECALL                  2
                       92 CALL                     2
                      102 STORE_FAST               2 (auth)
          
-          53         104 LOAD_GLOBAL              9 (NULL + asdict)
+          50         104 LOAD_GLOBAL              9 (NULL + asdict)
                      116 LOAD_FAST                2 (auth)
                      118 PRECALL                  1
                      122 CALL                     1
                      132 LOAD_GLOBAL             10 (ds)
                      144 LOAD_FAST                2 (auth)
                      146 LOAD_ATTR                6 (key)
                      156 STORE_SUBSCR
          
-          54         160 LOAD_GLOBAL             15 (NULL + _send_code)
+          51         160 LOAD_GLOBAL             15 (NULL + _send_code)
                      172 LOAD_FAST                2 (auth)
                      174 PRECALL                  1
                      178 CALL                     1
                      188 POP_TOP
                      190 LOAD_CONST               0 (None)
                      192 RETURN_VALUE
          consts
@@ -471,15 +471,15 @@
             ('phone', 'code')
          names      ('str', 'random', 'randint', 'Auth', 'asdict', 'ds', 'key', '_send_code')
          varnames   ('phone', 'auth_code', 'auth')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
          name       'send_code'
-         firstlineno 49
+         firstlineno 46
          lnotab 0x0202440122013801
       'code'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -493,94 +493,94 @@
             00740d00000000000000000000a6000000ab000000000000000000a60100
             00ab0100000000000000006b0400000000190000000000000000007d027c
             027c026403190000000000000000007c006b020000000019000000000000
             0000007d02740f000000000000000000007c02a6010000ab010000000000
             00000064046b0400000000721c7c02a00800000000000000000000000000
             000000000000006405ac06a6010000ab0100000000000000006404190000
             00000000000000530064005300
-          57           0 RESUME                   0
+          54           0 RESUME                   0
          
-          58           2 LOAD_FAST                0 (code)
+          55           2 LOAD_FAST                0 (code)
                        4 LOAD_METHOD              0 (strip)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               0 (code)
          
-          59          42 LOAD_GLOBAL              2 (ds)
+          56          42 LOAD_GLOBAL              2 (ds)
                       54 LOAD_METHOD              2 (keys)
                       76 PRECALL                  0
                       80 CALL                     0
                       90 STORE_FAST               1 (keys)
          
-          60          92 LOAD_GLOBAL              7 (NULL + pd)
+          57          92 LOAD_GLOBAL              7 (NULL + pd)
                      104 LOAD_ATTR                4 (DataFrame)
-                     114 LOAD_CONST               1 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 60>)
+                     114 LOAD_CONST               1 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py", line 57>)
                      116 MAKE_FUNCTION            0
                      118 LOAD_FAST                1 (keys)
                      120 GET_ITER
                      122 PRECALL                  0
                      126 CALL                     0
                      136 PRECALL                  1
                      140 CALL                     1
                      150 STORE_FAST               2 (df)
          
-          61         152 LOAD_FAST                2 (df)
+          58         152 LOAD_FAST                2 (df)
                      154 LOAD_FAST                2 (df)
                      156 LOAD_CONST               2 ('expires')
                      158 BINARY_SUBSCR
                      168 LOAD_GLOBAL             11 (NULL + int)
                      180 LOAD_GLOBAL             13 (NULL + time)
                      192 PRECALL                  0
                      196 CALL                     0
                      206 PRECALL                  1
                      210 CALL                     1
                      220 COMPARE_OP               4 (>)
                      226 BINARY_SUBSCR
                      236 STORE_FAST               2 (df)
          
-          62         238 LOAD_FAST                2 (df)
+          59         238 LOAD_FAST                2 (df)
                      240 LOAD_FAST                2 (df)
                      242 LOAD_CONST               3 ('code')
                      244 BINARY_SUBSCR
                      254 LOAD_FAST                0 (code)
                      256 COMPARE_OP               2 (==)
                      262 BINARY_SUBSCR
                      272 STORE_FAST               2 (df)
          
-          63         274 LOAD_GLOBAL             15 (NULL + len)
+          60         274 LOAD_GLOBAL             15 (NULL + len)
                      286 LOAD_FAST                2 (df)
                      288 PRECALL                  1
                      292 CALL                     1
                      302 LOAD_CONST               4 (0)
                      304 COMPARE_OP               4 (>)
                      310 POP_JUMP_FORWARD_IF_FALSE    28 (to 368)
          
-          65         312 LOAD_FAST                2 (df)
+          62         312 LOAD_FAST                2 (df)
                      314 LOAD_METHOD              8 (to_dict)
                      336 LOAD_CONST               5 ('records')
                      338 KW_NAMES                 6
                      340 PRECALL                  1
                      344 CALL                     1
                      354 LOAD_CONST               4 (0)
                      356 BINARY_SUBSCR
                      366 RETURN_VALUE
          
-          67     >>  368 LOAD_CONST               0 (None)
+          64     >>  368 LOAD_CONST               0 (None)
                      370 RETURN_VALUE
          consts
             None
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 19
                code
                   0x970067007c005d0f7d017400000000000000000000007c011900000000
                   000000000091028c105300
-                60           0 RESUME                   0
+                57           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                15 (to 38)
                              8 STORE_FAST               1 (k)
                             10 LOAD_GLOBAL              0 (ds)
                             22 LOAD_FAST                1 (k)
                             24 BINARY_SUBSCR
@@ -590,53 +590,53 @@
                consts
                names      ('ds',)
                varnames   ('.0', 'k')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
                name       '<listcomp>'
-               firstlineno 60
+               firstlineno 57
                lnotab 0x
             'expires'
             'code'
             0
             'records'
             ('orient',)
          names      ('strip', 'ds', 'keys', 'pd', 'DataFrame', 'int', 'time', 'len', 'to_dict')
          varnames   ('code', 'keys', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
          name       'authenticate'
-         firstlineno 57
+         firstlineno 54
          lnotab 0x0201280132013c015601240126023802
       'token'
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 1
          flags     : 3
          code 0x970064005300
-          70           0 RESUME                   0
+          67           0 RESUME                   0
          
-          71           2 LOAD_CONST               0 (None)
+          68           2 LOAD_CONST               0 (None)
                        4 RETURN_VALUE
          consts
             None
          names      ()
          varnames   ('token',)
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
          name       'validate'
-         firstlineno 70
+         firstlineno 67
          lnotab 0x0201
    names      ('os', 'random', 'dataclasses', 'asdict', 'dataclass', 'field', 'hashlib', 'md5', 'time', 'pandas', 'pd', 'twilio.rest', 'Client', 'gandai.secrets', 'access_secret_version', 'ds', 'twilio_client', 'Auth', '_send_code', 'str', 'send_code', 'authenticate', 'bool', 'validate')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/auth.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010801080114010c010c0208010c020c070401040128ff100502
+      0x00ff02010801080114010c010c0208010c020c040401040128ff100502
       0118ff0e01021010091008100d
```

### Comparing `gandai-1.3.5/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.3.6/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.3.6/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.3.6/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.3.6/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.3.6/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.3.6/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x9d8bbd64 (Sun Jul 23 20:20:45 2023 UTC)
+moddate:  0xcc5ec064 (Tue Jul 25 23:46:20 2023 UTC)
 files sz: 3030
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `gandai-1.3.5/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.3.6/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.3.6/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xb82dc064 (Tue Jul 25 20:16:56 2023 UTC)
+moddate:  0xaf27c164 (Wed Jul 26 14:03:27 2023 UTC)
 files sz: 20866
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `gandai-1.3.5/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.3.6/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xa787b564 (Mon Jul 17 18:25:43 2023 UTC)
+moddate:  0x8c33c064 (Tue Jul 25 20:41:48 2023 UTC)
 files sz: 1069
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `gandai-1.3.5/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.3.6/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.3.6/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,130 +1,135 @@
 magic:    0xa70d0d0a
-moddate:  0xeeb4bd64 (Sun Jul 23 23:17:02 2023 UTC)
-files sz: 10783
+moddate:  0xe75dc164 (Wed Jul 26 17:54:47 2023 UTC)
+files sz: 11623
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c005a00640064026c016d025a020100640064036c036d
-      045a040100640064046c056d065a060100640064016c075a07640064016c
-      085a08640064056c096d0a5a0a6d0b5a0b6d0c5a0c6d0d5a0d6d0e5a0e01
-      00640064066c0f6d105a100100020065076a110000000000000000020065
-      0e6a1200000000000000006407a6010000ab010000000000000000ac08a6
-      010000ab0100000000000000005a1364095a1402004700640a8400640ba6
-      020000ab0200000000000000005a1502004700640c8400640da6020000ab
-      0200000000000000005a1602004700640e8400640fa6020000ab02000000
-      00000000005a1764015300
+      0x9700640064016c005a00640064016c015a02640064026c036d045a0401
+      00640064036c056d065a060100640064046c076d085a080100640064016c
+      095a09640064016c0a5a0a640064056c0b6d0c5a0c6d0d5a0d6d0e5a0e6d
+      0f5a0f6d105a100100640064066c116d125a120100020065096a13000000
+      0000000000020065106a1400000000000000006407a6010000ab01000000
+      0000000000ac08a6010000ab0100000000000000005a1564095a16020047
+      00640a8400640ba6020000ab0200000000000000005a1702004700640c84
+      00640da6020000ab0200000000000000005a1802004700640e8400640fa6
+      020000ab0200000000000000005a1964015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (time)
                  8 STORE_NAME               0 (time)
    
      2          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               2 (('ThreadPoolExecutor',))
-                14 IMPORT_NAME              1 (concurrent.futures)
-                16 IMPORT_FROM              2 (ThreadPoolExecutor)
-                18 STORE_NAME               2 (ThreadPoolExecutor)
-                20 POP_TOP
+                12 LOAD_CONST               1 (None)
+                14 IMPORT_NAME              1 (pandas)
+                16 STORE_NAME               2 (pd)
    
-     3          22 LOAD_CONST               0 (0)
-                24 LOAD_CONST               3 (('partial',))
-                26 IMPORT_NAME              3 (functools)
-                28 IMPORT_FROM              4 (partial)
-                30 STORE_NAME               4 (partial)
-                32 POP_TOP
+     3          18 LOAD_CONST               0 (0)
+                20 LOAD_CONST               2 (('ThreadPoolExecutor',))
+                22 IMPORT_NAME              3 (concurrent.futures)
+                24 IMPORT_FROM              4 (ThreadPoolExecutor)
+                26 STORE_NAME               4 (ThreadPoolExecutor)
+                28 POP_TOP
    
-     4          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               4 (('List',))
-                38 IMPORT_NAME              5 (typing)
-                40 IMPORT_FROM              6 (List)
-                42 STORE_NAME               6 (List)
-                44 POP_TOP
+     4          30 LOAD_CONST               0 (0)
+                32 LOAD_CONST               3 (('partial',))
+                34 IMPORT_NAME              5 (functools)
+                36 IMPORT_FROM              6 (partial)
+                38 STORE_NAME               6 (partial)
+                40 POP_TOP
    
-     6          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               1 (None)
-                50 IMPORT_NAME              7 (googlemaps)
-                52 STORE_NAME               7 (googlemaps)
+     5          42 LOAD_CONST               0 (0)
+                44 LOAD_CONST               4 (('List',))
+                46 IMPORT_NAME              7 (typing)
+                48 IMPORT_FROM              8 (List)
+                50 STORE_NAME               8 (List)
+                52 POP_TOP
    
      7          54 LOAD_CONST               0 (0)
                 56 LOAD_CONST               1 (None)
-                58 IMPORT_NAME              8 (requests)
-                60 STORE_NAME               8 (requests)
+                58 IMPORT_NAME              9 (googlemaps)
+                60 STORE_NAME               9 (googlemaps)
    
-     9          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               5 (('gpt', 'helpers', 'models', 'query', 'secrets'))
-                66 IMPORT_NAME              9 (gandai)
-                68 IMPORT_FROM             10 (gpt)
-                70 STORE_NAME              10 (gpt)
-                72 IMPORT_FROM             11 (helpers)
-                74 STORE_NAME              11 (helpers)
-                76 IMPORT_FROM             12 (models)
-                78 STORE_NAME              12 (models)
-                80 IMPORT_FROM             13 (query)
-                82 STORE_NAME              13 (query)
-                84 IMPORT_FROM             14 (secrets)
-                86 STORE_NAME              14 (secrets)
-                88 POP_TOP
+     8          62 LOAD_CONST               0 (0)
+                64 LOAD_CONST               1 (None)
+                66 IMPORT_NAME             10 (requests)
+                68 STORE_NAME              10 (requests)
    
-    10          90 LOAD_CONST               0 (0)
-                92 LOAD_CONST               6 (('Search',))
-                94 IMPORT_NAME             15 (gandai.models)
-                96 IMPORT_FROM             16 (Search)
-                98 STORE_NAME              16 (Search)
-               100 POP_TOP
+    10          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               5 (('gpt', 'helpers', 'models', 'query', 'secrets'))
+                74 IMPORT_NAME             11 (gandai)
+                76 IMPORT_FROM             12 (gpt)
+                78 STORE_NAME              12 (gpt)
+                80 IMPORT_FROM             13 (helpers)
+                82 STORE_NAME              13 (helpers)
+                84 IMPORT_FROM             14 (models)
+                86 STORE_NAME              14 (models)
+                88 IMPORT_FROM             15 (query)
+                90 STORE_NAME              15 (query)
+                92 IMPORT_FROM             16 (secrets)
+                94 STORE_NAME              16 (secrets)
+                96 POP_TOP
    
-    12         102 PUSH_NULL
-               104 LOAD_NAME                7 (googlemaps)
-               106 LOAD_ATTR               17 (Client)
-               116 PUSH_NULL
-               118 LOAD_NAME               14 (secrets)
-               120 LOAD_ATTR               18 (access_secret_version)
-               130 LOAD_CONST               7 ('GOOLE_MAPS_KEY')
-               132 PRECALL                  1
-               136 CALL                     1
-               146 KW_NAMES                 8
-               148 PRECALL                  1
-               152 CALL                     1
-               162 STORE_NAME              19 (gmaps)
+    11          98 LOAD_CONST               0 (0)
+               100 LOAD_CONST               6 (('Search',))
+               102 IMPORT_NAME             17 (gandai.models)
+               104 IMPORT_FROM             18 (Search)
+               106 STORE_NAME              18 (Search)
+               108 POP_TOP
    
-    13         164 LOAD_CONST               9 (25)
-               166 STORE_NAME              20 (MAX_WORKERS)
+    13         110 PUSH_NULL
+               112 LOAD_NAME                9 (googlemaps)
+               114 LOAD_ATTR               19 (Client)
+               124 PUSH_NULL
+               126 LOAD_NAME               16 (secrets)
+               128 LOAD_ATTR               20 (access_secret_version)
+               138 LOAD_CONST               7 ('GOOLE_MAPS_KEY')
+               140 PRECALL                  1
+               144 CALL                     1
+               154 KW_NAMES                 8
+               156 PRECALL                  1
+               160 CALL                     1
+               170 STORE_NAME              21 (gmaps)
    
-    16         168 PUSH_NULL
-               170 LOAD_BUILD_CLASS
-               172 LOAD_CONST              10 (<code object GoogleMapsWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 16>)
-               174 MAKE_FUNCTION            0
-               176 LOAD_CONST              11 ('GoogleMapsWrapper')
-               178 PRECALL                  2
-               182 CALL                     2
-               192 STORE_NAME              21 (GoogleMapsWrapper)
+    14         172 LOAD_CONST               9 (25)
+               174 STORE_NAME              22 (MAX_WORKERS)
    
-   171         194 PUSH_NULL
-               196 LOAD_BUILD_CLASS
-               198 LOAD_CONST              12 (<code object GrataWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 171>)
-               200 MAKE_FUNCTION            0
-               202 LOAD_CONST              13 ('GrataWrapper')
-               204 PRECALL                  2
-               208 CALL                     2
-               218 STORE_NAME              22 (GrataWrapper)
+    17         176 PUSH_NULL
+               178 LOAD_BUILD_CLASS
+               180 LOAD_CONST              10 (<code object GoogleMapsWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 17>)
+               182 MAKE_FUNCTION            0
+               184 LOAD_CONST              11 ('GoogleMapsWrapper')
+               186 PRECALL                  2
+               190 CALL                     2
+               200 STORE_NAME              23 (GoogleMapsWrapper)
    
-   325         220 PUSH_NULL
-               222 LOAD_BUILD_CLASS
-               224 LOAD_CONST              14 (<code object SourceScrubWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 325>)
-               226 MAKE_FUNCTION            0
-               228 LOAD_CONST              15 ('SourceScrubWrapper')
-               230 PRECALL                  2
-               234 CALL                     2
-               244 STORE_NAME              23 (SourceScrubWrapper)
-               246 LOAD_CONST               1 (None)
-               248 RETURN_VALUE
+   172         202 PUSH_NULL
+               204 LOAD_BUILD_CLASS
+               206 LOAD_CONST              12 (<code object GrataWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 172>)
+               208 MAKE_FUNCTION            0
+               210 LOAD_CONST              13 ('GrataWrapper')
+               212 PRECALL                  2
+               216 CALL                     2
+               226 STORE_NAME              24 (GrataWrapper)
+   
+   344         228 PUSH_NULL
+               230 LOAD_BUILD_CLASS
+               232 LOAD_CONST              14 (<code object SourceScrubWrapper, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 344>)
+               234 MAKE_FUNCTION            0
+               236 LOAD_CONST              15 ('SourceScrubWrapper')
+               238 PRECALL                  2
+               242 CALL                     2
+               252 STORE_NAME              25 (SourceScrubWrapper)
+               254 LOAD_CONST               1 (None)
+               256 RETURN_VALUE
    consts
       0
       None
       ('ThreadPoolExecutor',)
       ('partial',)
       ('List',)
       ('gpt', 'helpers', 'models', 'query', 'secrets')
@@ -143,151 +148,151 @@
             04a6000000ab0000000000000000005a0865030900641664086504640965
             09650419000000000000000000640a650a6403650b6608640b8405a60000
             00ab0000000000000000005a0c650309006416640c650464086504640a65
             0a6403650b6608640d8405a6000000ab0000000000000000005a0d650309
             00641764056504640f650a641065046403650e6a0f000000000000000066
             0864118405a6000000ab0000000000000000005a106412650b6413650e6a
             1100000000000000006604641484045a12640e5300
-          16           0 RESUME                   0
+          17           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GoogleMapsWrapper')
                        8 STORE_NAME               2 (__qualname__)
          
-          17          10 LOAD_NAME                3 (staticmethod)
+          18          10 LOAD_NAME                3 (staticmethod)
          
-          18          12 LOAD_CONST              21 (('San Diego, CA',))
+          19          12 LOAD_CONST              21 (('San Diego, CA',))
                       14 LOAD_CONST               2 ('text')
                       16 LOAD_NAME                4 (str)
                       18 LOAD_CONST               3 ('return')
                       20 LOAD_NAME                5 (tuple)
                       22 BUILD_TUPLE              4
-                      24 LOAD_CONST               4 (<code object get_loc, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 17>)
+                      24 LOAD_CONST               4 (<code object get_loc, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 18>)
                       26 MAKE_FUNCTION            5 (defaults, annotations)
          
-          17          28 PRECALL                  0
+          18          28 PRECALL                  0
                       32 CALL                     0
          
-          18          42 STORE_NAME               6 (get_loc)
+          19          42 STORE_NAME               6 (get_loc)
          
-          22          44 LOAD_NAME                3 (staticmethod)
+          23          44 LOAD_NAME                3 (staticmethod)
          
-          23          46 LOAD_CONST               5 ('place_id')
+          24          46 LOAD_CONST               5 ('place_id')
                       48 LOAD_NAME                4 (str)
                       50 LOAD_CONST               3 ('return')
                       52 LOAD_NAME                7 (dict)
                       54 BUILD_TUPLE              4
-                      56 LOAD_CONST               6 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 22>)
+                      56 LOAD_CONST               6 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 23>)
                       58 MAKE_FUNCTION            4 (annotations)
          
-          22          60 PRECALL                  0
+          23          60 PRECALL                  0
                       64 CALL                     0
          
-          23          74 STORE_NAME               8 (enrich)
+          24          74 STORE_NAME               8 (enrich)
          
-          27          76 LOAD_NAME                3 (staticmethod)
+          28          76 LOAD_NAME                3 (staticmethod)
          
-          29          78 NOP
+          30          78 NOP
          
-          28          80 LOAD_CONST              22 ((25,))
+          29          80 LOAD_CONST              22 ((25,))
                       82 LOAD_CONST               8 ('search_phrase')
          
-          29          84 LOAD_NAME                4 (str)
+          30          84 LOAD_NAME                4 (str)
          
-          28          86 LOAD_CONST               9 ('locations')
+          29          86 LOAD_CONST               9 ('locations')
          
-          29          88 LOAD_NAME                9 (List)
+          30          88 LOAD_NAME                9 (List)
                       90 LOAD_NAME                4 (str)
                       92 BINARY_SUBSCR
          
-          28         102 LOAD_CONST              10 ('radius_miles')
+          29         102 LOAD_CONST              10 ('radius_miles')
          
-          29         104 LOAD_NAME               10 (int)
+          30         104 LOAD_NAME               10 (int)
          
-          28         106 LOAD_CONST               3 ('return')
+          29         106 LOAD_CONST               3 ('return')
          
-          30         108 LOAD_NAME               11 (list)
+          31         108 LOAD_NAME               11 (list)
          
-          28         110 BUILD_TUPLE              8
-                     112 LOAD_CONST              11 (<code object fetch_unique_place_ids, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 27>)
+          29         110 BUILD_TUPLE              8
+                     112 LOAD_CONST              11 (<code object fetch_unique_place_ids, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 28>)
                      114 MAKE_FUNCTION            5 (defaults, annotations)
          
-          27         116 PRECALL                  0
+          28         116 PRECALL                  0
                      120 CALL                     0
          
-          28         130 STORE_NAME              12 (fetch_unique_place_ids)
+          29         130 STORE_NAME              12 (fetch_unique_place_ids)
          
-          50         132 LOAD_NAME                3 (staticmethod)
+          51         132 LOAD_NAME                3 (staticmethod)
          
-          52         134 NOP
+          53         134 NOP
          
-          51         136 LOAD_CONST              22 ((25,))
+          52         136 LOAD_CONST              22 ((25,))
                      138 LOAD_CONST              12 ('location_text')
          
-          52         140 LOAD_NAME                4 (str)
+          53         140 LOAD_NAME                4 (str)
          
-          51         142 LOAD_CONST               8 ('search_phrase')
+          52         142 LOAD_CONST               8 ('search_phrase')
          
-          52         144 LOAD_NAME                4 (str)
+          53         144 LOAD_NAME                4 (str)
          
-          51         146 LOAD_CONST              10 ('radius_miles')
+          52         146 LOAD_CONST              10 ('radius_miles')
          
-          52         148 LOAD_NAME               10 (int)
+          53         148 LOAD_NAME               10 (int)
          
-          51         150 LOAD_CONST               3 ('return')
+          52         150 LOAD_CONST               3 ('return')
          
-          53         152 LOAD_NAME               11 (list)
+          54         152 LOAD_NAME               11 (list)
          
-          51         154 BUILD_TUPLE              8
-                     156 LOAD_CONST              13 (<code object _fetch_place_ids, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 50>)
+          52         154 BUILD_TUPLE              8
+                     156 LOAD_CONST              13 (<code object _fetch_place_ids, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 51>)
                      158 MAKE_FUNCTION            5 (defaults, annotations)
          
-          50         160 PRECALL                  0
+          51         160 PRECALL                  0
                      164 CALL                     0
          
-          51         174 STORE_NAME              13 (_fetch_place_ids)
+          52         174 STORE_NAME              13 (_fetch_place_ids)
          
-          90         176 LOAD_NAME                3 (staticmethod)
+          91         176 LOAD_NAME                3 (staticmethod)
          
-          92         178 NOP
+          93         178 NOP
          
-          91         180 LOAD_CONST              23 ((None,))
+          92         180 LOAD_CONST              23 ((None,))
                      182 LOAD_CONST               5 ('place_id')
          
-          92         184 LOAD_NAME                4 (str)
+          93         184 LOAD_NAME                4 (str)
          
-          91         186 LOAD_CONST              15 ('search_uid')
+          92         186 LOAD_CONST              15 ('search_uid')
          
-          92         188 LOAD_NAME               10 (int)
+          93         188 LOAD_NAME               10 (int)
          
-          91         190 LOAD_CONST              16 ('append_to_prompt')
+          92         190 LOAD_CONST              16 ('append_to_prompt')
          
-          92         192 LOAD_NAME                4 (str)
+          93         192 LOAD_NAME                4 (str)
          
-          91         194 LOAD_CONST               3 ('return')
+          92         194 LOAD_CONST               3 ('return')
          
-          93         196 LOAD_NAME               14 (models)
+          94         196 LOAD_NAME               14 (models)
                      198 LOAD_ATTR               15 (Company)
          
-          91         208 BUILD_TUPLE              8
-                     210 LOAD_CONST              17 (<code object build_target_from_place_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 90>)
+          92         208 BUILD_TUPLE              8
+                     210 LOAD_CONST              17 (<code object build_target_from_place_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 91>)
                      212 MAKE_FUNCTION            5 (defaults, annotations)
          
-          90         214 PRECALL                  0
+          91         214 PRECALL                  0
                      218 CALL                     0
          
-          91         228 STORE_NAME              16 (build_target_from_place_id)
+          92         228 STORE_NAME              16 (build_target_from_place_id)
          
-         161         230 LOAD_CONST              18 ('place_ids')
+         162         230 LOAD_CONST              18 ('place_ids')
                      232 LOAD_NAME               11 (list)
                      234 LOAD_CONST              19 ('search')
                      236 LOAD_NAME               14 (models)
                      238 LOAD_ATTR               17 (Search)
                      248 BUILD_TUPLE              4
-                     250 LOAD_CONST              20 (<code object build_place_ids_async, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 161>)
+                     250 LOAD_CONST              20 (<code object build_place_ids_async, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 162>)
                      252 MAKE_FUNCTION            4 (annotations)
                      254 STORE_NAME              18 (build_place_ids_async)
                      256 LOAD_CONST              14 (None)
                      258 RETURN_VALUE
          consts
             'GoogleMapsWrapper'
             'San Diego, CA'
@@ -301,24 +306,24 @@
                code
                   0x9700740000000000000000000000a00100000000000000000000000000
                   000000000000007c00a6010000ab0100000000000000007d017405000000
                   000000000000007c01640119000000000000000000640219000000000000
                   000000640319000000000000000000a00300000000000000000000000000
                   00000000000000a6000000ab000000000000000000a6010000ab01000000
                   00000000005300
-                17           0 RESUME                   0
+                18           0 RESUME                   0
                
-                19           2 LOAD_GLOBAL              0 (gmaps)
+                20           2 LOAD_GLOBAL              0 (gmaps)
                             14 LOAD_METHOD              1 (geocode)
                             36 LOAD_FAST                0 (text)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               1 (resp)
                
-                20          54 LOAD_GLOBAL              5 (NULL + tuple)
+                21          54 LOAD_GLOBAL              5 (NULL + tuple)
                             66 LOAD_FAST                1 (resp)
                             68 LOAD_CONST               1 (0)
                             70 BINARY_SUBSCR
                             80 LOAD_CONST               2 ('geometry')
                             82 BINARY_SUBSCR
                             92 LOAD_CONST               3 ('location')
                             94 BINARY_SUBSCR
@@ -335,51 +340,51 @@
                   'location'
                names      ('gmaps', 'geocode', 'tuple', 'values')
                varnames   ('text', 'resp')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'get_loc'
-               firstlineno 17
+               firstlineno 18
                lnotab 0x02023401
             'place_id'
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x9700740000000000000000000000a00100000000000000000000000000
                   000000000000007c00ac01a6010000ab0100000000000000007d017c0164
                   02190000000000000000005300
-                22           0 RESUME                   0
+                23           0 RESUME                   0
                
-                24           2 LOAD_GLOBAL              0 (gmaps)
+                25           2 LOAD_GLOBAL              0 (gmaps)
                             14 LOAD_METHOD              1 (place)
                             36 LOAD_FAST                0 (place_id)
                             38 KW_NAMES                 1
                             40 PRECALL                  1
                             44 CALL                     1
                             54 STORE_FAST               1 (resp)
                
-                25          56 LOAD_FAST                1 (resp)
+                26          56 LOAD_FAST                1 (resp)
                             58 LOAD_CONST               2 ('result')
                             60 BINARY_SUBSCR
                             70 RETURN_VALUE
                consts
                   None
                   ('place_id',)
                   'result'
                names      ('gmaps', 'place')
                varnames   ('place_id', 'resp')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'enrich'
-               firstlineno 22
+               firstlineno 23
                lnotab 0x02023601
             25
             'search_phrase'
             'locations'
             'radius_miles'
             code
                argcount  : 3
@@ -398,47 +403,47 @@
                   0000007c07a6010000ab010000000000000000a6010000ab010000000000
                   00000001008c262300741000000000000000000000240072197d08741300
                   0000000000000000007c08a6010000ab0100000000000000000100590064
                   007d087e088c4464007d087e0877017700780359007701740f0000000000
                   00000000007415000000000000000000007c06a6010000ab010000000000
                   000000a6010000ab0100000000000000007d067417000000000000000000
                   007c06a6010000ab01000000000000000001007c065300
-                27           0 RESUME                   0
+                28           0 RESUME                   0
                
-                31           2 LOAD_GLOBAL              1 (NULL + partial)
+                32           2 LOAD_GLOBAL              1 (NULL + partial)
                
-                32          14 LOAD_GLOBAL              2 (GoogleMapsWrapper)
+                33          14 LOAD_GLOBAL              2 (GoogleMapsWrapper)
                             26 LOAD_ATTR                2 (_fetch_place_ids)
                
-                33          36 LOAD_FAST                0 (search_phrase)
+                34          36 LOAD_FAST                0 (search_phrase)
                
-                34          38 LOAD_FAST                2 (radius_miles)
+                35          38 LOAD_FAST                2 (radius_miles)
                
-                31          40 KW_NAMES                 1
+                32          40 KW_NAMES                 1
                             42 PRECALL                  3
                             46 CALL                     3
                             56 STORE_FAST               3 (main_func)
                
-                36          58 LOAD_GLOBAL              7 (NULL + ThreadPoolExecutor)
+                37          58 LOAD_GLOBAL              7 (NULL + ThreadPoolExecutor)
                             70 LOAD_GLOBAL              8 (MAX_WORKERS)
                             82 KW_NAMES                 2
                             84 PRECALL                  1
                             88 CALL                     1
                             98 BEFORE_WITH
                            100 STORE_FAST               4 (exec)
                
-                37         102 LOAD_FAST                4 (exec)
+                38         102 LOAD_FAST                4 (exec)
                            104 LOAD_METHOD              5 (map)
                            126 LOAD_FAST                3 (main_func)
                            128 LOAD_FAST                1 (locations)
                            130 PRECALL                  2
                            134 CALL                     2
                            144 STORE_FAST               5 (futures)
                
-                36         146 LOAD_CONST               0 (None)
+                37         146 LOAD_CONST               0 (None)
                            148 LOAD_CONST               0 (None)
                            150 LOAD_CONST               0 (None)
                            152 PRECALL                  2
                            156 CALL                     2
                            166 POP_TOP
                            168 JUMP_FORWARD            11 (to 192)
                        >>  170 PUSH_EXC_INFO
@@ -449,77 +454,77 @@
                            180 POP_EXCEPT
                            182 RERAISE                  1
                        >>  184 POP_TOP
                            186 POP_EXCEPT
                            188 POP_TOP
                            190 POP_TOP
                
-                39     >>  192 BUILD_LIST               0
+                40     >>  192 BUILD_LIST               0
                            194 STORE_FAST               6 (place_ids)
                
-                40         196 LOAD_FAST                5 (futures)
+                41         196 LOAD_FAST                5 (futures)
                            198 GET_ITER
                        >>  200 FOR_ITER                75 (to 352)
                            202 STORE_FAST               7 (future)
                
-                41         204 NOP
+                42         204 NOP
                
-                42         206 LOAD_FAST                6 (place_ids)
+                43         206 LOAD_FAST                6 (place_ids)
                            208 LOAD_METHOD              6 (extend)
                            230 LOAD_GLOBAL             15 (NULL + list)
                            242 LOAD_FAST                7 (future)
                            244 PRECALL                  1
                            248 CALL                     1
                            258 PRECALL                  1
                            262 CALL                     1
                            272 POP_TOP
                            274 JUMP_BACKWARD           38 (to 200)
                        >>  276 PUSH_EXC_INFO
                
-                43         278 LOAD_GLOBAL             16 (Exception)
+                44         278 LOAD_GLOBAL             16 (Exception)
                            290 CHECK_EXC_MATCH
                            292 POP_JUMP_FORWARD_IF_FALSE    25 (to 344)
                            294 STORE_FAST               8 (e)
                
-                44         296 LOAD_GLOBAL             19 (NULL + print)
+                45         296 LOAD_GLOBAL             19 (NULL + print)
                            308 LOAD_FAST                8 (e)
                            310 PRECALL                  1
                            314 CALL                     1
                            324 POP_TOP
                            326 POP_EXCEPT
                            328 LOAD_CONST               0 (None)
                            330 STORE_FAST               8 (e)
                            332 DELETE_FAST              8 (e)
                            334 JUMP_BACKWARD           68 (to 200)
                        >>  336 LOAD_CONST               0 (None)
                            338 STORE_FAST               8 (e)
                            340 DELETE_FAST              8 (e)
                            342 RERAISE                  1
                
-                43     >>  344 RERAISE                  0
+                44     >>  344 RERAISE                  0
                        >>  346 COPY                     3
                            348 POP_EXCEPT
                            350 RERAISE                  1
                
-                46     >>  352 LOAD_GLOBAL             15 (NULL + list)
+                47     >>  352 LOAD_GLOBAL             15 (NULL + list)
                            364 LOAD_GLOBAL             21 (NULL + set)
                            376 LOAD_FAST                6 (place_ids)
                            378 PRECALL                  1
                            382 CALL                     1
                            392 PRECALL                  1
                            396 CALL                     1
                            406 STORE_FAST               6 (place_ids)
                
-                47         408 LOAD_GLOBAL             23 (NULL + len)
+                48         408 LOAD_GLOBAL             23 (NULL + len)
                            420 LOAD_FAST                6 (place_ids)
                            422 PRECALL                  1
                            426 CALL                     1
                            436 POP_TOP
                
-                48         438 LOAD_FAST                6 (place_ids)
+                49         438 LOAD_FAST                6 (place_ids)
                            440 RETURN_VALUE
                ExceptionTable:
                  100 to 144 -> 170 [1] lasti
                  170 to 176 -> 178 [3] lasti
                  184 to 184 -> 178 [3] lasti
                  206 to 272 -> 276 [1]
                  276 to 294 -> 346 [2] lasti
@@ -531,15 +536,15 @@
                   ('max_workers',)
                names      ('partial', 'GoogleMapsWrapper', '_fetch_place_ids', 'ThreadPoolExecutor', 'MAX_WORKERS', 'map', 'extend', 'list', 'Exception', 'print', 'set', 'len')
                varnames   ('search_phrase', 'locations', 'radius_miles', 'main_func', 'exec', 'futures', 'place_ids', 'future', 'e')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'fetch_unique_place_ids'
-               firstlineno 27
+               firstlineno 28
                lnotab
                   0x02040c011601020102fd12052c012cff2e030401080102014801120130
                   ff080338011e01
             'location_text'
             code
                argcount  : 3
                nlocals   : 11
@@ -564,124 +569,124 @@
                   0000000000000000007d097411000000000000000000007c019b0064087c
                   009b0064097c029b00640a7413000000000000000000007c09a6010000ab
                   0100000000000000009b00640b9d08a6010000ab01000000000000000001
                   007c0953002300741400000000000000000000240072247d0a7411000000
                   00000000000000640c7c009b00640d7c019b00640e7c0a9b009d06a60100
                   00ab010000000000000000010067006302590064007d0a7e0a530064007d
                   0a7e0a77017700780359007701
-                50           0 RESUME                   0
+                51           0 RESUME                   0
                
-                54           2 NOP
+                55           2 NOP
                
-                55           4 LOAD_CONST               1 (1609.34)
+                56           4 LOAD_CONST               1 (1609.34)
                              6 STORE_FAST               3 (METERS_PER_MILE)
                
-                56           8 LOAD_FAST                2 (radius_miles)
+                57           8 LOAD_FAST                2 (radius_miles)
                             10 LOAD_FAST                3 (METERS_PER_MILE)
                             12 BINARY_OP                5 (*)
                             16 STORE_FAST               4 (radius_meters)
                
-                58          18 LOAD_GLOBAL              0 (GoogleMapsWrapper)
+                59          18 LOAD_GLOBAL              0 (GoogleMapsWrapper)
                             30 LOAD_METHOD              1 (get_loc)
                             52 LOAD_FAST                0 (location_text)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 STORE_FAST               5 (loc)
                
-                60          70 BUILD_LIST               0
+                61          70 BUILD_LIST               0
                             72 STORE_FAST               6 (results)
                
-                62          74 LOAD_GLOBAL              4 (gmaps)
+                63          74 LOAD_GLOBAL              4 (gmaps)
                             86 LOAD_METHOD              3 (places)
                
-                63         108 LOAD_FAST                1 (search_phrase)
+                64         108 LOAD_FAST                1 (search_phrase)
                
-                64         110 LOAD_FAST                5 (loc)
+                65         110 LOAD_FAST                5 (loc)
                
-                65         112 LOAD_FAST                4 (radius_meters)
+                66         112 LOAD_FAST                4 (radius_meters)
                
-                62         114 KW_NAMES                 2
+                63         114 KW_NAMES                 2
                            116 PRECALL                  3
                            120 CALL                     3
                            130 STORE_FAST               7 (response)
                
-                68         132 LOAD_FAST                6 (results)
+                69         132 LOAD_FAST                6 (results)
                            134 LOAD_METHOD              4 (extend)
                            156 LOAD_FAST                7 (response)
                            158 LOAD_CONST               3 ('results')
                            160 BINARY_SUBSCR
                            170 PRECALL                  1
                            174 CALL                     1
                            184 POP_TOP
                
-                69         186 LOAD_FAST                7 (response)
+                70         186 LOAD_FAST                7 (response)
                            188 LOAD_METHOD              5 (get)
                            210 LOAD_CONST               4 ('next_page_token')
                            212 LOAD_CONST               0 (None)
                            214 PRECALL                  2
                            218 CALL                     2
                            228 STORE_FAST               8 (next_page_token)
                
-                70         230 LOAD_FAST                8 (next_page_token)
+                71         230 LOAD_FAST                8 (next_page_token)
                            232 POP_JUMP_FORWARD_IF_FALSE   101 (to 436)
                
-                71     >>  234 LOAD_GLOBAL             13 (NULL + time)
+                72     >>  234 LOAD_GLOBAL             13 (NULL + time)
                            246 LOAD_ATTR                7 (sleep)
                            256 LOAD_CONST               5 (2)
                            258 PRECALL                  1
                            262 CALL                     1
                            272 POP_TOP
                
-                72         274 LOAD_GLOBAL              4 (gmaps)
+                73         274 LOAD_GLOBAL              4 (gmaps)
                            286 LOAD_METHOD              3 (places)
                
-                73         308 LOAD_FAST                1 (search_phrase)
+                74         308 LOAD_FAST                1 (search_phrase)
                
-                74         310 LOAD_FAST                5 (loc)
+                75         310 LOAD_FAST                5 (loc)
                
-                75         312 LOAD_FAST                4 (radius_meters)
+                76         312 LOAD_FAST                4 (radius_meters)
                
-                76         314 LOAD_FAST                8 (next_page_token)
+                77         314 LOAD_FAST                8 (next_page_token)
                
-                72         316 KW_NAMES                 6
+                73         316 KW_NAMES                 6
                            318 PRECALL                  4
                            322 CALL                     4
                            332 STORE_FAST               7 (response)
                
-                78         334 LOAD_FAST                6 (results)
+                79         334 LOAD_FAST                6 (results)
                            336 LOAD_METHOD              4 (extend)
                            358 LOAD_FAST                7 (response)
                            360 LOAD_CONST               3 ('results')
                            362 BINARY_SUBSCR
                            372 PRECALL                  1
                            376 CALL                     1
                            386 POP_TOP
                
-                79         388 LOAD_FAST                7 (response)
+                80         388 LOAD_FAST                7 (response)
                            390 LOAD_METHOD              5 (get)
                            412 LOAD_CONST               4 ('next_page_token')
                            414 LOAD_CONST               0 (None)
                            416 PRECALL                  2
                            420 CALL                     2
                            430 STORE_FAST               8 (next_page_token)
                
-                70         432 LOAD_FAST                8 (next_page_token)
+                71         432 LOAD_FAST                8 (next_page_token)
                            434 POP_JUMP_BACKWARD_IF_TRUE   101 (to 234)
                
-                81     >>  436 LOAD_CONST               7 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 81>)
+                82     >>  436 LOAD_CONST               7 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 82>)
                            438 MAKE_FUNCTION            0
                            440 LOAD_FAST                6 (results)
                            442 GET_ITER
                            444 PRECALL                  0
                            448 CALL                     0
                            458 STORE_FAST               9 (place_ids)
                
-                82         460 LOAD_GLOBAL             17 (NULL + print)
+                83         460 LOAD_GLOBAL             17 (NULL + print)
                
-                83         472 LOAD_FAST                1 (search_phrase)
+                84         472 LOAD_FAST                1 (search_phrase)
                            474 FORMAT_VALUE             0
                            476 LOAD_CONST               8 (' in ')
                            478 LOAD_FAST                0 (location_text)
                            480 FORMAT_VALUE             0
                            482 LOAD_CONST               9 (' within ')
                            484 LOAD_FAST                2 (radius_miles)
                            486 FORMAT_VALUE             0
@@ -690,55 +695,55 @@
                            502 LOAD_FAST                9 (place_ids)
                            504 PRECALL                  1
                            508 CALL                     1
                            518 FORMAT_VALUE             0
                            520 LOAD_CONST              11 (' results')
                            522 BUILD_STRING             8
                
-                82         524 PRECALL                  1
+                83         524 PRECALL                  1
                            528 CALL                     1
                            538 POP_TOP
                
-                85         540 LOAD_FAST                9 (place_ids)
+                86         540 LOAD_FAST                9 (place_ids)
                            542 RETURN_VALUE
                        >>  544 PUSH_EXC_INFO
                
-                86         546 LOAD_GLOBAL             20 (Exception)
+                87         546 LOAD_GLOBAL             20 (Exception)
                            558 CHECK_EXC_MATCH
                            560 POP_JUMP_FORWARD_IF_FALSE    36 (to 634)
                            562 STORE_FAST              10 (e)
                
-                87         564 LOAD_GLOBAL             17 (NULL + print)
+                88         564 LOAD_GLOBAL             17 (NULL + print)
                            576 LOAD_CONST              12 ('Error with ')
                            578 LOAD_FAST                0 (location_text)
                            580 FORMAT_VALUE             0
                            582 LOAD_CONST              13 (' ')
                            584 LOAD_FAST                1 (search_phrase)
                            586 FORMAT_VALUE             0
                            588 LOAD_CONST              14 (': ')
                            590 LOAD_FAST               10 (e)
                            592 FORMAT_VALUE             0
                            594 BUILD_STRING             6
                            596 PRECALL                  1
                            600 CALL                     1
                            610 POP_TOP
                
-                88         612 BUILD_LIST               0
+                89         612 BUILD_LIST               0
                            614 SWAP                     2
                            616 POP_EXCEPT
                            618 LOAD_CONST               0 (None)
                            620 STORE_FAST              10 (e)
                            622 DELETE_FAST             10 (e)
                            624 RETURN_VALUE
                        >>  626 LOAD_CONST               0 (None)
                            628 STORE_FAST              10 (e)
                            630 DELETE_FAST             10 (e)
                            632 RERAISE                  1
                
-                86     >>  634 RERAISE                  0
+                87     >>  634 RERAISE                  0
                        >>  636 COPY                     3
                            638 POP_EXCEPT
                            640 RERAISE                  1
                ExceptionTable:
                  4 to 540 -> 544 [0]
                  544 to 562 -> 636 [1] lasti
                  564 to 612 -> 626 [1] lasti
@@ -756,15 +761,15 @@
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code
                         0x970067007c005d0a7d017c0164001900000000000000000091028c0b53
                         00
-                      81           0 RESUME                   0
+                      82           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                10 (to 28)
                                    8 STORE_FAST               1 (result)
                                   10 LOAD_FAST                1 (result)
                                   12 LOAD_CONST               0 ('place_id')
                                   14 BINARY_SUBSCR
@@ -775,30 +780,30 @@
                         'place_id'
                      names      ()
                      varnames   ('.0', 'result')
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '<listcomp>'
-                     firstlineno 81
+                     firstlineno 82
                      lnotab 0x
                   ' in '
                   ' within '
                   ' miles -> '
                   ' results'
                   'Error with '
                   ' '
                   ': '
                names      ('GoogleMapsWrapper', 'get_loc', 'gmaps', 'places', 'extend', 'get', 'time', 'sleep', 'print', 'len', 'Exception')
                varnames   ('location_text', 'search_phrase', 'radius_miles', 'METERS_PER_MILE', 'radius_meters', 'loc', 'results', 'response', 'next_page_token', 'place_ids', 'e')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       '_fetch_place_ids'
-               firstlineno 50
+               firstlineno 51
                lnotab
                   0x0204020104010a023402040222010201020102fd120636012c01040128
                   01220102010201020102fc120636012cf7040b18010c0134ff1003060112
                   01300116fe
             None
             'search_uid'
             'append_to_prompt'
@@ -839,267 +844,267 @@
                   0000006a1100000000000000007c01641664177c066a0d00000000000000
                   00641764187425000000000000000000006a1300000000000000007c05a6
                   010000ab0100000000000000009b009d026901ac19a6050000ab05000000
                   0000000000a6010000ab0100000000000000000100740500000000000000
                   0000006a1000000000000000007413000000000000000000006a11000000
                   00000000007c01641a641b7c066a0d0000000000000000ac1ca6040000ab
                   040000000000000000a6010000ab01000000000000000001007c065300
-                90           0 RESUME                   0
+                91           0 RESUME                   0
                
-                97           2 LOAD_GLOBAL              0 (GoogleMapsWrapper)
+                98           2 LOAD_GLOBAL              0 (GoogleMapsWrapper)
                             14 LOAD_METHOD              1 (enrich)
                             36 LOAD_FAST                0 (place_id)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               3 (place)
                
-                99          54 LOAD_GLOBAL              5 (NULL + query)
+               100          54 LOAD_GLOBAL              5 (NULL + query)
                             66 LOAD_ATTR                3 (unique_domains)
                             76 LOAD_FAST                1 (search_uid)
                             78 KW_NAMES                 1
                             80 PRECALL                  1
                             84 CALL                     1
                
-               100          94 LOAD_CONST               2 ('domain')
+               101          94 LOAD_CONST               2 ('domain')
                
-                99          96 BINARY_SUBSCR
+               100          96 BINARY_SUBSCR
                
-               101         106 LOAD_METHOD              4 (to_list)
+               102         106 LOAD_METHOD              4 (to_list)
                            128 PRECALL                  0
                            132 CALL                     0
                
-                99         142 STORE_FAST               4 (existing_search_domains)
+               100         142 STORE_FAST               4 (existing_search_domains)
                
-               103         144 LOAD_CONST               3 ('website')
+               104         144 LOAD_CONST               3 ('website')
                            146 LOAD_FAST                3 (place)
                            148 CONTAINS_OP              1
                            150 POP_JUMP_FORWARD_IF_FALSE    20 (to 192)
                
-               104         152 LOAD_GLOBAL             11 (NULL + print)
+               105         152 LOAD_GLOBAL             11 (NULL + print)
                            164 LOAD_CONST               4 ('no website for ')
                            166 LOAD_FAST                0 (place_id)
                            168 FORMAT_VALUE             0
                            170 BUILD_STRING             2
                            172 PRECALL                  1
                            176 CALL                     1
                            186 POP_TOP
                
-               105         188 LOAD_CONST               5 (None)
+               106         188 LOAD_CONST               5 (None)
                            190 RETURN_VALUE
                
-               107     >>  192 LOAD_GLOBAL             13 (NULL + helpers)
+               108     >>  192 LOAD_GLOBAL             13 (NULL + helpers)
                            204 LOAD_ATTR                7 (clean_domain)
                            214 LOAD_FAST                3 (place)
                            216 LOAD_CONST               3 ('website')
                            218 BINARY_SUBSCR
                            228 PRECALL                  1
                            232 CALL                     1
                            242 LOAD_FAST                4 (existing_search_domains)
                            244 CONTAINS_OP              0
                            246 POP_JUMP_FORWARD_IF_FALSE    29 (to 306)
                
-               108         248 LOAD_GLOBAL             11 (NULL + print)
+               109         248 LOAD_GLOBAL             11 (NULL + print)
                            260 LOAD_CONST               6 ('skipping ')
                            262 LOAD_FAST                3 (place)
                            264 LOAD_CONST               3 ('website')
                            266 BINARY_SUBSCR
                            276 FORMAT_VALUE             0
                            278 LOAD_CONST               7 (' - already in search_uid ')
                            280 LOAD_FAST                1 (search_uid)
                            282 FORMAT_VALUE             0
                            284 BUILD_STRING             4
                            286 PRECALL                  1
                            290 CALL                     1
                            300 POP_TOP
                
-               109         302 LOAD_CONST               5 (None)
+               110         302 LOAD_CONST               5 (None)
                            304 RETURN_VALUE
                
-               111     >>  306 LOAD_CONST               8 (' ')
+               112     >>  306 LOAD_CONST               8 (' ')
                            308 LOAD_METHOD              8 (join)
                
-               113         330 LOAD_CONST               9 ('Q: Based on these reviews:')
+               114         330 LOAD_CONST               9 ('Q: Based on these reviews:')
                
-               114         332 LOAD_CONST              10 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 114>)
+               115         332 LOAD_CONST              10 (<code object <listcomp>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 115>)
                            334 MAKE_FUNCTION            0
                            336 LOAD_FAST                3 (place)
                            338 LOAD_CONST              11 ('reviews')
                            340 BINARY_SUBSCR
                            350 GET_ITER
                            352 PRECALL                  0
                            356 CALL                     0
                            366 FORMAT_VALUE             0
                
-               115         368 LOAD_CONST              12 ('as well as what you already know about ')
+               116         368 LOAD_CONST              12 ('as well as what you already know about ')
                            370 LOAD_FAST                3 (place)
                            372 LOAD_CONST               3 ('website')
                            374 BINARY_SUBSCR
                            384 FORMAT_VALUE             0
                            386 LOAD_CONST              13 (',')
                            388 BUILD_STRING             3
                
-               116         390 LOAD_CONST              14 ('what products and services does ')
+               117         390 LOAD_CONST              14 ('what products and services does ')
                            392 LOAD_FAST                3 (place)
                            394 LOAD_CONST              15 ('name')
                            396 BINARY_SUBSCR
                            406 FORMAT_VALUE             0
                            408 LOAD_CONST              16 (' offer?')
                            410 BUILD_STRING             3
                
-               112         412 BUILD_LIST               4
+               113         412 BUILD_LIST               4
                
-               111         414 PRECALL                  1
+               112         414 PRECALL                  1
                            418 CALL                     1
                            428 STORE_FAST               5 (gpt_prompt)
                
-               119         430 LOAD_FAST                2 (append_to_prompt)
+               120         430 LOAD_FAST                2 (append_to_prompt)
                            432 POP_JUMP_FORWARD_IF_FALSE     8 (to 450)
                
-               120         434 LOAD_FAST                5 (gpt_prompt)
+               121         434 LOAD_FAST                5 (gpt_prompt)
                            436 LOAD_CONST               8 (' ')
                            438 LOAD_FAST                2 (append_to_prompt)
                            440 BINARY_OP                0 (+)
                            444 BINARY_OP               13 (+=)
                            448 STORE_FAST               5 (gpt_prompt)
                
-               123     >>  450 LOAD_GLOBAL             19 (NULL + models)
+               124     >>  450 LOAD_GLOBAL             19 (NULL + models)
                            462 LOAD_ATTR               10 (Company)
                
-               124         472 LOAD_FAST                3 (place)
+               125         472 LOAD_FAST                3 (place)
                            474 LOAD_CONST              15 ('name')
                            476 BINARY_SUBSCR
                
-               125         486 LOAD_GLOBAL             13 (NULL + helpers)
+               126         486 LOAD_GLOBAL             13 (NULL + helpers)
                            498 LOAD_ATTR                7 (clean_domain)
                            508 LOAD_FAST                3 (place)
                            510 LOAD_CONST               3 ('website')
                            512 BINARY_SUBSCR
                            522 PRECALL                  1
                            526 CALL                     1
                
-               126         536 LOAD_CONST              17 ('')
+               127         536 LOAD_CONST              17 ('')
                
-               123         538 KW_NAMES                18
+               124         538 KW_NAMES                18
                            540 PRECALL                  3
                            544 CALL                     3
                            554 STORE_FAST               6 (company)
                
-               129         556 LOAD_GLOBAL              5 (NULL + query)
+               130         556 LOAD_GLOBAL              5 (NULL + query)
                            568 LOAD_ATTR               11 (insert_company)
                            578 LOAD_FAST                6 (company)
                            580 PRECALL                  1
                            584 CALL                     1
                            594 POP_TOP
                
-               132         596 LOAD_GLOBAL              5 (NULL + query)
+               133         596 LOAD_GLOBAL              5 (NULL + query)
                            608 LOAD_ATTR               12 (find_company_by_domain)
                            618 LOAD_FAST                6 (company)
                            620 LOAD_ATTR               13 (domain)
                            630 PRECALL                  1
                            634 CALL                     1
                            644 STORE_FAST               6 (company)
                
-               133         646 LOAD_CONST              19 ('google_places')
+               134         646 LOAD_CONST              19 ('google_places')
                            648 LOAD_FAST                6 (company)
                            650 LOAD_ATTR               14 (meta)
                            660 CONTAINS_OP              1
                            662 POP_JUMP_FORWARD_IF_FALSE    10 (to 684)
                
-               134         664 BUILD_MAP                0
+               135         664 BUILD_MAP                0
                            666 LOAD_FAST                6 (company)
                            668 LOAD_ATTR               14 (meta)
                            678 LOAD_CONST              19 ('google_places')
                            680 STORE_SUBSCR
                
-               135     >>  684 LOAD_FAST                3 (place)
+               136     >>  684 LOAD_FAST                3 (place)
                            686 LOAD_FAST                6 (company)
                            688 LOAD_ATTR               14 (meta)
                            698 LOAD_CONST              19 ('google_places')
                            700 BINARY_SUBSCR
                            710 LOAD_FAST                0 (place_id)
                            712 STORE_SUBSCR
                
-               136         716 LOAD_GLOBAL              5 (NULL + query)
+               137         716 LOAD_GLOBAL              5 (NULL + query)
                            728 LOAD_ATTR               15 (update_company)
                            738 LOAD_FAST                6 (company)
                            740 PRECALL                  1
                            744 CALL                     1
                            754 POP_TOP
                
-               139         756 LOAD_GLOBAL             11 (NULL + print)
+               140         756 LOAD_GLOBAL             11 (NULL + print)
                            768 LOAD_CONST              20 ('adding ')
                            770 LOAD_FAST                6 (company)
                            772 LOAD_ATTR               13 (domain)
                            782 FORMAT_VALUE             0
                            784 LOAD_CONST              21 (' - search_uid ')
                            786 LOAD_FAST                1 (search_uid)
                            788 FORMAT_VALUE             0
                            790 BUILD_STRING             4
                            792 PRECALL                  1
                            796 CALL                     1
                            806 POP_TOP
                
-               140         808 LOAD_GLOBAL              5 (NULL + query)
+               141         808 LOAD_GLOBAL              5 (NULL + query)
                            820 LOAD_ATTR               16 (insert_event)
                
-               141         830 LOAD_GLOBAL             19 (NULL + models)
+               142         830 LOAD_GLOBAL             19 (NULL + models)
                            842 LOAD_ATTR               17 (Event)
                
-               142         852 LOAD_FAST                1 (search_uid)
+               143         852 LOAD_FAST                1 (search_uid)
                
-               143         854 LOAD_CONST              22 ('chatgpt')
+               144         854 LOAD_CONST              22 ('chatgpt')
                
-               144         856 LOAD_CONST              23 ('comment')
+               145         856 LOAD_CONST              23 ('comment')
                
-               145         858 LOAD_FAST                6 (company)
+               146         858 LOAD_FAST                6 (company)
                            860 LOAD_ATTR               13 (domain)
                
-               146         870 LOAD_CONST              23 ('comment')
+               147         870 LOAD_CONST              23 ('comment')
                            872 LOAD_CONST              24 ('chatgpt - ')
                            874 LOAD_GLOBAL             37 (NULL + gpt)
                            886 LOAD_ATTR               19 (ask_gpt)
                            896 LOAD_FAST                5 (gpt_prompt)
                            898 PRECALL                  1
                            902 CALL                     1
                            912 FORMAT_VALUE             0
                            914 BUILD_STRING             2
                            916 BUILD_MAP                1
                
-               141         918 KW_NAMES                25
+               142         918 KW_NAMES                25
                            920 PRECALL                  5
                            924 CALL                     5
                
-               140         934 PRECALL                  1
+               141         934 PRECALL                  1
                            938 CALL                     1
                            948 POP_TOP
                
-               150         950 LOAD_GLOBAL              5 (NULL + query)
+               151         950 LOAD_GLOBAL              5 (NULL + query)
                            962 LOAD_ATTR               16 (insert_event)
                
-               151         972 LOAD_GLOBAL             19 (NULL + models)
+               152         972 LOAD_GLOBAL             19 (NULL + models)
                            984 LOAD_ATTR               17 (Event)
                
-               152         994 LOAD_FAST                1 (search_uid)
+               153         994 LOAD_FAST                1 (search_uid)
                
-               153         996 LOAD_CONST              26 ('google')
+               154         996 LOAD_CONST              26 ('google')
                
-               154         998 LOAD_CONST              27 ('create')
+               155         998 LOAD_CONST              27 ('create')
                
-               155        1000 LOAD_FAST                6 (company)
+               156        1000 LOAD_FAST                6 (company)
                           1002 LOAD_ATTR               13 (domain)
                
-               151        1012 KW_NAMES                28
+               152        1012 KW_NAMES                28
                           1014 PRECALL                  4
                           1018 CALL                     4
                
-               150        1028 PRECALL                  1
+               151        1028 PRECALL                  1
                           1032 CALL                     1
                           1042 POP_TOP
                
-               159        1044 LOAD_FAST                6 (company)
+               160        1044 LOAD_FAST                6 (company)
                           1046 RETURN_VALUE
                consts
                   'takes in an (eriched) place and inserts it as a company'
                   ('search_uid',)
                   'domain'
                   'website'
                   'no website for '
@@ -1112,15 +1117,15 @@
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code
                         0x970067007c005d0a7d017c0164001900000000000000000091028c0b53
                         00
-                     114           0 RESUME                   0
+                     115           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                10 (to 28)
                                    8 STORE_FAST               1 (review)
                                   10 LOAD_FAST                1 (review)
                                   12 LOAD_CONST               0 ('text')
                                   14 BINARY_SUBSCR
@@ -1131,15 +1136,15 @@
                         'text'
                      names      ()
                      varnames   ('.0', 'review')
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '<listcomp>'
-                     firstlineno 114
+                     firstlineno 115
                      lnotab 0x
                   'reviews'
                   'as well as what you already know about '
                   ','
                   'what products and services does '
                   'name'
                   ' offer?'
@@ -1157,15 +1162,15 @@
                   ('search_uid', 'actor_key', 'type', 'domain')
                names      ('GoogleMapsWrapper', 'enrich', 'query', 'unique_domains', 'to_list', 'print', 'helpers', 'clean_domain', 'join', 'models', 'Company', 'insert_company', 'find_company_by_domain', 'domain', 'meta', 'update_company', 'insert_event', 'Event', 'gpt', 'ask_gpt')
                varnames   ('place_id', 'search_uid', 'append_to_prompt', 'place', 'existing_search_domains', 'gpt_prompt', 'company')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'build_target_from_place_id'
-               firstlineno 90
+               firstlineno 91
                lnotab
                   0x02073402280102ff0a0224fe0204080124010402380136010402180202
                   012401160116fc02ff10080401100316010e01320102fd12062803320112
                   011401200128033401160116010201020102010c0130fb10ff100a160116
                   010201020102010cfc10ff1009
             'place_ids'
             'search'
@@ -1178,49 +1183,49 @@
                   0x9700740100000000000000000000740200000000000000000000ac01a6
                   010000ab01000000000000000035007d027c0044005d297d037c02a00200
                   000000000000000000000000000000000000007406000000000000000000
                   006a0400000000000000007c037c016a050000000000000000ac02a60300
                   00ab03000000000000000001008c2a0900640064006400a6020000ab0200
                   000000000000000100640053002300310073047702780359007701010059
                   000100010064005300
-               161           0 RESUME                   0
+               162           0 RESUME                   0
                
-               162           2 LOAD_GLOBAL              1 (NULL + ThreadPoolExecutor)
+               163           2 LOAD_GLOBAL              1 (NULL + ThreadPoolExecutor)
                             14 LOAD_GLOBAL              2 (MAX_WORKERS)
                             26 KW_NAMES                 1
                             28 PRECALL                  1
                             32 CALL                     1
                             42 BEFORE_WITH
                             44 STORE_FAST               2 (executor)
                
-               163          46 LOAD_FAST                0 (place_ids)
+               164          46 LOAD_FAST                0 (place_ids)
                             48 GET_ITER
                        >>   50 FOR_ITER                41 (to 134)
                             52 STORE_FAST               3 (place_id)
                
-               164          54 LOAD_FAST                2 (executor)
+               165          54 LOAD_FAST                2 (executor)
                             56 LOAD_METHOD              2 (submit)
                
-               165          78 LOAD_GLOBAL              6 (GoogleMapsWrapper)
+               166          78 LOAD_GLOBAL              6 (GoogleMapsWrapper)
                             90 LOAD_ATTR                4 (build_target_from_place_id)
                
-               166         100 LOAD_FAST                3 (place_id)
+               167         100 LOAD_FAST                3 (place_id)
                
-               167         102 LOAD_FAST                1 (search)
+               168         102 LOAD_FAST                1 (search)
                            104 LOAD_ATTR                5 (uid)
                
-               164         114 KW_NAMES                 2
+               165         114 KW_NAMES                 2
                            116 PRECALL                  3
                            120 CALL                     3
                            130 POP_TOP
                            132 JUMP_BACKWARD           42 (to 50)
                
-               163     >>  134 NOP
+               164     >>  134 NOP
                
-               162         136 LOAD_CONST               0 (None)
+               163         136 LOAD_CONST               0 (None)
                            138 LOAD_CONST               0 (None)
                            140 LOAD_CONST               0 (None)
                            142 PRECALL                  2
                            146 CALL                     2
                            156 POP_TOP
                            158 LOAD_CONST               0 (None)
                            160 RETURN_VALUE
@@ -1247,26 +1252,26 @@
                   ('place_id', 'search_uid')
                names      ('ThreadPoolExecutor', 'MAX_WORKERS', 'submit', 'GoogleMapsWrapper', 'build_target_from_place_id', 'uid')
                varnames   ('place_ids', 'search', 'executor', 'place_id')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'build_place_ids_async'
-               firstlineno 161
+               firstlineno 162
                lnotab 0x02012c0108011801160102010cfd14ff02ff
             ('San Diego, CA',)
             (25,)
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'staticmethod', 'str', 'tuple', 'get_loc', 'dict', 'enrich', 'List', 'int', 'list', 'fetch_unique_place_ids', '_fetch_place_ids', 'models', 'Company', 'build_target_from_place_id', 'Search', 'build_place_ids_async')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
          name       'GoogleMapsWrapper'
-         firstlineno 16
+         firstlineno 17
          lnotab
             0x0a01020110ff0e01020402010eff0e010204020202ff040102ff02010e
             ff020102ff020202fe06ff0e010216020202ff040102ff020102ff020102
             ff020202fe06ff0e010227020202ff040102ff020102ff020102ff02020c
             fe06ff0e010246
       'GoogleMapsWrapper'
       code
@@ -1275,225 +1280,253 @@
          stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006401a60100
             00ab010000000000000000640264039c025a0564046506640565076a0800
             00000000000000640665096606640784045a0a640565076a080000000000
             0000006406650b6604640884045a0c640465066406650b6604640984045a
-            0d640565076a0800000000000000006406650b6604640a84045a0e640b53
-            00
-         171           0 RESUME                   0
+            0d640a650e6a0f00000000000000006406640b6604640c84045a10640565
+            076a0800000000000000006406650b6604640d84045a11640b5300
+         172           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('GrataWrapper')
                        8 STORE_NAME               2 (__qualname__)
          
-         173          10 PUSH_NULL
+         174          10 PUSH_NULL
                       12 LOAD_NAME                3 (secrets)
                       14 LOAD_ATTR                4 (access_secret_version)
                       24 LOAD_CONST               1 ('GRATA_API_TOKEN')
                       26 PRECALL                  1
                       30 CALL                     1
          
-         174          40 LOAD_CONST               2 ('application/json')
+         175          40 LOAD_CONST               2 ('application/json')
          
-         172          42 LOAD_CONST               3 (('Authorization', 'Content-Type'))
+         173          42 LOAD_CONST               3 (('Authorization', 'Content-Type'))
                       44 BUILD_CONST_KEY_MAP      2
                       46 STORE_NAME               5 (HEADERS)
          
-         177          48 LOAD_CONST               4 ('domain')
+         178          48 LOAD_CONST               4 ('domain')
                       50 LOAD_NAME                6 (str)
                       52 LOAD_CONST               5 ('search')
                       54 LOAD_NAME                7 (models)
                       56 LOAD_ATTR                8 (Search)
                       66 LOAD_CONST               6 ('return')
                       68 LOAD_NAME                9 (list)
                       70 BUILD_TUPLE              6
-                      72 LOAD_CONST               7 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 177>)
+                      72 LOAD_CONST               7 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 178>)
                       74 MAKE_FUNCTION            4 (annotations)
                       76 STORE_NAME              10 (find_similar)
          
-         196          78 LOAD_CONST               5 ('search')
+         200          78 LOAD_CONST               5 ('search')
                       80 LOAD_NAME                7 (models)
                       82 LOAD_ATTR                8 (Search)
                       92 LOAD_CONST               6 ('return')
                       94 LOAD_NAME               11 (dict)
                       96 BUILD_TUPLE              4
-                      98 LOAD_CONST               8 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 196>)
+                      98 LOAD_CONST               8 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 200>)
                      100 MAKE_FUNCTION            4 (annotations)
                      102 STORE_NAME              12 (find_by_criteria)
          
-         207         104 LOAD_CONST               4 ('domain')
+         211         104 LOAD_CONST               4 ('domain')
                      106 LOAD_NAME                6 (str)
                      108 LOAD_CONST               6 ('return')
                      110 LOAD_NAME               11 (dict)
                      112 BUILD_TUPLE              4
-                     114 LOAD_CONST               9 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 207>)
+                     114 LOAD_CONST               9 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 211>)
                      116 MAKE_FUNCTION            4 (annotations)
                      118 STORE_NAME              13 (enrich)
          
-         218         120 LOAD_CONST               5 ('search')
-                     122 LOAD_NAME                7 (models)
-                     124 LOAD_ATTR                8 (Search)
+         222         120 LOAD_CONST              10 ('targets')
+                     122 LOAD_NAME               14 (pd)
+                     124 LOAD_ATTR               15 (DataFrame)
                      134 LOAD_CONST               6 ('return')
-                     136 LOAD_NAME               11 (dict)
+                     136 LOAD_CONST              11 (None)
                      138 BUILD_TUPLE              4
-                     140 LOAD_CONST              10 (<code object _get_api_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 218>)
+                     140 LOAD_CONST              12 (<code object enrich_targets_async, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 222>)
                      142 MAKE_FUNCTION            4 (annotations)
-                     144 STORE_NAME              14 (_get_api_filter)
-                     146 LOAD_CONST              11 (None)
-                     148 RETURN_VALUE
+                     144 STORE_NAME              16 (enrich_targets_async)
+         
+         237         146 LOAD_CONST               5 ('search')
+                     148 LOAD_NAME                7 (models)
+                     150 LOAD_ATTR                8 (Search)
+                     160 LOAD_CONST               6 ('return')
+                     162 LOAD_NAME               11 (dict)
+                     164 BUILD_TUPLE              4
+                     166 LOAD_CONST              13 (<code object _get_api_filter, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 237>)
+                     168 MAKE_FUNCTION            4 (annotations)
+                     170 STORE_NAME              17 (_get_api_filter)
+                     172 LOAD_CONST              11 (None)
+                     174 RETURN_VALUE
          consts
             'GrataWrapper'
             'GRATA_API_TOKEN'
             'application/json'
             ('Authorization', 'Content-Type')
             'domain'
             'search'
             'return'
             code
                argcount  : 2
-               nlocals   : 5
-               stacksize : 8
+               nlocals   : 6
+               stacksize : 5
                flags     : 3
                code
                   0x9700740000000000000000000000a00100000000000000000000000000
-                  000000000000007c01a6010000ab0100000000000000007d027405000000
-                  000000000000006a03000000000000000064017400000000000000000000
-                  006a0400000000000000007c007c026402190000000000000000007c0264
-                  031900000000000000000064049c03ac05a6030000ab0300000000000000
-                  007d037c03a0050000000000000000000000000000000000000000a60000
-                  00ab0000000000000000007d047c04a00600000000000000000000000000
-                  0000000000000064066700a6020000ab0200000000000000007c0464073c
-                  0000007c046407190000000000000000005300
-               177           0 RESUME                   0
+                  000000000000007c01a6010000ab0100000000000000007d027c007c0264
+                  01190000000000000000007c026402190000000000000000007c02640319
+                  00000000000000000064049c047d037405000000000000000000007c03a6
+                  010000ab01000000000000000001007407000000000000000000006a0400
+                  0000000000000064057400000000000000000000006a0500000000000000
+                  007c03ac06a6030000ab0300000000000000007d047c04a0060000000000
+                  000000000000000000000000000000a6000000ab0000000000000000007d
+                  057c05a007000000000000000000000000000000000000000064076700a6
+                  020000ab0200000000000000007c0564083c0000007c0564081900000000
+                  00000000005300
+               178           0 RESUME                   0
                
-               178           2 LOAD_GLOBAL              0 (GrataWrapper)
+               179           2 LOAD_GLOBAL              0 (GrataWrapper)
                             14 LOAD_METHOD              1 (_get_api_filter)
                             36 LOAD_FAST                1 (search)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               2 (api_filters)
                
-               179          54 LOAD_GLOBAL              5 (NULL + requests)
-                            66 LOAD_ATTR                3 (post)
-               
-               180          76 LOAD_CONST               1 ('https://search.grata.com/api/v1.2/search-similar/')
-               
-               181          78 LOAD_GLOBAL              0 (GrataWrapper)
-                            90 LOAD_ATTR                4 (HEADERS)
-               
-               183         100 LOAD_FAST                0 (domain)
+               181          54 LOAD_FAST                0 (domain)
                
-               184         102 LOAD_FAST                2 (api_filters)
+               182          56 LOAD_FAST                2 (api_filters)
                
-               185         104 LOAD_CONST               2 ('grata_employees_estimates_range')
+               183          58 LOAD_CONST               1 ('grata_employees_estimates_range')
                
-               184         106 BINARY_SUBSCR
+               182          60 BINARY_SUBSCR
                
-               187         116 LOAD_FAST                2 (api_filters)
-                           118 LOAD_CONST               3 ('headquarters')
-                           120 BINARY_SUBSCR
-               
-               182         130 LOAD_CONST               4 (('domain', 'grata_employees_estimates_range', 'headquarters'))
-                           132 BUILD_CONST_KEY_MAP      3
-               
-               179         134 KW_NAMES                 5
-                           136 PRECALL                  3
-                           140 CALL                     3
-                           150 STORE_FAST               3 (response)
-               
-               190         152 LOAD_FAST                3 (response)
-                           154 LOAD_METHOD              5 (json)
-                           176 PRECALL                  0
-                           180 CALL                     0
-                           190 STORE_FAST               4 (data)
-               
-               192         192 LOAD_FAST                4 (data)
-                           194 LOAD_METHOD              6 (get)
-                           216 LOAD_CONST               6 ('results')
-                           218 BUILD_LIST               0
-                           220 PRECALL                  2
-                           224 CALL                     2
-                           234 LOAD_FAST                4 (data)
-                           236 LOAD_CONST               7 ('companies')
-                           238 STORE_SUBSCR
-               
-               194         242 LOAD_FAST                4 (data)
-                           244 LOAD_CONST               7 ('companies')
-                           246 BINARY_SUBSCR
-                           256 RETURN_VALUE
+               185          70 LOAD_FAST                2 (api_filters)
+                            72 LOAD_CONST               2 ('headquarters')
+                            74 BINARY_SUBSCR
+               
+               186          84 LOAD_FAST                2 (api_filters)
+                            86 LOAD_CONST               3 ('ownership')
+                            88 BINARY_SUBSCR
+               
+               180          98 LOAD_CONST               4 (('domain', 'grata_employees_estimates_range', 'headquarters', 'ownership'))
+                           100 BUILD_CONST_KEY_MAP      4
+                           102 STORE_FAST               3 (similiar_filters)
+               
+               188         104 LOAD_GLOBAL              5 (NULL + print)
+                           116 LOAD_FAST                3 (similiar_filters)
+                           118 PRECALL                  1
+                           122 CALL                     1
+                           132 POP_TOP
+               
+               189         134 LOAD_GLOBAL              7 (NULL + requests)
+                           146 LOAD_ATTR                4 (post)
+               
+               190         156 LOAD_CONST               5 ('https://search.grata.com/api/v1.2/search-similar/')
+               
+               191         158 LOAD_GLOBAL              0 (GrataWrapper)
+                           170 LOAD_ATTR                5 (HEADERS)
+               
+               192         180 LOAD_FAST                3 (similiar_filters)
+               
+               189         182 KW_NAMES                 6
+                           184 PRECALL                  3
+                           188 CALL                     3
+                           198 STORE_FAST               4 (response)
+               
+               194         200 LOAD_FAST                4 (response)
+                           202 LOAD_METHOD              6 (json)
+                           224 PRECALL                  0
+                           228 CALL                     0
+                           238 STORE_FAST               5 (data)
+               
+               196         240 LOAD_FAST                5 (data)
+                           242 LOAD_METHOD              7 (get)
+                           264 LOAD_CONST               7 ('results')
+                           266 BUILD_LIST               0
+                           268 PRECALL                  2
+                           272 CALL                     2
+                           282 LOAD_FAST                5 (data)
+                           284 LOAD_CONST               8 ('companies')
+                           286 STORE_SUBSCR
+               
+               198         290 LOAD_FAST                5 (data)
+                           292 LOAD_CONST               8 ('companies')
+                           294 BINARY_SUBSCR
+                           304 RETURN_VALUE
                consts
                   None
-                  'https://search.grata.com/api/v1.2/search-similar/'
                   'grata_employees_estimates_range'
                   'headquarters'
-                  ('domain', 'grata_employees_estimates_range', 'headquarters')
+                  'ownership'
+                  ('domain', 'grata_employees_estimates_range', 'headquarters', 'ownership')
+                  'https://search.grata.com/api/v1.2/search-similar/'
                   ('headers', 'json')
                   'results'
                   'companies'
-               names      ('GrataWrapper', '_get_api_filter', 'requests', 'post', 'HEADERS', 'json', 'get')
-               varnames   ('domain', 'search', 'api_filters', 'response', 'data')
+               names      ('GrataWrapper', '_get_api_filter', 'print', 'requests', 'post', 'HEADERS', 'json', 'get')
+               varnames   ('domain', 'search', 'api_filters', 'similiar_filters', 'response', 'data')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_similar'
-               firstlineno 177
-               lnotab 0x020134011601020116020201020102ff0a030efb04fd120b28023202
+               firstlineno 178
+               lnotab
+                  0x020134020201020102ff0a030e010efa06081e0116010201160102fd12
+                  0528023202
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x9700740000000000000000000000a00100000000000000000000000000
                   000000000000007c00a6010000ab0100000000000000007d017405000000
                   000000000000006a03000000000000000064017400000000000000000000
                   006a0400000000000000007c01ac02a6030000ab0300000000000000007d
                   027c02a0050000000000000000000000000000000000000000a6000000ab
                   0000000000000000007d03740d0000000000000000000064037c03a60200
                   00ab02000000000000000001007c036404190000000000000000005300
-               196           0 RESUME                   0
+               200           0 RESUME                   0
                
-               197           2 LOAD_GLOBAL              0 (GrataWrapper)
+               201           2 LOAD_GLOBAL              0 (GrataWrapper)
                             14 LOAD_METHOD              1 (_get_api_filter)
                             36 LOAD_FAST                0 (search)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               1 (api_filters)
                
-               198          54 LOAD_GLOBAL              5 (NULL + requests)
+               202          54 LOAD_GLOBAL              5 (NULL + requests)
                             66 LOAD_ATTR                3 (post)
                
-               199          76 LOAD_CONST               1 ('https://search.grata.com/api/v1.2/search/')
+               203          76 LOAD_CONST               1 ('https://search.grata.com/api/v1.2/search/')
                
-               200          78 LOAD_GLOBAL              0 (GrataWrapper)
+               204          78 LOAD_GLOBAL              0 (GrataWrapper)
                             90 LOAD_ATTR                4 (HEADERS)
                
-               201         100 LOAD_FAST                1 (api_filters)
+               205         100 LOAD_FAST                1 (api_filters)
                
-               198         102 KW_NAMES                 2
+               202         102 KW_NAMES                 2
                            104 PRECALL                  3
                            108 CALL                     3
                            118 STORE_FAST               2 (response)
                
-               203         120 LOAD_FAST                2 (response)
+               207         120 LOAD_FAST                2 (response)
                            122 LOAD_METHOD              5 (json)
                            144 PRECALL                  0
                            148 CALL                     0
                            158 STORE_FAST               3 (data)
                
-               204         160 LOAD_GLOBAL             13 (NULL + print)
+               208         160 LOAD_GLOBAL             13 (NULL + print)
                            172 LOAD_CONST               3 ('find_by_criteria: ')
                            174 LOAD_FAST                3 (data)
                            176 PRECALL                  2
                            180 CALL                     2
                            190 POP_TOP
                
-               205         192 LOAD_FAST                3 (data)
+               209         192 LOAD_FAST                3 (data)
                            194 LOAD_CONST               4 ('companies')
                            196 BINARY_SUBSCR
                            206 RETURN_VALUE
                consts
                   None
                   'https://search.grata.com/api/v1.2/search/'
                   ('headers', 'json')
@@ -1501,15 +1534,15 @@
                   'companies'
                names      ('GrataWrapper', '_get_api_filter', 'requests', 'post', 'HEADERS', 'json', 'print')
                varnames   ('search', 'api_filters', 'response', 'data')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_by_criteria'
-               firstlineno 196
+               firstlineno 200
                lnotab 0x0201340116010201160102fd120528012001
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
@@ -1517,58 +1550,58 @@
                   0000000000000000006a03000000000000000064027c006901ac03a60300
                   00ab0300000000000000007d017c01a00400000000000000000000000000
                   00000000000000a6000000ab0000000000000000007d027c02a005000000
                   00000000000000000000000000000000006404a6010000ab010000000000
                   0000007c0264053c0000007c02a005000000000000000000000000000000
                   00000000006406a6010000ab0100000000000000007c0264073c0000007c
                   025300
-               207           0 RESUME                   0
+               211           0 RESUME                   0
                
-               208           2 LOAD_GLOBAL              1 (NULL + requests)
+               212           2 LOAD_GLOBAL              1 (NULL + requests)
                             14 LOAD_ATTR                1 (post)
                
-               209          24 LOAD_CONST               1 ('https://search.grata.com/api/v1.2/enrich/')
+               213          24 LOAD_CONST               1 ('https://search.grata.com/api/v1.2/enrich/')
                
-               210          26 LOAD_GLOBAL              4 (GrataWrapper)
+               214          26 LOAD_GLOBAL              4 (GrataWrapper)
                             38 LOAD_ATTR                3 (HEADERS)
                
-               211          48 LOAD_CONST               2 ('domain')
+               215          48 LOAD_CONST               2 ('domain')
                             50 LOAD_FAST                0 (domain)
                             52 BUILD_MAP                1
                
-               208          54 KW_NAMES                 3
+               212          54 KW_NAMES                 3
                             56 PRECALL                  3
                             60 CALL                     3
                             70 STORE_FAST               1 (response)
                
-               213          72 LOAD_FAST                1 (response)
+               217          72 LOAD_FAST                1 (response)
                             74 LOAD_METHOD              4 (json)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 STORE_FAST               2 (data)
                
-               214         112 LOAD_FAST                2 (data)
+               218         112 LOAD_FAST                2 (data)
                            114 LOAD_METHOD              5 (get)
                            136 LOAD_CONST               4 ('social_linkedin')
                            138 PRECALL                  1
                            142 CALL                     1
                            152 LOAD_FAST                2 (data)
                            154 LOAD_CONST               5 ('linkedin')
                            156 STORE_SUBSCR
                
-               215         160 LOAD_FAST                2 (data)
+               219         160 LOAD_FAST                2 (data)
                            162 LOAD_METHOD              5 (get)
                            184 LOAD_CONST               6 ('ownership_status')
                            186 PRECALL                  1
                            190 CALL                     1
                            200 LOAD_FAST                2 (data)
                            202 LOAD_CONST               7 ('ownership')
                            204 STORE_SUBSCR
                
-               216         208 LOAD_FAST                2 (data)
+               220         208 LOAD_FAST                2 (data)
                            210 RETURN_VALUE
                consts
                   None
                   'https://search.grata.com/api/v1.2/enrich/'
                   'domain'
                   ('headers', 'json')
                   'social_linkedin'
@@ -1577,16 +1610,192 @@
                   'ownership'
                names      ('requests', 'post', 'GrataWrapper', 'HEADERS', 'json', 'get')
                varnames   ('domain', 'response', 'data')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'enrich'
-               firstlineno 207
+               firstlineno 211
                lnotab 0x020116010201160106fd1205280130013001
+            'targets'
+            None
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 4
+               flags     : 3
+               code
+                  0x8700870197006401740000000000000000000000640264006604880188
+                  0066026403840c8a0164005300
+                             0 MAKE_CELL                0 (targets)
+                             2 MAKE_CELL                1 (enrich_company_by_domain)
+               
+               222           4 RESUME                   0
+               
+               223           6 LOAD_CONST               1 ('domain')
+                             8 LOAD_GLOBAL              0 (str)
+                            20 LOAD_CONST               2 ('return')
+                            22 LOAD_CONST               0 (None)
+                            24 BUILD_TUPLE              4
+                            26 LOAD_CLOSURE             1 (enrich_company_by_domain)
+                            28 LOAD_CLOSURE             0 (targets)
+                            30 BUILD_TUPLE              2
+                            32 LOAD_CONST               3 (<code object enrich_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 223>)
+                            34 MAKE_FUNCTION           12 (annotations, closure)
+                            36 STORE_DEREF              1 (enrich_company_by_domain)
+                            38 LOAD_CONST               0 (None)
+                            40 RETURN_VALUE
+               consts
+                  None
+                  'domain'
+                  'return'
+                  code
+                     argcount  : 1
+                     nlocals   : 4
+                     stacksize : 6
+                     flags     : 19
+                     code
+                        0x950297007401000000000000000000006a0100000000000000007c00a6
+                        010000ab0100000000000000007d0164017c016a020000000000000000a0
+                        030000000000000000000000000000000000000000a6000000ab00000000
+                        000000000076017258740800000000000000000000a00500000000000000
+                        000000000000000000000000007c00a6010000ab0100000000000000007d
+                        027c02a00600000000000000000000000000000000000000006402a60100
+                        00ab0100000000000000007c015f07000000000000000069007c016a0200
+                        00000000000000a5017c02a5017c015f0200000000000000007401000000
+                        000000000000006a0800000000000000007c01a6010000ab010000000000
+                        00000001007413000000000000000000006403ac04a6010000ab01000000
+                        000000000035007d037c03a00a0000000000000000000000000000000000
+                        00000089048905640519000000000000000000a00b000000000000000000
+                        0000000000000000000000a6000000ab000000000000000000a6020000ab
+                        0200000000000000000100640064006400a6020000ab0200000000000000
+                        000100640053002300310073047702780359007701010059000100010064
+                        005300
+                                   0 COPY_FREE_VARS           2
+                     
+                     223           2 RESUME                   0
+                     
+                     224           4 LOAD_GLOBAL              1 (NULL + query)
+                                  16 LOAD_ATTR                1 (find_company_by_domain)
+                                  26 LOAD_FAST                0 (domain)
+                                  28 PRECALL                  1
+                                  32 CALL                     1
+                                  42 STORE_FAST               1 (company)
+                     
+                     225          44 LOAD_CONST               1 ('company_uid')
+                                  46 LOAD_FAST                1 (company)
+                                  48 LOAD_ATTR                2 (meta)
+                                  58 LOAD_METHOD              3 (keys)
+                                  80 PRECALL                  0
+                                  84 CALL                     0
+                                  94 CONTAINS_OP              1
+                                  96 POP_JUMP_FORWARD_IF_FALSE    88 (to 274)
+                     
+                     227          98 LOAD_GLOBAL              8 (GrataWrapper)
+                                 110 LOAD_METHOD              5 (enrich)
+                                 132 LOAD_FAST                0 (domain)
+                                 134 PRECALL                  1
+                                 138 CALL                     1
+                                 148 STORE_FAST               2 (resp)
+                     
+                     228         150 LOAD_FAST                2 (resp)
+                                 152 LOAD_METHOD              6 (get)
+                                 174 LOAD_CONST               2 ('description')
+                                 176 PRECALL                  1
+                                 180 CALL                     1
+                                 190 LOAD_FAST                1 (company)
+                                 192 STORE_ATTR               7 (description)
+                     
+                     229         202 BUILD_MAP                0
+                                 204 LOAD_FAST                1 (company)
+                                 206 LOAD_ATTR                2 (meta)
+                                 216 DICT_UPDATE              1
+                                 218 LOAD_FAST                2 (resp)
+                                 220 DICT_UPDATE              1
+                                 222 LOAD_FAST                1 (company)
+                                 224 STORE_ATTR               2 (meta)
+                     
+                     230         234 LOAD_GLOBAL              1 (NULL + query)
+                                 246 LOAD_ATTR                8 (update_company)
+                                 256 LOAD_FAST                1 (company)
+                                 258 PRECALL                  1
+                                 262 CALL                     1
+                                 272 POP_TOP
+                     
+                     232     >>  274 LOAD_GLOBAL             19 (NULL + ThreadPoolExecutor)
+                                 286 LOAD_CONST               3 (5)
+                                 288 KW_NAMES                 4
+                                 290 PRECALL                  1
+                                 294 CALL                     1
+                                 304 BEFORE_WITH
+                                 306 STORE_FAST               3 (executor)
+                     
+                     233         308 LOAD_FAST                3 (executor)
+                                 310 LOAD_METHOD             10 (map)
+                     
+                     234         332 LOAD_DEREF               4 (enrich_company_by_domain)
+                                 334 LOAD_DEREF               5 (targets)
+                                 336 LOAD_CONST               5 ('domain')
+                                 338 BINARY_SUBSCR
+                                 348 LOAD_METHOD             11 (tolist)
+                                 370 PRECALL                  0
+                                 374 CALL                     0
+                     
+                     233         384 PRECALL                  2
+                                 388 CALL                     2
+                                 398 POP_TOP
+                     
+                     232         400 LOAD_CONST               0 (None)
+                                 402 LOAD_CONST               0 (None)
+                                 404 LOAD_CONST               0 (None)
+                                 406 PRECALL                  2
+                                 410 CALL                     2
+                                 420 POP_TOP
+                                 422 LOAD_CONST               0 (None)
+                                 424 RETURN_VALUE
+                             >>  426 PUSH_EXC_INFO
+                                 428 WITH_EXCEPT_START
+                                 430 POP_JUMP_FORWARD_IF_TRUE     4 (to 440)
+                                 432 RERAISE                  2
+                             >>  434 COPY                     3
+                                 436 POP_EXCEPT
+                                 438 RERAISE                  1
+                             >>  440 POP_TOP
+                                 442 POP_EXCEPT
+                                 444 POP_TOP
+                                 446 POP_TOP
+                                 448 LOAD_CONST               0 (None)
+                                 450 RETURN_VALUE
+                     ExceptionTable:
+                       306 to 398 -> 426 [1] lasti
+                       426 to 432 -> 434 [3] lasti
+                       440 to 440 -> 434 [3] lasti
+                     consts
+                        None
+                        'company_uid'
+                        'description'
+                        5
+                        ('max_workers',)
+                        'domain'
+                     names      ('query', 'find_company_by_domain', 'meta', 'keys', 'GrataWrapper', 'enrich', 'get', 'description', 'update_company', 'ThreadPoolExecutor', 'map', 'tolist')
+                     varnames   ('domain', 'company', 'resp', 'executor')
+                     freevars   ('enrich_company_by_domain', 'targets')
+                     cellvars   ()
+                     filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
+                     name       'enrich_company_by_domain'
+                     firstlineno 223
+                     lnotab 0x04012801360234013401200128022201180134ff10ff
+               names      ('str',)
+               varnames   ('targets',)
+               freevars   ()
+               cellvars   ('targets', 'enrich_company_by_domain')
+               filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
+               name       'enrich_targets_async'
+               firstlineno 222
+               lnotab 0x0601
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 8
                flags     : 3
                code
                   0x8700870387049700690064016402930164036404930164056406930164
@@ -1611,356 +1820,356 @@
                   00000000000000000000000000000064706471a6020000ab020000000000
                   00000002007c01a6000000ab00000000000000000002007c02a6000000ab
                   00000000000000000064729c0264739c065300
                              0 MAKE_CELL                0 (search)
                              2 MAKE_CELL                3 (COUNTRIES)
                              4 MAKE_CELL                4 (STATES)
                
-               218           6 RESUME                   0
+               237           6 RESUME                   0
                
-               219           8 BUILD_MAP                0
+               238           8 BUILD_MAP                0
                
-               220          10 LOAD_CONST               1 ('AL')
+               239          10 LOAD_CONST               1 ('AL')
                             12 LOAD_CONST               2 ('Alabama')
                
-               219          14 MAP_ADD                  1
+               238          14 MAP_ADD                  1
                
-               221          16 LOAD_CONST               3 ('AK')
+               240          16 LOAD_CONST               3 ('AK')
                             18 LOAD_CONST               4 ('Alaska')
                
-               219          20 MAP_ADD                  1
+               238          20 MAP_ADD                  1
                
-               222          22 LOAD_CONST               5 ('AZ')
+               241          22 LOAD_CONST               5 ('AZ')
                             24 LOAD_CONST               6 ('Arizona')
                
-               219          26 MAP_ADD                  1
+               238          26 MAP_ADD                  1
                
-               223          28 LOAD_CONST               7 ('AR')
+               242          28 LOAD_CONST               7 ('AR')
                             30 LOAD_CONST               8 ('Arkansas')
                
-               219          32 MAP_ADD                  1
+               238          32 MAP_ADD                  1
                
-               224          34 LOAD_CONST               9 ('CA')
+               243          34 LOAD_CONST               9 ('CA')
                             36 LOAD_CONST              10 ('California')
                
-               219          38 MAP_ADD                  1
+               238          38 MAP_ADD                  1
                
-               225          40 LOAD_CONST              11 ('CO')
+               244          40 LOAD_CONST              11 ('CO')
                             42 LOAD_CONST              12 ('Colorado')
                
-               219          44 MAP_ADD                  1
+               238          44 MAP_ADD                  1
                
-               226          46 LOAD_CONST              13 ('CT')
+               245          46 LOAD_CONST              13 ('CT')
                             48 LOAD_CONST              14 ('Connecticut')
                
-               219          50 MAP_ADD                  1
+               238          50 MAP_ADD                  1
                
-               227          52 LOAD_CONST              15 ('DE')
+               246          52 LOAD_CONST              15 ('DE')
                             54 LOAD_CONST              16 ('Delaware')
                
-               219          56 MAP_ADD                  1
+               238          56 MAP_ADD                  1
                
-               228          58 LOAD_CONST              17 ('FL')
+               247          58 LOAD_CONST              17 ('FL')
                             60 LOAD_CONST              18 ('Florida')
                
-               219          62 MAP_ADD                  1
+               238          62 MAP_ADD                  1
                
-               229          64 LOAD_CONST              19 ('GA')
+               248          64 LOAD_CONST              19 ('GA')
                             66 LOAD_CONST              20 ('Georgia')
                
-               219          68 MAP_ADD                  1
+               238          68 MAP_ADD                  1
                
-               230          70 LOAD_CONST              21 ('HI')
+               249          70 LOAD_CONST              21 ('HI')
                             72 LOAD_CONST              22 ('Hawaii')
                
-               219          74 MAP_ADD                  1
+               238          74 MAP_ADD                  1
                
-               231          76 LOAD_CONST              23 ('ID')
+               250          76 LOAD_CONST              23 ('ID')
                             78 LOAD_CONST              24 ('Idaho')
                
-               219          80 MAP_ADD                  1
+               238          80 MAP_ADD                  1
                
-               232          82 LOAD_CONST              25 ('IL')
+               251          82 LOAD_CONST              25 ('IL')
                             84 LOAD_CONST              26 ('Illinois')
                
-               219          86 MAP_ADD                  1
+               238          86 MAP_ADD                  1
                
-               233          88 LOAD_CONST              27 ('IN')
+               252          88 LOAD_CONST              27 ('IN')
                             90 LOAD_CONST              28 ('Indiana')
                
-               219          92 MAP_ADD                  1
+               238          92 MAP_ADD                  1
                
-               234          94 LOAD_CONST              29 ('IA')
+               253          94 LOAD_CONST              29 ('IA')
                             96 LOAD_CONST              30 ('Iowa')
                
-               219          98 MAP_ADD                  1
+               238          98 MAP_ADD                  1
                
-               235         100 LOAD_CONST              31 ('KS')
+               254         100 LOAD_CONST              31 ('KS')
                            102 LOAD_CONST              32 ('Kansas')
                
-               219         104 MAP_ADD                  1
+               238         104 MAP_ADD                  1
                
-               236         106 LOAD_CONST              33 ('KY')
+               255         106 LOAD_CONST              33 ('KY')
                            108 LOAD_CONST              34 ('Kentucky')
                
-               219         110 MAP_ADD                  1
+               238         110 MAP_ADD                  1
                            112 BUILD_MAP                0
                
-               237         114 LOAD_CONST              35 ('LA')
+               256         114 LOAD_CONST              35 ('LA')
                            116 LOAD_CONST              36 ('Louisiana')
                
-               219         118 MAP_ADD                  1
+               238         118 MAP_ADD                  1
                
-               238         120 LOAD_CONST              37 ('ME')
+               257         120 LOAD_CONST              37 ('ME')
                            122 LOAD_CONST              38 ('Maine')
                
-               219         124 MAP_ADD                  1
+               238         124 MAP_ADD                  1
                
-               239         126 LOAD_CONST              39 ('MD')
+               258         126 LOAD_CONST              39 ('MD')
                            128 LOAD_CONST              40 ('Maryland')
                
-               219         130 MAP_ADD                  1
+               238         130 MAP_ADD                  1
                
-               240         132 LOAD_CONST              41 ('MA')
+               259         132 LOAD_CONST              41 ('MA')
                            134 LOAD_CONST              42 ('Massachusetts')
                
-               219         136 MAP_ADD                  1
+               238         136 MAP_ADD                  1
                
-               241         138 LOAD_CONST              43 ('MI')
+               260         138 LOAD_CONST              43 ('MI')
                            140 LOAD_CONST              44 ('Michigan')
                
-               219         142 MAP_ADD                  1
+               238         142 MAP_ADD                  1
                
-               242         144 LOAD_CONST              45 ('MN')
+               261         144 LOAD_CONST              45 ('MN')
                            146 LOAD_CONST              46 ('Minnesota')
                
-               219         148 MAP_ADD                  1
+               238         148 MAP_ADD                  1
                
-               243         150 LOAD_CONST              47 ('MS')
+               262         150 LOAD_CONST              47 ('MS')
                            152 LOAD_CONST              48 ('Mississippi')
                
-               219         154 MAP_ADD                  1
+               238         154 MAP_ADD                  1
                
-               244         156 LOAD_CONST              49 ('MO')
+               263         156 LOAD_CONST              49 ('MO')
                            158 LOAD_CONST              50 ('Missouri')
                
-               219         160 MAP_ADD                  1
+               238         160 MAP_ADD                  1
                
-               245         162 LOAD_CONST              51 ('MT')
+               264         162 LOAD_CONST              51 ('MT')
                            164 LOAD_CONST              52 ('Montana')
                
-               219         166 MAP_ADD                  1
+               238         166 MAP_ADD                  1
                
-               246         168 LOAD_CONST              53 ('NE')
+               265         168 LOAD_CONST              53 ('NE')
                            170 LOAD_CONST              54 ('Nebraska')
                
-               219         172 MAP_ADD                  1
+               238         172 MAP_ADD                  1
                
-               247         174 LOAD_CONST              55 ('NV')
+               266         174 LOAD_CONST              55 ('NV')
                            176 LOAD_CONST              56 ('Nevada')
                
-               219         178 MAP_ADD                  1
+               238         178 MAP_ADD                  1
                
-               248         180 LOAD_CONST              57 ('NH')
+               267         180 LOAD_CONST              57 ('NH')
                            182 LOAD_CONST              58 ('New Hampshire')
                
-               219         184 MAP_ADD                  1
+               238         184 MAP_ADD                  1
                
-               249         186 LOAD_CONST              59 ('NJ')
+               268         186 LOAD_CONST              59 ('NJ')
                            188 LOAD_CONST              60 ('New Jersey')
                
-               219         190 MAP_ADD                  1
+               238         190 MAP_ADD                  1
                
-               250         192 LOAD_CONST              61 ('NM')
+               269         192 LOAD_CONST              61 ('NM')
                            194 LOAD_CONST              62 ('New Mexico')
                
-               219         196 MAP_ADD                  1
+               238         196 MAP_ADD                  1
                
-               251         198 LOAD_CONST              63 ('NY')
+               270         198 LOAD_CONST              63 ('NY')
                            200 LOAD_CONST              64 ('New York')
                
-               219         202 MAP_ADD                  1
+               238         202 MAP_ADD                  1
                
-               252         204 LOAD_CONST              65 ('NC')
+               271         204 LOAD_CONST              65 ('NC')
                            206 LOAD_CONST              66 ('North Carolina')
                
-               219         208 MAP_ADD                  1
+               238         208 MAP_ADD                  1
                
-               253         210 LOAD_CONST              67 ('ND')
+               272         210 LOAD_CONST              67 ('ND')
                            212 LOAD_CONST              68 ('North Dakota')
                
-               219         214 MAP_ADD                  1
+               238         214 MAP_ADD                  1
                            216 DICT_UPDATE              1
                            218 BUILD_MAP                0
                
-               254         220 LOAD_CONST              69 ('OH')
+               273         220 LOAD_CONST              69 ('OH')
                            222 LOAD_CONST              70 ('Ohio')
                
-               219         224 MAP_ADD                  1
+               238         224 MAP_ADD                  1
                
-               255         226 LOAD_CONST              71 ('OK')
+               274         226 LOAD_CONST              71 ('OK')
                            228 LOAD_CONST              72 ('Oklahoma')
                
-               219         230 MAP_ADD                  1
+               238         230 MAP_ADD                  1
                
-               256         232 LOAD_CONST              73 ('OR')
+               275         232 LOAD_CONST              73 ('OR')
                            234 LOAD_CONST              74 ('Oregon')
                
-               219         236 MAP_ADD                  1
+               238         236 MAP_ADD                  1
                
-               257         238 LOAD_CONST              75 ('PA')
+               276         238 LOAD_CONST              75 ('PA')
                            240 LOAD_CONST              76 ('Pennsylvania')
                
-               219         242 MAP_ADD                  1
+               238         242 MAP_ADD                  1
                
-               258         244 LOAD_CONST              77 ('RI')
+               277         244 LOAD_CONST              77 ('RI')
                            246 LOAD_CONST              78 ('Rhode Island')
                
-               219         248 MAP_ADD                  1
+               238         248 MAP_ADD                  1
                
-               259         250 LOAD_CONST              79 ('SC')
+               278         250 LOAD_CONST              79 ('SC')
                            252 LOAD_CONST              80 ('South Carolina')
                
-               219         254 MAP_ADD                  1
+               238         254 MAP_ADD                  1
                
-               260         256 LOAD_CONST              81 ('SD')
+               279         256 LOAD_CONST              81 ('SD')
                            258 LOAD_CONST              82 ('South Dakota')
                
-               219         260 MAP_ADD                  1
+               238         260 MAP_ADD                  1
                
-               261         262 LOAD_CONST              83 ('TN')
+               280         262 LOAD_CONST              83 ('TN')
                            264 LOAD_CONST              84 ('Tennessee')
                
-               219         266 MAP_ADD                  1
+               238         266 MAP_ADD                  1
                
-               262         268 LOAD_CONST              85 ('TX')
+               281         268 LOAD_CONST              85 ('TX')
                            270 LOAD_CONST              86 ('Texas')
                
-               219         272 MAP_ADD                  1
+               238         272 MAP_ADD                  1
                
-               263         274 LOAD_CONST              87 ('UT')
+               282         274 LOAD_CONST              87 ('UT')
                            276 LOAD_CONST              88 ('Utah')
                
-               219         278 MAP_ADD                  1
+               238         278 MAP_ADD                  1
                
-               264         280 LOAD_CONST              89 ('VT')
+               283         280 LOAD_CONST              89 ('VT')
                            282 LOAD_CONST              90 ('Vermont')
                
-               219         284 MAP_ADD                  1
+               238         284 MAP_ADD                  1
                
-               265         286 LOAD_CONST              91 ('VA')
+               284         286 LOAD_CONST              91 ('VA')
                            288 LOAD_CONST              92 ('Virginia')
                
-               219         290 MAP_ADD                  1
+               238         290 MAP_ADD                  1
                
-               266         292 LOAD_CONST              93 ('WA')
+               285         292 LOAD_CONST              93 ('WA')
                            294 LOAD_CONST              94 ('Washington')
                
-               219         296 MAP_ADD                  1
+               238         296 MAP_ADD                  1
                
-               267         298 LOAD_CONST              95 ('WV')
+               286         298 LOAD_CONST              95 ('WV')
                            300 LOAD_CONST              96 ('West Virginia')
                
-               219         302 MAP_ADD                  1
+               238         302 MAP_ADD                  1
                
-               268         304 LOAD_CONST              97 ('WI')
+               287         304 LOAD_CONST              97 ('WI')
                            306 LOAD_CONST              98 ('Wisconsin')
                
-               219         308 MAP_ADD                  1
+               238         308 MAP_ADD                  1
                
-               269         310 LOAD_CONST              99 ('WY')
+               288         310 LOAD_CONST              99 ('WY')
                            312 LOAD_CONST             100 ('Wyoming')
                
-               219         314 MAP_ADD                  1
+               238         314 MAP_ADD                  1
                            316 DICT_UPDATE              1
                            318 STORE_DEREF              4 (STATES)
                
-               273         320 LOAD_CONST             101 ('United States')
+               292         320 LOAD_CONST             101 ('United States')
                
-               274         322 LOAD_CONST             102 ('Canada')
+               293         322 LOAD_CONST             102 ('Canada')
                
-               275         324 LOAD_CONST             103 ('Mexico')
+               294         324 LOAD_CONST             103 ('Mexico')
                
-               276         326 LOAD_CONST             104 ('United Kingdom')
+               295         326 LOAD_CONST             104 ('United Kingdom')
                
-               272         328 LOAD_CONST             105 (('USA', 'CAN', 'MEX', 'GBR'))
+               291         328 LOAD_CONST             105 (('USA', 'CAN', 'MEX', 'GBR'))
                            330 BUILD_CONST_KEY_MAP      4
                            332 STORE_DEREF              3 (COUNTRIES)
                
-               279         334 LOAD_CONST             106 ('return')
+               298         334 LOAD_CONST             106 ('return')
                            336 LOAD_GLOBAL              0 (list)
                            348 BUILD_TUPLE              2
                            350 LOAD_CLOSURE             3 (COUNTRIES)
                            352 LOAD_CLOSURE             4 (STATES)
                            354 LOAD_CLOSURE             0 (search)
                            356 BUILD_TUPLE              3
-                           358 LOAD_CONST             107 (<code object _hq_include, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 279>)
+                           358 LOAD_CONST             107 (<code object _hq_include, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 298>)
                            360 MAKE_FUNCTION           12 (annotations, closure)
                            362 STORE_FAST               1 (_hq_include)
                
-               304         364 LOAD_CONST             106 ('return')
+               323         364 LOAD_CONST             106 ('return')
                            366 LOAD_GLOBAL              0 (list)
                            378 BUILD_TUPLE              2
                            380 LOAD_CLOSURE             4 (STATES)
                            382 LOAD_CLOSURE             0 (search)
                            384 BUILD_TUPLE              2
-                           386 LOAD_CONST             108 (<code object _hq_exclude, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 304>)
+                           386 LOAD_CONST             108 (<code object _hq_exclude, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 323>)
                            388 MAKE_FUNCTION           12 (annotations, closure)
                            390 STORE_FAST               2 (_hq_exclude)
                
-               311         392 LOAD_CONST             109 ('any')
+               330         392 LOAD_CONST             109 ('any')
                
-               312         394 LOAD_DEREF               0 (search)
+               331         394 LOAD_DEREF               0 (search)
                            396 LOAD_ATTR                1 (inclusion)
                            406 LOAD_METHOD              2 (get)
                            428 LOAD_CONST             110 ('keywords')
                            430 BUILD_LIST               0
                            432 PRECALL                  2
                            436 CALL                     2
                
-               313         446 LOAD_DEREF               0 (search)
+               332         446 LOAD_DEREF               0 (search)
                            448 LOAD_ATTR                3 (exclusion)
                            458 LOAD_METHOD              2 (get)
                            480 LOAD_CONST             110 ('keywords')
                            482 BUILD_LIST               0
                            484 PRECALL                  2
                            488 CALL                     2
                
-               314         498 LOAD_DEREF               0 (search)
+               333         498 LOAD_DEREF               0 (search)
                            500 LOAD_ATTR                1 (inclusion)
                            510 LOAD_METHOD              2 (get)
                
-               315         532 LOAD_CONST             111 ('employees_range')
+               334         532 LOAD_CONST             111 ('employees_range')
                            534 BUILD_LIST               0
                
-               314         536 PRECALL                  2
+               333         536 PRECALL                  2
                            540 CALL                     2
                
-               317         550 LOAD_DEREF               0 (search)
+               336         550 LOAD_DEREF               0 (search)
                            552 LOAD_ATTR                1 (inclusion)
                            562 LOAD_METHOD              2 (get)
                            584 LOAD_CONST             112 ('ownership')
                            586 LOAD_CONST             113 ('')
                            588 PRECALL                  2
                            592 CALL                     2
                
-               319         602 PUSH_NULL
+               338         602 PUSH_NULL
                            604 LOAD_FAST                1 (_hq_include)
                            606 PRECALL                  0
                            610 CALL                     0
                
-               320         620 PUSH_NULL
+               339         620 PUSH_NULL
                            622 LOAD_FAST                2 (_hq_exclude)
                            624 PRECALL                  0
                            628 CALL                     0
                
-               318         638 LOAD_CONST             114 (('include', 'exclude'))
+               337         638 LOAD_CONST             114 (('include', 'exclude'))
                            640 BUILD_CONST_KEY_MAP      2
                
-               310         642 LOAD_CONST             115 (('op', 'include', 'exclude', 'grata_employees_estimates_range', 'ownership', 'headquarters'))
+               329         642 LOAD_CONST             115 (('op', 'include', 'exclude', 'grata_employees_estimates_range', 'ownership', 'headquarters'))
                            644 BUILD_CONST_KEY_MAP      6
                            646 RETURN_VALUE
                consts
                   None
                   'AL'
                   'Alabama'
                   'AK'
@@ -2089,134 +2298,134 @@
                         010000ab01000000000000000001008c207405000000000000000000007c
                         03a6010000ab01000000000000000064046b040000000072227c0344005d
                         1f7d067c00a0030000000000000000000000000000000000000000640389
                         077c06190000000000000000006901a6010000ab01000000000000000001
                         008c207c005300
                                    0 COPY_FREE_VARS           3
                      
-                     279           2 RESUME                   0
+                     298           2 RESUME                   0
                      
-                     280           4 BUILD_LIST               0
+                     299           4 BUILD_LIST               0
                                    6 STORE_FAST               0 (include)
                      
-                     281           8 LOAD_DEREF               9 (search)
+                     300           8 LOAD_DEREF               9 (search)
                                   10 LOAD_ATTR                0 (inclusion)
                                   20 LOAD_METHOD              1 (get)
                                   42 LOAD_CONST               1 ('city')
                                   44 BUILD_LIST               0
                                   46 PRECALL                  2
                                   50 CALL                     2
                                   60 STORE_FAST               1 (cities)
                      
-                     282          62 LOAD_DEREF               9 (search)
+                     301          62 LOAD_DEREF               9 (search)
                                   64 LOAD_ATTR                0 (inclusion)
                                   74 LOAD_METHOD              1 (get)
                                   96 LOAD_CONST               2 ('state')
                                   98 BUILD_LIST               0
                                  100 PRECALL                  2
                                  104 CALL                     2
                                  114 STORE_FAST               2 (states)
                      
-                     283         116 LOAD_DEREF               9 (search)
+                     302         116 LOAD_DEREF               9 (search)
                                  118 LOAD_ATTR                0 (inclusion)
                                  128 LOAD_METHOD              1 (get)
                                  150 LOAD_CONST               3 ('country')
                                  152 BUILD_LIST               0
                                  154 PRECALL                  2
                                  158 CALL                     2
                                  168 STORE_FAST               3 (countries)
                      
-                     285         170 LOAD_GLOBAL              5 (NULL + len)
+                     304         170 LOAD_GLOBAL              5 (NULL + len)
                                  182 LOAD_FAST                1 (cities)
                                  184 PRECALL                  1
                                  188 CALL                     1
                                  198 LOAD_CONST               4 (0)
                                  200 COMPARE_OP               4 (>)
                                  206 POP_JUMP_FORWARD_IF_FALSE    46 (to 300)
                      
-                     287         208 LOAD_DEREF               8 (STATES)
+                     306         208 LOAD_DEREF               8 (STATES)
                                  210 LOAD_FAST                2 (states)
                                  212 LOAD_CONST               4 (0)
                                  214 BINARY_SUBSCR
                                  224 BINARY_SUBSCR
                                  234 STORE_FAST               4 (state)
                      
-                     288         236 LOAD_FAST                1 (cities)
+                     307         236 LOAD_FAST                1 (cities)
                                  238 GET_ITER
                              >>  240 FOR_ITER                27 (to 296)
                                  242 STORE_FAST               5 (city)
                      
-                     289         244 LOAD_FAST                0 (include)
+                     308         244 LOAD_FAST                0 (include)
                                  246 LOAD_METHOD              3 (append)
                      
-                     290         268 LOAD_FAST                5 (city)
+                     309         268 LOAD_FAST                5 (city)
                                  270 LOAD_FAST                4 (state)
                                  272 LOAD_CONST               5 ('United States')
                                  274 LOAD_CONST               6 (('city', 'state', 'country'))
                                  276 BUILD_CONST_KEY_MAP      3
                      
-                     289         278 PRECALL                  1
+                     308         278 PRECALL                  1
                                  282 CALL                     1
                                  292 POP_TOP
                                  294 JUMP_BACKWARD           28 (to 240)
                      
-                     292     >>  296 LOAD_FAST                0 (include)
+                     311     >>  296 LOAD_FAST                0 (include)
                                  298 RETURN_VALUE
                      
-                     294     >>  300 LOAD_GLOBAL              5 (NULL + len)
+                     313     >>  300 LOAD_GLOBAL              5 (NULL + len)
                                  312 LOAD_FAST                2 (states)
                                  314 PRECALL                  1
                                  318 CALL                     1
                                  328 LOAD_CONST               4 (0)
                                  330 COMPARE_OP               4 (>)
                                  336 POP_JUMP_FORWARD_IF_FALSE    34 (to 406)
                      
-                     295         338 LOAD_FAST                2 (states)
+                     314         338 LOAD_FAST                2 (states)
                                  340 GET_ITER
                              >>  342 FOR_ITER                31 (to 406)
                                  344 STORE_FAST               4 (state)
                      
-                     297         346 LOAD_FAST                0 (include)
+                     316         346 LOAD_FAST                0 (include)
                                  348 LOAD_METHOD              3 (append)
                                  370 LOAD_CONST               2 ('state')
                                  372 LOAD_DEREF               8 (STATES)
                                  374 LOAD_FAST                4 (state)
                                  376 BINARY_SUBSCR
                                  386 BUILD_MAP                1
                                  388 PRECALL                  1
                                  392 CALL                     1
                                  402 POP_TOP
                                  404 JUMP_BACKWARD           32 (to 342)
                      
-                     299     >>  406 LOAD_GLOBAL              5 (NULL + len)
+                     318     >>  406 LOAD_GLOBAL              5 (NULL + len)
                                  418 LOAD_FAST                3 (countries)
                                  420 PRECALL                  1
                                  424 CALL                     1
                                  434 LOAD_CONST               4 (0)
                                  436 COMPARE_OP               4 (>)
                                  442 POP_JUMP_FORWARD_IF_FALSE    34 (to 512)
                      
-                     300         444 LOAD_FAST                3 (countries)
+                     319         444 LOAD_FAST                3 (countries)
                                  446 GET_ITER
                              >>  448 FOR_ITER                31 (to 512)
                                  450 STORE_FAST               6 (country)
                      
-                     301         452 LOAD_FAST                0 (include)
+                     320         452 LOAD_FAST                0 (include)
                                  454 LOAD_METHOD              3 (append)
                                  476 LOAD_CONST               3 ('country')
                                  478 LOAD_DEREF               7 (COUNTRIES)
                                  480 LOAD_FAST                6 (country)
                                  482 BINARY_SUBSCR
                                  492 BUILD_MAP                1
                                  494 PRECALL                  1
                                  498 CALL                     1
                                  508 POP_TOP
                                  510 JUMP_BACKWARD           32 (to 448)
                      
-                     302     >>  512 LOAD_FAST                0 (include)
+                     321     >>  512 LOAD_FAST                0 (include)
                                  514 RETURN_VALUE
                      consts
                         None
                         'city'
                         'state'
                         'country'
                         0
@@ -2224,15 +2433,15 @@
                         ('city', 'state', 'country')
                      names      ('inclusion', 'get', 'len', 'append')
                      varnames   ('include', 'cities', 'states', 'countries', 'state', 'city', 'country')
                      freevars   ('COUNTRIES', 'STATES', 'search')
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '_hq_include'
-                     firstlineno 279
+                     firstlineno 298
                      lnotab
                         0x0401040136013601360226021c01080118010aff12030402260108023c
                         02260108013c01
                   code
                      argcount  : 0
                      nlocals   : 2
                      stacksize : 6
@@ -2241,129 +2450,128 @@
                         0x9502970067007d0089036a000000000000000000a00100000000000000
                         0000000000000000000000000064016700a6020000ab0200000000000000
                         0044005d1f7d017c00a00200000000000000000000000000000000000000
                         00640189027c01190000000000000000006901a6010000ab010000000000
                         00000001008c207c005300
                                    0 COPY_FREE_VARS           2
                      
-                     304           2 RESUME                   0
+                     323           2 RESUME                   0
                      
-                     305           4 BUILD_LIST               0
+                     324           4 BUILD_LIST               0
                                    6 STORE_FAST               0 (exclude)
                      
-                     306           8 LOAD_DEREF               3 (search)
+                     325           8 LOAD_DEREF               3 (search)
                                   10 LOAD_ATTR                0 (exclusion)
                                   20 LOAD_METHOD              1 (get)
                                   42 LOAD_CONST               1 ('state')
                                   44 BUILD_LIST               0
                                   46 PRECALL                  2
                                   50 CALL                     2
                                   60 GET_ITER
                              >>   62 FOR_ITER                31 (to 126)
                                   64 STORE_FAST               1 (state)
                      
-                     307          66 LOAD_FAST                0 (exclude)
+                     326          66 LOAD_FAST                0 (exclude)
                                   68 LOAD_METHOD              2 (append)
                                   90 LOAD_CONST               1 ('state')
                                   92 LOAD_DEREF               2 (STATES)
                                   94 LOAD_FAST                1 (state)
                                   96 BINARY_SUBSCR
                                  106 BUILD_MAP                1
                                  108 PRECALL                  1
                                  112 CALL                     1
                                  122 POP_TOP
                                  124 JUMP_BACKWARD           32 (to 62)
                      
-                     308     >>  126 LOAD_FAST                0 (exclude)
+                     327     >>  126 LOAD_FAST                0 (exclude)
                                  128 RETURN_VALUE
                      consts
                         None
                         'state'
                      names      ('exclusion', 'get', 'append')
                      varnames   ('exclude', 'state')
                      freevars   ('STATES', 'search')
                      cellvars   ()
                      filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                      name       '_hq_exclude'
-                     firstlineno 304
+                     firstlineno 323
                      lnotab 0x040104013a013c01
                   'any'
                   'keywords'
                   'employees_range'
                   'ownership'
                   ''
                   ('include', 'exclude')
                   ('op', 'include', 'exclude', 'grata_employees_estimates_range', 'ownership', 'headquarters')
                names      ('list', 'inclusion', 'get', 'exclusion')
                varnames   ('search', '_hq_include', '_hq_exclude')
                freevars   ()
                cellvars   ('search', 'COUNTRIES', 'STATES')
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       '_get_api_filter'
-               firstlineno 218
+               firstlineno 237
                lnotab
                   0x0801020104ff020204fe020304fd020404fc020504fb020604fa020704
                   f9020804f8020904f7020a04f6020b04f5020c04f4020d04f3020e04f202
                   0f04f1021004f0021104ef041204ee021304ed021404ec021504eb021604
                   ea021704e9021804e8021904e7021a04e6021b04e5021c04e4021d04e302
                   1e04e2021f04e1022004e0022104df022204de062304dd022404dc022504
                   db022604da022704d9022804d8022904d7022a04d6022b04d5022c04d402
                   2d04d3022e04d2022f04d1023004d0023104cf023204ce06360201020102
                   0102fc06071e191c07020134013401220104ff0e033402120112fe04f8
-            None
-         names      ('__name__', '__module__', '__qualname__', 'secrets', 'access_secret_version', 'HEADERS', 'str', 'models', 'Search', 'list', 'find_similar', 'dict', 'find_by_criteria', 'enrich', '_get_api_filter')
+         names      ('__name__', '__module__', '__qualname__', 'secrets', 'access_secret_version', 'HEADERS', 'str', 'models', 'Search', 'list', 'find_similar', 'dict', 'find_by_criteria', 'enrich', 'pd', 'DataFrame', 'enrich_targets_async', '_get_api_filter')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
          name       'GrataWrapper'
-         firstlineno 171
-         lnotab 0x0a021e0102fe06051e131a0b100b
+         firstlineno 172
+         lnotab 0x0a021e0102fe06051e161a0b100b1a0f
       'GrataWrapper'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a026401650364026504640365056606640484045a
             0664026504640365056604640584045a0764016503640365056604640684
             045a0864075300
-         325           0 RESUME                   0
+         344           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SourceScrubWrapper')
                        8 STORE_NAME               2 (__qualname__)
          
-         326          10 LOAD_CONST               1 ('domain')
+         345          10 LOAD_CONST               1 ('domain')
                       12 LOAD_NAME                3 (str)
                       14 LOAD_CONST               2 ('search')
                       16 LOAD_NAME                4 (Search)
                       18 LOAD_CONST               3 ('return')
                       20 LOAD_NAME                5 (dict)
                       22 BUILD_TUPLE              6
-                      24 LOAD_CONST               4 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 326>)
+                      24 LOAD_CONST               4 (<code object find_similar, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 345>)
                       26 MAKE_FUNCTION            4 (annotations)
                       28 STORE_NAME               6 (find_similar)
          
-         329          30 LOAD_CONST               2 ('search')
+         348          30 LOAD_CONST               2 ('search')
                       32 LOAD_NAME                4 (Search)
                       34 LOAD_CONST               3 ('return')
                       36 LOAD_NAME                5 (dict)
                       38 BUILD_TUPLE              4
-                      40 LOAD_CONST               5 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 329>)
+                      40 LOAD_CONST               5 (<code object find_by_criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 348>)
                       42 MAKE_FUNCTION            4 (annotations)
                       44 STORE_NAME               7 (find_by_criteria)
          
-         332          46 LOAD_CONST               1 ('domain')
+         351          46 LOAD_CONST               1 ('domain')
                       48 LOAD_NAME                3 (str)
                       50 LOAD_CONST               3 ('return')
                       52 LOAD_NAME                5 (dict)
                       54 BUILD_TUPLE              4
-                      56 LOAD_CONST               6 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 332>)
+                      56 LOAD_CONST               6 (<code object enrich, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py", line 351>)
                       58 MAKE_FUNCTION            4 (annotations)
                       60 STORE_NAME               8 (enrich)
                       62 LOAD_CONST               7 (None)
                       64 RETURN_VALUE
          consts
             'SourceScrubWrapper'
             'domain'
@@ -2371,81 +2579,81 @@
             'return'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               326           0 RESUME                   0
+               345           0 RESUME                   0
                
-               327           2 LOAD_CONST               0 (None)
+               346           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('domain', 'search')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_similar'
-               firstlineno 326
+               firstlineno 345
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               329           0 RESUME                   0
+               348           0 RESUME                   0
                
-               330           2 LOAD_CONST               0 (None)
+               349           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('search',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'find_by_criteria'
-               firstlineno 329
+               firstlineno 348
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               332           0 RESUME                   0
+               351           0 RESUME                   0
                
-               333           2 LOAD_CONST               0 (None)
+               352           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('domain',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
                name       'enrich'
-               firstlineno 332
+               firstlineno 351
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'str', 'Search', 'dict', 'find_similar', 'find_by_criteria', 'enrich')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
          name       'SourceScrubWrapper'
-         firstlineno 325
+         firstlineno 344
          lnotab 0x0a0114031003
       'SourceScrubWrapper'
-   names      ('time', 'concurrent.futures', 'ThreadPoolExecutor', 'functools', 'partial', 'typing', 'List', 'googlemaps', 'requests', 'gandai', 'gpt', 'helpers', 'models', 'query', 'secrets', 'gandai.models', 'Search', 'Client', 'access_secret_version', 'gmaps', 'MAX_WORKERS', 'GoogleMapsWrapper', 'GrataWrapper', 'SourceScrubWrapper')
+   names      ('time', 'pandas', 'pd', 'concurrent.futures', 'ThreadPoolExecutor', 'functools', 'partial', 'typing', 'List', 'googlemaps', 'requests', 'gandai', 'gpt', 'helpers', 'models', 'query', 'secrets', 'gandai.models', 'Search', 'Client', 'access_secret_version', 'gmaps', 'MAX_WORKERS', 'GoogleMapsWrapper', 'GrataWrapper', 'SourceScrubWrapper')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/sources.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020108010c010c010c02080108021c010c023e0104031a7f001c1a
-      7f001b
+      0x00ff0201080108010c010c010c02080108021c010c023e0104031a7f00
+      1c1a7f002d
```

### Comparing `gandai-1.3.5/gandai/analytics.py` & `gandai-1.3.6/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/auth.py` & `gandai-1.3.6/gandai/auth.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/db.py` & `gandai-1.3.6/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/gpt.py` & `gandai-1.3.6/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/main.py` & `gandai-1.3.6/gandai/main.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.3.6/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/migrations/db_seed.py` & `gandai-1.3.6/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/migrations/dealcloud.py` & `gandai-1.3.6/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/migrations/sql/schema.sql` & `gandai-1.3.6/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/models.py` & `gandai-1.3.6/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/query.py` & `gandai-1.3.6/gandai/query.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/secrets.py` & `gandai-1.3.6/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.3.5/gandai/sources.py` & `gandai-1.3.6/gandai/sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+import pandas as pd
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 from typing import List
 
 import googlemaps
 import requests
 
@@ -172,24 +173,27 @@
     HEADERS = {
         "Authorization": secrets.access_secret_version("GRATA_API_TOKEN"),
         "Content-Type": "application/json",
     }
 
     def find_similar(domain: str, search: models.Search) -> list:
         api_filters = GrataWrapper._get_api_filter(search)
-        response = requests.post(
-            "https://search.grata.com/api/v1.2/search-similar/",
-            headers=GrataWrapper.HEADERS,
-            json={
+        similiar_filters = {
                 "domain": domain,
                 "grata_employees_estimates_range": api_filters[
                     "grata_employees_estimates_range"
                 ],
                 "headquarters": api_filters["headquarters"],
-            },
+                "ownership": api_filters["ownership"]
+            }
+        print(similiar_filters)
+        response = requests.post(
+            "https://search.grata.com/api/v1.2/search-similar/",
+            headers=GrataWrapper.HEADERS,
+            json=similiar_filters,
         )
         data = response.json()
         # print("find_similar:", data)
         data["companies"] = data.get("results", [])  # asking grata about this
 
         return data["companies"]
 
@@ -211,14 +215,29 @@
             json={"domain": domain},
         )
         data = response.json()
         data["linkedin"] = data.get("social_linkedin")
         data["ownership"] = data.get("ownership_status")
         return data
 
+    def enrich_targets_async(targets: pd.DataFrame) -> None:
+        def enrich_company_by_domain(domain: str) -> None:
+            company = query.find_company_by_domain(domain)
+            if "company_uid" not in company.meta.keys():
+                # print(company.name)
+                resp = GrataWrapper.enrich(domain)
+                company.description = resp.get("description")
+                company.meta = {**company.meta, **resp}  # merge 3.5+
+                query.update_company(company)
+
+            with ThreadPoolExecutor(max_workers=5) as executor:
+                executor.map(
+                    enrich_company_by_domain, targets["domain"].tolist()
+                )
+
     def _get_api_filter(search: models.Search) -> dict:
         STATES = {
             "AL": "Alabama",
             "AK": "Alaska",
             "AZ": "Arizona",
             "AR": "Arkansas",
             "CA": "California",
```

### Comparing `gandai-1.3.5/gandai.egg-info/SOURCES.txt` & `gandai-1.3.6/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

