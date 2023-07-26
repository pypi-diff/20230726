# Comparing `tmp/pyneople-0.0.6.tar.gz` & `tmp/pyneople-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneople-0.0.6.tar", last modified: Wed Jul 26 12:27:17 2023, max compression
+gzip compressed data, was "pyneople-0.0.7.tar", last modified: Wed Jul 26 12:30:39 2023, max compression
```

## Comparing `pyneople-0.0.6.tar` & `pyneople-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 12:27:17.304377 pyneople-0.0.6/
--rw-rw-rw-   0        0        0     1088 2023-07-21 05:43:07.000000 pyneople-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      579 2023-07-26 12:27:17.303655 pyneople-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-07-21 05:43:07.000000 pyneople-0.0.6/README.md
--rw-rw-rw-   0        0        0      108 2023-07-21 05:43:07.000000 pyneople-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 12:27:17.304377 pyneople-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-07-26 12:26:23.000000 pyneople-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:27:17.216771 pyneople-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 12:27:17.287768 pyneople-0.0.6/src/pyneople/
--rw-rw-rw-   0        0        0     2889 2023-07-24 04:27:44.000000 pyneople-0.0.6/src/pyneople/METADATA.py
--rw-rw-rw-   0        0        0      223 2023-07-24 04:51:23.000000 pyneople-0.0.6/src/pyneople/__init__.py
--rw-rw-rw-   0        0        0     1722 2023-07-21 05:43:07.000000 pyneople-0.0.6/src/pyneople/avatars.py
--rw-rw-rw-   0        0        0     3384 2023-07-26 12:26:49.000000 pyneople-0.0.6/src/pyneople/buff.py
--rw-rw-rw-   0        0        0     1403 2023-07-21 05:43:07.000000 pyneople-0.0.6/src/pyneople/character_search.py
--rw-rw-rw-   0        0        0     4643 2023-07-21 05:59:42.000000 pyneople-0.0.6/src/pyneople/equipments.py
--rw-rw-rw-   0        0        0     7209 2023-07-21 05:43:07.000000 pyneople-0.0.6/src/pyneople/functions.py
--rw-rw-rw-   0        0        0     3048 2023-07-21 05:43:07.000000 pyneople-0.0.6/src/pyneople/others.py
--rw-rw-rw-   0        0        0     1328 2023-07-21 05:43:07.000000 pyneople-0.0.6/src/pyneople/status.py
--rw-rw-rw-   0        0        0     3999 2023-07-21 05:43:07.000000 pyneople-0.0.6/src/pyneople/timeline.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:27:17.302648 pyneople-0.0.6/src/pyneople.egg-info/
--rw-rw-rw-   0        0        0      579 2023-07-26 12:27:17.000000 pyneople-0.0.6/src/pyneople.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-07-26 12:27:17.000000 pyneople-0.0.6/src/pyneople.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 12:27:17.000000 pyneople-0.0.6/src/pyneople.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 12:27:17.000000 pyneople-0.0.6/src/pyneople.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 12:30:39.483029 pyneople-0.0.7/
+-rw-rw-rw-   0        0        0     1088 2023-07-21 05:43:07.000000 pyneople-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      579 2023-07-26 12:30:39.482023 pyneople-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-07-21 05:43:07.000000 pyneople-0.0.7/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-21 05:43:07.000000 pyneople-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 12:30:39.483029 pyneople-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      833 2023-07-26 12:30:30.000000 pyneople-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:30:39.442021 pyneople-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 12:30:39.466021 pyneople-0.0.7/src/pyneople/
+-rw-rw-rw-   0        0        0     2889 2023-07-24 04:27:44.000000 pyneople-0.0.7/src/pyneople/METADATA.py
+-rw-rw-rw-   0        0        0      223 2023-07-24 04:51:23.000000 pyneople-0.0.7/src/pyneople/__init__.py
+-rw-rw-rw-   0        0        0     1722 2023-07-21 05:43:07.000000 pyneople-0.0.7/src/pyneople/avatars.py
+-rw-rw-rw-   0        0        0     3453 2023-07-26 12:30:17.000000 pyneople-0.0.7/src/pyneople/buff.py
+-rw-rw-rw-   0        0        0     1403 2023-07-21 05:43:07.000000 pyneople-0.0.7/src/pyneople/character_search.py
+-rw-rw-rw-   0        0        0     4643 2023-07-21 05:59:42.000000 pyneople-0.0.7/src/pyneople/equipments.py
+-rw-rw-rw-   0        0        0     7209 2023-07-21 05:43:07.000000 pyneople-0.0.7/src/pyneople/functions.py
+-rw-rw-rw-   0        0        0     3048 2023-07-21 05:43:07.000000 pyneople-0.0.7/src/pyneople/others.py
+-rw-rw-rw-   0        0        0     1328 2023-07-21 05:43:07.000000 pyneople-0.0.7/src/pyneople/status.py
+-rw-rw-rw-   0        0        0     3999 2023-07-21 05:43:07.000000 pyneople-0.0.7/src/pyneople/timeline.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:30:39.480022 pyneople-0.0.7/src/pyneople.egg-info/
+-rw-rw-rw-   0        0        0      579 2023-07-26 12:30:39.000000 pyneople-0.0.7/src/pyneople.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-07-26 12:30:39.000000 pyneople-0.0.7/src/pyneople.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 12:30:39.000000 pyneople-0.0.7/src/pyneople.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 12:30:39.000000 pyneople-0.0.7/src/pyneople.egg-info/top_level.txt
```

### Comparing `pyneople-0.0.6/LICENSE` & `pyneople-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.6/PKG-INFO` & `pyneople-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.0.6
+Version: 0.0.7
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/PyNeople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/PyNeople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneople-0.0.6/setup.py` & `pyneople-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyneople",
-    version="0.0.6",
+    version="0.0.7",
     author="ippo252525",
     author_email="ippo252525@gmail.com",
     description="Neople Open API wrapper for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ippo252525/PyNeople",
     project_urls={
```

### Comparing `pyneople-0.0.6/src/pyneople/METADATA.py` & `pyneople-0.0.7/src/pyneople/METADATA.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.6/src/pyneople/avatars.py` & `pyneople-0.0.7/src/pyneople/avatars.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.6/src/pyneople/buff.py` & `pyneople-0.0.7/src/pyneople/buff.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,8 +71,11 @@
                 try:
                     exec(f"self.buff_avatar_{avatar}.get_buff_avatar_data(one_slot(data, '{avatar.upper()}'))") 
                 except:
                     pass    
         data = get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/creature?apikey={self.__api_key}")
         data = data['skill']['buff']
         if data:
-            self.buff_creature = data['creature'][0]['itemName']
+            try:
+                self.buff_creature = data['creature'][0]['itemName']
+            except:
+                pass
```

### Comparing `pyneople-0.0.6/src/pyneople/character_search.py` & `pyneople-0.0.7/src/pyneople/character_search.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.6/src/pyneople/equipments.py` & `pyneople-0.0.7/src/pyneople/equipments.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.6/src/pyneople/functions.py` & `pyneople-0.0.7/src/pyneople/functions.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.6/src/pyneople/others.py` & `pyneople-0.0.7/src/pyneople/others.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.6/src/pyneople/status.py` & `pyneople-0.0.7/src/pyneople/status.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.6/src/pyneople/timeline.py` & `pyneople-0.0.7/src/pyneople/timeline.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.0.6/src/pyneople.egg-info/PKG-INFO` & `pyneople-0.0.7/src/pyneople.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.0.6
+Version: 0.0.7
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/PyNeople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/PyNeople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

