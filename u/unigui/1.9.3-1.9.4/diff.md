# Comparing `tmp/unigui-1.9.3.tar.gz` & `tmp/unigui-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.9.3.tar", last modified: Wed Jul 26 06:10:35 2023, max compression
+gzip compressed data, was "dist/unigui-1.9.4.tar", last modified: Wed Jul 26 16:10:40 2023, max compression
```

## Comparing `unigui-1.9.3.tar` & `unigui-1.9.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)     5250 2023-07-26 02:29:57.000000 unigui-1.9.3/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3567 2023-07-26 04:23:41.000000 unigui-1.9.3/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)     4299 2023-07-25 09:16:10.000000 unigui-1.9.3/unigui/tables.py
--rw-rw-r--   0 george    (1000) george    (1000)      128 2023-07-25 04:04:00.000000 unigui-1.9.3/unigui/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)     7315 2023-07-26 04:40:00.000000 unigui-1.9.3/unigui/autotest.py
--rw-r--r--   0 george    (1000) george    (1000)     2623 2023-07-24 13:07:39.000000 unigui-1.9.3/unigui/utils.py
--rw-rw-r--   0 george    (1000) george    (1000)     5565 2023-07-24 17:13:07.000000 unigui-1.9.3/unigui/reloader.py
--rw-rw-r--   0 george    (1000) george    (1000)     8686 2023-07-26 05:57:11.000000 unigui-1.9.3/unigui/users.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)     2750 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/css/344.ca964e27.css
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/css/vendor.f747ec02.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)  1436034 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/js/vendor.5659ce27.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)    48615 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/js/344.037a8712.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)     5923 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/js/app.1711f3eb.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-25 17:47:14.000000 unigui-1.9.3/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.3/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      642 2023-07-26 06:09:58.000000 unigui-1.9.3/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19239 2023-07-26 06:10:35.000000 unigui-1.9.3/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-26 06:10:35.000000 unigui-1.9.3/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18934 2023-07-17 14:52:22.000000 unigui-1.9.3/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.3/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       63 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19239 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.3/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1258 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-26 06:10:35.000000 unigui-1.9.3/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)     5250 2023-07-26 02:29:57.000000 unigui-1.9.4/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3558 2023-07-26 08:55:15.000000 unigui-1.9.4/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)     4299 2023-07-25 09:16:10.000000 unigui-1.9.4/unigui/tables.py
+-rw-rw-r--   0 george    (1000) george    (1000)      128 2023-07-25 04:04:00.000000 unigui-1.9.4/unigui/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)     7362 2023-07-26 09:52:46.000000 unigui-1.9.4/unigui/autotest.py
+-rw-r--r--   0 george    (1000) george    (1000)     2623 2023-07-24 13:07:39.000000 unigui-1.9.4/unigui/utils.py
+-rw-rw-r--   0 george    (1000) george    (1000)     5565 2023-07-24 17:13:07.000000 unigui-1.9.4/unigui/reloader.py
+-rw-rw-r--   0 george    (1000) george    (1000)     8713 2023-07-26 09:11:50.000000 unigui-1.9.4/unigui/users.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/css/vendor.f747ec02.css
+-rw-rw-r--   0 george    (1000) george    (1000)     2750 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/css/750.ca964e27.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)  1436034 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/js/vendor.5659ce27.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5923 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/js/app.df555111.js
+-rw-rw-r--   0 george    (1000) george    (1000)    48813 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/js/750.4831ed09.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-26 16:07:15.000000 unigui-1.9.4/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.9.4/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      642 2023-07-26 16:04:11.000000 unigui-1.9.4/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19239 2023-07-26 16:10:40.000000 unigui-1.9.4/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-26 16:10:40.000000 unigui-1.9.4/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    18934 2023-07-17 14:52:22.000000 unigui-1.9.4/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.9.4/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       63 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19239 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.9.4/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1258 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-26 16:10:40.000000 unigui-1.9.4/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.9.3/unigui/guielements.py` & `unigui-1.9.4/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/server.py` & `unigui-1.9.4/unigui/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,39 +42,39 @@
 
 async def websocket_handler(request):
     ws = web.WebSocketResponse()
     await ws.prepare(request)
     user, ok = make_user()
 
     async def send(res):
-        res = jsonString(user.prepare_result(res))
+        if type(res) != str:
+            res = jsonString(user.prepare_result(res))
         await ws.send_str(res)   
 
     user.send = send     
     user.session = request.remote    
-    await ws.send_str(jsonString(user.screen if ok else empty_app)) 
+    await send(user.screen if ok else empty_app) 
     try:
         async for msg in ws:
             if msg.type == WSMsgType.TEXT:
                 if msg.data == 'close':
                     await ws.close()
                 else:
                     input = json.loads(msg.data)            
                     result = user.result4message(input)
-                    if result:            
-                        result = user.prepare_result(result)
-                        await ws.send_str(jsonString(result))
+                    if result:                                    
+                        await send(result)
                     if recorder.record_file:
                         recorder.accept(input, result)
                     if config.mirror and not screen_switch_message(input):                        
                         if result:
                             broadcast(result, user)                            
                         msg_object = user.find_element(input)                         
                         if not isinstance(result, Message) or not result.contains(msg_object):                                                        
-                            broadcast(msg_object, user)
+                            broadcast(jsonString(user.prepare_result(msg_object)), user)
             elif msg.type == WSMsgType.ERROR:
                 user.log('ws connection closed with exception %s' % ws.exception())
     except:        
         user.log(traceback.format_exc())
 
     if User.reflections:
         User.reflections.remove(user)
```

### Comparing `unigui-1.9.3/unigui/tables.py` & `unigui-1.9.4/unigui/tables.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/autotest.py` & `unigui-1.9.4/unigui/autotest.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,32 +90,30 @@
                         err = value['_message']
                         print(f"\nTest {filename} is failed on message {user_message}!\n {err}\n")
     return not error
 
 test_name = Edit('Name test file', '', focus = True)
 rewrite = Switch('Overwrite existing', False, type = 'check')
 
-def button_clicked(x,y):
+def button_clicked(_,__):
     test_name.value = ''
     test_name.complete = smart_complete(os.listdir(testdir))
     return Dialog('Create autotest..', ask_create_test, test_name, rewrite)
 
 def create_test(fname):
-    fname = f'{testdir}/{fname}'
-    if not os.path.exists(testdir):
-        os.makedirs(testdir)
+    fname = f'{testdir}/{fname}'    
     if os.path.exists(fname) and not rewrite.value:
         return Warning(f'Test file {fname} already exists!')              
     
     button.mode = 'red'   
     button.tooltip = 'Stop test recording'
     button.changed = recorder.stop_recording
     recorder.start(fname)
     
-    return Info('Recording is running.. ',button)     
+    return Info('Recording is running.. press the same button to stop',button)     
 
 def ask_create_test(_, bname):
     if bname == 'Ok':            
         return create_test(test_name.value) if test_name.value else\
             Warning('Test file name is not defined!')
 
 button = Button('_Add test', button_clicked, 
@@ -162,23 +160,25 @@
                 block_names.add(bl.name)
             errors += check_dialog(bl)
     if errors:
         errors.insert(0, f"\nErrors in screen {self.name}, file name {module.__file__}:")
     return errors
     
 def run_tests():
+    if not os.path.exists(testdir):
+        os.makedirs(testdir)
     user = User.UserType()
     user.load()
     errors = []
     for module in user.screens:
         errors += check_screen(module)
     if errors:
         errors.insert(0, f'\n!!----Unigui detected errors in screens:')
         print('\n'.join(errors), '\n')
-    else:
+    elif user.screens:
         print(f'\n----Screens definitions are correct. ')
         
     files = config.autotest
     ok = True
     process = False
     if os.path.exists(testdir):
         for file in os.listdir(testdir):
```

### Comparing `unigui-1.9.3/unigui/utils.py` & `unigui-1.9.4/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/reloader.py` & `unigui-1.9.4/unigui/reloader.py`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/users.py` & `unigui-1.9.4/unigui/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
     def prepare_result(self, raw):
         if raw == UpdateScreen:
             raw = self.screen                        
         else:
             if isinstance(raw, Message):
                 raw.fill_paths4(self)                
-            elif isinstance(raw,Gui):
+            elif isinstance(raw,Gui) and raw is not self.screen:
                 raw = Message(raw, user = self)                 
             elif isinstance(raw, (list, tuple)) and all(isinstance(e,Gui) for e in raw):
                 raw = Message(*raw, user = self)
         return raw
 
     def process(self,arr):
         self.last_input = arr
```

### Comparing `unigui-1.9.3/unigui/web/favicon.ico` & `unigui-1.9.4/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/css/344.ca964e27.css` & `unigui-1.9.4/unigui/web/css/750.ca964e27.css`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/css/vendor.f747ec02.css` & `unigui-1.9.4/unigui/web/css/vendor.f747ec02.css`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/icons/favicon-96x96.png` & `unigui-1.9.4/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/icons/favicon-16x16.png` & `unigui-1.9.4/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/icons/favicon-32x32.png` & `unigui-1.9.4/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/icons/favicon-128x128.png` & `unigui-1.9.4/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `unigui-1.9.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.9.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.9.4/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.9.4/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.9.4/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/js/vendor.5659ce27.js` & `unigui-1.9.4/unigui/web/js/vendor.5659ce27.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/js/430.591e9a73.js` & `unigui-1.9.4/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/js/344.037a8712.js` & `unigui-1.9.4/unigui/web/js/750.4831ed09.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [344], {
-        8344: (e, t, a) => {
+    [750], {
+        8750: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => la
+                default: () => sa
             });
             var s = a(3673),
                 l = a(2323);
             const i = (0, s._)("div", {
                     class: "q-pa-md"
                 }, null, -1),
                 n = (0, s._)("div", {
@@ -15,16 +15,16 @@
                 }, null, -1);
 
             function o(e, t, a, o, d, r) {
                 const c = (0, s.up)("q-item-label"),
                     h = (0, s.up)("element"),
                     u = (0, s.up)("q-tab"),
                     p = (0, s.up)("q-tabs"),
-                    g = (0, s.up)("q-space"),
-                    m = (0, s.up)("q-tooltip"),
+                    m = (0, s.up)("q-space"),
+                    g = (0, s.up)("q-tooltip"),
                     f = (0, s.up)("q-btn"),
                     y = (0, s.up)("q-toolbar"),
                     w = (0, s.up)("q-header"),
                     b = (0, s.up)("zone"),
                     k = (0, s.up)("q-page"),
                     v = (0, s.up)("q-page-container"),
                     x = (0, s.up)("q-layout");
@@ -74,22 +74,22 @@
                                     class: "justify-center text-white shadow-2",
                                     "no-caps": "",
                                     name: t.name,
                                     label: t.name,
                                     onClick: a => e.tabclick(t.name)
                                 }, null, 8, ["name", "label", "onClick"]))])))), 256))])),
                                 _: 1
