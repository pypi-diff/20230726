# Comparing `tmp/veilcord-0.0.2.tar.gz` & `tmp/veilcord-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veilcord-0.0.2.tar", last modified: Sat May 20 22:11:22 2023, max compression
+gzip compressed data, was "veilcord-0.0.3.tar", last modified: Wed Jul 26 01:49:30 2023, max compression
```

## Comparing `veilcord-0.0.2.tar` & `veilcord-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 22:11:22.905793 veilcord-0.0.2/
--rw-rw-rw-   0        0        0     1085 2023-05-20 20:15:11.000000 veilcord-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2826 2023-05-20 22:11:22.905793 veilcord-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1598 2023-05-20 14:17:39.000000 veilcord-0.0.2/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-20 22:11:22.905793 veilcord-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1753 2023-05-20 22:10:30.000000 veilcord-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 22:11:22.898575 veilcord-0.0.2/veilcord/
--rw-rw-rw-   0        0        0     9187 2023-05-20 22:10:32.000000 veilcord-0.0.2/veilcord/__init__.py
--rw-rw-rw-   0        0        0    13660 2023-05-20 22:05:34.000000 veilcord-0.0.2/veilcord/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 22:11:22.904796 veilcord-0.0.2/veilcord.egg-info/
--rw-rw-rw-   0        0        0     2826 2023-05-20 22:11:22.000000 veilcord-0.0.2/veilcord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-05-20 22:11:22.000000 veilcord-0.0.2/veilcord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 22:11:22.000000 veilcord-0.0.2/veilcord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-05-20 22:11:22.000000 veilcord-0.0.2/veilcord.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 22:11:22.000000 veilcord-0.0.2/veilcord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 01:49:30.817815 veilcord-0.0.3/
+-rw-rw-rw-   0        0        0     1085 2023-05-20 20:15:11.000000 veilcord-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3035 2023-07-26 01:49:30.816818 veilcord-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1817 2023-05-28 18:28:19.000000 veilcord-0.0.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 veilcord-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 01:49:30.817815 veilcord-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1665 2023-07-26 01:32:32.000000 veilcord-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:49:30.801012 veilcord-0.0.3/veilcord/
+-rw-rw-rw-   0        0        0     9239 2023-07-26 01:48:06.000000 veilcord-0.0.3/veilcord/__init__.py
+-rw-rw-rw-   0        0        0    10441 2023-06-15 00:37:07.000000 veilcord-0.0.3/veilcord/__main__.py
+-rw-rw-rw-   0        0        0     5071 2023-07-26 01:25:57.000000 veilcord-0.0.3/veilcord/__session__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:49:30.815822 veilcord-0.0.3/veilcord.egg-info/
+-rw-rw-rw-   0        0        0     3035 2023-07-26 01:49:30.000000 veilcord-0.0.3/veilcord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-07-26 01:49:30.000000 veilcord-0.0.3/veilcord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 01:49:30.000000 veilcord-0.0.3/veilcord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-26 01:49:30.000000 veilcord-0.0.3/veilcord.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 01:49:30.000000 veilcord-0.0.3/veilcord.egg-info/top_level.txt
```

### Comparing `veilcord-0.0.2/LICENSE` & `veilcord-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `veilcord-0.0.2/PKG-INFO` & `veilcord-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.2
-Summary: VeilCord // vast#1337
+Version: 0.0.3
+Summary: VeilCord // @imvast
 Home-page: http://pypi.python.org/pypi/veilcord
-Author: vast#1337
-Author-email: vastcord@proton.me
+Author: @imvast
+Author-email: dev@vast.sh
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VeilCord.
 <img src="https://img.shields.io/pypi/v/veilcord?style=for-the-badge&logo=python">
 <img alt="followers" src="https://img.shields.io/github/followers/imvast?color=f429ff&style=for-the-badge&logo=github&label=Follow"/>
 
@@ -54,30 +54,35 @@
     user_agent = None # for custom user agent
 )
 
 # GETTING X-Super-Properties
 xsup = veilcord.generateXProp()
 print(f"(+) Retrieved XSup: {xsup}")
 
+
 # GETTING ALL THE COOKIES AND FINGERPRINT
-cookies = veilcord.getFingerprint(xsup)
-print(f"(+) Retrieved Fingerprint: {cookies[0]}")
-# returns a set.  [0] - Fingerprint  |  [1] - COOKIESJAR
+fp, cookies = veilcord.getFingerprint(xsup, cookieType="json")
+print(f"(+) Retrieved Fingerprint: {fp}")
+print(f"(+) Retrieved Cookies: {cookies}")
+# returns a set.  [0] - Fingerprint  |  [1] - COOKIESJAR or JSON
 
 
 # GET THE NEW SESSION ID BS
+session = veilcord.openSession()
+
 token = ""
-sessionid = veilcord.getSession(
-      token = token, # obv the token 
-      type = 1, # type : 1 - web | 2 - app
-      keepAlive = False # keep the session alive | only needed if ur code is slow (avg. session is live for ~40 seconds.)
+sessionID = veilcord.getSession(
+    session = session, # the session returned from veilcord.openSession()
+    token = token, # obv the token
+    keep_alive = False,  # keep the session alive | only needed if ur code is slow (avg. session is live for ~40 seconds.)
+    show_hb = False # prints when it sends the heartbeat and when the next one is
 )
-print(f"(+) Got Session ID: {sessionid}")
+print(f"(+) Got Session ID: {sessionID}")
 
 # close the session, if keepAlive is enabled.
-# veilcord.closeSession(token)
+# veilcord.closeSession(session)
 
 ```
 
 ---
 
 ## * [vast#1337](https://discord.com/users/1109124745477246988) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
