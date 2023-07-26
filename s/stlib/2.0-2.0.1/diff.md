# Comparing `tmp/stlib-2.0.tar.gz` & `tmp/stlib-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stlib-2.0.tar", last modified: Thu Jul 20 16:56:17 2023, max compression
+gzip compressed data, was "stlib-2.0.1.tar", last modified: Wed Jul 26 21:24:32 2023, max compression
```

## Comparing `stlib-2.0.tar` & `stlib-2.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:56:17.636408 stlib-2.0/
--rwxr-xr-x   0 root         (0) root         (0)    34916 2023-07-20 16:54:45.000000 stlib-2.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       55 2023-07-20 16:54:45.000000 stlib-2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4341 2023-07-20 16:56:17.636408 stlib-2.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     3206 2023-07-20 16:54:45.000000 stlib-2.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1302 2023-07-20 16:54:45.000000 stlib-2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 16:56:17.636408 stlib-2.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2577 2023-07-20 16:54:45.000000 stlib-2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:56:17.632408 stlib-2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:56:17.632408 stlib-2.0/src/steamworks/
--rw-r--r--   0 root         (0) root         (0)      817 2023-07-20 16:54:45.000000 stlib-2.0/src/steamworks/common.cpp
--rw-r--r--   0 root         (0) root         (0)    13290 2023-07-20 16:54:45.000000 stlib-2.0/src/steamworks/steam_api.cpp
--rw-r--r--   0 root         (0) root         (0)    11647 2023-07-20 16:54:45.000000 stlib-2.0/src/steamworks/steam_gameserver.cpp
--rw-r--r--   0 root         (0) root         (0)     2390 2023-07-20 16:54:45.000000 stlib-2.0/src/steamworks/steamworks.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:56:17.632408 stlib-2.0/src/stlib/
--rwxr-xr-x   0 root         (0) root         (0)     4017 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4101 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/client.py
--rw-r--r--   0 root         (0) root         (0)    24601 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/community.py
--rw-r--r--   0 root         (0) root         (0)     7551 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/internals.py
--rw-r--r--   0 root         (0) root         (0)    11034 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/login.py
--rw-r--r--   0 root         (0) root         (0)     5366 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/plugins.py
--rwxr-xr-x   0 root         (0) root         (0)     5688 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/universe.py
--rw-r--r--   0 root         (0) root         (0)    15087 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/utils.py
--rw-r--r--   0 root         (0) root         (0)    11695 2023-07-20 16:54:45.000000 stlib-2.0/src/stlib/webapi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:56:17.636408 stlib-2.0/src/stlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4341 2023-07-20 16:56:17.000000 stlib-2.0/src/stlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      562 2023-07-20 16:56:17.000000 stlib-2.0/src/stlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:56:17.000000 stlib-2.0/src/stlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:56:17.000000 stlib-2.0/src/stlib.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-20 16:56:17.000000 stlib-2.0/src/stlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-20 16:56:17.000000 stlib-2.0/src/stlib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 21:24:32.080685 stlib-2.0.1/
+-rwxr-xr-x   0 root         (0) root         (0)    34916 2023-07-26 21:22:40.000000 stlib-2.0.1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-26 21:22:40.000000 stlib-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4236 2023-07-26 21:24:32.080685 stlib-2.0.1/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     3099 2023-07-26 21:22:40.000000 stlib-2.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-07-26 21:22:40.000000 stlib-2.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 21:24:32.080685 stlib-2.0.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2577 2023-07-26 21:22:40.000000 stlib-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 21:24:32.076685 stlib-2.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 21:24:32.076685 stlib-2.0.1/src/steamworks/
+-rw-r--r--   0 root         (0) root         (0)      817 2023-07-26 21:22:40.000000 stlib-2.0.1/src/steamworks/common.cpp
+-rw-r--r--   0 root         (0) root         (0)    13290 2023-07-26 21:22:40.000000 stlib-2.0.1/src/steamworks/steam_api.cpp
+-rw-r--r--   0 root         (0) root         (0)    11647 2023-07-26 21:22:40.000000 stlib-2.0.1/src/steamworks/steam_gameserver.cpp
+-rw-r--r--   0 root         (0) root         (0)     2390 2023-07-26 21:22:40.000000 stlib-2.0.1/src/steamworks/steamworks.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 21:24:32.080685 stlib-2.0.1/src/stlib/
+-rwxr-xr-x   0 root         (0) root         (0)     4017 2023-07-26 21:22:40.000000 stlib-2.0.1/src/stlib/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4101 2023-07-26 21:22:40.000000 stlib-2.0.1/src/stlib/client.py
+-rw-r--r--   0 root         (0) root         (0)    24822 2023-07-26 21:22:40.000000 stlib-2.0.1/src/stlib/community.py
+-rw-r--r--   0 root         (0) root         (0)     7551 2023-07-26 21:22:40.000000 stlib-2.0.1/src/stlib/internals.py
+-rw-r--r--   0 root         (0) root         (0)    11034 2023-07-26 21:22:40.000000 stlib-2.0.1/src/stlib/login.py
+-rw-r--r--   0 root         (0) root         (0)     5366 2023-07-26 21:22:40.000000 stlib-2.0.1/src/stlib/plugins.py
+-rwxr-xr-x   0 root         (0) root         (0)     5688 2023-07-26 21:22:40.000000 stlib-2.0.1/src/stlib/universe.py
+-rw-r--r--   0 root         (0) root         (0)    15087 2023-07-26 21:22:40.000000 stlib-2.0.1/src/stlib/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11695 2023-07-26 21:22:40.000000 stlib-2.0.1/src/stlib/webapi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 21:24:32.080685 stlib-2.0.1/src/stlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4236 2023-07-26 21:24:32.000000 stlib-2.0.1/src/stlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      562 2023-07-26 21:24:32.000000 stlib-2.0.1/src/stlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 21:24:32.000000 stlib-2.0.1/src/stlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 21:24:31.000000 stlib-2.0.1/src/stlib.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-26 21:24:32.000000 stlib-2.0.1/src/stlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-26 21:24:32.000000 stlib-2.0.1/src/stlib.egg-info/top_level.txt
```

### Comparing `stlib-2.0/LICENSE.md` & `stlib-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stlib-2.0/PKG-INFO` & `stlib-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stlib
-Version: 2.0
+Version: 2.0.1
 Summary: Async library that provides features related to Steam client and compatible stuffs
 Author: Lara Maia
 Author-email: dev@lara.monster
 License: GPLv3
 Project-URL: homepage, https://github.com/calendulish/stlib
 Project-URL: documentation, https://lara.monster/stlib
 Project-URL: repository, https://github.com