-                            }, 8, ["modelValue"]), (0, s.Wm)(g), (0, s.Wm)(f, {
+                            }, 8, ["modelValue"]), (0, s.Wm)(m), (0, s.Wm)(f, {
                                 "no-caps": "",
                                 dense: "",
                                 round: "",
                                 icon: e.Dark.isActive ? "light_mode" : "dark_mode",
                                 onClick: e.switchTheme
                             }, {
-                                default: (0, s.w5)((() => [(0, s.Wm)(m, {
+                                default: (0, s.w5)((() => [(0, s.Wm)(g, {
                                     class: "text-body2"
                                 }, {
                                     default: (0, s.w5)((() => [(0, s.Uk)("Dark/Light mode")])),
                                     _: 1
                                 })])),
                                 _: 1
                             }, 8, ["icon", "onClick"])])),
@@ -144,147 +144,150 @@
             }
             a(71);
             var r = a(698),
                 c = a(8603);
             let h = null,
                 u = {};
             var p;
-            let g = !0;
-            const m = ["graph", "docviewer", "linechart", "block"];
+            let m = !0;
+            const g = ["graph", "docviewer", "linechart", "block"];
             const f = window.location.host,
                 y = `${window.location.protocol}//${f}`,
                 w = !1;
             let b = {},
                 k = {},
                 v = {};
 
             function C(e) {
                 p = new WebSocket(w ? "ws://localhost:8000/ws" : `ws://${f}/ws`), p.onopen = () => e.statusConnect = !0, p.onmessage = t => {
-                    g && console.log("incoming message", t.data), e.processMessage(JSON.parse(t.data))
+                    m && console.log("incoming message", t.data), e.processMessage(JSON.parse(t.data))
                 }, p.onerror = t => e.error(t), p.onclose = t => {
-                    t.wasClean ? e.info("Connection was finished by the server.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, g && console.info("close code : " + t.code + " reason: " + t.reason)
+                    t.wasClean ? e.info("Connection was finished by the server.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, m && console.info("close code : " + t.code + " reason: " + t.reason)
                 }, h = e
             }
 
             function _(e) {
                 console.log("sended", e), p.send(JSON.stringify(e))
             }
-            let q, A = 0,
-                D = !0;
+            let q = 0,
+                A = !0;
 
-            function S(e) {
-                D = e, e || (v = {})
+            function D(e) {
+                A = e, e || (v = {})
             }
 
-            function j(e) {
-                if (D) {
+            function S(e) {
+                if (A) {
                     let t = v[e.fullname];
                     if (t) return t.styleSize;
-                    D = !1
+                    A = !1
                 }
                 return ""
             }
 
-            function z(e, t, a, s = "complete") {
-                let l = ++A,
+            function j(e, t, a, s = "complete") {
+                let l = ++q,
                     i = [e.pdata.name, e.data.name, s, t, l];
                 _(i), u[l] = a
             }
 
-            function Z() {
-                b = {}, v = k, D = !0, k = {}
+            function z() {
+                b = {}, v = k, A = !0, k = {}
             }
 
-            function M(e, t) {
+            function Z(e, t) {
                 Object.assign(e.data, t), e.updated = t.value, e.value = t.value
             }
 
-            function $(e) {
+            function M(e) {
                 for (let t of e) {
                     let e = t.path;
                     if (e.length > 1) {
                         e.reverse();
                         let a = e.join("@"),
                             s = k[a];
-                        M(s, t.data)
+                        Z(s, t.data)
                     } else {
                         let a = b[e[0]];
                         Object.assign(a.data, t.data)
                     }
                 }
             }
 
-            function V(e) {
+            function $(e) {
                 "string" == typeof e.value ? h.error(e.value) : u[e.id](e.value), delete u[e.id]
             }
 
-            function E(e) {
+            function W(e) {
                 let t = [];
                 for (let s of e) s instanceof Array ? t.push(s) : t.push([s]);
                 let a = t.shift();
                 return t.reduce(((e, t) => e.flatMap((e => t.map((t => e instanceof Array ? [...e, t] : [e, t]))))), a)
             }
 
-            function W(e = !1) {
-                for (let [t, a] of Object.entries(k)) !a.expanding || e && !m.includes(a.type) || (a.styleSize = "");
+            function V(e = !1) {
+                for (let [t, a] of Object.entries(k)) !a.expanding || e && !g.includes(a.type) || (a.styleSize = "");
                 (0, s.Y3)((() => {
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
-                            Q()
+                            K(document.documentElement.scrollWidth > window.innerWidth)
                         }))
                     }))
                 }))
             }
-            let K = (0, c.debounce)(W, 200);
+            let E = (0, c.debounce)(V, 200);
 
-            function Q(e) {
-                Array.isArray(e) && (e = null), q && (q.disconnect(), q = null), g && console.log("------------------recalc design");
-                const t = H(e),
-                    a = O(e);
+            function K(e) {
+                m && console.log("------------------recalc design");
+                const t = Q(e),
+                    a = H(e);
                 for (let [s, l] of Object.entries(t)) {
-                    let e = k[s],
-                        t = a[s];
-                    const [i, n] = t || [0, 1];
-                    let o, d = e.geom(),
-                        r = d.el,
-                        c = e.pdata ? e.pdata.name : e.name,
-                        h = b[c];
-                    for (let a of h.data.value.slice(1))
-                        if (Array.isArray(a)) {
-                            if (a.find((t => t.name == e.data.name))) {
-                                let e = a[a.length - 1],
-                                    t = `${e.name}@${c}`;
-                                o = k[t];
+                    let t = k[s],
+                        i = a[s];
+                    const [n, o] = i || [0, 1];
+                    let d, r = t.geom(),
+                        c = r.el,
+                        h = t.pdata ? t.pdata.name : t.name,
+                        u = b[h];
+                    for (let e of u.data.value.slice(1))
+                        if (Array.isArray(e)) {
+                            if (e.find((e => e.name == t.data.name))) {
+                                let t = e[e.length - 1],
+                                    a = `${t.name}@${h}`;
+                                d = k[a];
                                 break
                             }
-                        } else if (a.name == e.data.name) {
-                        o = e;
+                        } else if (e.name == t.data.name) {
+                        d = t;
                         break
                     }
-                    let u = i;
-                    u /= n;
-                    let p = m.includes(e.type) ? `width:${Math.ceil(r.clientWidth+u)}px` : "",
-                        g = s.startsWith("_scroll@") ? d.inner.clientHeight : r.clientHeight;
-                    e.styleSize = `height: ${g+l}px; ${p}`
+                    let p = n;
+                    p /= o;
+                    let m = e || g.includes(t.type);
+                    if (m || "" == t.styleSize) {
+                        let e = m ? `width:${Math.ceil(c.clientWidth+p)}px` : "",
+                            a = s.startsWith("_scroll@") ? r.inner.clientHeight : c.clientHeight;
+                        a < 0 && (a = 20), t.styleSize = `height: ${a+l}px; ${e}`
+                    }
                 }
             }
 
-            function H(e) {
+            function Q(e) {
                 const t = h.screen.blocks;
                 let a = window.innerHeight;
                 a += 14;
                 let s = {},
                     l = new Map,
                     i = {};
                 for (let [d, r] of Object.entries(b)) i[r.name] = r.$el.getBoundingClientRect().height;
                 let n = [];
                 for (let d of t) {
                     const e = [];
                     let t = d instanceof Array,
-                        o = t ? E(d) : [
+                        o = t ? W(d) : [
                             [d]
                         ];
                     for (let a of o) {
                         let e = 0,
                             t = !0;
                         for (let s of a) e += i[s.name] + 12, b[s.name].only_fixed_elems || (t = !1);
                         if (t) {
@@ -335,95 +338,97 @@
                 }
                 let o = Array.from(l.entries());
                 o.sort(((e, t) => e[0] in s || e[1] in s ? -1 : 1));
                 for (let [d, r] of o) r in s ? s[d] = s[r] : s[r] = s[d];
                 return s
             }
 
-            function O(e) {
-                e = null;
-                const t = e ? [e] : h.screen.blocks;
-                let a = window.innerWidth - 15,
-                    s = [],
-                    l = {};
-                for (let o of t)
-                    if (0 == s.length)
-                        if (Array.isArray(o))
-                            for (let e of o) s.push(Array.isArray(e) ? e : [e]);
-                        else s = [
-                            [o]
+            function H(e) {
+                let t = null;
+                const a = t ? [t] : h.screen.blocks;
+                let s = window.innerWidth - 15,
+                    l = [],
+                    i = {};
+                for (let d of a)
+                    if (0 == l.length)
+                        if (Array.isArray(d))
+                            for (let e of d) l.push(Array.isArray(e) ? e : [e]);
+                        else l = [
+                            [d]
                         ];
                 else {
                     let e = [];
-                    if (Array.isArray(o))
-                        for (let t of o)
-                            for (let a of s) e.push(Array.isArray(t) ? a.concat(t) : [...a, t]);
+                    if (Array.isArray(d))
+                        for (let t of d)
+                            for (let a of l) e.push(Array.isArray(t) ? a.concat(t) : [...a, t]);
                     else
-                        for (let t of s) e.push([...t, o]);
-                    s = e
+                        for (let t of l) e.push([...t, d]);
+                    l = e
                 }
-                s.sort(((e, t) => e.length > t.length ? -1 : e.length == t.length ? 0 : 1));
-                const i = [];
-                let n = new Map;
-                for (let o of s) {
-                    let e = Array.isArray(o) ? o[o.length - 1] : o,
-                        t = b[e.name].$el.getBoundingClientRect().right;
-                    e = Array.isArray(o) ? o[0] : o;
-                    let s = b[e.name].$el.getBoundingClientRect().left,
-                        l = a - t + s - 10;
-                    const d = [];
-                    for (let [a, i] of Object.entries(k))
-                        if (i.expanding_width && (i.fullname.startsWith("_scroll@") || m.includes(i.type))) {
-                            let e = a.split("@")[1];
-                            if (o.find((t => t.name == e))) {
+                l.sort(((e, t) => e.length > t.length ? -1 : e.length == t.length ? 0 : 1));
+                const n = [];
+                let o = new Map;
+                for (let d of l) {
+                    let t = Array.isArray(d) ? d[d.length - 1] : d,
+                        a = b[t.name].$el.getBoundingClientRect().right;
+                    t = Array.isArray(d) ? d[0] : d;
+                    let l = b[t.name].$el.getBoundingClientRect().left,
+                        i = s - a + l - 10;
+                    const r = [];
+                    for (let [s, n] of Object.entries(k))
+                        if (n.expanding_width && (n.fullname.startsWith("_scroll@") || e || g.includes(n.type))) {
+                            let e = s.split("@")[1];
+                            if (d.find((t => t.name == e))) {
                                 let e = !0,
-                                    t = i.geom().left;
-                                for (let [a, s] of d.entries())
-                                    if (s !== i && s.geom().left == t) {
-                                        s.geom().scrollWidth < i.geom().scrollWidth ? (d[a] = i, n.set(s.fullname, i.fullname)) : n.set(i.fullname, s.fullname), e = !1;
+                                    t = n.geom().left;
+                                for (let [a, s] of r.entries())
+                                    if (s !== n && s.geom().left == t) {
+                                        s.geom().scrollWidth < n.geom().scrollWidth ? (r[a] = n, o.set(s.fullname, n.fullname)) : o.set(n.fullname, s.fullname), e = !1;
                                         break
-                                    } e && d.push(i)
+                                    } e && r.push(n)
                             }
-                        } d.length && i.push([l, d])
+                        } r.length && n.push([i, r])
                 }
-                for (let [o, d] of i) {
-                    d.sort(((e, t) => e.geom().scrollWidth - t.geom().scrollWidth));
-                    let e = d.length,
-                        t = {};
-                    for (let a = 0; a < d.length; a++) {
-                        let s = d[a],
-                            i = s.parent_name,
-                            n = i || s.name;
-                        if (t[n] ? t[n]++ : t[n] = 1, n = s.parent_name, n) {
+                for (let [d, r] of n) {
+                    r.sort(((e, t) => e.geom().scrollWidth - t.geom().scrollWidth));
+                    let e = r.length,
+                        t = 0;
+                    for (let a = 0; a < r.length; a++) {
+                        let s = r[a],
+                            l = s.parent_name,
+                            n = l || s.name,
+                            o = s.geom();
+                        if (t += o.scrollWidth, n = s.parent_name, n) {
                             let e = b[n];
                             if (e.data.width) {
                                 let t = a + 1,
-                                    i = d[t];
-                                if (i && i.parent_name != n) {
-                                    let t = s.geom().right - s.geom().left,
+                                    l = r[t];
+                                if (l && l.parent_name != n) {
+                                    let t = o.right - o.left,
                                         a = e.data.width - t;
-                                    l[s.fullname] = [a, 1]
+                                    i[s.fullname] = a
                                 }
                             }
                         }
-                        let r = l[s.fullname];
-                        r && (e--, o -= r[0] / r[1])
+                        let c = i[s.fullname];
+                        c && (e--, d -= c)
                     }
-                    for (let a of d) {
-                        let s = l[a.fullname];
+                    for (let a = 0; a < r.length; a++) {
+                        let e = r[a],
+                            s = i[e.fullname];
                         if (void 0 === s) {
-                            let s = a.pdata ? a.pdata.name : a.name;
-                            l[a.fullname] = [Math.floor(o / e), t[s]]
+                            e.pdata ? e.pdata.name : e.name;
+                            s = Math.floor(d * e.geom().scrollWidth / t), i[e.fullname] = [s, 1]
                         }
                     }
                 }
-                for (let [o, d] of n.entries()) d in l ? l[o] = l[d] : l[d] = l[o];
-                return l
+                for (let [d, r] of o.entries()) r in i ? i[d] = i[r] : i[r] = i[d];
+                return i
             }
-            const U = (0, s.aZ)({
+            const O = (0, s.aZ)({
                 name: "menubar",
                 methods: {
                     send() {
                         _(["root", this.name])
                     }
                 },
                 props: {
@@ -433,81 +438,81 @@
                     },
                     icon: {
                         type: String,
                         default: ""
                     }
                 }
             });
-            var N = a(4260),
-                T = a(3414),
-                F = a(2035),
-                P = a(4554),
-                I = a(2350),
-                R = a(7518),
-                L = a.n(R);
-            const B = (0, N.Z)(U, [
+            var U = a(4260),
+                N = a(3414),
+                T = a(2035),
+                F = a(4554),
+                P = a(2350),
+                I = a(7518),
+                R = a.n(I);
+            const L = (0, U.Z)(O, [
                     ["render", d]
                 ]),
-                Y = B;
-            L()(U, "components", {
-                QItem: T.Z,
-                QItemSection: F.Z,
-                QIcon: P.Z,
-                QItemLabel: I.Z
+                B = L;
+            R()(O, "components", {
+                QItem: N.Z,
+                QItemSection: T.Z,
+                QIcon: F.Z,
+                QItemLabel: P.Z
             });
-            const X = {
+            const Y = {
                     key: 0,
                     class: "row q-col-gutter-xs q-py-xs"
                 },
-                G = {
+                X = {
                     class: "q-col-gutter-xs"
                 },
-                J = {
+                G = {
                     key: 0,
                     class: "column q-col-gutter-xs"
                 };
 
-            function ee(e, t, a, l, i, n) {
+            function J(e, t, a, l, i, n) {
                 const o = (0, s.up)("zone", !0),
                     d = (0, s.up)("block");
-                return e.data instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", X, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.data, (e => ((0, s.wg)(), (0, s.iD)("div", G, [e instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", J, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e, (e => ((0, s.wg)(), (0, s.j4)(o, {
+                return e.data instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", Y, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.data, (e => ((0, s.wg)(), (0, s.iD)("div", X, [e instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", G, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e, (e => ((0, s.wg)(), (0, s.j4)(o, {
                     class: "q-col-gutter-xs q-py-xs",
                     data: e
                 }, null, 8, ["data"])))), 256))])) : ((0, s.wg)(), (0, s.j4)(d, {
                     key: 1,
                     data: e
                 }, null, 8, ["data"]))])))), 256))])) : ((0, s.wg)(), (0, s.j4)(d, {
                     key: 1,
                     data: e.data
                 }, null, 8, ["data"]))
             }
-            const te = {
+            const ee = {
                     class: "row"
                 },
-                ae = ["data", "pdata"],
-                se = {
+                te = ["data", "pdata"],
+                ae = {
                     key: 0,
                     class: "row"
                 },
-                le = ["data", "pdata"],
-                ie = {
+                se = ["data", "pdata"],
+                le = {
                     key: 0,
-                    class: "row"
+                    class: "row no-wrap"
                 };
 
-            function ne(e, t, a, i, n, o) {
+            function ie(e, t, a, i, n, o) {
                 const d = (0, s.up)("element"),
                     r = (0, s.up)("q-icon"),
                     c = (0, s.up)("q-scroll-area"),
                     h = (0, s.up)("q-card");
                 return (0, s.wg)(), (0, s.j4)(h, {
                     class: "my-card q-ma-xs",
                     style: (0, l.j5)(e.only_fixed_elems ? e.styleSize : "")
                 }, {
-                    default: (0, s.w5)((() => [(0, s._)("div", te, [e.data.logo ? ((0, s.wg)(), (0, s.j4)(d, {
+                    default: (0, s.w5)((() => [(0, s._)("div", ee, [e.data.logo ? ((0, s.wg)(), (0, s.j4)(d, {
                         key: 0,
                         class: "q-ma-sm",
                         data: e.data.logo,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])) : e.data.icon ? ((0, s.wg)(), (0, s.j4)(r, {
                         key: 1,
                         class: "q-mt-sm",
@@ -532,118 +537,118 @@
                         "thumb-style": e.thumbStyle,
                         "bar-style": e.barStyle
                     }, {
                         default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.data.value.slice(1), (t => ((0, s.wg)(), (0, s.iD)("div", {
                             class: "column",
                             data: t,
                             pdata: e.data
-                        }, [t instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", se, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(t, (t => ((0, s.wg)(), (0, s.j4)(d, {
+                        }, [t instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", ae, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(t, (t => ((0, s.wg)(), (0, s.j4)(d, {
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
                         }, null, 8, ["data", "pdata"])))), 256))])) : ((0, s.wg)(), (0, s.j4)(d, {
                             key: 1,
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
-                        }, null, 8, ["data", "pdata"]))], 8, ae)))), 256))])),
+                        }, null, 8, ["data", "pdata"]))], 8, te)))), 256))])),
                         _: 1
                     }, 8, ["style", "thumb-style", "bar-style"])) : ((0, s.wg)(!0), (0, s.iD)(s.HY, {
                         key: 1
                     }, (0, s.Ko)(e.data.value.slice(1), (t => ((0, s.wg)(), (0, s.iD)("div", {
                         class: "column",
                         data: t,
                         pdata: e.data
-                    }, [t instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", ie, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(t, (t => ((0, s.wg)(), (0, s.j4)(d, {
+                    }, [t instanceof Array ? ((0, s.wg)(), (0, s.iD)("div", le, [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(t, (t => ((0, s.wg)(), (0, s.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])))), 256))])) : ((0, s.wg)(), (0, s.j4)(d, {
                         key: 1,
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
-                    }, null, 8, ["data", "pdata"]))], 8, le)))), 256))])),
+                    }, null, 8, ["data", "pdata"]))], 8, se)))), 256))])),
                     _: 1
                 }, 8, ["style"])
             }
