# Comparing `tmp/unigui-1.9.2.tar.gz` & `tmp/unigui-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.9.2.tar", last modified: Tue Jul 25 17:54:52 2023, max compression
+gzip compressed data, was "dist/unigui-1.9.3.tar", last modified: Wed Jul 26 06:10:35 2023, max compression
```

## Comparing `unigui-1.9.2.tar` & `unigui-1.9.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)     5365 2023-07-25 04:13:41.000000 unigui-1.9.2/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3583 2023-07-25 06:24:07.000000 unigui-1.9.2/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)     4299 2023-07-25 09:16:10.000000 unigui-1.9.2/unigui/tables.py
--rw-rw-r--   0 george    (1000) george    (1000)      128 2023-07-25 04:04:00.000000 unigui-1.9.2/unigui/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)     7226 2023-07-25 05:54:26.000000 unigui-1.9.2/unigui/autotest.py
--rw-r--r--   0 george    (1000) george    (1000)     2623 2023-07-24 13:07:39.000000 unigui-1.9.2/unigui/utils.py
--rw-rw-r--   0 george    (1000) george    (1000)     5565 2023-07-24 17:13:07.000000 unigui-1.9.2/unigui/reloader.py
--rw-rw-r--   0 george    (1000) george    (1000)     8678 2023-07-24 17:31:39.000000 unigui-1.9.2/unigui/users.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)     2750 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/css/344.ca964e27.css
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/css/vendor.f747ec02.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)  1436034 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/js/vendor.5659ce27.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)    48615 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/js/344.037a8712.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)     5923 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/js/app.1711f3eb.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-25 17:47:14.000000 unigui-1.9.2/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.2/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      630 2023-07-25 17:54:11.000000 unigui-1.9.2/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19239 2023-07-25 17:54:52.000000 unigui-1.9.2/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-25 17:54:52.000000 unigui-1.9.2/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18934 2023-07-17 14:52:22.000000 unigui-1.9.2/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.2/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       54 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19239 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.2/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1258 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-25 17:54:52.000000 unigui-1.9.2/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)     5250 2023-07-26 02:29:57.000000 unigui-1.9.3/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3567 2023-07-26 04:23:41.000000 unigui-1.9.3/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)     4299 2023-07-25 09:16:10.000000 unigui-1.9.3/unigui/tables.py
+-rw-rw-r--   0 george    (1000) george    (1000)      128 2023-07-25 04:04:00.000000 unigui-1.9.3/unigui/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7315 2023-07-26 04:40:00.000000 unigui-1.9.3/unigui/autotest.py
+-rw-r--r--   0 george    (1000) george    (1000)     2623 2023-07-24 13:07:39.000000 unigui-1.9.3/unigui/utils.py
+-rw-rw-r--   0 george    (1000) george    (1000)     5565 2023-07-24 17:13:07.000000 unigui-1.9.3/unigui/reloader.py
+-rw-rw-r--   0 george    (1000) george    (1000)     8686 2023-07-26 05:57:11.000000 unigui-1.9.3/unigui/users.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)     2750 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/css/344.ca964e27.css
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/css/vendor.f747ec02.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)  1436034 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/js/vendor.5659ce27.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)    48615 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/js/344.037a8712.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5923 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/js/app.1711f3eb.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.3/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      642 2023-07-26 06:09:58.000000 unigui-1.9.3/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19239 2023-07-26 06:10:35.000000 unigui-1.9.3/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-26 06:10:35.000000 unigui-1.9.3/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    18934 2023-07-17 14:52:22.000000 unigui-1.9.3/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.3/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       63 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19239 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.3/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1258 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.9.2/unigui/guielements.py` & `unigui-1.9.3/unigui/guielements.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,15 @@
         
     def add(self, kwargs):              
         for key, value in kwargs.items():
             setattr(self, key, value) 
 
     def mutate(self, obj):
         self.__dict__ = obj.__dict__ 
-
-    def __getstate__(self):
-        return {key: value for key,value in self.__dict__.items() if '__' not in key}    
-
+    
     def accept(self, value):
         if hasattr(self, 'changed'):
             self.changed(self, value)
         else:
             self.value = value
 
 Line = Gui("Line", type = 'line')