@@ -28,15 +28,14 @@
 
 stlib
 -----
 
 [![windows build status](https://badges.lara.monster/calendulish/.github/stlib-windows-build)](https://github.com/calendulish/stlib/actions/workflows/build.yml)
 [![linux build status](https://badges.lara.monster/calendulish/.github/stlib-linux-build)](https://github.com/calendulish/stlib/actions/workflows/build.yml)
 [![Coverage](https://codecov.io/gh/calendulish/stlib/branch/master/graph/badge.svg?token=DMKFKEUUZP)](https://codecov.io/gh/calendulish/stlib)
-[![Quality](https://api.codiga.io/project/33228/score/svg)](https://app.codiga.io/project/33228/dashboard)
 [![GitHub license](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](https://www.gnu.org/licenses/gpl-3.0.html)
 [![GitHub release](https://img.shields.io/github/release/calendulish/stlib.svg?style=flat)](https://github.com/calendulish/stlib/releases)
 
 Async library that provides features related to Steam client and compatible stuff
 
 WARNING: stlib is not intended to be used in game development, there is no support to callbacks, and I'll not work on that.
 stlib is intended to develop console or GUI applications that need interaction with SteamAPI or SteamWebAPI.
```

### Comparing `stlib-2.0/README.md` & `stlib-2.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 stlib
 -----
 
 [![windows build status](https://badges.lara.monster/calendulish/.github/stlib-windows-build)](https://github.com/calendulish/stlib/actions/workflows/build.yml)
 [![linux build status](https://badges.lara.monster/calendulish/.github/stlib-linux-build)](https://github.com/calendulish/stlib/actions/workflows/build.yml)
 [![Coverage](https://codecov.io/gh/calendulish/stlib/branch/master/graph/badge.svg?token=DMKFKEUUZP)](https://codecov.io/gh/calendulish/stlib)
-[![Quality](https://api.codiga.io/project/33228/score/svg)](https://app.codiga.io/project/33228/dashboard)
 [![GitHub license](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](https://www.gnu.org/licenses/gpl-3.0.html)
 [![GitHub release](https://img.shields.io/github/release/calendulish/stlib.svg?style=flat)](https://github.com/calendulish/stlib/releases)
 
 Async library that provides features related to Steam client and compatible stuff
 
 WARNING: stlib is not intended to be used in game development, there is no support to callbacks, and I'll not work on that.
 stlib is intended to develop console or GUI applications that need interaction with SteamAPI or SteamWebAPI.
```

### Comparing `stlib-2.0/pyproject.toml` & `stlib-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stlib"
-version = "2.0"
+version = "2.0.1"
 description = "Async library that provides features related to Steam client and compatible stuffs"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "GPLv3"}
 keywords = ["steam", "valve"]
 authors = [{email = "dev@lara.monster"}, {name = "Lara Maia"}]
 classifiers = [
```

### Comparing `stlib-2.0/setup.py` & `stlib-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `stlib-2.0/src/steamworks/common.cpp` & `stlib-2.0.1/src/steamworks/common.cpp`

 * *Files identical despite different names*

### Comparing `stlib-2.0/src/steamworks/steam_api.cpp` & `stlib-2.0.1/src/steamworks/steam_api.cpp`

 * *Files identical despite different names*

### Comparing `stlib-2.0/src/steamworks/steam_gameserver.cpp` & `stlib-2.0.1/src/steamworks/steam_gameserver.cpp`

 * *Files identical despite different names*

### Comparing `stlib-2.0/src/steamworks/steamworks.cpp` & `stlib-2.0.1/src/steamworks/steamworks.cpp`

 * *Files identical despite different names*

### Comparing `stlib-2.0/src/stlib/__init__.py` & `stlib-2.0.1/src/stlib/__init__.py`

 * *Files identical despite different names*

### Comparing `stlib-2.0/src/stlib/client.py` & `stlib-2.0.1/src/stlib/client.py`

 * *Files identical despite different names*

### Comparing `stlib-2.0/src/stlib/community.py` & `stlib-2.0.1/src/stlib/community.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,16 +396,20 @@
 
             if not json_data['success']:
                 raise AttributeError(f"Unable to get details for confirmation {confirmation['id']}")
 
             html = BeautifulSoup(json_data["html"], 'html.parser')
 
             if confirmation['type'] in (1, 2):
-                offer_friend = html.find('div', class_="mobileconf_offer_friend")
-                to = offer_friend.find_next('span').text.strip()
+                try:
+                    offer_friend = html.find('div', class_="mobileconf_offer_friend")
+                    to = offer_friend.find_next('span').text.strip()
+                except AttributeError:
+                    trade_partner = html.find('span', class_="trade_partner_headline_sub")
+                    to = trade_partner.get_text().strip()
 
                 item_list = html.find_all('div', class_="tradeoffer_item_list")
 
                 give = []
                 for item in item_list[0].find_all('div', class_='trade_item'):
                     appid, classid = item['data-economy-item'].split('/')[1:3]
                     name = await self.get_item_name(appid, classid)
@@ -432,15 +436,15 @@
 
                     if json_data['type']:
                         give[0] += f" - {json_data['type']}"
                 else:
                     give = [json_data['type']]
 
                 if quantity := listing_prices.find(
-                    text=lambda element: 'Quantity' in element.text
+                        text=lambda element: 'Quantity' in element.text
                 ):
                     give[0] = f'{quantity.next.next.strip()} {give[0]}'
             elif confirmation['type'] == 5:
                 to = "Steam"
                 give = ["Change phone number"]
                 receive = ["Phone number has not been entered yet"]
             elif confirmation['type'] == 6:
```

### Comparing `stlib-2.0/src/stlib/internals.py` & `stlib-2.0.1/src/stlib/internals.py`

 * *Files identical despite different names*

### Comparing `stlib-2.0/src/stlib/login.py` & `stlib-2.0.1/src/stlib/login.py`

 * *Files identical despite different names*

### Comparing `stlib-2.0/src/stlib/plugins.py` & `stlib-2.0.1/src/stlib/plugins.py`

 * *Files identical despite different names*

### Comparing `stlib-2.0/src/stlib/universe.py` & `stlib-2.0.1/src/stlib/universe.py`

 * *Files identical despite different names*

### Comparing `stlib-2.0/src/stlib/utils.py` & `stlib-2.0.1/src/stlib/utils.py`

 * *Files identical despite different names*

### Comparing `stlib-2.0/src/stlib/webapi.py` & `stlib-2.0.1/src/stlib/webapi.py`

 * *Files identical despite different names*

### Comparing `stlib-2.0/src/stlib.egg-info/PKG-INFO` & `stlib-2.0.1/src/stlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stlib
-Version: 2.0
+Version: 2.0.1
 Summary: Async library that provides features related to Steam client and compatible stuffs
 Author: Lara Maia
 Author-email: dev@lara.monster
 License: GPLv3
 Project-URL: homepage, https://github.com/calendulish/stlib
 Project-URL: documentation, https://lara.monster/stlib
 Project-URL: repository, https://github.com
@@ -28,15 +28,14 @@
 
 stlib
 -----
 
 [![windows build status](https://badges.lara.monster/calendulish/.github/stlib-windows-build)](https://github.com/calendulish/stlib/actions/workflows/build.yml)
 [![linux build status](https://badges.lara.monster/calendulish/.github/stlib-linux-build)](https://github.com/calendulish/stlib/actions/workflows/build.yml)
 [![Coverage](https://codecov.io/gh/calendulish/stlib/branch/master/graph/badge.svg?token=DMKFKEUUZP)](https://codecov.io/gh/calendulish/stlib)
-[![Quality](https://api.codiga.io/project/33228/score/svg)](https://app.codiga.io/project/33228/dashboard)
 [![GitHub license](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](https://www.gnu.org/licenses/gpl-3.0.html)
 [![GitHub release](https://img.shields.io/github/release/calendulish/stlib.svg?style=flat)](https://github.com/calendulish/stlib/releases)
 
 Async library that provides features related to Steam client and compatible stuff
 
 WARNING: stlib is not intended to be used in game development, there is no support to callbacks, and I'll not work on that.
 stlib is intended to develop console or GUI applications that need interaction with SteamAPI or SteamWebAPI.
```

### Comparing `stlib-2.0/src/stlib.egg-info/SOURCES.txt` & `stlib-2.0.1/src/stlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

