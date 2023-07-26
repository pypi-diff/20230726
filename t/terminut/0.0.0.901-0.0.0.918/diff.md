# Comparing `tmp/terminut-0.0.0.901.tar.gz` & `tmp/terminut-0.0.0.918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminut-0.0.0.901.tar", last modified: Sun May 28 17:03:42 2023, max compression
+gzip compressed data, was "terminut-0.0.0.918.tar", last modified: Wed Jul 26 01:50:17 2023, max compression
```

## Comparing `terminut-0.0.0.901.tar` & `terminut-0.0.0.918.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 17:03:42.816017 terminut-0.0.0.901/
--rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 terminut-0.0.0.901/LICENSE
--rw-rw-rw-   0        0        0     2632 2023-05-28 17:03:42.816017 terminut-0.0.0.901/PKG-INFO
--rw-rw-rw-   0        0        0     1452 2023-05-09 02:05:42.000000 terminut-0.0.0.901/README.md
--rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 terminut-0.0.0.901/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 17:03:42.816017 terminut-0.0.0.901/setup.cfg
--rw-rw-rw-   0        0        0     1600 2023-05-28 16:59:59.000000 terminut-0.0.0.901/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:03:42.800706 terminut-0.0.0.901/terminut/
--rw-rw-rw-   0        0        0      722 2023-05-28 17:03:17.000000 terminut-0.0.0.901/terminut/__init__.py
--rw-rw-rw-   0        0        0     3058 2023-05-28 17:02:51.000000 terminut-0.0.0.901/terminut/console.py
--rw-rw-rw-   0        0        0     6083 2023-05-19 01:42:55.000000 terminut-0.0.0.901/terminut/customs.py
-drwxrwxrwx   0        0        0        0 2023-05-28 17:03:42.815018 terminut-0.0.0.901/terminut.egg-info/
--rw-rw-rw-   0        0        0     2632 2023-05-28 17:03:42.000000 terminut-0.0.0.901/terminut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-05-28 17:03:42.000000 terminut-0.0.0.901/terminut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 17:03:42.000000 terminut-0.0.0.901/terminut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-28 17:03:42.000000 terminut-0.0.0.901/terminut.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 17:03:42.000000 terminut-0.0.0.901/terminut.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 01:50:17.683284 terminut-0.0.0.918/
+-rw-rw-rw-   0        0        0     1085 2023-05-08 01:47:46.000000 terminut-0.0.0.918/LICENSE
+-rw-rw-rw-   0        0        0     2993 2023-07-26 01:50:17.683284 terminut-0.0.0.918/PKG-INFO
+-rw-rw-rw-   0        0        0     1771 2023-07-26 01:46:58.000000 terminut-0.0.0.918/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-08 02:01:12.000000 terminut-0.0.0.918/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 01:50:17.683284 terminut-0.0.0.918/setup.cfg
+-rw-rw-rw-   0        0        0     1571 2023-07-26 01:47:38.000000 terminut-0.0.0.918/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:50:17.676767 terminut-0.0.0.918/terminut/
+-rw-rw-rw-   0        0        0      770 2023-07-26 01:48:40.000000 terminut-0.0.0.918/terminut/__init__.py
+-rw-rw-rw-   0        0        0      557 2023-06-19 21:29:47.000000 terminut-0.0.0.918/terminut/colors.py
+-rw-rw-rw-   0        0        0     3222 2023-07-26 01:41:31.000000 terminut-0.0.0.918/terminut/console.py
+-rw-rw-rw-   0        0        0     2868 2023-07-26 01:39:42.000000 terminut-0.0.0.918/terminut/legacy.py
+-rw-rw-rw-   0        0        0     1390 2023-07-26 01:40:39.000000 terminut-0.0.0.918/terminut/log.py
+-rw-rw-rw-   0        0        0     3368 2023-07-26 01:39:37.000000 terminut-0.0.0.918/terminut/unique.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:50:17.682286 terminut-0.0.0.918/terminut.egg-info/
+-rw-rw-rw-   0        0        0     2993 2023-07-26 01:50:17.000000 terminut-0.0.0.918/terminut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-07-26 01:50:17.000000 terminut-0.0.0.918/terminut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 01:50:17.000000 terminut-0.0.0.918/terminut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-26 01:50:17.000000 terminut-0.0.0.918/terminut.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 01:50:17.000000 terminut-0.0.0.918/terminut.egg-info/top_level.txt
```

### Comparing `terminut-0.0.0.901/LICENSE` & `terminut-0.0.0.918/LICENSE`

 * *Files identical despite different names*

### Comparing `terminut-0.0.0.901/PKG-INFO` & `terminut-0.0.0.918/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.901
-Summary: Terminut // vast#1337
+Version: 0.0.0.918
+Summary: Terminut // @imvast
 Home-page: http://pypi.python.org/pypi/terminut
