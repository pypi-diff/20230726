# Comparing `tmp/veilcord-0.0.3.tar.gz` & `tmp/veilcord-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilcord-0.0.3.tar", last modified: Wed Jul 26 01:49:30 2023, max compression
+gzip compressed data, was "veilcord-0.0.3.1.tar", last modified: Wed Jul 26 02:27:07 2023, max compression
```

## Comparing `veilcord-0.0.3.tar` & `veilcord-0.0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 01:49:30.817815 veilcord-0.0.3/
--rw-rw-rw-   0        0        0     1085 2023-05-20 20:15:11.000000 veilcord-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3035 2023-07-26 01:49:30.816818 veilcord-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1817 2023-05-28 18:28:19.000000 veilcord-0.0.3/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 01:49:30.817815 veilcord-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1665 2023-07-26 01:32:32.000000 veilcord-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:49:30.801012 veilcord-0.0.3/veilcord/
--rw-rw-rw-   0        0        0     9239 2023-07-26 01:48:06.000000 veilcord-0.0.3/veilcord/__init__.py
--rw-rw-rw-   0        0        0    10441 2023-06-15 00:37:07.000000 veilcord-0.0.3/veilcord/__main__.py
--rw-rw-rw-   0        0        0     5071 2023-07-26 01:25:57.000000 veilcord-0.0.3/veilcord/__session__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:49:30.815822 veilcord-0.0.3/veilcord.egg-info/
--rw-rw-rw-   0        0        0     3035 2023-07-26 01:49:30.000000 veilcord-0.0.3/veilcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-07-26 01:49:30.000000 veilcord-0.0.3/veilcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 01:49:30.000000 veilcord-0.0.3/veilcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-26 01:49:30.000000 veilcord-0.0.3/veilcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 01:49:30.000000 veilcord-0.0.3/veilcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 02:27:07.828716 veilcord-0.0.3.1/
+-rw-rw-rw-   0        0        0     1085 2023-05-20 20:15:11.000000 veilcord-0.0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     3040 2023-07-26 02:27:07.828716 veilcord-0.0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1820 2023-07-26 01:58:21.000000 veilcord-0.0.3.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 02:27:07.829716 veilcord-0.0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1667 2023-07-26 02:26:31.000000 veilcord-0.0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 02:27:07.814480 veilcord-0.0.3.1/veilcord/
+-rw-rw-rw-   0        0        0     9213 2023-07-26 02:26:47.000000 veilcord-0.0.3.1/veilcord/__init__.py
+-rw-rw-rw-   0        0        0    10505 2023-07-26 02:25:10.000000 veilcord-0.0.3.1/veilcord/__main__.py
+-rw-rw-rw-   0        0        0     5228 2023-07-26 02:26:23.000000 veilcord-0.0.3.1/veilcord/__session__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 02:27:07.827309 veilcord-0.0.3.1/veilcord.egg-info/
+-rw-rw-rw-   0        0        0     3040 2023-07-26 02:27:07.000000 veilcord-0.0.3.1/veilcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-07-26 02:27:07.000000 veilcord-0.0.3.1/veilcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 02:27:07.000000 veilcord-0.0.3.1/veilcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-26 02:27:07.000000 veilcord-0.0.3.1/veilcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 02:27:07.000000 veilcord-0.0.3.1/veilcord.egg-info/top_level.txt
```

### Comparing `veilcord-0.0.3/LICENSE` & `veilcord-0.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.3/PKG-INFO` & `veilcord-0.0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: VeilCord // @imvast
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: @imvast
 Author-email: dev@vast.sh
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
@@ -81,8 +81,8 @@
 # close the session, if keepAlive is enabled.
 # veilcord.closeSession(session)
 
 ```
 
 ---
 
-## * [vast#1337](https://discord.com/users/1109124745477246988) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
+## * [imvast@discord](https://discord.com/users/1118654675898617891) | [imvast@github](https://github.com/imvast) | [vast.sh](https://vast.sh) *
```