```

### Comparing `veilcord-0.0.2/README.md` & `veilcord-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -24,30 +24,35 @@
     user_agent = None # for custom user agent
 )
 
 # GETTING X-Super-Properties
 xsup = veilcord.generateXProp()
 print(f"(+) Retrieved XSup: {xsup}")
 
+
 # GETTING ALL THE COOKIES AND FINGERPRINT
-cookies = veilcord.getFingerprint(xsup)
-print(f"(+) Retrieved Fingerprint: {cookies[0]}")
-# returns a set.  [0] - Fingerprint  |  [1] - COOKIESJAR
+fp, cookies = veilcord.getFingerprint(xsup, cookieType="json")
+print(f"(+) Retrieved Fingerprint: {fp}")
+print(f"(+) Retrieved Cookies: {cookies}")
+# returns a set.  [0] - Fingerprint  |  [1] - COOKIESJAR or JSON
 
 
 # GET THE NEW SESSION ID BS
+session = veilcord.openSession()
+
 token = ""
-sessionid = veilcord.getSession(
-      token = token, # obv the token 
-      type = 1, # type : 1 - web | 2 - app
-      keepAlive = False # keep the session alive | only needed if ur code is slow (avg. session is live for ~40 seconds.)
+sessionID = veilcord.getSession(
+    session = session, # the session returned from veilcord.openSession()
+    token = token, # obv the token
+    keep_alive = False,  # keep the session alive | only needed if ur code is slow (avg. session is live for ~40 seconds.)
+    show_hb = False # prints when it sends the heartbeat and when the next one is
 )
-print(f"(+) Got Session ID: {sessionid}")
+print(f"(+) Got Session ID: {sessionID}")
 
 # close the session, if keepAlive is enabled.
-# veilcord.closeSession(token)
+# veilcord.closeSession(session)
 
 ```
 
 ---
 
 ## * [vast#1337](https://discord.com/users/1109124745477246988) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
```

### Comparing `veilcord-0.0.2/setup.py` & `veilcord-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.2"
-    
-setup(name="veilcord",
-      version=vers,
-      description="VeilCord // vast#1337",
-      long_description_content_type="text/markdown",
-      long_description=open("README.md", encoding="utf-8").read(),
-      packages=find_packages(exclude=['tests']),
-      author="vast#1337",
-      url=f"http://pypi.python.org/pypi/veilcord",
-      author_email="vastcord@proton.me",
-      license="MIT",
-      classifiers=[
-          "Development Status :: 3 - Alpha",
-          "Intended Audience :: Developers",
-          "License :: OSI Approved :: MIT License",
-          "Natural Language :: English",
-          "Programming Language :: Python",
-          "Programming Language :: Python :: 3",
-          "Programming Language :: Python :: 3.7",
-          "Programming Language :: Python :: 3.8",
-          "Programming Language :: Python :: 3.9",
-          "Programming Language :: Python :: 3.10",
-          "Topic :: Scientific/Engineering",
-          "Topic :: Scientific/Engineering :: Information Analysis",
-          "Topic :: Scientific/Engineering :: Mathematics",
-          "Topic :: Scientific/Engineering :: Visualization",
-          "Topic :: Software Development :: Libraries",
-          "Topic :: Utilities",
-      ],
-      project_urls={
-        'Homepage': 'https://github.com/imvast/veilcord',
-        'Suggestions': 'https://github.com/imvast/veilcord/issues',
-      },
-    
-      python_requires="~=3.7",
+vers = "0.0.3"
 
-      install_requires=[
-          "terminut>=0.0.0.869",
-          "colorama>=0.4.6",
-          "requests>=2.30.0",
-          "tls_client>=0.2.1",
-          "websocket-client>=1.5.1"
-      ]
+setup(
+    name="veilcord",
+    version=vers,
+    description="VeilCord // @imvast",
+    long_description_content_type="text/markdown",
+    long_description=open("README.md", encoding="utf-8").read(),
+    packages=find_packages(exclude=["tests"]),
+    author="@imvast",
+    url=f"http://pypi.python.org/pypi/veilcord",
+    author_email="dev@vast.sh",
+    license="MIT",
+    classifiers=[
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Topic :: Scientific/Engineering",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Topic :: Scientific/Engineering :: Mathematics",
+        "Topic :: Scientific/Engineering :: Visualization",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Utilities",
+    ],
+    project_urls={
+        "Homepage": "https://github.com/imvast/veilcord",
+        "Suggestions": "https://github.com/imvast/veilcord/issues",
+    },
+    python_requires="~=3.8",
+    install_requires=[
+        "terminut>=0.0.0.901",
+        "colorama>=0.4.6",
+        "requests>=2.30.0",
+        "tls_client>=0.2.1",
+        "websocket-client>=1.5.1",
+    ],
 )
```

### Comparing `veilcord-0.0.2/veilcord/__init__.py` & `veilcord-0.0.3/veilcord/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from .__main__    import *
+from .__session__ import *
+
 from terminut     import printf as print
 from colorama     import Fore
 from os           import system
+from sys          import executable
 from requests     import get
 
 
-__author__ = "github.com/imvast"                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=False
-__title__ = 'VeilCord'                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           ;print("MADE BY VAST DONT CHANGE CREDITS U QUEER") if __author__ != "github.com/imvast" else None                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
-__version__ = '0.0.2'
+__author__  = "github.com/imvast"                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   ;_0110001001101111011011110110110001110101011100110110010101100100011000100110010101100110011011110111001001100101=False
+__title__   = 'VeilCord'                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           ;print("MADE BY VAST DONT CHANGE CREDITS U QUEER") if __author__ != "github.com/imvast" else None                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
+__version__ = '0.0.3'
 
-response = get('https://pypi.org/project/veilcord/').text
-CURRENT_VERSION = str(response.split('<h1 class="package-header__name">\n        veilcord ')[1].split('\n')[0])
+CURRENT_VERSION = str(get('https://pypi.org/project/veilcord/').text.split('<h1 class="package-header__name">\n        veilcord ')[1].split('\n')[0])
 
 
 if __version__ < CURRENT_VERSION:
     print(
         f"[VeilCord] Version Out-of-Date. Please upgrade by using: \"python.exe -m pip install -U veilcord\"", 
         mainCol=Fore.RED,
         showTimestamp=False
     )
-    system('python.exe -m pip install -U veilcord  -q')
+    system(f'{executable} -m pip install -U veilcord  -q')
```

### Comparing `veilcord-0.0.2/veilcord/__main__.py` & `veilcord-0.0.3/veilcord/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from .__session__ import SessionManager
+
 from base64       import b64encode
 from json         import dumps
 from tls_client   import Session
-from typing       import Optional, Literal
-from websocket    import WebSocket
+from typing       import Optional, Literal, List, Union
 from json         import dumps, loads
 from time         import sleep, time
 from terminut     import printf as print
-from threading    import Thread
 from httpx        import get
 from re           import search
+import asyncio
+
 
 
 class HTTPClient:
     def __init__(self):
         self.session = Session(client_identifier="firefox_113", random_tls_extension_order=True)
 
 
@@ -21,131 +23,127 @@
     sessionThread = None
     sessionOn = True
 
 
 class VeilCord:
     def __init__(
         self, 
-        session: Optional[Session] = HTTPClient().session,
-        device_type: Literal["browser", "mobile", "app"] = "browser", 
-        user_agent: Optional[str] = None
+        session:        Optional[Session] = HTTPClient().session,
+        device_type:    Literal["browser", "mobile", "app"] = "browser", 
+        user_agent:     Optional[str] = None,
+        device_version: Optional[str] = None
     ) -> None:
         self.session = HTTPClient().session if session is None else session
         self.user_agent_browser = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0"
         self.user_agent_mobile  = "Discord-Android/170014;RNA"
         self.user_agent_app     = "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) discord/1.0.9013 Chrome/108.0.5359.215 Electron/22.3.2 Safari/537.36"
         self.device_type_browser = "Windows"
         self.device_type_mobile  = "Android"
-
+        self.currentBuildNUM = 199933
+        if user_agent and not device_version:
+            raise SyntaxError("If using custom useragent you must provide the version. Such as: 113.0")
         if device_type == "browser":
             self.device_type = "browser"
-            if user_agent is not None:
-                self.user_agent_browser = user_agent
+            self.user_agent = self.user_agent_browser if user_agent is None else user_agent
         elif device_type == "mobile":
             self.device_type = "mobile"
-            if user_agent is not None:
-                self.user_agent_mobile = user_agent
+            self.user_agent = self.user_agent_mobile if user_agent is None else user_agent
         elif device_type == "app":
             self.device_type = "app"
-            if user_agent is not None:
-                self.user_agent_app = user_agent
+            self.user_agent = self.user_agent_app if user_agent is None else user_agent
         else:
             raise ValueError("An invalid device_type was provided. Acceptable values: ['browser', 'mobile', 'app']")
         
     
     def generateXProp(
         self,
         browser_name: Optional[str] = None, 
         browser_vers: Optional[str] = None,
-        build_num:   Optional[int] = None
+        build_num:    Optional[int] = None
     ):
         if self.device_type == "mobile":
             xsup = {
                 "os": self.device_type_mobile,
                 "browser": "Discord Android",
                 "device": "RMX2117L1",
                 "system_locale": "en-US",
                 "client_version": "177.21 - rn",
                 "release_channel": "googleRelease",
                 "device_vendor_id": "c3c29b3e-4e06-48ff-af49-ec05c504c63e",
-                "browser_user_agent": "",
-                "browser_version": "",
                 "os_version": "31",
                 "client_build_number": 1750160087099,
-                "client_event_source": None,
-                "design_id": 0
             }
         elif self.device_type == "browser":
             xsup = {
                 "os": self.device_type_browser,
                 "browser": browser_name if browser_name else "Firefox",
-                "device": "",
                 "system_locale": "en-US",
-                "browser_user_agent": self.user_agent_browser,
-                "browser_version": browser_vers if browser_vers else "113.0",
+                "browser_user_agent": self.user_agent,
+                "browser_version": browser_vers if browser_vers else "113.0.0.0",
                 "os_version": "10",
-                "referrer": "",
-                "referring_domain": "",
-                "referrer_current": "",
-                "referring_domain_current": "",
                 "release_channel": "stable",
-                "client_build_number": 199686,
-                "client_event_source": None
+                "client_build_number": build_num if build_num else self.currentBuildNUM,
             }
         elif self.device_type == "app":
             xsup = {
                 "os": self.device_type_browser,
                 "browser": "Discord Client",
                 "release_channel": "stable",
-                "client_version": "1.0.9013",
+                "client_version": browser_vers if browser_vers else "1.0.9013",
                 "os_version": "10.0.22621",
                 "os_arch": "x64",
                 "system_locale": "en-US",
                 "browser_user_agent": self.user_agent_app,
                 "browser_version": "22.3.2",
-                "client_build_number": 199686,
+                "client_build_number": build_num if build_num else self.currentBuildNUM,
                 "native_build_number": 32266,
-                "client_event_source": None,
-                "design_id": 0
             }
         else:
             raise ValueError("An invalid type for generateXProp() was provided. Acceptable values: ['browser', 'mobile', 'app']")
         
+        xsup["client_event_source"] = None
+        xsup["design_id"] = 0
+        xsup["referrer"] = ""
+        xsup["referring_domain"] = ""
+        xsup["referrer_current"] = ""
+        xsup["referring_domain_current"] = ""
+        
         return b64encode(dumps(xsup, separators=(',', ':')).encode()).decode()
 
 
     def getFingerprint(
         self,
         xsup: Optional[str] = None,
-        withCookies: Optional[bool] = True
-    ) -> list:
+        withCookies: Optional[bool] = True,
+        cookieType: Literal["json", "cookiejar"] = "cookiejar"
+    ) -> Union[str, List[str]]:
         if not xsup:
             xsup = self.generateXProp()
         if self.device_type == "mobile":
             headers = {
                 'Host': 'discord.com',
                 'X-Super-Properties': xsup,
                 'Accept-Language': 'en-US',
                 'X-Discord-Locale': 'en-US',
                 'X-Debug-Options': 'bugReporterEnabled',
-                'User-Agent': self.user_agent_mobile,
+                'User-Agent': self.user_agent,
                 'Content-Type': 'application/json',
             }
         elif self.device_type == "browser":
             headers = {
                 "accept": "*/*",
                 "accept-encoding": "gzip, deflate, br",
                 "accept-language": "en-US,en;q=0.5",
                 "connection": "keep-alive",
                 "host": "discord.com",
                 "referer": "https://discord.com/register",
                 "sec-fetch-dest": "empty",
                 "sec-fetch-mode": "cors",
                 "sec-fetch-site": "same-origin",
-                "user-agent": self.user_agent_browser,
+                "user-agent": self.user_agent,
                 "x-debug-options": "bugReporterEnabled",
                 "x-discord-locale": "en-US",
                 "x-super-properties": xsup
             }
         elif self.device_type == "app":
             headers = {
                 "authority": "discord.com",
@@ -157,127 +155,28 @@
                 "referer": "https://discord.com/",
                 'sec-ch-ua': '"Not?A_Brand";v="8", "Chromium";v="108"',
                 'sec-ch-ua-mobile': '?0',
                 'sec-ch-ua-platform': '"Windows"',
                 'sec-fetch-dest': 'empty',
                 'sec-fetch-mode': 'cors',
                 'sec-fetch-site': 'same-origin',
-                "user-agent": self.user_agent_app,
+                "user-agent": self.user_agent,
                 "x-debug-options": "bugReporterEnabled",
                 "x-discord-locale": "en-US",
                 "x-discord-timezone": "America/New_York",
                 "x-super-properties": xsup,
             }
         else: raise ValueError("An invalid type for getFingerprint() was provided. Acceptable values: ['browser', 'mobile', 'app']")
         response = self.session.get('https://discord.com/api/v9/experiments', headers=headers)
         if withCookies:
-            return response.json().get("fingerprint"), response.cookies
+            cookies = response.cookies if cookieType == "cookiejar" else dumps(response.cookies.get_dict())
+            return response.json().get("fingerprint"), cookies
         return response.json().get("fingerprint")
 
 
-    def _wsconn(self, token, keepAlive):
-        ws = WebSocket()
-        ws.connect("wss://gateway.discord.gg/?encoding=json&v=9")
-        message = {
-            "op": 2,
-            "d": {
-                "token": token,
-                "capabilities": 8189,
-                "properties": {
-                    "os": "Windows",
-                    "device": "",
-                    "system_locale": "en-US",
-                    "release_channel": "stable",
-                    "client_build_number": 199356,
-                    "client_event_source": None,
-                    "design_id": 0
-                },
-                "presence": {
-                    "status": "online",
-                    "since": 0,
-                    "activities": [],
-                    "afk": False
-                },
-                "compress": False,
-                "client_state": {
-                    "guild_versions": {},
-                    "highest_last_message_id": "0",
-                    "read_state_version": 0,
-                    "user_guild_settings_version": -1,
-                    "user_settings_version": -1,
-                    "private_channels_version": "0",
-                    "api_code_version": 0
-                }
-            }
-        }
-
-        if self.device_type == "browser":
-            message["d"]["properties"]["browser"] = "Chrome"
-            message["d"]["properties"]["browser_user_agent"] = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36"
-            message["d"]["properties"]["browser_version"] = "113.0.0.0"
-            message["d"]["properties"]["os_version"] = "10"
-        elif self.device_type == "app":
-            message["d"]["properties"]["browser"] = "Discord Client"
-            message["d"]["properties"]["browser_user_agent"] = "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) discord/1.0.9013 Chrome/108.0.5359.215 Electron/22.3.2 Safari/537.36"
-            message["d"]["properties"]["browser_version"] = "22.3.2"
-            message["d"]["properties"]["client_version"] = "1.0.9013"
-            message["d"]["properties"]["os_version"] = "10.0.22621"
-            message["d"]["properties"]["os_arch"] = "x64"
-            message["d"]["properties"]["native_build_number"] = 32266
-        # elif self.device_type == "mobile":
-        #     pass
-        
-        else: raise ValueError("An invalid type for getSession() was provided. Acceptable values: ['browser', 'app']")
-
-        ws.send(
-            dumps(message)
-        )
-        for _ in range(5):
-            try:
-                result = loads(ws.recv())
-            except:
-                print("(!) Error Getting WS (probably invalid token)")
-            if "heartbeat_interval" in dumps(result):
-                rpbeat = result["d"].get("heartbeat_interval")
-                # print(f"(~) HB: {rpbeat}")
-            if "session_id" in dumps(result):
-                session_id = result['d'].get("session_id")
-                if not keepAlive: return session_id
-                Globals.session_id = session_id
-                # print(f"(~) SessionID: {session_id}")
-                break
-                
-        if keepAlive:
-            while Globals.sessionOn:
-                sleep(rpbeat / 1000)
-                ws.send(dumps({"op":1,"d":10}))
-                # print(f"(*) Sent HB.")
-            
-
-    def getSession(self, token: str, type: int = 1, keepAlive: bool = False):
-        if keepAlive: 
-            print("[WARN] KeepAlive is expirimental")
-            t1 = Thread(target=self._wsconn, args=[token, keepAlive])
-            Globals.sessionThread = t1
-            t1.start()
-            while Globals.session_id is None:
-                sleep(0.1)
-            return Globals.session_id
-        else:
-            return self._wsconn(token, keepAlive)
-    
-    def closeSession(self, token):
-        Globals.sessionOn = False
-        if Globals.sessionThread is None:
-            return print("(!) Cannot close an unopened session.")
-        Globals.sessionThread.join()
-        return
-    
-    
-    
     
     # non self #
     
     def getBuildNum():
         headers = {
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0',
             'Accept': '*/*',
@@ -314,14 +213,40 @@
             try:
                 return match.group(1)
             except:
                 return match.group(0)
         else:
             return None
         
+        
+        
+    def openSession(self):
+        session_manager = SessionManager()
+        return session_manager
+        
+    def getSession(
+        self, 
+        session, 
+        token: str, 
+        keep_alive: bool = False, 
+        show_hb: bool = False
+    ) -> Union[str, None]:
+        if session is None:
+            session = SessionManager()
+            if keep_alive:
+                raise SyntaxError("Session cannot be null with keepAlive enabled.")
+        session_id = asyncio.run(session.get_session(token, keep_alive, show_hb))
+        return session_id
+
+    def closeSession(self, session):
+        session.close_session()
+        return True
+    
+    
+
       
         
         
         
         
         
 ## out of the class for old projects use
```

### Comparing `veilcord-0.0.2/veilcord.egg-info/PKG-INFO` & `veilcord-0.0.3/veilcord.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: veilcord
-Version: 0.0.2
-Summary: VeilCord // vast#1337
+Version: 0.0.3
+Summary: VeilCord // @imvast
 Home-page: http://pypi.python.org/pypi/veilcord
-Author: vast#1337
-Author-email: vastcord@proton.me
+Author: @imvast
+Author-email: dev@vast.sh
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/veilcord
 Project-URL: Suggestions, https://github.com/imvast/veilcord/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VeilCord.
 <img src="https://img.shields.io/pypi/v/veilcord?style=for-the-badge&logo=python">
 <img alt="followers" src="https://img.shields.io/github/followers/imvast?color=f429ff&style=for-the-badge&logo=github&label=Follow"/>
 
@@ -54,30 +54,35 @@
     user_agent = None # for custom user agent
 )
 
 # GETTING X-Super-Properties
 xsup = veilcord.generateXProp()
 print(f"(+) Retrieved XSup: {xsup}")
 
+
 # GETTING ALL THE COOKIES AND FINGERPRINT
-cookies = veilcord.getFingerprint(xsup)
-print(f"(+) Retrieved Fingerprint: {cookies[0]}")
-# returns a set.  [0] - Fingerprint  |  [1] - COOKIESJAR
+fp, cookies = veilcord.getFingerprint(xsup, cookieType="json")
+print(f"(+) Retrieved Fingerprint: {fp}")
+print(f"(+) Retrieved Cookies: {cookies}")
+# returns a set.  [0] - Fingerprint  |  [1] - COOKIESJAR or JSON
 
 
 # GET THE NEW SESSION ID BS
+session = veilcord.openSession()
+
 token = ""
-sessionid = veilcord.getSession(
-      token = token, # obv the token 
-      type = 1, # type : 1 - web | 2 - app
-      keepAlive = False # keep the session alive | only needed if ur code is slow (avg. session is live for ~40 seconds.)
+sessionID = veilcord.getSession(
+    session = session, # the session returned from veilcord.openSession()
+    token = token, # obv the token
+    keep_alive = False,  # keep the session alive | only needed if ur code is slow (avg. session is live for ~40 seconds.)
+    show_hb = False # prints when it sends the heartbeat and when the next one is
 )
-print(f"(+) Got Session ID: {sessionid}")
+print(f"(+) Got Session ID: {sessionID}")
 
 # close the session, if keepAlive is enabled.
-# veilcord.closeSession(token)
+# veilcord.closeSession(session)
 
 ```
 
 ---
 
 ## * [vast#1337](https://discord.com/users/1109124745477246988) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
```