```

### Comparing `unigui-1.9.2/unigui/server.py` & `unigui-1.9.3/unigui/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     User.UserType = user_type    
 
     if config.autotest:
         run_tests()
 
     http_handlers.insert(0, web.get('/ws', websocket_handler))        
-    http_handlers += [web.static(f'/{config.upload_dir}', f"/{app_dir}/{upload_dir}"), 
+    http_handlers += [web.static(f'/{config.upload_dir}', upload_dir), 
         web.get('/{tail:.*}', static_serve), web.post('/', post_handler)]
 
     print(f'Start {appname} web server..')    
     app = web.Application()
     app.add_routes(http_handlers)    
     web.run_app(app,  port=port)
```

### Comparing `unigui-1.9.2/unigui/tables.py` & `unigui-1.9.3/unigui/tables.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/autotest.py` & `unigui-1.9.3/unigui/autotest.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,25 +170,27 @@
     user.load()
     errors = []
     for module in user.screens:
         errors += check_screen(module)
     if errors:
         errors.insert(0, f'\n!!----Unigui detected errors in screens:')
         print('\n'.join(errors), '\n')
+    else:
+        print(f'\n----Screens definitions are correct. ')
         
     files = config.autotest
     ok = True
     process = False
     if os.path.exists(testdir):
         for file in os.listdir(testdir):
             if not os.path.isdir(file) and (files == '*' or file in files):
                 process = True
                 if not test(file,user):
                     ok = False
     if process and ok:
         print('-----Autotests successfully passed.-----')
-    
+    User.last_user = None
     User.toolbar.append(button)
```

### Comparing `unigui-1.9.2/unigui/utils.py` & `unigui-1.9.3/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/reloader.py` & `unigui-1.9.3/unigui/reloader.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/users.py` & `unigui-1.9.3/unigui/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             'prepare' : None,            
             'blocks' : [],
             'header' : config.appname,                        
             'toolbar' : [], 
             'order' : 0
         }             
         name = file[:-3]        
-        path = f'{screens_dir}/{file}'                
+        path = f'{screens_dir}{divpath}{file}'                
         spec = importlib.util.spec_from_file_location(name,path)
         module = importlib.util.module_from_spec(spec)        
                 
         module.user = self                               
         
         spec.loader.exec_module(module)            
         screen = Screen(module.name)
```

### Comparing `unigui-1.9.2/unigui/web/favicon.ico` & `unigui-1.9.3/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/css/344.ca964e27.css` & `unigui-1.9.3/unigui/web/css/344.ca964e27.css`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/css/vendor.f747ec02.css` & `unigui-1.9.3/unigui/web/css/vendor.f747ec02.css`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/icons/favicon-96x96.png` & `unigui-1.9.3/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/icons/favicon-16x16.png` & `unigui-1.9.3/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/icons/favicon-32x32.png` & `unigui-1.9.3/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/icons/favicon-128x128.png` & `unigui-1.9.3/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `unigui-1.9.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.9.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.9.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.9.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/js/vendor.5659ce27.js` & `unigui-1.9.3/unigui/web/js/vendor.5659ce27.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/js/430.591e9a73.js` & `unigui-1.9.3/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/js/344.037a8712.js` & `unigui-1.9.3/unigui/web/js/344.037a8712.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/js/193.283445be.js` & `unigui-1.9.3/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/js/app.1711f3eb.js` & `unigui-1.9.3/unigui/web/js/app.1711f3eb.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui/web/index.html` & `unigui-1.9.3/unigui/web/index.html`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/LICENSE` & `unigui-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/setup.py` & `unigui-1.9.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.9.2',      
+      version='1.9.3',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
       url="https://github.com/Claus1/unigui" ,      
       include_package_data=True,
       install_requires=[
-          'websockets','jsonpickle', 'aiohttp', 'watchdog', 'jsoncomparison'
+          'websockets','jsonpickle', 'aiohttp', 'watchdog', 'jsoncomparison', 'requests'
       ],
       zip_safe=False)
```

### Comparing `unigui-1.9.2/PKG-INFO` & `unigui-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.2
+Version: 1.9.3
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.9.2/README.md` & `unigui-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.9.2/unigui.egg-info/PKG-INFO` & `unigui-1.9.3/unigui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.2
+Version: 1.9.3
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.9.2/unigui.egg-info/SOURCES.txt` & `unigui-1.9.3/unigui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