-Author: vast#1337
-Author-email: vastcord@proton.me
+Author: @imvast
+Author-email: dev@vast.sh
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/terminut
 Project-URL: Suggestions, https://github.com/imvast/terminut/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
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
 
 # Terminut.
 <img src="https://img.shields.io/pypi/v/terminut?style=for-the-badge&logo=python">
 <img alt="followers" src="https://img.shields.io/github/followers/imvast?color=f429ff&style=for-the-badge&logo=github&label=Follow"/>
 
@@ -50,29 +51,45 @@
 ```py
 # default shit if u want to only import for ease - auto switches #
 
 from terminut import printf as print, inputf as input, init
 
 init(debug=False)
 
-print("[DEBUG] Should Not Show")
+print("[DEBUG] Should NOT Show")
+print("(~) Should NOT Show")
 print("[INFO] Should Show")
+print("(*) Should Show")
 
 # --------------------------------------------------------- #
+# log format: [21:14:38] INF > test
 
+from terminut import log
+
+log.info(
+    "info",
+    sep=">" # separator OPTIONAL
+)
+log.error("error")
+log.fatal("fatal")
+log.success("success")
+
+# --------------------------------------------------------- #
 # this is for custom cool stuff as seen here: 
 # https://cdn.discordapp.com/attachments/1099515953223569420/1105295220414885998/2023-05-08_20-46-22.mp4
 
 import time
 from terminut import BetaConsole
+
 c = BetaConsole(speed=2)
+
 while True:
     try:
         timestamp = c.getTimestamp()
         c.alphaPrint("[INF]", f"[{timestamp}] made by vast :D", increment=False)
         time.sleep(0.001)
     except KeyboardInterrupt: exit(0)
 ```
 
 ---
 
-## * [vast#1337](https://discord.com/users/852976920148967485) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
+## * [imvast@discord](https://discord.com/users/1118654675898617891) | [imvast@github](https://github.com/imvast) | [vast.sh](https://vast.sh) *
```

### Comparing `terminut-0.0.0.901/README.md` & `terminut-0.0.0.918/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -21,29 +21,45 @@
 ```py
 # default shit if u want to only import for ease - auto switches #
 
 from terminut import printf as print, inputf as input, init
 
 init(debug=False)
 
-print("[DEBUG] Should Not Show")
+print("[DEBUG] Should NOT Show")
+print("(~) Should NOT Show")
 print("[INFO] Should Show")
+print("(*) Should Show")
 
 # --------------------------------------------------------- #
+# log format: [21:14:38] INF > test
 
+from terminut import log
+
+log.info(
+    "info",
+    sep=">" # separator OPTIONAL
+)
+log.error("error")
+log.fatal("fatal")
+log.success("success")
+
+# --------------------------------------------------------- #
 # this is for custom cool stuff as seen here: 
 # https://cdn.discordapp.com/attachments/1099515953223569420/1105295220414885998/2023-05-08_20-46-22.mp4
 
 import time
 from terminut import BetaConsole
+
 c = BetaConsole(speed=2)
+
 while True:
     try:
         timestamp = c.getTimestamp()
         c.alphaPrint("[INF]", f"[{timestamp}] made by vast :D", increment=False)
         time.sleep(0.001)
     except KeyboardInterrupt: exit(0)
 ```
 
 ---
 
-## * [vast#1337](https://discord.com/users/852976920148967485) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
+## * [imvast@discord](https://discord.com/users/1118654675898617891) | [imvast@github](https://github.com/imvast) | [vast.sh](https://vast.sh) *
```

### Comparing `terminut-0.0.0.901/setup.py` & `terminut-0.0.0.918/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 #! /usr/bin/env python
 
 from setuptools import setup, find_packages
 