### Comparing `veilcord-0.0.3/README.md` & `veilcord-0.0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 # close the session, if keepAlive is enabled.
 # veilcord.closeSession(session)
 
 ```
 
 ---
 
-## * [vast#1337](https://discord.com/users/1109124745477246988) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
+## * [imvast@discord](https://discord.com/users/1118654675898617891) | [imvast@github](https://github.com/imvast) | [vast.sh](https://vast.sh) *
```

### Comparing `veilcord-0.0.3/setup.py` & `veilcord-0.0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.3"
+vers = "0.0.3.1"
 
 setup(
     name="veilcord",
     version=vers,
     description="VeilCord // @imvast",
     long_description_content_type="text/markdown",
     long_description=open("README.md", encoding="utf-8").read(),
```

### Comparing `veilcord-0.0.3/veilcord/__init__.py` & `veilcord-0.0.3.1/veilcord/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from .__main__    import *
-from .__session__ import *
 
 from terminut     import printf as print
 from colorama     import Fore
 from os           import system
 from sys          import executable
 from requests     import get
 
 
 __author__  = "github.com/imvast"                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=False
 __title__   = 'VeilCord'                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           ;print("MADE BY VAST DONT CHANGE CREDITS U QUEER") if __author__ != "github.com/imvast" else None                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
-__version__ = '0.0.3'
+__version__ = '0.0.3.1'
 
 CURRENT_VERSION = str(get('https://pypi.org/project/veilcord/').text.split('<h1 class="package-header__name">\n        veilcord ')[1].split('\n')[0])
 
 
 if __version__ < CURRENT_VERSION:
     print(
         f"[VeilCord] Version Out-of-Date. Please upgrade by using: \"python.exe -m pip install -U veilcord\"",
```

### Comparing `veilcord-0.0.3/veilcord/__main__.py` & `veilcord-0.0.3.1/veilcord/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 
 from base64       import b64encode
 from json         import dumps
 from tls_client   import Session
 from typing       import Optional, Literal, List, Union
 from json         import dumps, loads
 from time         import sleep, time
-from terminut     import printf as print
 from httpx        import get
 from re           import search
-import asyncio
+from asyncio      import run
 
 
 
 class HTTPClient:
     def __init__(self):
         self.session = Session(client_identifier="firefox_113", random_tls_extension_order=True)
 
@@ -216,43 +215,42 @@
                 return match.group(0)
         else:
             return None
         
         
         
     def openSession(self):
-        session_manager = SessionManager()
+        session_manager = SessionManager(self.user_agent, self.currentBuildNUM, self.device_type)
         return session_manager
         
     def getSession(
         self, 
         session, 
         token: str, 
         keep_alive: bool = False, 
         show_hb: bool = False
     ) -> Union[str, None]:
         if session is None:
-            session = SessionManager()
+            session = SessionManager(self.user_agent, self.currentBuildNUM, self.device_type)
             if keep_alive:
                 raise SyntaxError("Session cannot be null with keepAlive enabled.")
-        session_id = asyncio.run(session.get_session(token, keep_alive, show_hb))
+        session_id = run(session.get_session(token, keep_alive, show_hb))
         return session_id
 
     def closeSession(self, session):
         session.close_session()
         return True
     
     
 
       
         
         
         
         
-        
 ## out of the class for old projects use
 
 def extractCode(invite):
     """Extracts the invite code from a Discord invite link"""
     code_regex = r"(?:(?:http:\/\/|https:\/\/)?discord\.gg\/|discordapp\.com\/invite\/|discord\.com\/invite\/)?([a-zA-Z0-9-]+)"
     match = search(code_regex, invite)
     if match:
```

### Comparing `veilcord-0.0.3/veilcord/__session__.py` & `veilcord-0.0.3.1/veilcord/__session__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-from .__main__ import VeilCord
 from websocket import WebSocket
 from json      import dumps, loads
-import asyncio
+from terminut  import printf as print
+from asyncio   import sleep, create_task
 
 
 class SessionManager:
-    def __init__(self):
+    def __init__(self, user_agent, build_num, device_type):
         self.session_id = None
         self.session_task = None
         self.session_on = False
         self.ws = WebSocket()
+        
+        self.user_agent = user_agent
+        self.build_num = build_num
+        self.device_type = device_type
+        
 
     async def _wsconn(self, token):
         self.ws.connect("wss://gateway.discord.gg/?encoding=json&v=9")
         message = {
             "op": 2,
             "d": {
                 "token": token,
                 "capabilities": 8189,
                 "properties": {
                     "os": "Windows",
-                    "browser_user_agent": VeilCord().user_agent,
+                    "browser_user_agent": self.user_agent,
                     "device": "",
                     "system_locale": "en-US",
                     "release_channel": "stable",
-                    "client_build_number": VeilCord().currentBuildNUM,
+                    "client_build_number": self.build_num,
                     "client_event_source": None,
                     "design_id": 0
                 },
                 "presence": {
                     "status": "online",
                     "since": 0,
                     "activities": [{
@@ -48,19 +53,19 @@
                     "user_settings_version": -1,
                     "private_channels_version": "0",
                     "api_code_version": 0
                 }
             }
         }
 
-        if VeilCord().device_type == "browser":
+        if self.device_type == "browser":
             message["d"]["properties"]["browser"] = "Chrome"
             message["d"]["properties"]["browser_version"] = "113.0.0.0"
             message["d"]["properties"]["os_version"] = "10"
-        elif VeilCord().device_type == "app":
+        elif self.device_type == "app":
             message["d"]["properties"]["browser"] = "Discord Client"
             message["d"]["properties"]["browser_version"] = "22.3.2"
             message["d"]["properties"]["client_version"] = "1.0.9013"
             message["d"]["properties"]["os_version"] = "10.0.22621"
             message["d"]["properties"]["os_arch"] = "x64"
             message["d"]["properties"]["native_build_number"] = 32266
         # elif self.device_type == "mobile":
@@ -96,26 +101,26 @@
         return self.session_id
 
     async def keepSessionAlive(self, showHB):
         while self.session_on:
             try:
                 self.ws.send(dumps({"op": 1, "d": 10}))
                 if showHB: print(f"(*) Sent HB. | Next: {self.rpBeat/1000}s")
-                await asyncio.sleep(self.rpBeat / 1000)
+                await sleep(self.rpBeat / 1000)
             except Exception as e:
                 print(f"(!) Error sending HB: {e}")
                 break
 
     async def get_session(self, token: str, keep_alive: bool = False, show_hb: bool = False):
         try:
             session_id = await self._wsconn(token)
             if keep_alive:
                 print("[WARN] KeepAlive is experimental.", showTimestamp=False)
                 self.session_on = True
-                self.session_task = asyncio.create_task(self.keepSessionAlive(show_hb))
+                self.session_task = create_task(self.keepSessionAlive(show_hb))
                 return session_id
             else:
                 return session_id
         except KeyboardInterrupt:
             if self.session_on:
                 self.session_on = False  # Stop the keep-alive loop
                 await self.session_task  # Wait for the task to complete
```

### Comparing `veilcord-0.0.3/veilcord.egg-info/PKG-INFO` & `veilcord-0.0.3.1/veilcord.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.3
+Version: 0.0.3.1
 Summary: VeilCord // @imvast
 Home-page: http://pypi.python.org/pypi/veilcord
 Author: @imvast
 Author-email: dev@vast.sh
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
@@ -81,8 +81,8 @@
 # close the session, if keepAlive is enabled.
 # veilcord.closeSession(session)
 
 ```
 
 ---
 
-## * [vast#1337](https://discord.com/users/1109124745477246988) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
+## * [imvast@discord](https://discord.com/users/1118654675898617891) | [imvast@github](https://github.com/imvast) | [vast.sh](https://vast.sh) *
```