-            var oe = a(8880);
-            const de = e => ((0, s.dD)("data-v-5682537f"), e = e(), (0, s.Cn)(), e),
-                re = {
+            var ne = a(8880);
+            const oe = e => ((0, s.dD)("data-v-5682537f"), e = e(), (0, s.Cn)(), e),
+                de = {
                     key: 4,
                     class: "{'bg-blue-grey-9': Dark.isActive}"
                 },
-                ce = ["width", "height"],
-                he = ["src"],
-                ue = {
+                re = ["width", "height"],
+                ce = ["src"],
+                he = {
                     key: 17,
                     class: "web-camera-container"
                 },
-                pe = {
+                ue = {
                     class: "camera-button"
                 },
-                ge = {
+                pe = {
                     key: 0
                 },
                 me = {
                     key: 1
                 },
-                fe = {
+                ge = {
                     class: "camera-loading"
                 },
-                ye = de((() => (0, s._)("ul", {
+                fe = oe((() => (0, s._)("ul", {
                     class: "loader-circle"
                 }, [(0, s._)("li"), (0, s._)("li"), (0, s._)("li")], -1))),
-                we = [ye],
+                ye = [fe],
+                we = ["height"],
                 be = ["height"],
-                ke = ["height"],
-                ve = {
+                ke = {
                     key: 1,
                     class: "camera-shoot"
                 },
-                xe = de((() => (0, s._)("img", {
+                ve = oe((() => (0, s._)("img", {
                     src: "https://img.icons8.com/material-outlined/50/000000/camera--v2.png"
                 }, null, -1))),
-                Ce = [xe],
-                _e = {
+                xe = [ve],
+                Ce = {
                     key: 2,
                     class: "camera-download"
                 };
 
-            function qe(e, t, a, i, n, o) {
+            function _e(e, t, a, i, n, o) {
                 const d = (0, s.up)("q-icon"),
                     r = (0, s.up)("q-img"),
                     c = (0, s.up)("q-badge"),
                     h = (0, s.up)("q-select"),
                     u = (0, s.up)("q-checkbox"),
                     p = (0, s.up)("q-toggle"),
-                    g = (0, s.up)("q-btn"),
-                    m = (0, s.up)("q-btn-toggle"),
+                    m = (0, s.up)("q-btn"),
+                    g = (0, s.up)("q-btn-toggle"),
                     f = (0, s.up)("utable"),
                     y = (0, s.up)("linechart"),
                     w = (0, s.up)("q-input"),
                     b = (0, s.up)("q-tree"),
                     k = (0, s.up)("q-scroll-area"),
                     v = (0, s.up)("q-separator"),
                     x = (0, s.up)("q-uploader"),
                     C = (0, s.up)("cgraph"),
                     _ = (0, s.up)("q-tooltip"),
                     q = (0, s.up)("q-spinner-puff");
                 return "image" == e.type ? ((0, s.wg)(), (0, s.j4)(r, {
                     key: 0,
                     src: e.data.name,
                     "spinner-color": "blue",
-                    onClick: (0, oe.iM)(e.switchValue, ["stop"]),
+                    onClick: (0, ne.iM)(e.switchValue, ["stop"]),
                     fit: "cover",
                     style: (0, l.j5)(e.elemSize)
                 }, {
                     default: (0, s.w5)((() => [e.data.header ? ((0, s.wg)(), (0, s.iD)("div", {
                         key: 0,
                         class: "absolute-bottom-right text-subtitle2 custom-caption",
-                        onClick: t[0] || (t[0] = (0, oe.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
+                        onClick: t[0] || (t[0] = (0, ne.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
                     }, (0, l.zw)(e.data.header), 1)) : (0, s.kq)("", !0), e.value ? ((0, s.wg)(), (0, s.j4)(d, {
                         key: 1,
                         class: "absolute all-pointer-events",
                         size: "32px",
                         name: "check_circle",
                         color: "light-blue-2",
                         style: {
@@ -683,22 +688,22 @@
                 }, null, 8, ["modelValue", "label"])) : "switch" == e.type ? ((0, s.wg)(), (0, s.j4)(p, {
                     key: 3,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[3] || (t[3] = t => e.value = t),
                     color: "primary",
                     label: e.nameLabel,
                     "left-label": ""
-                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, s.wg)(), (0, s.iD)("div", re, [e.showname ? ((0, s.wg)(), (0, s.j4)(g, {
+                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, s.wg)(), (0, s.iD)("div", de, [e.showname ? ((0, s.wg)(), (0, s.j4)(m, {
                     key: 0,
                     ripple: !1,
                     color: "indigo-10",
                     disable: "",
                     label: e.name,
                     "no-caps": ""
-                }, null, 8, ["label"])) : (0, s.kq)("", !0), (0, s.Wm)(m, {
+                }, null, 8, ["label"])) : (0, s.kq)("", !0), (0, s.Wm)(g, {
                     modelValue: e.value,
                     "onUpdate:modelValue": t[4] || (t[4] = t => e.value = t),
                     class: (0, l.C_)({
                         "bg-blue-grey-9": e.Dark.isActive
                     }),
                     "no-caps": "",
                     options: e.data.options.map((e => ({
@@ -719,27 +724,27 @@
                     key: 7,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[5] || (t[5] = t => e.value = t),
                     label: e.name,
                     ref: "inputRef",
                     autogrow: e.data.autogrow,
                     dense: "",
-                    onKeyup: (0, oe.D2)(e.pressedEnter, ["enter"]),
+                    onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"]),
                     readonly: !1 === e.data.edit
                 }, null, 8, ["modelValue", "label", "autogrow", "onKeyup", "readonly"])) : "number" == e.type ? ((0, s.wg)(), (0, s.j4)(w, {
                     key: 8,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[6] || (t[6] = t => e.value = t),
                     modelModifiers: {
                         number: !0
                     },
                     label: e.name,
                     ref: "inputRef",
                     dense: "",
-                    onKeyup: (0, oe.D2)(e.pressedEnter, ["enter"]),
+                    onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"]),
                     type: "number",
                     readonly: !1 === e.data.edit
                 }, null, 8, ["modelValue", "label", "onKeyup", "readonly"])) : "autoedit" == e.type ? ((0, s.wg)(), (0, s.j4)(h, {
                     key: 9,
                     dense: "",
                     modelValue: e.value,
                     "onUpdate:modelValue": t[7] || (t[7] = t => e.value = t),
@@ -749,15 +754,15 @@
                     outlined: "",
                     "hide-bottom-space": "",
                     "fill-input": "",
                     "input-debounce": "0",
                     options: e.options,
                     onFilter: e.complete,
                     label: e.name,
-                    onKeyup: (0, oe.D2)(e.pressedEnter, ["enter"])
+                    onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"])
                 }, null, 8, ["modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, s.wg)(), (0, s.j4)(k, {
                     key: 10,
                     style: (0, l.j5)(e.styleSize),
                     "thumb-style": e.thumbStyle,
                     "bar-style": e.barStyle
                 }, {
                     default: (0, s.w5)((() => [(0, s.Wm)(b, {
@@ -779,27 +784,27 @@
                         "text-white": e.Dark.isActive
                     }]),
                     "onUpdate:modelValue": t[10] || (t[10] = t => e.value = t),
                     filled: "",
                     type: "textarea",
                     style: (0, l.j5)(e.elemSize)
                 }, null, 6)), [
-                    [oe.nr, e.value]
+                    [ne.nr, e.value]
                 ]) : "line" == e.type ? ((0, s.wg)(), (0, s.j4)(v, {
                     key: 12,
                     color: "green"
                 })) : "video" == e.type ? ((0, s.wg)(), (0, s.iD)("video", {
                     width: e.data.width,
                     height: e.data.height,
                     key: e.data.src,
                     controls: ""
                 }, [(0, s._)("source", {
                     src: e.data.src,
                     type: "video/mp4"
-                }, null, 8, he)], 8, ce)) : "uploader" == e.type ? ((0, s.wg)(), (0, s.j4)(x, {
+                }, null, 8, ce)], 8, re)) : "uploader" == e.type ? ((0, s.wg)(), (0, s.j4)(x, {
                     key: 14,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: e.host_path,
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
@@ -824,56 +829,56 @@
                     }),
                     color: e.Dark.isActive ? "purple-10" : "blue"
                 }, null, 8, ["label", "url", "onUploaded", "onAdded", "class", "color"])) : "graph" == e.type ? ((0, s.wg)(), (0, s.j4)(C, {
                     key: 16,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.elemSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, s.wg)(), (0, s.iD)("div", ue, [(0, s._)("div", pe, [(0, s._)("button", {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, s.wg)(), (0, s.iD)("div", he, [(0, s._)("div", ue, [(0, s._)("button", {
                     class: (0, l.C_)(["button is-rounded", {
                         "is-primary": !e.isCameraOpen,
                         "is-danger": e.isCameraOpen
                     }]),
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.toggleCamera && e.toggleCamera(...t))
-                }, [e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("span", me, "Close Camera")) : ((0, s.wg)(), (0, s.iD)("span", ge, "Open Camera"))], 2)]), (0, s.wy)((0, s._)("div", fe, we, 512), [
-                    [oe.F8, e.isCameraOpen && e.isLoading]
+                }, [e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("span", me, "Close Camera")) : ((0, s.wg)(), (0, s.iD)("span", pe, "Open Camera"))], 2)]), (0, s.wy)((0, s._)("div", ge, ye, 512), [
+                    [ne.F8, e.isCameraOpen && e.isLoading]
                 ]), e.isCameraOpen ? (0, s.wy)(((0, s.wg)(), (0, s.iD)("div", {
                     key: 0,
                     class: (0, l.C_)(["camera-box", {
                         flash: e.isShotPhoto
                     }])
                 }, [(0, s._)("div", {
                     class: (0, l.C_)(["camera-shutter", {
                         flash: e.isShotPhoto
                     }])
                 }, null, 2), (0, s.wy)((0, s._)("video", {
                     ref: "camera",
                     width: 450,
                     height: 337.5,
                     autoplay: ""
-                }, null, 8, be), [
-                    [oe.F8, !e.isPhotoTaken]
+                }, null, 8, we), [
+                    [ne.F8, !e.isPhotoTaken]
                 ]), (0, s.wy)((0, s._)("canvas", {
                     id: "photoTaken",
                     ref: "canvas",
                     width: 450,
                     height: 337.5
-                }, null, 8, ke), [
-                    [oe.F8, e.isPhotoTaken]
+                }, null, 8, be), [
+                    [ne.F8, e.isPhotoTaken]
                 ])], 2)), [
-                    [oe.F8, !e.isLoading]
-                ]) : (0, s.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, s.wg)(), (0, s.iD)("div", ve, [(0, s._)("button", {
+                    [ne.F8, !e.isLoading]
+                ]) : (0, s.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, s.wg)(), (0, s.iD)("div", ke, [(0, s._)("button", {
                     class: "button",
                     type: "button",
                     onClick: t[12] || (t[12] = (...t) => e.takePhoto && e.takePhoto(...t))
-                }, Ce)])) : (0, s.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("div", _e, [(0, s.Wm)(g, {
+                }, xe)])) : (0, s.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, s.wg)(), (0, s.iD)("div", Ce, [(0, s.Wm)(m, {
                     onClick: e.downloadImage,
                     label: "Send"
-                }, null, 8, ["onClick"])])) : (0, s.kq)("", !0)])) : "" != e.showname ? ((0, s.wg)(), (0, s.j4)(g, {
+                }, null, 8, ["onClick"])])) : (0, s.kq)("", !0)])) : "" != e.showname ? ((0, s.wg)(), (0, s.j4)(m, {
                     key: 18,
                     "no-caps": "",
                     class: (0, l.C_)({
                         "bg-blue-grey-9": e.Dark.isActive
                     }),
                     label: e.name,
                     icon: e.data.icon,
@@ -883,15 +888,15 @@
                         key: 0,
                         class: "text-body2"
                     }, {
                         default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, s.kq)("", !0)])),
                     _: 1
-                }, 8, ["class", "label", "icon", "onClick"])) : e.data.mode ? ((0, s.wg)(), (0, s.j4)(g, {
+                }, 8, ["class", "label", "icon", "onClick"])) : e.data.mode ? ((0, s.wg)(), (0, s.j4)(m, {
                     key: 20,
                     "no-caps": "",
                     dense: "",
                     round: "",
                     class: (0, l.C_)({
                         "bg-grey-9": e.Dark.isActive
                     }),
@@ -903,15 +908,15 @@
                         key: 0,
                         class: "text-body2"
                     }, {
                         default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, s.kq)("", !0)])),
                     _: 1
-                }, 8, ["class", "onClick"])) : ((0, s.wg)(), (0, s.j4)(g, {
+                }, 8, ["class", "onClick"])) : ((0, s.wg)(), (0, s.j4)(m, {
                     key: 19,
                     "no-caps": "",
                     dense: "",
                     round: "",
                     class: (0, l.C_)({
                         "bg-grey-9": e.Dark.isActive
                     }),
@@ -924,31 +929,31 @@
                     }, {
                         default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, s.kq)("", !0)])),
                     _: 1
                 }, 8, ["class", "icon", "onClick"]))
             }
-            const Ae = {
+            const qe = {
                     key: 0
                 },
-                De = {
+                Ae = {
                     class: "row"
                 },
-                Se = ["onClick"];
+                De = ["onClick"];
 
-            function je(e, t, a, i, n, o) {
+            function Se(e, t, a, i, n, o) {
                 const d = (0, s.up)("q-icon"),
                     r = (0, s.up)("q-tooltip"),
                     c = (0, s.up)("q-input"),
                     h = (0, s.up)("q-btn"),
                     u = (0, s.up)("q-th"),
                     p = (0, s.up)("q-tr"),
-                    g = (0, s.up)("q-checkbox"),
-                    m = (0, s.up)("q-select"),
+                    m = (0, s.up)("q-checkbox"),
+                    g = (0, s.up)("q-select"),
                     f = (0, s.up)("q-td"),
                     y = (0, s.up)("q-table");
                 return (0, s.wg)(), (0, s.j4)(y, {
                     "virtual-scroll": "",
                     dense: e.data.dense,
                     style: (0, l.j5)(e.styleSize),
                     flat: "",
@@ -961,15 +966,15 @@
                     title: e.name,
                     rows: e.rows,
                     columns: e.columns,
                     selection: e.singleMode ? "single" : "multiple",
                     selected: e.selected,
                     "onUpdate:selected": t[2] || (t[2] = t => e.selected = t)
                 }, {
-                    "top-right": (0, s.w5)((() => [!1 !== e.data.tools ? ((0, s.wg)(), (0, s.iD)("div", Ae, [(0, s._)("div", De, [(0, s.Wm)(c, {
+                    "top-right": (0, s.w5)((() => [!1 !== e.data.tools ? ((0, s.wg)(), (0, s.iD)("div", qe, [(0, s._)("div", Ae, [(0, s.Wm)(c, {
                         modelValue: e.search,
                         "onUpdate:modelValue": t[1] || (t[1] = t => e.search = t),
                         label: "Search",
                         dense: "",
                         ref: "searchField"
                     }, (0, s.Nv)({
                         append: (0, s.w5)((() => ["" != e.search ? ((0, s.wg)(), (0, s.j4)(d, {
@@ -1142,21 +1147,21 @@
                         props: t,
                         onClick: e => t.selected = !t.selected
                     }, {
                         default: (0, s.w5)((() => [((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(e.columns, ((a, i) => ((0, s.wg)(), (0, s.j4)(f, {
                             key: a.name,
                             props: t
                         }, {
-                            default: (0, s.w5)((() => ["boolean" == typeof t.row[a.name] ? ((0, s.wg)(), (0, s.j4)(g, {
+                            default: (0, s.w5)((() => ["boolean" == typeof t.row[a.name] ? ((0, s.wg)(), (0, s.j4)(m, {
                                 key: 0,
                                 modelValue: t.row[a.name],
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, s => e.change_switcher(t.row, a.name, i)],
                                 dense: "",
                                 disable: !e.editMode
-                            }, null, 8, ["modelValue", "onUpdate:modelValue", "disable"])) : e.editMode && "complete" in e.data && i == e.cedit && e.redit == t.row.iiid ? ((0, s.wg)(), (0, s.j4)(m, {
+                            }, null, 8, ["modelValue", "onUpdate:modelValue", "disable"])) : e.editMode && "complete" in e.data && i == e.cedit && e.redit == t.row.iiid ? ((0, s.wg)(), (0, s.j4)(g, {
                                 key: 1,
                                 dense: "",
                                 "model-value": t.row[a.name],
                                 "use-input": "",
                                 "hide-selected": "",
                                 "fill-input": "",
                                 autofocus: "",
@@ -1174,35 +1179,35 @@
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, e.change],
                                 dense: "",
                                 onKeydown: e.keyInput,
                                 autofocus: ""
                             }, null, 8, ["modelValue", "onUpdate:modelValue", "onKeydown"])) : ((0, s.wg)(), (0, s.iD)("div", {
                                 key: 3,
                                 onClick: a => e.select(t.row.iiid, i)
-                            }, (0, l.zw)(t.row[a.name]), 9, Se))])),
+                            }, (0, l.zw)(t.row[a.name]), 9, De))])),
                             _: 2
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props", "onClick"])])),
                     _: 1
                 }, 8, ["dense", "style", "filter", "title", "rows", "columns", "selection", "selected"])
             }
-            var ze = a(1959),
-                Ze = a(9058);
+            var je = a(1959),
+                ze = a(9058);
 
-            function Me(e, t) {
+            function Ze(e, t) {
                 return e.length === t.length && e.every(((e, a) => t[a] && e.iiid == t[a].iiid))
             }
-            const $e = (0, s.aZ)({
+            const Me = (0, s.aZ)({
                 name: "utable",
                 setup(e) {
                     const {
                         data: t,
                         pdata: a
-                    } = (0, ze.BK)(e);
+                    } = (0, je.BK)(e);
                     let l = (0, s.Fl)((() => {
                             let e = [],
                                 a = t.value;
                             const s = a.headers,
                                 l = s.length,
                                 i = a.rows,
                                 n = i.length;
@@ -1216,61 +1221,61 @@
                         })),
                         i = () => {
                             let e = t.value,
                                 a = null === e.value || 0 == l.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => l.value[e])) : [l.value[e.value]];
                             return a
                         },
                         n = i(),
-                        o = (0, ze.iH)(n),
-                        d = (0, ze.iH)(n),
-                        r = (0, ze.iH)(!Array.isArray(t.value.value)),
+                        o = (0, je.iH)(n),
+                        d = (0, je.iH)(n),
+                        r = (0, je.iH)(!Array.isArray(t.value.value)),
                         c = (e, s) => {
                             _([a.value.name, t.value.name, e, s])
                         },
                         h = (0, s.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
                         u = (0, s.Fl)((() => t.value.value));
                     return (0, s.YP)(l, ((e, t) => {
                         d.value = i(), o.value = d.value
                     })), (0, s.YP)(t, ((e, a) => {
-                        g && console.log("data update", a.name), d.value = i(), o.value = d.value, r.value = !Array.isArray(t.value.value)
+                        m && console.log("data update", a.name), d.value = i(), o.value = d.value, r.value = !Array.isArray(t.value.value)
                     })), {
                         rows: l,
                         value: h,
                         selected: d,
                         singleMode: r,
                         sendMessage: c,
                         datavalue: u,
                         updated: o
                     }
                 },
                 data() {
                     return {
-                        Dark: Ze.Z,
+                        Dark: ze.Z,
                         search: "",
                         editMode: !1,
                         options: [],
                         cedit: null
                     }
                 },
                 methods: {
                     select(e, t) {
-                        this.editMode && (this.cedit = t, g && console.log("selected", e, this.cedit))
+                        this.editMode && (this.cedit = t, m && console.log("selected", e, this.cedit))
                     },
                     change_switcher(e, t, a) {
                         if (console.log(e, t, a, e[t]), this.editMode) {
                             this.cedit = a;
                             const s = e.iiid;
                             let l = this.data.rows;
                             l[s][a] = e[t], this.sendMessage("modify", [e[t],
                                 [s, a]
                             ])
                         }
                     },
                     change(e) {
-                        if (g && console.log("changed", this.data.headers[this.cedit], e), this.editMode && this.selected.length) {
+                        if (m && console.log("changed", this.data.headers[this.cedit], e), this.editMode && this.selected.length) {
                             const t = this.selected[0].iiid;
                             let a = this.data.rows;
                             a[t][this.cedit] = e, this.sendMessage("modify", [e, [t, this.cedit]])
                         }
                     },
                     keyInput(e) {
                         if ("Control" == e.key) return;
@@ -1318,25 +1323,25 @@
                                         a = typeof t.rows[e][this.cedit];
                                     "string" != a && "number" != a || (t.value = e), this.selected = [this.rows[e]]
                                 }
                                 break
                         }
                     },
                     complete(e, t, a) {
-                        z(this, [e, [this.redit, this.cedit]], (e => t((() => {
+                        j(this, [e, [this.redit, this.cedit]], (e => t((() => {
                             this.options = e
                         }))))
                     },
                     append() {
                         let e = this.data.rows,
                             t = e.length,
                             a = this;
-                        z(this, [t, this.search], (function(s) {
+                        j(this, [t, this.search], (function(s) {
                             if (!Array.isArray(s)) return h.error(s);
-                            g && console.log("added row", s), a.search = "", e.push(s), setTimeout((() => {
+                            m && console.log("added row", s), a.search = "", e.push(s), setTimeout((() => {
                                 let e = a.rows;
                                 a.selected = [e[t]], a.showSelected(), a.editMode || a.switchEdit(), a.select(e[t], 0)
                             }), 100)
                         }), "append")
                     },
                     showSelected() {
                         let e = this.$refs.table;
@@ -1369,15 +1374,15 @@
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
                         const t = this.data;
-                        if (!Me(this.updated, this.selected)) {
+                        if (!Ze(this.updated, this.selected)) {
                             let e = this.selected.length;
                             this.sendMessage("changed", this.singleMode ? 1 == e ? this.selected[0].iiid : null : this.selected.map((e => e.iiid))), this.updated = this.selected
                         }
                         t.show && (this.showSelected(), t.show = !1), this.editMode && this.selected.length && (t.value = this.selected[0].iiid)
                     }
                 },
                 computed: {
@@ -1402,52 +1407,52 @@
                 },
                 props: {
                     data: Object,
                     pdata: Object,
                     styleSize: String
                 }
             });
-            var Ve = a(9267),
-                Ee = a(4842),
-                We = a(8870),
-                Ke = a(2165),
-                Qe = a(8186),
-                He = a(2414),
-                Oe = a(3884),
-                Ue = a(5735),
-                Ne = a(7208);
-            const Te = (0, N.Z)($e, [
-                    ["render", je]
+            var $e = a(9267),
+                We = a(4842),
+                Ve = a(8870),
+                Ee = a(2165),
+                Ke = a(8186),
+                Qe = a(2414),
+                He = a(3884),
+                Oe = a(5735),
+                Ue = a(7208);
+            const Ne = (0, U.Z)(Me, [
+                    ["render", Se]
                 ]),
-                Fe = Te;
-            L()($e, "components", {
-                QTable: Ve.Z,
-                QInput: Ee.Z,
-                QIcon: P.Z,
-                QTooltip: We.Z,
-                QBtn: Ke.Z,
-                QTr: Qe.Z,
-                QTh: He.Z,
-                QTd: Oe.Z,
-                QCheckbox: Ue.Z,
-                QSelect: Ne.Z
+                Te = Ne;
+            R()(Me, "components", {
+                QTable: $e.Z,
+                QInput: We.Z,
+                QIcon: F.Z,
+                QTooltip: Ve.Z,
+                QBtn: Ee.Z,
+                QTr: Ke.Z,
+                QTh: Qe.Z,
+                QTd: He.Z,
+                QCheckbox: Oe.Z,
+                QSelect: Ue.Z
             });
-            const Pe = ["nodes", "edges"];
+            const Fe = ["nodes", "edges"];
 
-            function Ie(e, t, a, i, n, o) {
+            function Pe(e, t, a, i, n, o) {
                 return (0, s.wg)(), (0, s.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, l.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Pe)
+                }, null, 12, Fe)
             }
-            var Re = a(2393),
-                Le = a.n(Re);
-            const Be = Le().stylesheet().selector("node").css({
+            var Ie = a(2393),
+                Re = a.n(Ie);
+            const Le = Re().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#4286f4",
                     "font-size": "14px"
                 }).selector(".selected").css({
                     "background-color": "#ff5555",
                     "border-color": "#ff5555",
                     "font-size": "14px"
@@ -1473,50 +1478,50 @@
                     label: "data(label)",
                     "text-rotation": "autorotate",
                     "text-margin-x": "-8px",
                     "text-margin-y": "-8px",
                     color: "gray",
                     "font-size": "12px"
                 }),
-                Ye = {
+                Be = {
                     animate: !0,
                     randomize: !0
                 };
 
-            function Xe(e, t) {
+            function Ye(e, t) {
                 if (e.length != t.length) return !0;
                 for (let a = 0; a < e.length; a++)
                     if (e[a].id != t[a].id || e[a].label != t[a].label) return !0;
                 return !1
             }
-            const Ge = (0, s.aZ)({
+            const Xe = (0, s.aZ)({
                     name: "cgraph",
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
                         return {
                             cy: null,
-                            style: Be,
-                            layoutOptions: Ye,
+                            style: Le,
+                            layoutOptions: Be,
                             selectedNodes: [],
                             selectedEdges: [],
                             oldNodes: [],
                             oldEdges: [],
                             shiftKey: !1
                         }
                     },
                     beforeUnmount() {
                         window.removeEventListener("keydown", this.handleKeyDown), window.removeEventListener("keyup", this.handleKeyUp)
                     },
                     mounted() {
                         window.addEventListener("keydown", this.handleKeyDown), window.addEventListener("keyup", this.handleKeyUp);
-                        let e = Le()({
+                        let e = Re()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
@@ -1529,16 +1534,16 @@
                         this.cy = e;
                         let s = this;
                         e.on("tap", "node", (t => {
                             const a = t.target;
                             if (a.hasClass("selected")) {
                                 a.removeClass("selected");
                                 let e = a.id();
-                                s.selectedNodes = s.shiftKey ? s.selectedNodes.filter((t => t !== e)) : []
-                            } else !s.shiftKey && s.selectedEdges.length > 0 && (e.$(".selected").removeClass("selected"), s.selectedEdges = []), a.addClass("selected"), s.selectedNodes.push(a.id());
+                                s.selectedNodes = s.shiftKey ? s.selectedNodes.filter((t => t != e)) : []
+                            } else !s.shiftKey && s.selectedNodes.length > 0 && (e.$(".selected").removeClass("selected"), s.selectedNodes = []), a.addClass("selected"), s.selectedNodes.push(a.id());
                             s.sendMessage("changed", {
                                 nodes: s.selectedNodes,
                                 edges: s.selectedEdges
                             })
                         })), e.on("click", (function(t) {
                             let a = t.target;
                             if ("id" in a && (a === e || "edges" == t.target.group())) {
@@ -1638,15 +1643,15 @@
                                 for (let t of e) a.edges("[id='" + t + "']").addClass("highlighted")
                             }
                         },
                         data: {
                             handler(e, t) {
                                 let a = e.value,
                                     s = !1;
-                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Xe(e.nodes, this.oldNodes) && (s = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Xe(e.edges, this.oldEdges) && (s = !0, this.oldEdges = e.edges), s && null != this.cy) {
+                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Ye(e.nodes, this.oldNodes) && (s = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Ye(e.edges, this.oldEdges) && (s = !0, this.oldEdges = e.edges), s && null != this.cy) {
                                     this.cy.json({
                                         elements: {
                                             nodes: this.nodes,
                                             edges: this.edges
                                         }
                                     });
                                     let e = this.data.method;
@@ -1663,53 +1668,53 @@
                             this.cy.style(e)
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
-                Je = (0, N.Z)(Ge, [
-                    ["render", Ie]
+                Ge = (0, U.Z)(Xe, [
+                    ["render", Pe]
                 ]),
-                et = Je;
+                Je = Ge;
 
-            function tt(e, t, a, i, n, o) {
+            function et(e, t, a, i, n, o) {
                 const d = (0, s.up)("v-chart");
                 return (0, s.wg)(), (0, s.j4)(d, {
                     ref: "chart",
                     option: n.options,
                     style: (0, l.j5)(a.styleSize ? a.styleSize : "width: 300px; height: 200px"),
                     autoresize: !0
                 }, null, 8, ["option", "style"])
             }
-            var at = a(7559),
-                st = a(4447),
-                lt = a(1006),
-                it = a(3526),
-                nt = a(763),
-                ot = a(546),
-                dt = a(6902),
-                rt = a(2826),
-                ct = a(5256),
-                ht = a(3825),
-                ut = a(8825);
-            (0, nt.D)([st.N, lt.N, it.N]), (0, nt.D)([ot.N, dt.N, rt.N, ct.N, ht.N]);
-            let pt = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"];
-            const gt = {
+            var tt = a(7559),
+                at = a(4447),
+                st = a(1006),
+                lt = a(3526),
+                it = a(763),
+                nt = a(546),
+                ot = a(6902),
+                dt = a(2826),
+                rt = a(5256),
+                ct = a(3825),
+                ht = a(8825);
+            (0, it.D)([at.N, st.N, lt.N]), (0, it.D)([nt.N, ot.N, dt.N, rt.N, ct.N]);
+            let ut = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"];
+            const pt = {
                     name: "linechart",
                     components: {
-                        VChart: at.ZP
+                        VChart: tt.ZP
                     },
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
-                        const e = (0, ut.Z)();
+                        const e = (0, ht.Z)();
                         return {
                             $q: e,
                             model: !1,
                             options: {
                                 responsive: !0,
                                 maintainAspectRatio: !1,
                                 legend: {
@@ -1785,49 +1790,49 @@
                             let l = [];
                             for (let n = 0; n < s.length; n++) s[n] = "i" == s[n] ? -1 : parseInt(s[n]), l.push([]), n && (this.options.series.push({
                                 name: t[s[n]],
                                 type: "line",
                                 symbol: "none",
                                 sampling: "lttb",
                                 itemStyle: {
-                                    color: pt[n]
+                                    color: ut[n]
                                 },
                                 data: l[n]
                             }), this.options.legend.data.push(t[s[n]]));
                             this.options.xAxis.data = l[0];
                             let i = this.data.rows;
                             for (let n = 0; n < i.length; n++)
                                 for (let e = 0; e < s.length; e++) l[e].push(-1 == s[e] ? n : i[n][s[e]]);
                             this.$refs.chart.setOption(this.options), this.$refs.chart.chart.on("click", (e => alert("!")))
                         }
                     },
                     mounted() {
                         this.calcSeries()
                     }
                 },
-                mt = (0, N.Z)(gt, [
-                    ["render", tt],
+                mt = (0, U.Z)(pt, [
+                    ["render", et],
                     ["__scopeId", "data-v-12be25e8"]
                 ]),
-                ft = mt;
+                gt = mt;
 
-            function yt(e) {
+            function ft(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
                 a.open("POST", y, !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const wt = (0, s.aZ)({
+            const yt = (0, s.aZ)({
                 name: "element",
                 components: {
-                    utable: Fe,
-                    cgraph: et,
-                    linechart: ft
+                    utable: Te,
+                    cgraph: Je,
+                    linechart: gt
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
                     onAdded(e) {
                         0 !== e.length && (0 !== this.fileArr.length ? (this.$refs.uploaderRef.removeFile(this.fileArr[0]), this.fileArr.splice(0, 1, e[0])) : this.fileArr.push(e[0]))
@@ -1848,15 +1853,15 @@
                     switchValue() {
                         this.value = !this.value
                     },
                     setValue(e) {
                         this.value = e
                     },
                     complete(e, t, a) {
-                        "" != e && z(this, e, (e => t((() => {
+                        "" != e && j(this, e, (e => t((() => {
                             this.options = e
                         }))))
                     },
                     lens() {
                         h.lens(this.data)
                     },
                     toggleCamera() {
@@ -1889,15 +1894,15 @@
                             }), e)
                         }
                         this.isPhotoTaken = !this.isPhotoTaken;
                         const e = this.$refs.canvas.getContext("2d");
                         e.drawImage(this.$refs.camera, 0, 0, 450, 337.5)
                     },
                     downloadImage() {
-                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(yt, "image/jpeg")
+                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(ft, "image/jpeg")
                     },
                     rect() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         return e.getBoundingClientRect()
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
@@ -1920,17 +1925,17 @@
                     k[this.fullname] = this
                 },
                 mounted() {
                     k[this.fullname] = this, this.data.focus && this.$refs.inputRef.$el.focus()
                 },
                 data() {
                     return {
-                        Dark: Ze.Z,
+                        Dark: ze.Z,
                         value: this.data.value,
-                        styleSize: h.visibility ? j(this) : "",
+                        styleSize: h.visibility ? S(this) : "",
                         host_path: y,
                         options: [],
                         expandedKeys: [],
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
@@ -2044,58 +2049,58 @@
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
                         this.styleSize || (this.styleSize = ""), this.value = this.data.value, this.updated = this.value, k[this.fullname] = this
                     }
                 }
             });
-            var bt = a(4027),
-                kt = a(9721),
-                vt = a(8886),
-                xt = a(8761),
-                Ct = a(1232),
-                _t = a(5551),
-                qt = a(5869),
-                At = a(1745),
-                Dt = a(8430);
-            const St = (0, N.Z)(wt, [
-                    ["render", qe],
+            var wt = a(4027),
+                bt = a(9721),
+                kt = a(8886),
+                vt = a(8761),
+                xt = a(1232),
+                Ct = a(5551),
+                _t = a(5869),
+                qt = a(1745),
+                At = a(8430);
+            const Dt = (0, U.Z)(yt, [
+                    ["render", _e],
                     ["__scopeId", "data-v-5682537f"]
                 ]),
-                jt = St;
+                St = Dt;
 
-            function zt(e) {
+            function jt(e) {
                 let t = e.type;
                 return "tree" == t || "table" == t || "list" == t || "docviewer" == t || "graph" == t || "linechart" == t
             }
-            L()(wt, "components", {
-                QImg: bt.Z,
-                QIcon: P.Z,
-                QSelect: Ne.Z,
-                QBadge: kt.Z,
-                QCheckbox: Ue.Z,
-                QToggle: vt.Z,
-                QBtn: Ke.Z,
-                QBtnToggle: xt.Z,
-                QInput: Ee.Z,
-                QScrollArea: Ct.Z,
-                QTree: _t.Z,
-                QSeparator: qt.Z,
-                QUploader: At.Z,
-                QTooltip: We.Z,
-                QSpinnerPuff: Dt.Z
+            R()(yt, "components", {
+                QImg: wt.Z,
+                QIcon: F.Z,
+                QSelect: Ue.Z,
+                QBadge: bt.Z,
+                QCheckbox: Oe.Z,
+                QToggle: kt.Z,
+                QBtn: Ee.Z,
+                QBtnToggle: vt.Z,
+                QInput: We.Z,
+                QScrollArea: xt.Z,
+                QTree: Ct.Z,
+                QSeparator: _t.Z,
+                QUploader: qt.Z,
+                QTooltip: Ve.Z,
+                QSpinnerPuff: At.Z
             });
-            const Zt = (0, s.aZ)({
+            const zt = (0, s.aZ)({
                 name: "block",
                 components: {
-                    element: jt
+                    element: St
                 },
                 data() {
                     return {
-                        Dark: Ze.Z,
+                        Dark: ze.Z,
                         styleSize: "",
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
                             width: "4px",
                             opacity: .75
@@ -2152,16 +2157,16 @@
                         return this.expanding
                     },
                     only_fixed_elems() {
                         if (this.data.scroll) return !1;
                         for (let e of this.data.value)
                             if (Array.isArray(e)) {
                                 for (let t of e)
-                                    if (zt(t)) return !1
-                            } else if (zt(e)) return !1;
+                                    if (jt(t)) return !1
+                            } else if (jt(e)) return !1;
                         return !0
                     },
                     expanding_height() {
                         return !this.data.height && (this.expanding || this.only_fixed_elems)
                     },
                     tops() {
                         let e = this.data.value;
@@ -2172,111 +2177,112 @@
                     data: {
                         type: Object,
                         required: !0
                     }
                 },
                 watch: {
                     data(e) {
-                        g && console.log("data update", this.name), b[this.name] = this, this.expanding && (this.styleSize = h.visibility ? j(this) : "", k[this.fullname] = this)
+                        m && console.log("data update", this.name), b[this.name] = this, this.expanding && (this.styleSize = h.visibility ? S(this) : "", k[this.fullname] = this)
                     }
                 }
             });
-            var Mt = a(151);
-            const $t = (0, N.Z)(Zt, [
-                    ["render", ne]
+            var Zt = a(151);
+            const Mt = (0, U.Z)(zt, [
+                    ["render", ie]
                 ]),
-                Vt = $t;
+                $t = Mt;
 
-            function Et() {
-                let e = D && k.size == v.size;
+            function Wt() {
+                console.log();
+                let e = A && k.size == v.size;
                 if (e)
                     for (let [t, a] of Object.entries(k))
                         if (!v[t]) {
                             e = !1;
                             break
-                        } e || (Q(), (0, s.Y3)((() => {
+                        } e || (K(document.documentElement.scrollWidth > window.innerWidth), (0, s.Y3)((() => {
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
                             h.visible(!0)
                         }))
                     }))
                 })))
             }
-            L()(Zt, "components", {
-                QCard: Mt.Z,
-                QIcon: P.Z,
-                QScrollArea: Ct.Z
+            R()(zt, "components", {
+                QCard: Zt.Z,
+                QIcon: F.Z,
+                QScrollArea: xt.Z
             });
-            const Wt = (0, s.aZ)({
+            const Vt = (0, s.aZ)({
                     name: "zone",
                     components: {
-                        block: Vt
+                        block: $t
                     },
                     props: {
                         data: Object
                     },
                     updated(e) {
                         (0, s.Y3)((() => {
                             requestAnimationFrame((() => {
-                                requestAnimationFrame(Et)
+                                requestAnimationFrame(Wt)
                             }))
                         }))
                     }
                 }),
-                Kt = (0, N.Z)(Wt, [
-                    ["render", ee]
+                Et = (0, U.Z)(Vt, [
+                    ["render", J]
                 ]),
-                Qt = Kt,
-                Ht = {
+                Kt = Et,
+                Qt = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function Ot(e, t, a, i, n, o) {
+            function Ht(e, t, a, i, n, o) {
                 const d = (0, s.up)("block"),
                     r = (0, s.up)("q-item-label"),
                     c = (0, s.up)("q-space"),
                     h = (0, s.up)("q-btn"),
                     u = (0, s.up)("q-card"),
                     p = (0, s.up)("q-dialog");
                 return (0, s.wg)(), (0, s.j4)(p, {
                     ref: "dialog",
                     onHide: o.onDialogHide,
-                    onKeyup: (0, oe.D2)(o.pressedEnter, ["enter"])
+                    onKeyup: (0, ne.D2)(o.pressedEnter, ["enter"])
                 }, {
                     default: (0, s.w5)((() => [(0, s.Wm)(u, {
                         class: "q-dialog-plugin q-pa-md items-start q-gutter-md",
                         bordered: "",
                         style: (0, l.j5)(a.data.internal ? "width: 800px; max-width: 80vw;" : "")
                     }, {
                         default: (0, s.w5)((() => [a.data ? ((0, s.wg)(), (0, s.j4)(d, {
                             key: 0,
                             data: a.data
                         }, null, 8, ["data"])) : (0, s.kq)("", !0), (0, s.Wm)(r, {
                             class: "text-h6"
                         }, {
                             default: (0, s.w5)((() => [(0, s.Uk)((0, l.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, s._)("div", Ht, [(0, s.Wm)(c), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(a.buttons, (e => ((0, s.wg)(), (0, s.j4)(h, {
+                        }), (0, s._)("div", Qt, [(0, s.Wm)(c), ((0, s.wg)(!0), (0, s.iD)(s.HY, null, (0, s.Ko)(a.buttons, (e => ((0, s.wg)(), (0, s.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => o.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
                     _: 1
                 }, 8, ["onHide", "onKeyup"])
             }
-            const Ut = {
+            const Ot = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
-                    block: Vt
+                    block: $t
                 },
                 emits: ["ok", "hide"],
                 methods: {
                     show() {
                         this.$refs.dialog.show()
                     },
                     sendMessage(e) {
@@ -2295,86 +2301,86 @@
                         this.$emit("ok"), this.hide()
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
-            var Nt = a(5926),
-                Tt = a(2025);
-            const Ft = (0, N.Z)(Ut, [
-                    ["render", Ot]
+            var Ut = a(5926),
+                Nt = a(2025);
+            const Tt = (0, U.Z)(Ot, [
+                    ["render", Ht]
                 ]),
-                Pt = Ft;
-            L()(Ut, "components", {
-                QDialog: Nt.Z,
-                QCard: Mt.Z,
-                QItemLabel: I.Z,
-                QSpace: Tt.Z,
-                QBtn: Ke.Z
+                Ft = Tt;
+            R()(Ot, "components", {
+                QDialog: Ut.Z,
+                QCard: Zt.Z,
+                QItemLabel: P.Z,
+                QSpace: Nt.Z,
+                QBtn: Ee.Z
             });
-            var It = a(589);
-            let Rt = "theme";
+            var Pt = a(589);
+            let It = "theme";
             try {
-                Ze.Z.set(It.Z.getItem(Rt))
-            } catch (ia) {}
-            let Lt = null;
-            const Bt = (0, s.aZ)({
+                ze.Z.set(Pt.Z.getItem(It))
+            } catch (la) {}
+            let Rt = null;
+            const Lt = (0, s.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
-                        Dark: Ze.Z,
+                        Dark: ze.Z,
                         menu: [],
                         tab: "",
                         tooldata: {
                             name: "toolbar"
                         },
                         localServer: !0,
                         statusConnect: !1,
                         screen: {
                             blocks: []
                         },
                         visibility: !1
                     }
                 },
                 components: {
-                    menubar: Y,
-                    zone: Qt,
-                    element: jt
+                    menubar: B,
+                    zone: Kt,
+                    element: St
                 },
                 created() {
                     C(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
                 methods: {
                     switchTheme() {
-                        Ze.Z.set(!Ze.Z.isActive), It.Z.set(Rt, Ze.Z.isActive)
+                        ze.Z.set(!ze.Z.isActive), Pt.Z.set(It, ze.Z.isActive)
                     },
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
                         _(["root", e])
                     },
                     visible(e) {
                         this.$refs.page.$el.style.visibility = e ? "" : "hidden", this.visibility = e
                     },
                     onResize(e) {
-                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), K()
+                        m && console.log("window has been resized", window.innerHeight, window.innerWidth), E()
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: Pt
+                                component: Ft
                             },
                             {
                                 height: a,
                                 ...s
                             } = e;
                         s.width = 750;
                         let l = {
@@ -2393,89 +2399,89 @@
                         let a = t,
                             s = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == Lt ? (s = {
+                        "progress" == t ? null == Rt ? (s = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, Lt = this.$q.notify(s)) : null == e ? (Lt(), Lt = null) : (s = {
+                        }, Rt = this.$q.notify(s)) : null == e ? (Rt(), Rt = null) : (s = {
                             caption: e
-                        }, Lt(s)) : ("error" == t && s.type, this.$q.notify(s))
+                        }, Rt(s)) : ("error" == t && s.type, this.$q.notify(s))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
-                        if ("screen" == e.type) Z(), this.screen.name != e.name && (S(!1), this.visible(!1)), this.screen = e, this.menu = e.menu.map((e => ({
+                        if ("screen" == e.type) z(), this.screen.name != e.name && (D(!1), this.visible(!1)), this.screen = e, this.menu = e.menu.map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
                         }))), this.tab = this.screen.name;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = Pt, t.componentProps = {
+                            t.component = Ft, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
-                        } else if ("answer" == e.type) V(e);
+                        } else if ("answer" == e.type) $(e);
                         else {
                             let t = e.updates && e.updates.length;
-                            t && $(e.updates);
+                            t && M(e.updates);
                             let a = !1;
                             ["error", "progress", "warning", "info"].includes(e.type) && (this.notify(e.value, e.type), a = !0), a || t || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        Lt && "progress" != e.type && this.notify(null, "progress")
+                        Rt && "progress" != e.type && this.notify(null, "progress")
                     }
                 },
                 mounted() {
                     window.addEventListener("resize", this.onResize);
                     const e = new ResizeObserver((e => {
-                        let t = document.documentElement.scrollHeight > window.innerHeight;
-                        t && W(!0)
+                        let t = document.documentElement.scrollWidth > window.innerWidth || document.documentElement.scrollHeight > window.innerHeight;
+                        t && V(!0)
                     }));
                     let t = this.$refs.page.$el;
                     e.observe(t)
                 }
             });
-            var Yt = a(9214),
-                Xt = a(3812),
-                Gt = a(9570),
-                Jt = a(7547),
-                ea = a(3269),
-                ta = a(2652),
-                aa = a(4379);
-            const sa = (0, N.Z)(Bt, [
+            var Bt = a(9214),
+                Yt = a(3812),
+                Xt = a(9570),
+                Gt = a(7547),
+                Jt = a(3269),
+                ea = a(2652),
+                ta = a(4379);
+            const aa = (0, U.Z)(Lt, [
                     ["render", o]
                 ]),
-                la = sa;
-            L()(Bt, "components", {
-                QLayout: Yt.Z,
-                QHeader: Xt.Z,
-                QToolbar: Gt.Z,
-                QBtn: Ke.Z,
-                QItemLabel: I.Z,
-                QTabs: Jt.Z,
-                QTab: ea.Z,
-                QSpace: Tt.Z,
-                QTooltip: We.Z,
-                QPageContainer: ta.Z,
-                QPage: aa.Z
+                sa = aa;
+            R()(Lt, "components", {
+                QLayout: Bt.Z,
+                QHeader: Yt.Z,
+                QToolbar: Xt.Z,
+                QBtn: Ee.Z,
+                QItemLabel: P.Z,
+                QTabs: Gt.Z,
+                QTab: Jt.Z,
+                QSpace: Nt.Z,
+                QTooltip: Ve.Z,
+                QPageContainer: ea.Z,
+                QPage: ta.Z
             })
         }
     }
 ]);
```

### Comparing `unigui-1.9.3/unigui/web/js/193.283445be.js` & `unigui-1.9.4/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui/web/js/app.1711f3eb.js` & `unigui-1.9.4/unigui/web/js/app.df555111.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(344)]).then(r.bind(r, 8344)),
+                        component: () => Promise.all([r.e(736), r.e(750)]).then(r.bind(r, 8750)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -163,25 +163,25 @@
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, o) => (r.f[o](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "283445be",
-            344: "037a8712",
-            430: "591e9a73"
+            430: "591e9a73",
+            750: "4831ed09"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            344: "ca964e27",
-            736: "f747ec02"
+            736: "f747ec02",
+            750: "ca964e27"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -264,15 +264,15 @@
                 e(o, l, n, a)
             })),
             n = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                344: 1
+                750: 1
             };
             n[e] ? t.push(n[e]) : 0 !== n[e] && r[e] && t.push(n[e] = o(e).then((() => {
                 n[e] = 0
             }), (t => {
                 throw delete n[e], t
             })))
         }
```

### Comparing `unigui-1.9.3/unigui/web/index.html` & `unigui-1.9.4/unigui/web/index.html`

 * *Files 9% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.5659ce27.js></script><script defer src=js/app.1711f3eb.js></script><link href=css/vendor.f747ec02.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.5659ce27.js></script><script defer src=js/app.df555111.js></script><link href=css/vendor.f747ec02.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.9.3/LICENSE` & `unigui-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/setup.py` & `unigui-1.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.9.3',      
+      version='1.9.4',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.9.3/PKG-INFO` & `unigui-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.3
+Version: 1.9.4
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.9.3/README.md` & `unigui-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.9.3/unigui.egg-info/PKG-INFO` & `unigui-1.9.4/unigui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.9.3
+Version: 1.9.4
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.9.3/unigui.egg-info/SOURCES.txt` & `unigui-1.9.4/unigui.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/344.ca964e27.css
+unigui/web/css/750.ca964e27.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.f747ec02.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -30,11 +30,11 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.283445be.js
-unigui/web/js/344.037a8712.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/app.1711f3eb.js
+unigui/web/js/750.4831ed09.js
+unigui/web/js/app.df555111.js
 unigui/web/js/vendor.5659ce27.js
```