-vers = "0.0.0.901"
-    
-setup(name="terminut",
-      version=vers,
-      description="Terminut // vast#1337",
-      long_description_content_type="text/markdown",
-      long_description=open("README.md", encoding="utf-8").read(),
-      packages=find_packages(exclude=['tests']),
-      author="vast#1337",
-      url=f"http://pypi.python.org/pypi/terminut",
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
-          "Topic :: Scientific/Engineering",
-          "Topic :: Scientific/Engineering :: Information Analysis",
-          "Topic :: Scientific/Engineering :: Mathematics",
-          "Topic :: Scientific/Engineering :: Visualization",
-          "Topic :: Software Development :: Libraries",
-          "Topic :: Utilities",
-      ],
-      project_urls={
-        'Homepage': 'https://github.com/imvast/terminut',
-        'Suggestions': 'https://github.com/imvast/terminut/issues',
-      },
-    
-      python_requires="~=3.7",
+vers = "0.0.0.918"
 
-      install_requires=[
-          "colorama>=0.4.6",
-          "requests>=2.30.0"
-      ]
+setup(
+    name="terminut",
+    version=vers,
+    description="Terminut // @imvast",
+    long_description_content_type="text/markdown",
+    long_description=open("README.md", encoding="utf-8").read(),
+    packages=find_packages(exclude=["tests"]),
+    author="@imvast",
+    url=f"http://pypi.python.org/pypi/terminut",
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
+        "Homepage": "https://github.com/imvast/terminut",
+        "Suggestions": "https://github.com/imvast/terminut/issues",
+    },
+    python_requires="~=3.8",
+    install_requires=[
+        "colorama>=0.4.6", 
+        "requests>=2.30.0"
+    ],
 )
```

### Comparing `terminut-0.0.0.901/terminut/__init__.py` & `terminut-0.0.0.918/terminut/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 __title__ = 'terminut'
 __author__ = 'vast#1337'
-__version__ = '0.0.0.901'
+__version__ = '0.0.0.918'
 
 
 from .console import *
-from .customs import *
+from .legacy  import *
+from .log     import *
+from .unique  import *
 
 
 ## VERSION CHECKER ##
 from requests import get
 from os import system; from sys import executable
 response = get('https://pypi.org/project/terminut/').text
 CURRENT_VERSION = str(response.split('<h1 class="package-header__name">\n        terminut ')[1].split('\n')[0])
```

### Comparing `terminut-0.0.0.901/terminut/console.py` & `terminut-0.0.0.918/terminut/console.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-from colorama import Fore, Style
+from colorama import Fore
 from datetime import datetime
 from time     import time
 from re       import sub
 
 
 class Settings:
     initialized = False
     debug = True 
     timestamp = True
+    wrapTime = False
     c_MAIN = Fore.LIGHTBLUE_EX
     c_SECO = Fore.LIGHTBLACK_EX
 
 
 def init(
     debug: bool = True,
     showTimestamp: bool = True,
+    wrapTime: bool = True,
     colMain = Fore.LIGHTBLUE_EX,
     colSeco = Fore.LIGHTBLACK_EX,
     madeBy = "vast#1337"
 ):
     Settings.initialized = True
     Settings.debug = debug
     Settings.timestamp = showTimestamp
     Settings.c_MAIN = colMain
     Settings.c_SECO = colSeco
-
+    Settings.wrapTime = wrapTime
+    
 
 @staticmethod
 def printf(content: str, mainCol=None, showTimestamp=None):
     """
     Print the content with optional colored text and timestamp.
 
     Args:
@@ -42,15 +45,18 @@
     if (
         ("(!)" in content)
         or ("(-)" in content)
         or ("(~)" in content) 
         or ("debug" in content.lower())
         ) and (Settings.debug == False): return
     
-    timestamp = f'{Settings.c_SECO}{datetime.fromtimestamp(time()).strftime("%H:%M:%S")}{Fore.RESET} ' if (showTimestamp) else ''
+    timestamp = ""
+    if showTimestamp:
+        timestamp = f"[{Settings.c_SECO}{datetime.fromtimestamp(time()).strftime('%H:%M:%S')}{Fore.RESET}]"
+        if not Settings.wrapTime: timestamp = timestamp[1:-1]
     
     content   = sub(r'\[(.*?)]', rf'{Settings.c_SECO}[{mainCol}\1{Settings.c_SECO}]{Fore.RESET}', content)
     content   = content\
         .replace("|", f"{Settings.c_SECO}|{mainCol}")\
         .replace("->", f"{Settings.c_SECO}->{mainCol}")\
         .replace("(+)", f"{Settings.c_SECO}({Fore.GREEN}+{Settings.c_SECO}){mainCol}")\
         .replace("($)", f"{Settings.c_SECO}({Fore.GREEN}${Settings.c_SECO}){mainCol}")\
@@ -59,15 +65,15 @@
         .replace("(~)", f"{Settings.c_SECO}({Fore.YELLOW}~{Settings.c_SECO}){mainCol}")\
         .replace("(#)", f"{Settings.c_SECO}({Fore.BLUE}#{Settings.c_SECO}){mainCol}")\
         .replace("(*)", f"{Settings.c_SECO}({Fore.CYAN}*{Settings.c_SECO}){mainCol}")
     
         # .replace("(", f"{Settings.c_SECO}({Fore.RESET}").replace(")", f"{Settings.c_SECO}){Fore.RESET}")
         # .replace("[", f"{Settings.c_SECO}[{mainCol}")\
         
-    return print(timestamp + content, end=f"{Fore.RESET}\n")
+    return print(timestamp, content, end=f"{Fore.RESET}\n")
     
     
 @staticmethod
 def inputf(content: str):
     if "(?)" not in content: x = f"{Settings.c_SECO}({Settings.c_MAIN}?{Settings.c_SECO}){Fore.RESET} "
     else: x = ""
     content = x + content\
```

### Comparing `terminut-0.0.0.901/terminut.egg-info/PKG-INFO` & `terminut-0.0.0.918/terminut.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: terminut
-Version: 0.0.0.901
-Summary: Terminut // vast#1337
+Version: 0.0.0.918
+Summary: Terminut // @imvast
 Home-page: http://pypi.python.org/pypi/terminut
-Author: vast#1337
-Author-email: vastcord@proton.me
+Author: @imvast
+Author-email: dev@vast.sh
 License: MIT
 Project-URL: Homepage, https://github.com/imvast/terminut
 Project-URL: Suggestions, https://github.com/imvast/terminut/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
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
 
 # Terminut.
 <img src="https://img.shields.io/pypi/v/terminut?style=for-the-badge&logo=python">
 <img alt="followers" src="https://img.shields.io/github/followers/imvast?color=f429ff&style=for-the-badge&logo=github&label=Follow"/>
 
@@ -50,29 +51,45 @@
 ```py
 # default shit if u want to only import for ease - auto switches #
 
 from terminut import printf as print, inputf as input, init
 
 init(debug=False)
 
-print("[DEBUG] Should Not Show")
+print("[DEBUG] Should NOT Show")
+print("(~) Should NOT Show")
 print("[INFO] Should Show")
+print("(*) Should Show")
 
 # --------------------------------------------------------- #
+# log format: [21:14:38] INF > test
 
+from terminut import log
+
+log.info(
+    "info",
+    sep=">" # separator OPTIONAL
+)
+log.error("error")
+log.fatal("fatal")
+log.success("success")
+
+# --------------------------------------------------------- #
 # this is for custom cool stuff as seen here: 
 # https://cdn.discordapp.com/attachments/1099515953223569420/1105295220414885998/2023-05-08_20-46-22.mp4
 
 import time
 from terminut import BetaConsole
+
 c = BetaConsole(speed=2)
+
 while True:
     try:
         timestamp = c.getTimestamp()
         c.alphaPrint("[INF]", f"[{timestamp}] made by vast :D", increment=False)
         time.sleep(0.001)
     except KeyboardInterrupt: exit(0)
 ```
 
 ---
 
-## * [vast#1337](https://discord.com/users/852976920148967485) | [imvast@github](https://github.com/imvast) | [vast.gay](https://vast.gay) *
+## * [imvast@discord](https://discord.com/users/1118654675898617891) | [imvast@github](https://github.com/imvast) | [vast.sh](https://vast.sh) *
```

